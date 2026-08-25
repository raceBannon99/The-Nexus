# ELI5: Claude Skills — What Are They, How Do You Use, Create, and Share Them?

**Question:** Eli5: Claude Skills. What are they? How do you use them? How do you create your own? How do you use other people's skills?

## Bradlee's Synthesis

A Skill is a folder on disk with one required file, `SKILL.md`, containing a short description ("what this does, when to use it") plus instructions in plain markdown. That's the whole primitive. The cleverness is in when Claude reads it — not in the format itself.

Every Skill loads in three stages, and this is the idea to actually remember. **Level 1** is just the name and one-paragraph description — that's always sitting in Claude's context, for every installed Skill, costing about 100 tokens each. Claude compares your request against these descriptions to decide what's relevant. **Level 2** is the actual body of `SKILL.md` — the real instructions — and it only loads once Claude decides a Skill applies to what you're doing. **Level 3** is everything else the Skill bundles — reference docs, templates, scripts — and those load only if the Level 2 instructions point Claude at them, sometimes not at all. This is why you can have dozens of Skills installed with no real context cost: almost all of that content sits on disk, untouched, until it's actually needed. Tufte's diagram below shows this concretely, with the token costs at each stage.

**Using** a Skill you already have is nothing — you don't do anything. Claude reads the installed Skills' descriptions automatically and reaches for one when your request matches. In Claude Code specifically, you can also force it directly by typing `/skill-name`, which is how you're reading this: this entire report ran because Rick typed `/nexus`, a Skill. Euclid's section below doesn't leave that abstract — it walks through that exact Skill's real numbers.

**Creating your own** is: make a folder, write a `SKILL.md` with a `name`/`description` header and instructions underneath. In Claude Code, drop it in `~/.claude/skills/` (personal — works in every project you open) or `.claude/skills/` inside a specific repo (project-only, and — critically for The Nexus — checked into git, so it travels with the repo and everyone with access gets it). On claude.ai you upload a zip through Settings instead. The two are separate installs; a Skill built in Claude Code doesn't automatically appear on claude.ai or vice versa.

**Using someone else's Skill** means installing their folder into one of those same locations — nothing more exotic than that. The lowest-friction path in Claude Code is a plugin marketplace (`/plugin marketplace add`, then `/plugin install`), which Anthropic runs one of for its own official Skills. But "install" here means "let this text and code direct Claude's actions on your machine," and Anthropic's own documentation is blunt about the implication: use Skills only from yourself or from Anthropic, and treat anything else the way you'd treat installing unfamiliar software — because a Skill can steer Claude into running commands well outside what its description advertises.

That last point is the one place this report pushed back hard on itself, and it's worth stating plainly rather than burying it: "Skills are simple to create" is true, and "Skills are simple to trust" is not the same claim. Popper's objection below and Seldon's response to it both center on this gap — the mechanics are genuinely as easy as described; the judgment calls around whose Skills to run are not, and no amount of tooling currently automates that judgment away. Ryan found no adversary or named campaign angle here — this is a platform-mechanics question, not an intelligence one — so that stage passed through unchanged.

## Clarifying Questions

