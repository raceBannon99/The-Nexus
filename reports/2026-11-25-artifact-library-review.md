# Artifact Library Review: Delete, Update, or Keep

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

**Question:** Review the documents in the private artifacts library and make a recommendation about each file to either delete it because it's not useful anymore, find an updated document because the current one is out of date, or keep because it might be useful in the future.

**Date:** 2026-11-25

## So, What's the Answer?

Of the 44 artifacts in the private library, keep 35, update 8, and delete 1. The library is in good shape. Most of it is reference material that doesn't age (attribution frameworks, Tufte principles, the Emacs primary record, Rick's own book graphics), or it was refreshed within the last week (the Who's Who roster and the AI Timeline Forecasting chart, both current as of today's figures).

The one deletion is the October 3 snapshot of the AI Timeline Forecasting chart (`images/ai-timeline-forecasting-summary.png`). Every number on its four date panels has since moved. A faithful recreation of the same design now carries the current figures, and the history of each move is kept in the five forecast files' Evidence Logs. The snapshot no longer does anything the current chart and those logs don't do better.

The eight updates fall into three groups.

**Two items are dated by events.** The US Federal AI Legislation fact sheet and its spectrum diagram still show status "as of Oct. 2026" and point at a November 3 midterm deadline that has now passed. The bigger date is January 3, 2027, when the 119th Congress ends and every bill that hasn't been enacted dies. Update the status column for the lame-duck session now. Then, on January 3, freeze the sheet as a historical record of the 119th Congress and start a new one for the 120th. The public copy of the diagram (go/29) would need a re-sync at the same time.

**Four items still print forecast ranges Nexus has since retired.** The Named AGI Predictions ledger and its timeline image still show the old AGI range (2028, 2036, 2100). The current range is 2029, 2045, 2075. The AGI vs. Singularity fact sheet quotes the September 18 Singularity range (2027, 2042, 2100) as the standing forecast. The current range is 2031, 2046, 2075. The method in that fact sheet is still sound. Only its quoted snapshot is wrong, so the fix is to replace it with a pointer to the live file.

The ledger has a second, more urgent problem. It hasn't gained a row since September 19, and three of its ten predictions (Altman, Amodei, Musk) name the end of 2026. They resolve in five weeks. Scoring them in January would be worth more than almost anything else in the library.

**Two attribution fact sheets have been overtaken by newer evidence.** The CyberAv3ngers fact sheet calls the attribution "a live, unresolved dispute." For the US water-utility campaign it no longer is. On September 7 the State Department named the IRGC Cyber-Electronic Command leader, Amir Yaryab, and posted a $10 million reward, which makes this a Tier 1 government attribution. A new dispute has opened on a second campaign. On November 10 France attributed sabotage of refrigeration controllers at about 700 retail sites to the same IRGC unit, but US intelligence reportedly holds that link at only low confidence, so it stays Tier 2. *(Corrected 2026-11-25 during the update pass: the first version of this report said the dispute was over without separating the two campaigns.)* The sheet's TTP mapping still stands, but its attribution section needs rewriting.

The Tool vs. Campaign vs. Actor fact sheet's worked example counts eight ARTEX-linked campaigns, four of them with a named operator. Since November 12 the Adversary Tracking Report has added three more ARTEX-linked rows, all unattributed:

- an AI vendor's never-retired cloud key (November 16)
- CERT-EU's European Commission outage (November 20)
- the breach of a CIA/ODNI open-source system (today)

That moves the named-operator share from 50% to about 36% (4 of 11). That is already at the 35% median the originating report forecast for the coming year. This is early, small-sample support for that forecast, not a confirmation of it, but the worked example should say so.

**One sheet needs a light check.** The Broken Windows fact sheet labels its 2025 NYC figures preliminary. Confirm them against NYPD's final year-end numbers before Rick's Gladwell reviews cite them.

Three "keep" items have a known expiry worth noting now:

- **TPCRM baseline, its infographic and the infographic's source file:** re-verify when the 2027 DBIR lands, expected in spring 2027.
- **CIR Coverage Baseline:** next used at the Cybersecurity Dive trial review on December 7.
- **Who's Who roster:** carries its own weeks-not-months shelf-life warning.

