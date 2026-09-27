---
name: nexus-slides-to-video
description: Render a Google Slides deck (or a local .pptx) into a narrated video using the local pipeline at "Slides to Video Project" — speaker notes become the narration script, read by a local Piper TTS voice, each slide held on screen for exactly as long as its narration takes. Use when Rick asks to turn a slide deck / Google Slides link into a video, references the "Slides to Video" project, or wants a Lessig-style deck rendered for YouTube.
---

# Nexus Slides to Video

Converts a slide deck into a narrated video: each slide's Google Slides speaker-notes text becomes the voiceover script, synthesized with a local open-source TTS voice (Piper), with the slide image held on screen for exactly as long as its narration takes. Built for Rick's Lessig-style decks (many short slides, ~300–500 per deck, full narration script in the Notes section of each slide).

Project lives at `/Users/rickhoward/Desktop/1-my-system/projects/Slides to Video Project` (a plain folder, not a git repo). This skill just runs the pipeline that already lives there — it does not reimplement it.

## Running it

**CLI** (fastest for Rick to ask you to run directly):
```
cd "/Users/rickhoward/Desktop/1-my-system/projects/Slides to Video Project"
./venv/bin/python3 tools/build_video.py "<Google Slides URL, or a local .pptx path>"
```

**Web UI** (added 2026-09-06 — a local Flask app with a form + live progress bar + video playback):
```
cd "/Users/rickhoward/Desktop/1-my-system/projects/Slides to Video Project"
./venv/bin/python3 tools/SlidesToVideo.py
```
Each voice in the picker has a **Preview button** (added 2026-09-09, confirmed working on all three voices) that plays a short shared sample line so you can compare voices before rendering — fetches `/voice-sample/<voice-stem>` (synthesized once, cached in `tools/.voice_samples/`) and plays it from a Blob URL rather than pointing `<audio>` directly at the endpoint, which was observed hanging against Flask's dev server.