None asked. The question — what Claude Skills are, and how to use/create/share them — was well-scoped as posed: a single well-defined feature with an authoritative source of truth (Anthropic's own documentation), no ambiguity about timeframe, scope, or definition that would change the shape of the answer. Bradlee passed it to Alexandria without modification.

## What We Already Know

Alexandria checked the artifact library (`raceBannon99/nexus-artifacts`) first: nothing there answers this — no fact sheet, essay, or reference on Claude Skills exists yet. A search of prior Nexus reports (`raceBannon99/The-Nexus`) turned up one adjacent document, `reports/2026-07-20-nexus-harness-architecture.md`, which describes The Nexus's own agent chain as implemented via three Claude Code Skills (`nexus`, `nexus-daily-report`, `nexus-artifact-submit`) — useful as a real, working example of a project Skill, but it documents The Nexus's internal architecture, not the Skills feature itself, and it predates Ryan and Bradlee joining the chain. No other report addresses the question directly. This is a fresh topic for the archive.

## Euclid: What Are Skills, From First Principles

Strip away the product language and a Skill is one thing: **a piece of context that Claude loads conditionally instead of unconditionally.**

Every other way of giving Claude durable knowledge — a system prompt, a `CLAUDE.md` file, pasting instructions into a conversation — loads *unconditionally*: it's in context whether or not the current task needs it, all the time, for every turn. That's fine for a small amount of guidance. It stops being fine once you have twenty small procedures you want available, because now you're paying the token cost of all twenty on every single turn regardless of which one (if any) applies right now.

A Skill fixes this with a filesystem trick, not an algorithmic one: split the content into a cheap, always-loaded *pointer* (the name + description, ~100 tokens) and an expensive, conditionally-loaded *body* (the actual instructions, loaded only when the pointer matches). This is why the docs call it "progressive disclosure" — it's the same idea as a table of contents versus the book. You keep the table of contents open at all times because it's cheap; you only open the chapter you need.

That one design choice determines almost everything else about how Skills behave:

- **Why they scale:** because the unused ones cost ~100 tokens each rather than their full body, you can install far more Skills than you could ever paste into a system prompt.
- **Why the `description` field matters so much:** it's the *only* thing Claude sees before deciding whether to load the rest. A vague description means Claude either misses Skills it should use or loads ones it shouldn't — this is a real, named failure mode with real tooling built to catch it (see Popper, below).
- **Why creating one is genuinely just "write a markdown file":** there's no compiler, no registration step, no API call required for the personal/project case. The folder *is* the registration. Claude Code watches the skills directories and picks up new or edited ones without a restart.
- **Why "using someone else's Skill" is just "put their folder where your Skills live":** there's no separate installation mechanism, no sandboxed permission model baked into the format itself (Claude Code skills get the same filesystem/network access as anything else you run locally) — the folder is the whole artifact, and putting it in the right place is the whole install.
- **Why it doesn't travel between claude.ai, the API, and Claude Code automatically:** each surface has its own execution environment (a claude.ai sandbox with variable network access, an API container with none, your actual machine in Claude Code) and its own storage location for Skills. Progressive disclosure describes *when* content loads; it says nothing about syncing that content across products, and Anthropic hasn't unified that separately.

Concretely, then:

- **What they are:** a folder with a required `SKILL.md` (YAML header: `name`, `description`; body: instructions), optionally bundling reference docs and scripts.
- **How you use one that exists:** nothing, usually — Claude reaches for it automatically when your request matches its description. In Claude Code you can also invoke it explicitly with `/skill-name`.
- **How you create your own:** write the folder and file, save it to `~/.claude/skills/<name>/` (personal, all projects) or `.claude/skills/<name>/` (this project only, shareable via git). Claude Code detects it live.
- **How you use someone else's:** get their folder into one of your Skills locations — by hand, via a Claude Code plugin marketplace (`/plugin install <skill>@<marketplace>`), or (for claude.ai) by uploading the zip they give you through Settings.

### A Real-World Example: The `nexus` Skill Itself

Every abstraction above maps onto something already sitting in this vault — the actual Skill that produced this report, `.claude/skills/nexus/SKILL.md`. It's a genuine project Skill, checked into the repo so anyone with access gets it, and Sherlock pulled its real numbers directly from the file rather than illustrating with round ones:

```yaml
---
name: nexus
description: Run an ad-hoc question or topic through The Nexus's nine-agent workflow (Bradlee first checks the question for clarifying questions, then Alexandria opens, then Sherlock, Ryan, Euclid, Popper, Seldon, Tufte, Turing, Bradlee synthesizes the answer, and Alexandria closes and publishes) and publish the result directly to main. Use when Rick brings a new question or topic to "The Nexus" outside of the recurring daily report — e.g. "let's use Nexus to figure out X," "ask the Nexus team about Y."
---
```

- **Level 1 (metadata):** the `description` above is 495 characters — roughly 124 tokens, noticeably above the docs' rough ~100-token average. That's the description-tuning tradeoff Popper raises below, made visible with a real number: this Skill has to reliably trigger on loosely-phrased requests like "let's use Nexus to figure out X," so it spells out the full nine-agent roster up front rather than staying terse. A longer always-loaded pointer, paid on every single session, bought in exchange for triggering more reliably.
- **Level 2 (instructions):** the full `SKILL.md` body — the eleven-stage sequence, the Update Pass triage table, the publishing mechanics — runs about 4,900 tokens across 75 lines. That sits right at the edge of the "under 5,000 tokens" ceiling the docs recommend for Level 2 content, and it loads in full only once Claude decides the Skill applies — when Rick actually types `/nexus` or asks a Nexus-shaped question — not on every turn of every session.
- **Level 3 (resources and code):** this Skill doesn't bundle its own `scripts/` folder, but its instructions direct Claude to run existing repo scripts via bash — `.claude/scripts/nexus-search-reports.sh` for searching prior reports, `.claude/scripts/nexus-git-publish.sh` for the publish step that put this very report on `main`. Same Level 3 mechanic the docs describe — the script runs, only its output enters context, the script's own code never does — the resource just lives alongside the Skill in the repo rather than inside its own folder, which the format allows.

It's also, concretely, the "using someone else's Skill" question turned inward: this one isn't from a stranger, it's Rick's own — first-party by construction, exactly the trust profile Popper's objection (below) says to look for. It's the version of Skill-sharing that already carries no open trust question, sitting right next to the version that does.

## Popper: Where This Gets Harder Than "Just a Markdown File"

Euclid's account is accurate as far as it goes, but it describes the mechanics in a way that makes the whole feature sound frictionless, and two parts of it aren't.

**First — the description problem is not hypothetical, it's the documented failure mode.** Because Level 1 (the description) is the *only* signal Claude uses to decide whether to load a Skill, a badly-written description silently breaks the feature in two directions: too vague and Claude never triggers it when it should ("false negative"), too broad and Claude triggers it on requests it shouldn't touch ("false positive"). This isn't a minor edge case — Anthropic built a whole plugin (`skill-creator`) specifically to run should-trigger / should-not-trigger prompt batches against a Skill and tune the description automatically, which is a tacit admission that getting the description right by hand is genuinely hard, not a five-minute afterthought the way "just write a markdown file" implies.

**Second, and more serious — "use other people's Skills" glosses over a real trust boundary that the format does nothing to enforce.** A Skill is not sandboxed data; it's an instruction set that can direct Claude to run bash, hit the network, or touch your filesystem — and in Claude Code specifically, a Skill someone else wrote gets the same access to your machine as anything else you run. Anthropic's own security guidance says, in effect: only run Skills from yourself or from Anthropic, and treat anything else like installing unfamiliar software, because a malicious or merely careless Skill can direct actions that don't match its stated purpose, and a Skill that fetches external content is riskier still since that fetched content can carry its own instructions. That's not a footnote — it directly contradicts the plain reading of "how do you use other people's Skills," which sounds like it should be as easy as installing one of your own. It isn't, or rather: it's mechanically identical but it shouldn't be treated as equally safe.

Neither of these breaks the feature. Both mean the honest answer to "how do you create/share Skills" has to include "and here's the part that isn't automatic yet" rather than stopping at the folder-and-file mechanics.

## Seldon: Resolving Popper's Objections, and What's Next

Taking each objection in turn rather than letting either sit unaddressed:

**On the description-tuning problem:** this is resolved, not dismissed — Popper is right that hand-tuning is genuinely hard, but the `skill-creator` eval workflow he cites *is* the resolution mechanism, not just evidence the problem exists. It runs a Skill with and without a candidate description change against realistic prompts in isolated subagent runs, grades trigger accuracy, and proposes description edits — that's a real, working answer to "how do I know my description is good," not a hypothetical one. The residual risk is adoption, not absence of tooling: most people writing a personal Skill for their own use won't run a formal eval loop, and for a single-user Skill that's a reasonable trade of rigor for speed. It matters more once a Skill is shared broadly enough that a wrong trigger affects people other than its author — which is exactly when Turing's and Rick's own judgment about whether to invest in an eval loop should scale up too.

**On the trust boundary:** this one Seldon does *not* fully resolve, and says so rather than smoothing it over — Popper's objection stands as a real, currently-unclosed gap. The mitigations that exist today are partial: Anthropic's own official Skills are implicitly trusted by virtue of the publisher, Claude Enterprise organizations can turn on content scanning for Skills uploaded through claude.ai and Cowork, and plugin marketplaces provide a thin layer of provenance (you at least know which repository a Skill came from) — but content scanning doesn't cover the Skills API or Console upload paths, and there is no equivalent for an individual or small team pulling a Skill off GitHub. The practical answer today is manual audit, exactly as Anthropic's docs recommend, and that remains the honest state of the world rather than a solved problem.

**Forward-looking, in plain language rather than point estimates:**

- *How much of the current audit burden gets automated away.* The trajectory (skill-creator's evals, Enterprise content scanning, marketplace curation) is toward more tooling, not less — but "more tooling exists" and "casual users actually use it before installing a stranger's Skill" are different claims. The share of Skill installs outside Anthropic's own official set that get any kind of automated safety check before use — a year from now — plausibly runs from roughly a quarter to maybe two-thirds, with a median guess of somewhere around 40%. The low end assumes scanning stays Enterprise-gated and manual audit remains the default everywhere else; the high end assumes marketplace-level automatic scanning becomes standard the way app-store scanning did.
- *How long until Skills are genuinely portable across claude.ai, the API, and Claude Code without a separate upload per surface.* This is a product-unification question more than a technical one — nothing about progressive disclosure prevents a shared registry, it just doesn't exist yet. A reasonable range is about 1 to 3 years, with a median around 18 months, driven mainly by how much Anthropic prioritizes cross-surface identity/account unification versus keeping each surface's execution model (and therefore its trust boundary) deliberately separate — which is itself a judgment call, not a foregone conclusion, since the separation is partly a safety feature and not purely an oversight.

Both ranges are reasoned judgment based on the maturity of the tooling already shipped and the pace of the last year of Skills-related product changes (skill-creator, `context: fork`, `skillOverrides`, Enterprise scanning all landing within roughly the same window per the documentation reviewed) — not measured data, and Rick should weight them accordingly.

## Tufte: How a Skill Actually Loads

The three-level loading model is the one part of this answer that's a genuine sequential/branching process rather than a comparison of facts — worth a real diagram rather than a table pretending to be one.

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-08-25-eli5-claude-skills/progressive-disclosure.png" alt="Diagram: How a Skill loads via progressive disclosure — Level 1 metadata (always, ~100 tokens), Level 2 instructions (when triggered, under 5,000 tokens), Level 3 resources and code (only if referenced, zero cost until accessed)">

The two other places this report needed structure are genuinely tabular — a straight comparison of facts, not a flow — so they stay as tables rather than forced into images:

**Where a Skill lives determines who can use it (Claude Code):**

| Location | Path | Applies to |
|---|---|---|
| Personal | `~/.claude/skills/<name>/SKILL.md` | All your projects |
| Project | `.claude/skills/<name>/SKILL.md` | This project only (shareable via git) |
| Plugin | `<plugin>/skills/<name>/SKILL.md` | Wherever the plugin is enabled |
| Enterprise | managed settings directory | Every user in the organization |

**Where custom Skills work, and what "using someone else's" looks like on each surface:**

| Surface | How you create/upload | How you get someone else's | Sharing scope |
|---|---|---|---|
| Claude Code | Save a folder to `~/.claude/skills/` or `.claude/skills/` | Copy their folder in, or `/plugin install <skill>@<marketplace>` | Personal, or project-wide via git |
| claude.ai | Upload a `.zip` via Settings → Features | They send you the zip; you upload it yourself | Individual user only — not org-shared, no admin push |
| Claude API | Upload via the `/v1/skills` endpoint | A workspace member uploads it once | Workspace-wide, all members |

## New Skills

None. This engagement was documentation lookup and synthesis against an already-current, well-organized official source — it didn't surface a repeatable procedure, tool integration, or research technique novel enough to warrant packaging as a Skill. Turing says so plainly rather than manufacturing one.

## Sources

**Primary/official (Anthropic documentation, fetched directly):**
- [Agent Skills — Overview](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview) — Anthropic Claude Platform Docs. Supports: the three-level progressive disclosure model, token costs per level, where Skills work across claude.ai/API/Claude Code, required frontmatter fields, security guidance on trusted sources.
- [Extend Claude with skills](https://code.claude.com/docs/en/skills) — Claude Code documentation. Supports: personal vs. project skill locations, live change detection, `/skill-name` invocation, plugin marketplace install flow (`/plugin install`, `/plugin marketplace add`), the `skill-creator` eval workflow, frontmatter field reference, sharing/removal mechanics.
- [GitHub: anthropics/skills](https://github.com/anthropics/skills) — Anthropic's public repository of open-source Agent Skills (referenced for the existence and scope of Anthropic's own published Skills; not separately fetched in full).

**Internal precedent (raceBannon99/The-Nexus):**
- `reports/2026-07-20-nexus-harness-architecture.md` — prior Nexus report documenting The Nexus's own agent chain as implemented via three Claude Code Skills (`nexus`, `nexus-daily-report`, `nexus-artifact-submit`). Supports: a concrete, working example of a project-level Skill, cited in Bradlee's synthesis and Euclid's draft. Note: this report predates Ryan and Bradlee joining the agent chain and describes internal Nexus architecture, not the Skills feature generally — background context, not a source for the feature-level claims above.
- `.claude/skills/nexus/SKILL.md` (this project's local vault, `raceBannon99/The-Nexus` clone) — the actual Skill that ran this engagement. Supports: the worked example in Euclid's section — its real `description` length (495 characters / ~124 tokens) and full-body length (~4,900 tokens / 75 lines), read directly from the file rather than estimated, plus its references to `.claude/scripts/nexus-search-reports.sh` and `.claude/scripts/nexus-git-publish.sh` as its Level 3 resources.

No claim in this report rests on an uncited or unverifiable source; nothing here needed general-coverage hedging.

## Library Recommendations

**Recommended for archiving — awaiting Rick's decision, not yet submitted:**

- **Candidate:** "Claude Skills: How They Work" (working title)
- **Category:** `fact-sheets`
- **Why it's reusable beyond this report:** This is exactly the kind of platform-mechanics reference the library is meant to hold — the three-level progressive-disclosure model, the where-skills-live table, and the trust-boundary caveat from Popper's stage don't change often and will be relevant to any future Nexus engagement that touches Skills, plugins, or Claude Code configuration (the `nexus-harness-architecture` precedent found above shows this has already come up once). Distilling Euclid's first-principles explanation, the `nexus` Skill worked example, and Tufte's diagram into a standalone fact sheet would save re-deriving this from Anthropic's docs — and from this vault's own Skill files — on a future ad-hoc question.
- **Status:** Recommended by Alexandria; final call is Rick's.

No other artifact from this run rose to the same bar — Popper's and Seldon's sections are report-specific reasoning about *this* draft rather than durable reference material, so they weren't separately flagged.
