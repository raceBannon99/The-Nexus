---
name: nexus-artifact-submit
description: Propose an artifact (essay, book review, fact sheet, image, or other reference material) for Alexandria's Library — the private nexus-artifacts repo — via a Pull Request that Rick must approve. Also handles pulling an existing artifact back out of the repo on request, and checking the repo for open/pending artifact PRs. Use when any Nexus agent (during a nexus or nexus-daily-report engagement, or standalone) surfaces something worth archiving permanently, when Rick asks to add something to the archive/library, when Rick asks to pull/export an artifact, or when checking for pending artifact approvals.
---

# Nexus Artifact Submission, Retrieval & Pending-Approval Check

Manages the lifecycle of https://github.com/raceBannon99/nexus-artifacts (private) — Alexandria's Library. Full lifecycle detail lives in `Nexus Artifact Repository.md` in the vault; re-read it before running in case it has changed since this skill was written. That doc, not this one, is the source of truth if they drift.

**Critical:** this repo's git policy is the opposite of `raceBannon99/The-Nexus` (the reports repo, direct-to-main). Every artifact addition here goes through a Pull Request — never commit directly to `main` on this repo.

## Before running

Confirm GitHub access: `gh auth status`. Stop and ask Rick to run `gh auth login` if not authenticated.

## Submitting a new artifact

1. Pick the category folder: `essays/`, `book-reviews/`, `fact-sheets/`, `images/`, or `other/`.
2. Prepare the artifact file (and its updated `INDEX.md`, see step 5) at local scratch paths first — don't clone/branch/commit by hand.
3. Branch name: `artifact/<kebab-case-slug>`.
4. The file itself. **No date-prefixed filenames** — kebab-case title only.
   - Markdown artifacts (essay/book-review/fact-sheet) get YAML frontmatter:
     ```yaml
     ---
     title: "..."
     category: essay | book-review | fact-sheet
     author: "Rick Howard" | "<external author name>"
     source_url: "<original URL, or 'n/a — original work'>"
     rights_holder: "<author/publisher>"
     date_added: YYYY-MM-DD
     added_by: Alexandria | Sherlock | Euclid | Popper | Seldon | Turing
     tags: [tag1, tag2]
     ---
     ```
   - Binary artifacts (images, PDFs) get no frontmatter — they're catalogued entirely via their `INDEX.md` row.
5. Add the corresponding row to `INDEX.md` in the same commit — title, category, path, author/source, rights holder, date added, added by, one-line note. Fetch the current `INDEX.md` (`gh api repos/raceBannon99/nexus-artifacts/contents/INDEX.md`), edit it locally with the new row appended, save as a local scratch file.
6. Publish steps 2–5 in one shot with `.claude/scripts/nexus-git-publish.sh "https://github.com/raceBannon99/nexus-artifacts.git" <clone-parent-dir> artifact/<kebab-case-slug> "Add fact-sheet: <title>" "<local-artifact-file>:<category>/<kebab-case-slug>.md" "<local-index-file>:INDEX.md"` (already allowlisted as a single fixed command — clones fresh, creates the branch since it isn't `main`, copies both files in, commits, and pushes the branch with `-u`). **Do not hand-write the clone/branch/commit/push sequence** — every time this has been done by hand instead of through the script, it's ended up wrapped in a `CLONE_DIR="..."` variable that breaks the permission allowlist and prompts on every step. Then `gh pr create` (a separate call — its title/body need real drafting, the script doesn't do this step) filling in the repo's PR template: artifact title/category/path, which agent is proposing it, a rationale paragraph (what claim or recurring need this supports — same discipline as a Nexus report's Sources entries), and provenance (author, rights holder, original date). If this artifact came from a specific report's "Library Recommendations" entry, link that report in the PR body.
7. **If step 6's artifact came from a report's Library Recommendations entry, close the loop now — don't wait for merge.** Run an Update Pass (per the `nexus` skill) on that report immediately: change the entry's status from "Recommended — awaiting decision" to "Submitted — PR #N, awaiting merge," linked to the PR just opened. A report shouldn't keep claiming a decision is pending once Rick has actually made one.
8. Report the PR URL back to Rick. **Do not merge it.** Rick is the sole merge authority — no agent merges its own or another agent's artifact PR under any circumstance.

## Checking for pending (open) artifact PRs

Run this as a footer check whenever this skill, `nexus`, or `nexus-daily-report` runs (per [[Nexus Artifact Repository]]'s reminder mechanism):

```
gh pr list --repo raceBannon99/nexus-artifacts --state open
```

If any are open, report the count and a one-line list (PR title + URL) to Rick. If none are open, no need to mention it.

## Closing the loop on merged PRs

Also check merged PRs, not just open ones — a report that recommended an artifact needs a second Update Pass once that artifact actually lands, and nothing else will remind you of that but this check:

```
gh pr list --repo raceBannon99/nexus-artifacts --state merged
```

For any merged PR whose description references an originating `raceBannon99/The-Nexus` report, open that report and check its Library Recommendations status. If it still says "Submitted" or "Recommended" rather than "Added to Library," the loop isn't closed — flag it to Rick and, on confirmation, run the Update Pass: status → "Added to Library" (linked to the artifact's final path in `nexus-artifacts`), and add a new Sources-section entry in that report citing the artifact directly. The report's own current status text is the only tracking mechanism needed here — no separate log to maintain.

## Exporting / retrieving an artifact

When Rick asks for a copy of something already in the archive:

- `gh api repos/raceBannon99/nexus-artifacts/contents/<path>` to fetch file content directly, or clone/`git show` against a working copy for a bulk pull.
- Write it wherever Rick specifies (vault note, Desktop, etc.) using normal file tools — no special export tooling needed, this is just an authenticated read against a private repo.

## After any action

Report back what happened plainly: PR URL for a new submission, the pending-PR list for a check, confirmation of where an exported file was written, or which report(s) got closed out once a recommended artifact merged.
