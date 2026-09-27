---
name: nexus-forecast-narrative
description: Compute and phrase the standing "uncertainty window" and "years-to-50%-chance" narrative that must accompany every range Agent Seldon produces or cites anywhere in the Nexus — the three standing AI forecast files (P5/P50/P95 notation), the daily report's AI Timeline Forecasting section and per-category repeat lines, and any ad-hoc `nexus` engagement forecast (plain-language notation). Use whenever citing, updating, or newly establishing a Seldon range, in the daily report or an ad-hoc engagement.
---

# Nexus Forecast Range Narrative

Per Rick's direct instruction (2026-09-27): any time Seldon states or cites a P5/P50/P95 range (or, in an ad-hoc `nexus` engagement, its plain-language equivalent — see below), two derived figures go with it. This is the single canonical spec for that narrative — every other Nexus doc that mentions it points back here rather than restating the formula.

## The two figures

- **Uncertainty window** = P95 − P5, in years. How wide the whole plausible range is.
- **Years to 50% chance** = P50 − P5, in years. How long after the earliest plausible date (P5) the coin-flip date (P50) falls.

**Always recompute both from that citation's current P5/P50/P95 — never carry a number forward from a prior report.** They move whenever the range does. If a range is unchanged since its last update, the two figures are also unchanged, but they're still restated (recomputed, not copy-pasted) every time the range is cited — the same "recompute, don't cache" discipline the forecast files already apply to their own Evidence Log entries.

## Standard phrasing — P5/P50/P95 notation

Used for the three standing forecast files (Singularity, AGI, Superintelligence Forecast Reports) and every place the daily report cites one of them:

```
P5 [date] · P50 [date] · P95 [date]: a [P95−P5]-year uncertainty window and a 50% chance we could reach this milestone in [P50−P5] years.(unchanged since [date])
```

Note the exact punctuation: a colon after P95, the two-figure sentence, then the "(unchanged since ...)" parenthetical immediately abutting the period with no space before it — this is the established house style, not a typo.

**Worked example** (AGI Forecast Report, as read 2026-09-27): P5 2028 · P50 2036 · P95 2100 → window = 2100 − 2028 = **72 years**; years-to-50% = 2036 − 2028 = **8 years** →

> P5 2028 · P50 2036 · P95 2100: a 72-year uncertainty window and a 50% chance we could reach this milestone in 8 years.(unchanged since 2026-09-18)

This phrasing applies everywhere one of the three standing files' ranges is cited, not only its own At-a-Glance line:
- The daily report's standing **"AI Timeline Forecasting"** section (all three entries, every run — see `Instructions-CIR-Project.md`).
- Any per-category section elsewhere in the daily report body that repeats its own current-range line at its own top (the 2026-09-15 convention) — same figures, same phrasing, recomputed.
- Any ad-hoc `nexus` engagement that cites one of the three standing files as a source, when it quotes the file's own P5/P50/P95 figures directly rather than restating them in Seldon's own plain-language voice.

## Plain-language phrasing — ad-hoc `nexus` engagement forecasts

Per `Agent Seldon Concept.md`'s standing rule, ad-hoc Nexus forecasts never use "P5/P95" statistical notation — Seldon states a range with a median in prose ("the range runs from about X to Y, with a median around Z"). The same two derived figures still belong in that prose, phrased in kind rather than bolted on as notation:

```
the range runs from about [P5] to [P95] — a [P95−P5]-year span — with a median around [P50], roughly [P50−P5] years out from the earliest plausible date
```

Adapt the exact wording to the sentence Seldon is already writing (a date range, a dollar range, a percentage range, etc.) — the two figures (span width, distance from the near edge to the median) are the fixed content; the sentence carrying them is not a rigid template the way the P5/P50/P95 house style above is.

## Worked reference table (as of 2026-09-27)

| Standing file | P5 | P50 | P95 | Uncertainty window | Years to 50% |
|---|---|---|---|---|---|
| AGI Forecast Report | 2028 | 2036 | 2100 | 72 years | 8 years |
| Singularity Forecast Report | 2027 | 2042 | 2100 | 73 years | 15 years |
| Superintelligence Forecast Report | 2029 | 2045 | 2100 | 71 years | 16 years |

This table is a worked reference, not a cache — if any of the three ranges has moved since 2026-09-27, recompute its row from the file's own current At-a-Glance line rather than trusting this table.

## Where this is wired in

- `Instructions-CIR-Project.md`'s "AI Timeline Forecasting" section spec, and its note on the per-category repeat-line convention, both point here as the canonical format for the daily report.
- `nexus-daily-report/SKILL.md`'s Turing step (assembling the report) applies it when building both the standing section and any per-category repeat line.
- `nexus/SKILL.md`'s Seldon step applies the plain-language version to any ad-hoc range, alongside its existing no-statistical-notation rule.
- Each of the three standing forecast files' own Rules section notes that every citation of its range — not just its At-a-Glance line — carries this narrative.

## Origin

Added 2026-09-27, per Rick's direct instruction, after he asked for the same two figures to be added retroactively to that day's already-published daily report (commits `2808854` and `dc4e4d8` on `raceBannon99/The-Nexus`) and then asked for the convention generalized into a standing skill rather than reapplied by hand each run.