Opens `http://127.0.0.1:5001` in Chrome specifically (not just whatever the OS default browser is — falls back to the default only if Chrome isn't installed), waiting for the server to actually accept connections first so the browser never lands on a stale/wrong page from a startup race. **Port 5001, not 5000** (changed 2026-09-09): macOS's Control Center (AirPlay Receiver) listens on port 5000 by default and answers any non-AirPlay request with its own "Access ... was denied / HTTP ERROR 403" page — visually indistinguishable from a real server error, hit for real during testing. There's also a double-click launcher at the project root, `Start Slides to Video.command` — opens Terminal, starts the server, opens Chrome; closing that Terminal window (or Ctrl+C in it) stops the server. Both the CLI and the web UI call the exact same underlying pipeline (`tools/pipeline.py`) — no divergent logic between them. The web UI only allows one render at a time — a second submission while one is running redirects to the home page, which shows an "already in progress" banner with a link to that job's live status page, not a silent bounce; if you need to run a second instance yourself, note port 5001 will already be taken while an instance is up. The status page has a **Cancel** button (checked between slides, not mid-subprocess, so it can take a few seconds to land); an uploaded `.pptx`'s temp copy in `tools/.uploads/` is deleted automatically once its job ends, whether it finished, errored, or was cancelled. The form also has a **voice picker** (any `.onnx`+`.onnx.json` pair in `tools/voices/`, auto-discovered) and a **silence-seconds** field for slides with no speaker notes (default 3s) — both also available on the CLI as `--voice` and `--silence-seconds`.

Always use the project's own venv Python (`./venv/bin/python3`), not system Python — `piper-tts`, `python-pptx`, and the Google API client libraries only live in that venv.

**Input** — either:
- A Google Slides URL/edit link (or bare file ID) — pulled live via the Slides API.
- A local `.pptx` file path that exists on disk — rendered via LibreOffice + poppler instead.

**Output** — always written to `Completed Videos/` in the project folder, named `<deck title> - <YYYY-MM-DD>.mp4` (deck title pulled from the Slides API for Drive links, or the filename stem for local files; date is the render date, not the deck's date). Pass `-o <path>` to override.

## What happens internally (for troubleshooting, not something to re-derive)

- **Google Slides URL path** (`tools/drive_import.py`'s `fetch_slides_deck`): reads the deck slide-by-slide via the **Slides API** (`presentations.get` for notes text + title, `presentations.pages.getThumbnail` per slide for the image) — NOT Drive's `files.export`. This matters: `files.export` has a hard size cap and fails outright ("This file is too large to be exported") on any real ~300+ slide deck. The Slides API per-page approach has no such limit and is the only path that works on Rick's actual decks.
- **Local `.pptx` path**: `soffice --headless --convert-to pdf` (LibreOffice) renders the deck to PDF, then `pdftoppm` (poppler) rasterizes each page to PNG; notes text comes from `python-pptx`.
- Both paths converge in `tools/pipeline.py`'s `run_pipeline()`, which first runs every slide's notes through `strip_chunk_markers()` (added 2026-09-10) — removes any line that's *only* a number and a colon ("1:", "12:"), Rick's convention for marking where one slide's notes break into several narration chunks (narration text starts on the next line). Only whole-line matches are stripped, so a number that's part of actual narration content (sharing a line with other text) is never touched, and slides with no such lines pass through completely unchanged. Then each slide's (cleaned) notes text (or `silence_seconds` of silence if empty, default 3s) is synthesized with `piper-tts` (voice model defaults to `tools/voices/en_US-lessac-medium.onnx`, but any voice returned by `pipeline.list_voices()` can be passed — `en_US-amy-medium` and `en_US-joe-medium` are also installed as of 2026-09-09), ffmpeg builds one MP4 segment per slide holding the image for exactly that audio's duration, then all segments are concatenated into the final video. `run_pipeline()` takes an optional `progress` callback — the CLI prints it, the web UI feeds it into a per-job status dict that the status page polls. Which slides ended up silent (no notes) is reported via one `"silent-slides"` progress message before concatenation, not applied invisibly.

## Voice cloning (added 2026-09-09, engine swapped 2026-09-10)

The "Clone Your Voice" section on the web UI lets Rick narrate in his own (AI-cloned) voice instead of a Piper voice: upload a recording of yourself talking (any format, **at least 10 seconds** of clear speech) and name it — it shows up in the voice picker alongside the Piper voices afterward, with the same Preview button. Also on the CLI: `--clone-voice "Rick" /path/to/recording.m4a` to create one, `--voice cloned:rick` to render with it, `--list-voices` to see cloned voices too.

**Built on Coqui XTTS-v2** (`tools/voice_clone.py`, via the `coqui-tts` PyPI package) — a fully generative clone, not a conversion layer on top of Piper. **This replaced an original OpenVoice V2 build from the day before**, after Rick tested OpenVoice twice (once with a bad reference — a 28-minute podcast with music mixed in — once with a verified-clean 60-second solo recording) and it didn't sound like him either time. Clean input still failing pointed at OpenVoice's real limitation: it only converts timbre, never cadence or delivery style. **Rick was told explicitly, twice, that XTTS-v2's license (CPML) restricts commercial use of the model — a real concern for paid-talk videos — and chose to switch anyway.** That's a live, acknowledged risk in this project, not an oversight; don't quietly "fix" it by reverting without asking, and surface it again if this project's usage ever needs a defensible answer.

Full architecture, the auto-migration path for voices enrolled under the old OpenVoice system (no re-upload needed — the reference recording was always kept), the four real compatibility bugs found and fixed (a `transformers` version pin, a `torchcodec` extra, the `[cpu]` extra requirement, and the license-prompt bypass), and measured performance numbers are all in the `project_slides_to_video` memory file — don't re-derive any of that, it took real trial and error on this exact machine.

**Cost to know about, and it's a bigger deal than the license question:** a one-time ~1.87GB checkpoint download (first use only, cached at `~/Library/Application Support/tts/`, not project-local), and **cloned-voice rendering runs meaningfully slower per slide** than either Piper alone or the old OpenVoice build — roughly **2-13 seconds per slide** depending on narration length (measured on this machine, using Apple Silicon's MPS backend automatically when available). A 350-400 slide deck could add **on the order of an hour**, not a few minutes, to the usual 30-40 minute render. Say this out loud before Rick kicks off a full-deck render with a cloned voice for the first time. The web UI's clone-creation form is still a synchronous wait (not a background job — one-time action, not worth the extra machinery), now a wider ~15-45s range depending on whether the checkpoint needs downloading.

**XTTS hard-fails past ~400 tokens in one call** (`enable_text_splitting=True` now handles this transparently, requires the `spacy[ja]` package — see memory for why). Hit for real on slide 1 of a real 407-slide deck; fixed and verified 2026-09-10.

**Verification status:** mechanism thoroughly tested end-to-end (CLI, the real Flask app, a full render, the auto-migration path) using Rick's own real reference recording, not a synthetic stand-in. **Conditioning window widened 2026-09-10 after Rick's own listening test** — XTTS's own defaults only used a 6-second slice of the reference for speaking-style, wasting most of a 60-second clean recording; now uses the full reference by default (`voice_clone.COND_MAX_REF_LENGTH`/`COND_GPT_LEN`/`COND_GPT_CHUNK_LEN`), confirmed as a real improvement in a direct side-by-side. Full detail, including which other tuning knobs were tried and ruled out (temperature, reference normalization — neither helped), is in the `project_slides_to_video` memory file.

## Known gotchas

- **Slides API rate limit on `getThumbnail`** (hit 2026-09-06, on the 88-slide deck, at slide 69): `presentations.pages.getThumbnail` is billed against a separate "Expensive read requests" quota, capped at 60/min per user — distinct from general API quota. A fast network can blow through 60 calls in under a minute, and the reactive retry-on-429 backoff isn't always enough to recover cleanly mid-run. Fixed by proactively pacing thumbnail calls to ~1.2s apart (`MIN_THUMBNAIL_INTERVAL_SECONDS` in `drive_import.py`) rather than relying on retries alone. If a run ever errors out with `RATE_LIMIT_EXCEEDED` / `expensive_read_requests` again, that constant is the first thing to check/increase.

## Timing expectations

A ~350–400 slide deck takes **30–40 minutes end to end** (Slides API fetch is fast, ~5 slides/sec; the narration+ffmpeg stage is the slow part, roughly one slide every few seconds). Always run it as a background task and check back periodically (every 5–10 min) rather than blocking on it or polling tightly.

## One-time Google Cloud setup (already done as of 2026-09-06 — reference only if it needs redoing)

Credentials live at `tools/credentials.json` (OAuth "Desktop app" client secret) and `tools/token.json` (cached token; delete it to force re-authorization, e.g. after a scope change). If either is missing or auth starts failing, see the full trial-and-error writeup in memory (`project_slides_to_video` memory file) — short version:

- Cloud project "Slides to Video Project", OAuth consent screen on Google's newer "Google Auth Platform" UI (Branding / Audience / Data Access tabs).
- Required scopes (under **Data Access**, not Branding): `https://www.googleapis.com/auth/drive.readonly` + `https://www.googleapis.com/auth/presentations.readonly`. The scope picker is easy to mis-click since several Drive scopes look similar — use the search box with the full scope URL to disambiguate.
- Both the **Drive API** and **Google Slides API** must be individually enabled under APIs & Services → Library — enabling one does not enable the other.
- The authorizing account (`rahhoward@gmail.com`) is also the project owner, so it's automatically authorized in Testing status — Google will refuse to let you add it as a "test user" ("ineligible for designation"). That's expected, not a bug.
- `InstalledAppFlow.run_local_server()`'s auto browser-open doesn't work when the script runs as a backgrounded subprocess — it still prints the authorization URL to stdout; open that URL manually in a real browser and it redirects to the local callback server fine.

## Known limitations

**All five gaps tracked here as of 2026-09-06 were closed or found already-handled on 2026-09-09** (see the `project_slides_to_video` memory file for full detail on each):

- ~~Empty-notes slides just get a flat 3-second silence; no smarter handling.~~ Fixed — `--silence-seconds`/UI field, and a `"silent-slides"` progress message names which slides went silent.
- ~~A slide-count mismatch aborts with a generic error rather than pinpointing which slide.~~ Fixed — `pipeline.SlideRenderMismatch` names which side (image rendering vs. the deck's real slide count) diverged and points at `--keep-work-dir`'s intermediate files.
- ~~The web UI's one-render-at-a-time guard bounces back to the form with no explanation.~~ Turned out to already be handled — the redirect lands on the home page, which already shows an "already in progress, view its progress" banner with a link. No code change needed; the doc describing this as a gap was just stale.
- ~~Error messages in the web UI show the raw Python exception string.~~ Fixed — `SlidesToVideo._friendly_error()` maps known failure shapes (missing OAuth credentials, a failed subprocess, a Slides API HTTP error) to a short banner message; the full raw exception still always lands in the job log for debugging.
- ~~No way to pick a different Piper voice from the UI.~~ Fixed — voice picker (radio list, one row per voice), auto-populated from whatever's in `tools/voices/`; two more voices (`en_US-amy-medium`, `en_US-joe-medium`) downloaded alongside the original so the picker has real choices, not just one.

No other gaps are currently tracked. If a new rough edge turns up in real use, add it here.

## Validated on real decks

Three real production decks have rendered successfully end to end via this pipeline (2026-09-06): a 349-slide deck (36 min output, CLI), a 407-slide deck (38 min output, CLI), and an 88-slide deck (17 min output, both CLI and — after the rate-limit fix — through the web UI). All included embedded photos and AI-generated graphics rendering correctly, not just plain text slides.