Pending PR #74 (the Bloomberg Nvidia graphic) isn't in the library yet, so it isn't part of this review.

## Clarifying Questions

None asked. The question is well-scoped: three named outcomes, one library. Assumptions logged:

1. "Each file" means each catalogued artifact (the 44 rows in `INDEX.md`). The repo's infrastructure files (`README.md`, `INDEX.md`, the PR template and the `.gitkeep` placeholders) are covered in one line rather than individually.
2. This is a recommendation only. Nothing is deleted or changed until Rick decides, and each change would go through its own pull request.
3. Open PR #74 (Bloomberg Nvidia graphic, opened today) is out of scope because it isn't merged.

## Alexandria (Opening): What Do We Already Know?

The library holds 44 catalogued artifacts. The `INDEX.md` row count matches the file tree exactly, so there are no orphan files and no rows without files.

| Category | Count |
|---|---|
| Fact sheets | 24, of which 20 are Markdown and 4 are images filed under `fact-sheets/` |
| Images | 15 |
| Other | 4: one spreadsheet, one PDF and two HTML render sources |
| Book reviews | 1 |
| Essays | 0, so the `essays/` folder is still empty |

The library has had 74 pull requests since July. Its most active items are the Who's Who roster (refreshed 2026-11-23) and the AI Timeline Forecasting chart (six refreshes since 2026-10-23).

No prior Nexus report has audited the library as a whole. The closest precedent is the per-artifact shelf-life warnings that several fact sheets carry in their own text (Who's Who, Named AGI Predictions, US AI Legislation, TPCRM). This review uses those warnings as its first checklist.

## Sherlock: What Are the Facts?

Each time-sensitive artifact was checked against the current standing files and the published report archive (112 reports since 2026-09-19).

- **Current forecast ranges:** from today's daily report.
  - AGI: 2029 / 2045 / 2075
  - Singularity: 2031 / 2046 / 2075
  - Superintelligence: 2030 / 2046 / 2076
  - P(Doom) When: 2034 / 2063 / 2091
  - Harm Probability: 15% / 30% / 55%

  `images/ai-timeline-forecasting.png` matches all five, so it is current.
- **Named AGI Predictions ledger:** it still states the AGI Forecast Report's range as "P5 2028 · P50 2036 · P95 2100." A search of every report after 2026-09-19 found no new dated AGI statement from Altman, Amodei, Musk, Hassabis, Kaplan, Gomez or Mensch. So the ledger isn't missing rows that Nexus captured elsewhere. Nobody has looked since September.
- **AGI vs. Singularity fact sheet:** it quotes the Singularity forecast as "P5 2027 · P50 2042 · P95 2100 as of 2026-09-18." That is out of date.
- **US AI Legislation fact sheet:** no Nexus report since 2026-10-08 mentions any of its eight bills. Its status column is a month and a half old, and it spans the midterms.
- **CyberAv3ngers fact sheet:** it says the attribution is "unresolved." Today's Adversary Tracking Report (row 7) shows the 09-07 State Department naming of Amir Yaryab with a $10M reward, plus the 11-10 French attribution to the IRGC for the ~700-site refrigeration sabotage.
- **Tool vs. Campaign vs. Actor worked example:** it lists 8 campaigns as of 2026-11-12. Three ARTEX rows first appear in the tracker after that date: 2026-11-16 (the never-retired cloud key), 2026-11-20 (CERT-EU, European Commission) and 2026-11-25 (CIA/ODNI system). All three are unattributed.
- **Broken Windows fact sheet:** it reads "Re-verify the 2025 figures once final NYPD year-end data is published."
- **Nexus Backup field guide:** the `nexus-backup` skill hasn't been modified since 2026-10-29, the date the guide was written. The guide is current.
- **Omar Sangurima review:** the original LinkedIn URL is still missing (`source_url: "n/a ... original post URL not yet provided"`).
- **Democratic candidates chart:** it still has no source URL or publication date.
- **Da Vinci of Data style reference:** `Agent Tufte Concept.md` still lists it as a mandatory style reference, so it's still in use.
- **D&D alignment chart:** it was used in `reports/2026-08-05-odysseus-dnd-alignment-check.md`, so it's still the book-review reference.

## Ryan: What Does the Adversary Playbook Look Like Here?

Two artifacts are adversary-specific, and both are behind the tracker.

1. **CyberAv3ngers.** The water-utility campaign is now a named-leader, Tier 1 government attribution. The French refrigeration wave is government-attributed (France) but contested (US intelligence holds it at low confidence, per the NYT), so it is Tier 2.
   - The vendor-assigned group name (CyberAv3ngers) and the sponsor (IRGC Cyber-Electronic Command) are now joined by an official US government finding. A second government (France) attributes a second campaign to the same unit, but an allied intelligence service doubts it.
   - Keep the technique section. The opportunistic exploitation of internet-exposed Unitronics/Schneider PLCs is unchanged.
   - Rewrite the attribution section. Its "how to write about contested attribution" lesson should become a before-and-after case of a disputed attribution that later got confirmed. That is more useful for teaching than the original.
2. **ARTEX worked example.** Keep tool, campaign, actor and sponsor as four separate labels exactly as the sheet says. Its own rule held up across all three new rows: none was linked to an operator through the tool alone. The count and the named share need refreshing, not the method.

No other artifact touches adversary characterization.

## Euclid: What Must Be Fundamentally True?

An artifact earns its place in a library if a future question will need it and it would cost more to rebuild than to maintain. That gives three tests.

1. **Durable method or primary record.** Keep it indefinitely, because it doesn't age. This covers the attribution frameworks, the Tufte material, the Emacs record, Rick's book graphics, the RSI bill draft, the licensing checklist and the Floor-not-Shield diagnostic.
2. **Dated snapshot.** Keep it only if no newer artifact carries its information. The Oct-3 forecast chart fails this test. The AI Achievements timeline (April 2024 to October 2026) passes, because nothing else holds that dual-track view. It should stay a closed, dated snapshot rather than be extended.
3. **Living reference.** It must match current reality or it is a hazard, because it will be cited as current. All eight updates fall here. The worst cases are the ones that print a retired Nexus forecast as "standing," since a reader can't tell they are stale without opening the forecast files.

By these tests, none of the third-party works qualify for deletion. They are private reference copies, explicitly barred from the public mirror and cheap to keep.

## Popper: How Could We Be Wrong?

1. **Rick deliberately archived the Oct-3 snapshot as a historical record.** Deleting it overrides a choice he made a month ago.
2. **"Find an updated document" may be the wrong verb for the forecast-citing sheets.** Some quote a range as an example of the merging error that was caught, not as a live figure. Removing the number would destroy the lesson.
3. **The ARTEX trend is three rows.** Calling it support for the 35% forecast reads a pattern into noise.
4. **The 2026-12-07 date may slip.** Calling the CIR baseline "keep" assumes that review actually happens.

## Seldon: What Is Likely to Happen Next?

Each objection, resolved:

1. **Oct-3 snapshot: the recommendation stands, but it's flagged as Rick's call and low-stakes.** The current chart is a faithful recreation of the same design. Its `INDEX.md` row and the five Evidence Logs record every move since October 3. So the snapshot's historical value is already preserved twice. If Rick wants to keep it anyway, the cost of being wrong is about 1.1 MB of storage.
2. **Forecast-citing sheets: partly accepted.** In the AGI vs. Singularity sheet, the 2028/2036/2100 triple is the merging-error example and must stay. Only the separate "standing Singularity range" line (2027/2042/2100) is a live claim, and that is what gets replaced with a pointer to the live file. The Named AGI ledger's "How this has been used" paragraph is a historical record of a 09-19 decision. Keep it, but date-stamp the range as "at the time," and add a current pointer.
3. **ARTEX: accepted.** The write-up calls it early, small-sample support, not confirmation. The update is still warranted, because the count itself is a fact that changed.
4. **The December 7 review: accepted as a dependency.** If the review slips, the baseline doesn't go stale. It just waits.

What happens next if nothing is done:

- The legislation sheet becomes outright wrong on January 3, 2027, when every bill in it dies with the 119th Congress.
- The three end-of-2026 AGI predictions expire unscored on January 1.
- TPCRM ages out around spring 2027, when the next DBIR replaces its headline figure.

These are judgments about the calendar, not modeled forecasts, so no probability range is offered.

## Tufte: How Do We Make This Clear?

A per-file decision table is the right tool here, since every row has the same columns and nothing depends on layout or flow. So there is no diagram this time. The table groups rows by verdict so the 9 delete-or-update actions read first, and the keeps follow by category.

### Delete (1)

| Artifact | Why |
|---|---|
| `images/ai-timeline-forecasting-summary.png` (Oct-3 snapshot) | Every date panel is superseded. `images/ai-timeline-forecasting.png` recreates the same design with current figures, and the Evidence Logs hold the history. |

### Find an Updated Version (8)

| # | Artifact | What's out of date | Suggested update | Urgency |
|---|---|---|---|---|
| 1 | `fact-sheets/us-federal-ai-legislation-landscape-119th-congress.md` | Status column "as of Oct. 2026"; the midterm deadline it cites has passed | Lame-duck status pass now; freeze as a historical record on Jan. 3, 2027; start a 120th Congress tracker | High |
| 2 | `images/where-congress-ai-bills-sit.png` | Depends on #1; public copy at go/29 | Re-render after #1, then offer a public re-sync | High (with #1) |
| 3 | `fact-sheets/named-agi-predictions-frontier-ai-leaders.md` | No rows added since 09-19; cites the retired AGI range; 3 predictions resolve Dec. 31 | Fresh sweep of roster statements now; score Altman, Amodei and Musk in January | High |
| 4 | `images/agi-ceo-predictions-timeline.png` | Reference band shows retired range 2028/2036/2100 (current 2029/2045/2075) | Re-render after #3 | Medium |
| 5 | `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` | Quotes the 09-18 Singularity range as standing | Replace that one line with a pointer to the live file; keep the merging-error example as is | Medium |
| 6 | `fact-sheets/cyberavengers-iran-plc-exploitation-ttp.md` | Calls the attribution "unresolved"; predates the Yaryab naming, the $10M reward and the French attribution | Rewrite the attribution section; keep the ATT&CK mapping | Medium |
| 7 | `fact-sheets/tool-vs-campaign-vs-actor-agentic-intrusions.md` | Worked example frozen at 8 campaigns, 50% named; now 11 and about 36% | Refresh the count and add the 3 new rows | Low to medium |
| 8 | `fact-sheets/broken-windows-stop-and-frisk-evidence.md` | 2025 NYC figures marked preliminary | Confirm against final NYPD year-end data | Low (unless a Gladwell review is imminent) |

### Keep (35)

**Methodology and frameworks (keep indefinitely):**

| Artifact | Note |
|---|---|
| `fact-sheets/evidence-tier-framework.md` | Core convention, used in every Ryan tag |
| `fact-sheets/campaign-vs-actor-attribution.md` | Standing Popper check |
| `fact-sheets/state-proxy-independent-wartime-cyber-attribution.md` | Standing Popper check |
| `fact-sheets/b2c-reach-b2b-revenue-soundness-test.md` | Reusable business-model test |
| `fact-sheets/emerging-technology-licensing-design-checklist.md` | Domain-agnostic |
| `fact-sheets/compliance-floor-not-shield-deterrence-diagnostic.md` | Proven across two domains |
| `fact-sheets/rsi-safety-act-draft-legislation.md` | Original drafted bill; doesn't age |

**Rick's own works and book material:**

| Artifact | Note |
|---|---|
| `fact-sheets/first-principles-infographic.png` | Book's core diagram |
| `fact-sheets/dnd-alignment-chart-framework.png` | Book-review reference (used 08-05) |
| `book-reviews/omar-sangurima-review-cybersecurity-first-principles.md` | Optional: add the original LinkedIn URL if Rick has it |

**Tufte and visual reference:**

| Artifact | Note |
|---|---|
| `fact-sheets/edward-tufte-visualization-principles.md` | Tufte's standing reference |
| `fact-sheets/edward-tufte-truthfulness-density-quadrant.png` | Companion |
| `fact-sheets/the-da-vinci-of-data-tufte-principles-by-antoine-buteau.png` | Still listed as a mandatory style reference in `Agent Tufte Concept.md`; private only |
| `images/social-funnel-wide-to-narrow.png` | Keynote diagram; timeless |

**Current, recently refreshed:**

| Artifact | Note |
|---|---|
| `fact-sheets/whos-who-in-frontier-ai.md` | Refreshed 11-23; weeks-long shelf life by its own warning |
| `images/whos-who-in-frontier-ai.png` | Refreshed 11-23; public copy in sync |
| `images/ai-timeline-forecasting.png` | Matches all five of today's ranges |
| `images/from-agi-to-the-singularity.png` | Definitions only; no figures to go stale |

**AI timeline and policy (dated snapshot, kept on purpose):**

| Artifact | Note |
|---|---|
| `images/ai-achievements-controversies-timeline.jpg` | Closed window, April 2024 to October 2026; don't extend |

**Operational:**

| Artifact | Note |
|---|---|
| `fact-sheets/nexus-backup-restore-field-guide.md` | Matches the unchanged 10-29 backup skill |
| `images/nexus-backup-restore-infographic.png` | Companion |
| `other/nexus-backup-restore-infographic-source.html` | Needed to re-render |
| `fact-sheets/nexus-cir-coverage-baseline-2026-11.md` | Next use 2026-12-07 |
| `other/home-maintenance-checklist.xlsx` | Family working copy |

**Topical fact sheets with a known re-check date:**

| Artifact | Note |
|---|---|
| `fact-sheets/tpcrm-2026-baseline-statistics.md` | Re-verify after the 2027 DBIR (spring 2027) |
| `images/tpcrm-exposure-vs-program.png` | Same |
| `other/tpcrm-exposure-vs-program-infographic-source.html` | Edit the numbers here when the DBIR lands |

**History and primary sources:**

| Artifact | Note |
|---|---|
| `fact-sheets/emacs-lore-1978-origin-record.md` | Primary record |
| `images/emacs-at-50-lineage.png` | Companion; public copy current |
| `fact-sheets/kim-zetter-countdown-to-zero-day-appearance-bibliography.md` | A floor, not a census; reusable for Canon/Stuxnet work |
| `other/kim-zetter-house-testimony-stuxnet-15-years-2025-07-22.pdf` | Copy held against link rot |

**Third-party reference copies (private only, never the public mirror):**

| Artifact | Note |
|---|---|
| `images/democratic-presidential-candidates.png` | Optional: locate the original NYT/Silver URL and date |
| `images/cybersecurity-vendor-platform-breadth.jpg` | Added 11-24; tied to the CrowdStrike–Zscaler deal |
| `images/9-ai-concepts-ai-architecture-explainer.gif` | Added 11-24 |
| `images/what-is-an-ai-harness.gif` | Added 11-24 |

**Repo infrastructure** (`README.md`, `INDEX.md`, `.github/PULL_REQUEST_TEMPLATE.md`, and the `.gitkeep` placeholders) is keep. One housekeeping note: the `INDEX.md` row for the AI Timeline Forecasting chart has grown into a roughly 4,000-character changelog. The forecast files' Evidence Logs already hold that history. Trimming it to the current figures plus a one-line pointer would make the index readable again. That would be its own small PR, done with the read-whole-file, check-row-count discipline.

## Turing: Should Any of This Become a Skill?

**Update, 2026-11-25:** at Rick's direction, this method is now the `nexus-library-audit` skill, run quarterly. The original assessment follows. No skill built. A library audit is plausibly recurring (quarterly, say), but this is the first one. The useful part of the method was:

- reading each artifact's own shelf-life warning;
- diffing quoted forecast ranges against the live files;
- diffing worked examples against the Adversary Tracking Report.

That method is written down in this report. If Rick wants this on a schedule, the next run is the right time to turn it into a `nexus-library-audit` skill, using this report as the template.

## Sources

**Internal: library (`raceBannon99/nexus-artifacts`, private)**
- `INDEX.md` (44 rows) and the full file tree, read 2026-11-25. These are the inventory.
- Each Markdown fact sheet listed above, read in full or at its dated claims. These are the staleness evidence quoted in Sherlock's section.
- The commit history (74 PRs since July). This gives the refresh dates.

**Internal: standing state (vault)**
- `Intelligence Reports/Adversary Tracking Report.md`, as published at `reports/2026-11-25-adversary-tracking-report.md`. It supplies the CyberAv3ngers row 7 attribution history and the ARTEX row count.
- `reports/2026-11-16-adversary-tracking-report.md`, `reports/2026-11-20-adversary-tracking-report.md` and `reports/2026-11-25-adversary-tracking-report.md`. These are the first appearances of the three post-11-12 ARTEX rows.
- `Nexus Agents/Agent Tufte/Agent Tufte Concept.md`. It shows the Buteau style reference is still listed as mandatory.
- `.claude/skills/nexus-backup/SKILL.md`, last modified 2026-10-29. It shows the backup guide is current.

**Internal: reports (`raceBannon99/The-Nexus`)**
- [2026-11-25 Daily Intelligence Report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-25-daily-intelligence-report.md). It has today's five forecast ranges.
- [2026-10-08 AI kill-switch / AGI / superintelligence legislation](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-10-08-ai-kill-switch-agi-superintelligence-legislation.md). It is the last report covering the eight bills.
- [2026-09-19 AGI CEO predictions](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-09-19-agi-ceo-predictions.md). It is the source of the Named AGI ledger. A sweep of the 112 reports since then found no new dated leader statements.
- [2026-11-12 ARTEX agentic pentesting attribution](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-12-artex-agentic-pentesting-attribution.md). It is the source of the 35% named-operator forecast.
- [2026-08-05 Odysseus D&D alignment check](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-08-05-odysseus-dnd-alignment-check.md). It shows the alignment chart in use.

**External (via the tracker's own citations)**
- US State Department Rewards for Justice posting on Amir Yaryab (09-04/09-07) and France's Cyber Crisis Coordination Centre attribution (11-10), both as cited in tracker row 7. Uncited here beyond the tracker's own links.

## New Skills

**`nexus-library-audit`** (built 2026-11-25 at Rick's direction, after publication). Quarterly audit of the private artifact library. It classifies every `INDEX.md` row as delete, update, or keep using this report's three tests (durable method, dated snapshot, living reference) and its staleness checks: shelf-life warnings, quoted forecast ranges against the live files, worked examples against the Adversary Tracking Report, and calendar-dated items. It publishes a review report, then opens grouped PRs only on Rick's approval. This report is its first worked example.

## Library Recommendations

Nothing new is recommended for archiving. This engagement's recommendations concern existing artifacts:

| Candidate | Category | Action | Status |
|---|---|---|---|
| `images/ai-timeline-forecasting-summary.png` | image | Delete (superseded) | Removed ([PR #80](https://github.com/raceBannon99/nexus-artifacts/pull/80), merged 2026-11-25) |
| `INDEX.md` AI Timeline row | index | Trim the changelog to current figures plus a pointer | Updated ([PR #80](https://github.com/raceBannon99/nexus-artifacts/pull/80), merged 2026-11-25) |
| AGI ledger, AGI timeline image, AGI vs. Singularity fact sheet | fact-sheet / image | Refresh | Updated ([PR #75](https://github.com/raceBannon99/nexus-artifacts/pull/75), merged 2026-11-25) |
| AI legislation fact sheet and spectrum diagram | fact-sheet / image | Lame-duck refresh; freeze Jan. 3, 2027 | Updated ([PR #76](https://github.com/raceBannon99/nexus-artifacts/pull/76)), merged 2026-11-25; public copy (go/29) is stale, re-sync offered to Rick |
| CyberAv3ngers fact sheet | fact-sheet | Rewrite attribution section | Updated ([PR #77](https://github.com/raceBannon99/nexus-artifacts/pull/77), merged 2026-11-25) |
| Tool vs. Campaign vs. Actor fact sheet | fact-sheet | Extend ARTEX worked example | Updated ([PR #78](https://github.com/raceBannon99/nexus-artifacts/pull/78), merged 2026-11-25) |
| Broken Windows fact sheet | fact-sheet | Confirm 2025 NYPD figures | Updated ([PR #79](https://github.com/raceBannon99/nexus-artifacts/pull/79), merged 2026-11-25) |

All approved by Rick on 2026-11-25. The changes were grouped into six PRs whose `INDEX.md` edits don't touch neighboring rows, and a local test merge confirmed that all of them, plus #74, merge cleanly in any order.

Pending approvals: 1 open PR, [#74 Add image: How Nvidia and OpenAI Fuel the AI Money Machine (Bloomberg)](https://github.com/raceBannon99/nexus-artifacts/pull/74).
