# What Frontier AI's Leaders Say About When AGI Arrives

**Question:** Using the "Who's Who in Frontier AI" diagram from the artifacts library (`images/whos-who-in-frontier-ai.png`), which lists thought leaders and CEOs for each of 16 frontier AI companies — find out whether they have made a prediction for when the AI industry will reach the AGI milestone, and build a range of predictions from the answers.

Among the roughly 45 named individuals on that roster, only about a dozen have made a specific, attributable public statement about when AGI arrives — and they disagree by more than a decade. The most aggressive predictions (OpenAI's Sam Altman, Anthropic's Dario Amodei, xAI's Elon Musk, Moonshot AI's Yang Zhilin) cluster around 2026–2027. A more measured group (Google DeepMind's Demis Hassabis, Anthropic co-founder Jared Kaplan) points to around 2030. A third group — Mistral's Arthur Mensch, Cohere's Aidan Gomez, and Baidu's Robin Li — either declines to name a date, rejects the premise that AGI is a discrete moment at all, or places arrival more than ten years out. Treating these statements as one informal sample, the center of gravity sits somewhere around 2029–2030 — years earlier than the 2036 median in Nexus's own standing, externally-anchored AGI Forecast Report.

That gap is not a reason to move the standing forecast. Every aggressive date in this sample comes from a leader whose company's valuation, hiring, and fundraising benefit directly from AGI feeling close; every skeptical or refusing voice comes from a leader with comparatively less commercial upside in claiming one, and each explicitly criticizes the framing on those grounds. This is exactly the kind of source bias Nexus's standing forecast already discounts by anchoring to forecasting-market and expert-survey data rather than company statements. What this survey adds is corroboration of *why* that anchoring choice matters, not a reason to abandon it — and one genuinely new fact for the standing file's own record: a Chinese lab CEO (Yang Zhilin) has now joined the aggressive-timeline camp publicly, a data point that previously skewed entirely toward US labs in Nexus's evidence base.

Two structural findings matter as much as the dates themselves. First, most of the roster — including nearly every named "thought leader" who isn't also a CEO or co-founder, and every leader at the smaller regional labs (TII/G42, Naver, Sakana AI, AI21 Labs, Zhipu AI, Alibaba's Qwen team) — has made no public, dated AGI prediction at all; silence dominates the sample, not disagreement. Second, several widely-repeated "AGI predictions" attributed to roster members are not actually AGI predictions once checked against Nexus's own definitional standard: Alexandr Wang's "five-year horizon" is a superintelligence claim, a higher and later bar than AGI by Nexus's own methodology, and several secondary sources conflate the two. Sorting predictions by which milestone they actually name, not just which word appears near a date, changes the shape of the range presented below.

## Clarifying Questions

The question was well-scoped enough to proceed without stopping to ask Rick anything, with one assumption logged rather than left implicit: **"the AGI milestone" reuses the definition already standing in `Intelligence Reports/AGI Forecast Report.md`** — a machine matching or exceeding broad human performance across essentially every intellectual domain — for consistency with existing Nexus methodology, rather than accepting each individual's own (often different) operational definition of "AGI" at face value. Where a roster member's own definition differs materially from this standard (several do), that difference is noted rather than silently normalized away. A second, related judgment call: "prediction" means a dated, publicly attributable statement — an interview, essay, testimony, or investor briefing with direct quotes or credible paraphrase — not an inferred position, a rumor, or a company mission statement ("we aim to build AGI") with no date attached.

## What Do We Already Know? (Alexandria — Opening)

A search of the artifact library and a full-text search of prior `raceBannon99/The-Nexus` reports (`.claude/scripts/nexus-search-reports.sh`, terms "AGI prediction," "AGI timeline," "when AGI") turned up no prior report compiling named individuals' AGI-timeline predictions — this is a genuinely new angle on existing material, not a duplicate.

Two things in the library are directly relevant and were used, not duplicated:

- **`fact-sheets/whos-who-in-frontier-ai.md`** and its companion roster graphic (`images/whos-who-in-frontier-ai.png`), both added 2026-08-31, are the source of the roster itself — 16 companies, their CEOs, and their named thought leaders. The fact-sheet carries its own explicit shelf-life warning (Popper P2: "org-chart facts in this sector go stale within months; verify before reciting") — which turned out to be justified twice over during this engagement's own research (see Popper's section below).
- **`Intelligence Reports/AGI Forecast Report.md`**, created 2026-09-18, already carries a live, externally-anchored P5/P50/P95 range for AGI arrival (currently **P5 2028 · P50 2036 · P95 2100**). This report's forecast section below compares the roster's own statements against that standing range directly, and considers whether they justify a change to it.
- **`fact-sheets/agi-vs-singularity-forecasting-thresholds.md`** (nexus-artifacts, PR #17) supplies the standing discipline against conflating AGI, superintelligence, and the Singularity — applied directly to sort several of the roster's public statements by which milestone they actually name.

## The Facts (Sherlock)

Research proceeded company by company through the full roster (16 companies, 16 CEOs, ~30 named thought leaders). Predictions below are reported with the milestone each statement actually names, per the definitional discipline in the Clarifying Questions section — several widely-repeated paraphrases blur "AGI," "superintelligence," and "powerful AI" together, and that blurring is flagged, not repeated, wherever it appears in the sourcing.

**OpenAI (United States) — CEO Sam Altman; thought leaders Mark Chen, Noam Brown, Richard Ho.** Altman has said he expects OpenAI to have an internal system he would personally call AGI by the end of 2026 — by his own, company-specific definition of the term, which OpenAI's own materials frame around highly autonomous systems outperforming humans at economically valuable work. Prediction markets give this specific claim only 9–15% odds as of this reporting. Chief Research Officer Mark Chen has separately said OpenAI is "roughly 80 percent of the way" to AGI — a magnitude claim, not a date. Noam Brown, when asked directly about a 2030 prediction, said "I don't know what the world looks like in 2030. That's the truth" — an explicit refusal to forecast — but noted OpenAI's own internal objective of a fully autonomous AI researcher by March 2028, a narrower, dated capability target distinct from full AGI. No public AGI-timeline statement was found from Richard Ho.

**Anthropic (United States) — CEO Dario Amodei; thought leaders Chris Olah, Sam McCandlish, Jared Kaplan.** Amodei has said "powerful AI" at a Nobel-laureate capability level could arrive "as soon as late 2026 or early 2027, though there are also ways it could take much longer" — a hedged near-term claim, not a firm commitment. Co-founder and chief scientist Jared Kaplan, in a December 2025 interview, framed 2027–2030 as the window in which humanity must decide whether to let AI systems train themselves, with human-level AI plausible by 2030 in his framing; he separately estimated a 50% chance theoretical physicists are "mostly replaced" by AI within two to three years, a narrower domain-specific claim. No public AGI-timeline statement was found from Chris Olah or Sam McCandlish.

**Google DeepMind (United States) — no standalone CEO since August 2026; thought leaders Jeff Dean, Oriol Vinyals, Demis Hassabis.** Demis Hassabis (DeepMind's CEO through the August 2026 restructuring, and still the lab's most publicly attributed voice on this question) has repeatedly placed AGI "only a few years away... maybe 2030, plus or minus a year" — though secondary sources report this inconsistently, with some paraphrasing it as a 2030–2035 window and others as "three to ten years" from a 2026 reading; the inconsistency across secondary sources is itself worth flagging rather than picking one figure and presenting false precision. **Jeff Dean and Oriol Vinyals both left Google in August 2026** to co-found a new venture ("Discovery Loop," alongside Sanjay Ghemawat and Quoc Le) — a material org-chart change post-dating the roster diagram's own August 2026 publication date, and a direct, fast-turnaround illustration of the fact-sheet's own shelf-life warning. No public AGI-timeline statement was found from either.

**Meta Superintelligence Labs (United States) — Chief AI Officer Alexandr Wang; thought leader Shengjia Zhao.** Wang told the India AI Impact Summit (March 2026) that superintelligence sits on a roughly five-year horizon — **a superintelligence claim, not an AGI claim**, and therefore a later, higher bar than this report's target question by Nexus's own standing definitional split (see `fact-sheets/agi-vs-singularity-forecasting-thresholds.md`). No AGI-specific dated statement from Wang was found in this research pass, and none was found from Shengjia Zhao.

**xAI / SpaceXAI (United States) — Chairman Elon Musk; thought leaders Jimmy Ba, Tony Wu.** Musk has made multiple, escalating and partially expired claims: an earlier prediction (superseded) of AI "smarter than the smartest human" within one to two years; a live claim that xAI will have AI "smarter than any one human" by the end of 2026; and a claim that AI could exceed all of humanity combined by roughly 2030–2031 — the last of these again closer to a superintelligence framing than a strict AGI-arrival claim. No statement was found from Jimmy Ba or Tony Wu.

**DeepSeek (China) — CEO Liang Wenfeng; thought leaders Daya Guo, Damai Dai, Chenggang Zhao.** In a closed-door investor briefing (May 20, 2026, later leaked and widely reported, not independently confirmed by Liang), Liang described a staged AGI roadmap — general agents, then continuous learning, then AI self-iteration and embodied intelligence — without committing to specific years for any stage. This is a real, substantive AGI-strategy statement but explicitly not a dated prediction, and is reported here as such rather than forced into a year. No statement was found from the other three named DeepSeek researchers.

**Alibaba · Qwen (China) — CEO Eddie Wu; thought leader Zhou Jingren.** No public, dated AGI-timeline statement was found from either in this research pass.

**Moonshot AI (China) — CEO Yang Zhilin; thought leaders Zhou Xinyu, Wu Yuxin.** A third-party prediction-tracking database (theagiclock.com, itself not independently verified against Yang's own original words in this pass) lists a 2026–2027 AGI-arrival prediction attributed to Yang, dated July 2026, at high credibility. This is reported here as **aggregator-sourced, not primary-verified** — a real data point, but one carrying weaker sourcing confidence than the direct-quote statements above from Altman, Amodei, Kaplan, and Musk, and flagged as such rather than presented with equal confidence. No statement was found from the other two named Moonshot researchers.

**Zhipu AI · Z.ai (China) — CEO Zhang Peng; thought leaders Tang Jie, Li Juanzi.** No public, dated AGI-timeline statement was found from any of the three in this research pass.

**Baidu (China) — CEO Robin Li; thought leader Wang Haifeng.** Li said in May 2024 that AGI is "more than 10 years away," arguing current models remain far from human-level intelligence and that the path to it isn't yet understood. In a more recent January 2026 interview, Li said "I don't think about AGI a lot," framing Baidu's own model work around solving concrete application problems rather than pursuing AGI as a goal — a deprioritization of the question, not a reversal of the 10-plus-year estimate. No statement was found from Wang Haifeng.

**Mistral AI (France) — CEO Arthur Mensch; thought leaders Timothée Lacroix, Guillaume Lample.** Mensch has explicitly declined to forecast a date, calling the pursuit of AGI itself "a marketing move" and criticizing the broader industry's "AGI rhetoric" as "about creating God" — a rejection of the framing, not merely an absence of a number. No statement was found from Lacroix or Lample.

**Cohere + Aleph Alpha (Canada / Germany) — CEO Aidan Gomez; thought leaders Phil Blunsom, Joëlle Pineau, Nick Frosst.** Gomez rejects AGI as a discrete, binary event ("It's not a binary. It's not discrete; it's continuous. We're already quite far along that road") and has said "we already have AGI to a large extent" — but separately projects that within five years, AI will be able to "automate any human task that we decide we don't want to do," a dated capability claim (roughly 2030–2031) that functions as a de facto AGI-adjacent estimate even though Gomez himself resists calling it that. No statement was found from Blunsom, Pineau, or Frosst.

**TII (Falcon) / G42 (United Arab Emirates) — CEOs Najwa Aaraj (TII) and Peng Xiao (G42); thought leader Ebtesam Almazrouei.** No public, dated AGI-timeline statement was found from any of the three in this research pass.

**Naver (South Korea) — CEO Choi Soo-yeon; thought leader Nako Sung.** No public, dated AGI-timeline statement was found from either in this research pass.

**Sakana AI (Japan) — CEO David Ha; thought leader Llion Jones.** No public, dated AGI-timeline statement was found from either in this research pass.

**AI21 Labs (Israel) — Co-CEOs Ori Goshen and Yoav Shoham; thought leader Amnon Shashua.** No public, dated AGI-timeline statement was found from any of the three in this research pass.

**Summary count:** of 16 CEOs (counting co-CEOs and dual leadership as one company-level entry each), 9 have a findable public statement bearing on AGI timing (Altman, Amodei, Hassabis as DeepMind's de facto voice, Wang, Musk, Liang, Robin Li, Yang Zhilin, Mensch, Gomez — note this is 10 names against 9 company slots, since DeepMind's CEO seat is vacant and Hassabis fills the role informally); of roughly 30 named thought leaders, only 2 (Mark Chen, Noam Brown at OpenAI) and one Anthropic co-founder acting in a thought-leader-adjacent capacity (Jared Kaplan) produced anything usable, and none of the thought leaders at any of the eight non-US, non-French, non-Canadian/German companies (all of China, UAE, South Korea, Japan, Israel) had a findable statement in this pass.

## Adversary Playbook Assessment (Ryan)

This question carries no adversary, campaign, or attribution angle — it's a survey of public statements by named industry figures, not an incident, intrusion, or influence operation. No entry is warranted in `Intelligence Reports/Adversary Tracking Report.md`, and this section is included only to confirm that check was made rather than skipped.

## First Principles Analysis (Euclid)

Strip away the branding and the roster collapses to one structural fact: **every dated AGI prediction in the sample comes from someone with a direct commercial or reputational stake in AGI arriving soon, and every skeptical or absent voice comes from someone without that stake or with a stake in the opposite framing.** Altman, Amodei, Musk, Wang, and Yang Zhilin all lead labs actively fundraising, recruiting, or selling enterprise contracts on the strength of imminent transformative capability — their forecasts are also, unavoidably, sales collateral. Mensch (explicitly rejecting the AGI framing as "a marketing move") and Robin Li (explicitly deprioritizing the question) both lead labs whose commercial pitch rests on shipping useful, bounded products rather than a civilization-scale narrative — their skepticism is also, unavoidably, a different sales pitch. Gomez sits in between, denying AGI is a coherent discrete event while still offering his own five-year capability estimate. None of this makes any individual prediction dishonest, but it means the roster's spread of dates is at least partly a spread of business models, not purely a spread of technical judgment — and the two are entangled in a way no amount of additional interviews will fully untangle.

A second structural point: the roster's own predictions don't share a referent. When Altman, Amodei, and Hassabis name a year, they are each naming the year *their own lab's internal capability bar* gets cleared — bars that are not published in comparable form and are not obligated to match each other, Nexus's, or any academic definition. Liang's staged roadmap and Wang's five-year superintelligence estimate aren't dates for the same milestone as the others at all — one is an unstamped process, the other is a materially higher bar. Treating all of these as points on one number line, as most secondary aggregation (including the aggregator database used for Yang's data point above) implicitly does, manufactures a false precision the underlying statements don't support. Any range built from this sample has to be read as a range of *when different people expect to clear their own goalposts*, not a range of predictions about one shared event — which is itself informative (it shows the industry has not converged on what it's even racing toward) but is a different, humbler claim than "the industry thinks AGI arrives between X and Y."

## Devil's Advocate (Popper)

Six objections, in descending order of how much they should discount the resulting range:

1. **Self-interest bias is not a minor caveat, it may be the whole signal.** Every near-term (2026–2028) prediction in the sample comes from a lab CEO currently raising capital or defending a valuation against the claim that transformative capability is close. There is no independent, disinterested voice in the entire dataset predicting an early date — the only two people offering later or non-committal answers (Mensch, Robin Li, and Brown's explicit refusal) all lead or work at organizations with less to gain from an "AGI is imminent" narrative. A range built mostly from interested parties is not a neutral estimate; it may simply be reproducing the industry's fundraising calendar.
2. **The sample is small, non-random, and English/US-skewed.** 9 of 16 company-level leaders and 3 of ~30 named thought leaders produced usable data — and of those 9, six lead US or French/Canadian labs whose CEOs give frequent English-language press interviews; the entire Chinese, Gulf, Korean, Japanese, and Israeli cohorts (8 of 16 companies) are represented by at most three data points (Liang, Robin Li, Yang Zhilin), two of which are hedged or non-dated. A range drawn from this sample risks describing "what English-speaking, press-active US/French lab CEOs say," not "what the AI industry believes."
3. **Definitional inconsistency undermines comparability, as Euclid noted above** — Wang's estimate is for superintelligence, not AGI, by Nexus's own standing taxonomy, and including it in an "AGI predictions" range at all would be a category error; several others (Altman's OpenAI-internal bar, Hassabis's inconsistently-reported figure) may not share a common operational definition either, even though they're all nominally answering the same question.
4. **Sourcing confidence is uneven.** The Altman, Amodei, Kaplan, Musk, Mensch, Gomez, and Robin Li statements trace to direct quotes in named interviews or testimony. The Yang Zhilin data point traces to a third-party prediction-tracking aggregator not independently verified against his original words in this research pass, and the Liang Wenfeng data point traces to a leaked, not officially confirmed, investor briefing. Weighting all seven-plus-two data points equally would overstate confidence in the weaker two.
5. **The roster itself is decaying in real time**, which is a live demonstration of the underlying fact-sheet's own shelf-life warning, not a hypothetical risk: Jeff Dean and Oriol Vinyals — both named DeepMind thought leaders on the very diagram this engagement started from — left the company in August 2026, weeks after the Who's Who diagram was published. Anyone treating that diagram as a current org chart today would already be wrong about two of its named individuals' employers, and by extension about whose opinion counts as "Google DeepMind's" institutional view going forward (arguably now Hassabis's alone, by default rather than by design).
6. **Silence is not evidence of a later date, and the report should resist reading it that way.** Roughly 33 of the ~45 roster names — including all thought leaders outside OpenAI and Anthropic — produced no dated public prediction in this pass. That is very likely a research-coverage limit (non-English sources, non-press-active roles, statements buried in venues this pass didn't check) rather than a considered position of "no opinion" or "later than the sample." The forecast below is built only from the ~10 people who spoke, and should not be read as representing the other ~35.

Each of these is addressed explicitly, not just logged, in Seldon's forecast below.

## Forecast (Seldon)

**This survey's own raw statements, read naively, span roughly the end of 2026 to the mid-2030s, with a naive center of gravity around 2029–2030 — but that naive reading should not move Nexus's standing AGI forecast, and the standing range in `AGI Forecast Report.md` (P5 2028, P50 2036, P95 2100) stands unchanged.** Working through Popper's six objections in order:

On self-interest bias (objection 1) — the single largest discount — this survey doesn't add new information so much as it explains, with unusual clarity, *why* the standing forecast was already anchored to forecasting markets and expert surveys rather than company statements in the first place. Four of the five earliest dates in this sample (Altman, Amodei, Musk, Yang Zhilin) come from CEOs whose fundraising and valuation benefit directly from an "AGI is imminent" narrative; treating their 2026–2027 cluster as a credible near-term signal, rather than as evidence of what the sector needs to say publicly right now, would double-count a bias the standing methodology already prices out. This is why the roster's aggressive cluster does not pull the range's P5 earlier than 2028.

On sample size and skew (objection 2), the ten usable data points are too few, too press-selected, and too US/French-weighted to function as an independent basket the way Metaculus, Samotsvety, and the AI Impacts survey do — each of those anchors aggregates hundreds to thousands of forecasters or expert respondents. This survey is evidence *about the industry's public messaging*, not a competing forecasting instrument, and is weighted accordingly: it corroborates or informs the standing range's qualitative picture without being allowed to move its quantitative one.

On definitional inconsistency (objection 3), Wang's five-year figure is excluded from this AGI range entirely, as a superintelligence claim under Nexus's own standing split — it belongs in `Superintelligence Forecast Report.md`'s own evidence base, not here (see that file's own evidence-log decision below). The remaining company-specific bars (Altman's OpenAI-internal threshold, Hassabis's inconsistently-reported figure) are read as loose corroboration of a general direction, not as precise data points on a shared scale.

On sourcing confidence (objection 4), the Yang Zhilin (aggregator-sourced) and Liang Wenfeng (leaked, unconfirmed) data points are weighted below the seven direct-quote statements, and neither is allowed, on its own, to shift a range built on far larger and more rigorously sourced external baskets.

On roster decay (objection 5) — the Dean/Vinyals departure — this bears on the reliability of the Who's Who roster as an org chart, not on the AGI-timeline question itself; it's noted here as a genuine finding (and a Turing/Alexandria consideration below) but has no forecasting weight.

On silence (objection 6), the ~33 non-responding roster members are treated as missing data, not as an implicit "no opinion" or "later" vote, and are excluded from the range rather than assumed into either tail.

**Net effect:** no change to `AGI Forecast Report.md`. The one genuinely new fact worth recording for that file's own future reference — not because it moves the range, but because it changes the shape of Nexus's evidence base — is that a Chinese lab CEO (Yang Zhilin) has now joined the aggressive-timeline camp on the record (albeit via aggregator sourcing), where Nexus's prior evidence for that file skewed entirely toward US voices; an Evidence Log entry recording "evidence noted, no change" has been appended to `AGI Forecast Report.md` accordingly, with the self-interest-bias reasoning above written into the chain so a future reader doesn't have to re-derive why a cluster of CEO statements didn't move an externally-anchored range.

Separately, and outside the scope of the AGI Forecast Report itself: Wang's superintelligence claim (~2031, per his "five-year horizon" stated March 2026) sits inside `Superintelligence Forecast Report.md`'s own P5 2029–P95 2100 range and does not conflict with or require a change to that file either — it's a single, self-interested, unconfirmed-methodology data point consistent with, not additive to, the existing floor-rule-and-transition-gap reasoning already documented there.

## Visualizing the Landscape (Tufte)

This is a genuine diagram, not a tabular fact — the question is fundamentally about *where each voice sits relative to the others and relative to Nexus's own range*, which spatial position on a timeline carries and a table's rows/columns can't. Built via the `epic-infographics` pipeline (`check.mjs` preflight — 0 errors, 1 expected `hero-weak` warning on a dense reference chart — then `render.mjs`, 1600px wide, tall preset), First Principles Consulting mark stamped bottom-left via a new `stamp_logo_left.py` (a mirrored variant of the existing bottom-right `stamp_logo.py`, saved for reuse since this diagram's own footer already fills both bottom corners with legend/note text and needs the canvas-extension approach rather than either stock corner):

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-09-19-agi-ceo-predictions/agi-ceo-predictions-timeline.png">

Three clusters (aggressive/moderate/skeptical) run along a shared 2026–2040 axis; hollow markers flag aggregator-sourced (not primary-verified) data; Robin Li's marker carries an arrow noting the underlying 2024 statement was "more than 10 years away" rather than a fixed year; Mensch appears as text only, since he offered no date to plot. Nexus's own AGI Forecast Report range runs beneath the roster as a shaded band (P5 2028–P50 2036) with a dashed tail to P95 2100, so the reader can see directly that the roster's aggressive cluster sits inside Nexus's own P5–P50 window rather than ahead of it — the disagreement is real but smaller than the "CEOs say 2026, Nexus says 2036" framing would suggest at a glance.

## New Skills (Turing)

One reusable fix, not a new skill: the `epic-infographics` plugin's `check.mjs`/`render.mjs` depend on a `playwright` package that isn't installed inside the plugin's own directory (`~/.claude/plugins/marketplaces/epic-infographics/...`), and running them there fails with `ERR_MODULE_NOT_FOUND` even though Node's ESM loader ignores `NODE_PATH` as a workaround. The project's own `.claude/skills/node_modules` already has `playwright` installed (from earlier skill setup) — the fix, applied here and worth remembering, is to copy `check.mjs`/`render.mjs` into `.claude/skills/epic-infographics-scripts/` (now saved in this vault) and run them from there, where Node's normal `node_modules` resolution finds the dependency without any path juggling. Future Tufte diagrams should invoke the scripts from that saved location rather than the plugin's own `scripts/` directory. This isn't substantial enough to warrant a standalone skill file, but it is the kind of one-time gotcha worth a paper trail so it isn't re-debugged from scratch next time.

## Numbers Check (Popper)

Every date cited in prose against the diagram and against original sourcing:

| Claim | Prose | Diagram | Consistent? |
|---|---|---|---|
| Altman | End of 2026 | 2026 marker | Yes |
| Amodei | Late 2026/early 2027 | 2026.5 marker | Yes |
| Musk | End of 2026 | 2026.5 marker | Yes |
| Yang Zhilin | 2026–2027, aggregator-sourced | 2026.5, hollow marker | Yes |
| Hassabis | ~2030 (2029–2031 reported range) | Range bar 2029–2031, dot at 2030 | Yes |
| Kaplan | 2027–2030 window, "plausible by 2030" | Range bar 2027–2030, dot at 2029 | Yes |
| Gomez | ~2030–2031 de facto | 2030.5 marker | Yes |
| Robin Li | "More than 10 years" from 2024 → 2034+ | 2034 marker with forward arrow | Yes |
| Mensch | No date | Text-only row, no marker | Yes |
| Wang | Excluded (superintelligence, not AGI) | Excluded, noted in footer | Yes |
| Nexus AGI Forecast Report | P5 2028 · P50 2036 · P95 2100 | Band 2028–2036, dashed tail to 2100 label | Yes |
| Superintelligence Forecast Report | P5 2029 · P50 2045 · P95 2100 | Not plotted (out of this diagram's scope) | Yes, cross-referenced correctly in prose |

No discrepancies found. The AGI Forecast Report's own range was not changed by this engagement — confirmed by re-reading the file after Seldon's edit, and the "Evidence noted, no change" language in the newly-added Evidence Log row matches the At-a-Glance line, which was correctly left untouched.

## Sources

**Primary quotes / interviews / testimony:**
- Sam Altman, various 2026 public remarks on OpenAI's internal AGI timeline and prediction-market odds.
- Mark Chen (OpenAI), public remarks on OpenAI's progress toward AGI ("roughly 80 percent of the way").
- Noam Brown (OpenAI), public remarks declining to forecast 2030 and citing OpenAI's internal autonomous-researcher target (March 2028).
- Dario Amodei (Anthropic), public remarks on "powerful AI" arriving "as soon as late 2026 or early 2027."
- Jared Kaplan (Anthropic), December 2025 interview on the 2027–2030 decision window and human-level AI by 2030.
- Demis Hassabis (Google DeepMind), multiple public remarks placing AGI "a few years away, maybe 2030."
- Alexandr Wang (Meta Superintelligence Labs), remarks at the India AI Impact Summit, March 2026, on a five-year superintelligence horizon.
- Elon Musk (xAI), multiple public statements (escalating/partially superseded) on AI exceeding human intelligence by end of 2026 and humanity combined by ~2030–2031.
- Liang Wenfeng (DeepSeek), closed-door investor briefing, May 20, 2026 (leaked, not independently confirmed), on a staged AGI roadmap.
- Robin Li (Baidu), May 2024 remarks ("more than 10 years away") and a January 2026 interview ("I don't think about AGI a lot").
- Arthur Mensch (Mistral AI), public remarks rejecting the AGI framing as "a marketing move" and "about creating God."
- Aidan Gomez (Cohere), public remarks rejecting AGI as a discrete/binary event and projecting broad task automation within five years.

**Aggregator / tracking sources (weighted lower per Popper's objection 4 above):**
- theagiclock.com — third-party AGI-prediction tracking database; source for the Yang Zhilin (Moonshot AI) 2026–2027 data point.

**Nexus internal standing files:**
- `Intelligence Reports/AGI Forecast Report.md` (P5 2028 · P50 2036 · P95 2100, unchanged by this engagement; Evidence Log entry added 2026-09-19).
- `Intelligence Reports/Superintelligence Forecast Report.md` (P5 2029 · P50 2045 · P95 2100, cross-referenced for Wang's superintelligence claim, unchanged).
- `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` (nexus-artifacts, PR #17) — definitional split applied to sort Wang's claim out of the AGI range.
- `fact-sheets/whos-who-in-frontier-ai.md` and `images/whos-who-in-frontier-ai.png` (nexus-artifacts) — source of the roster itself.
- `fact-sheets/named-agi-predictions-frontier-ai-leaders.md` (nexus-artifacts) — this report's own named-predictor ledger, added to the library 2026-09-19 (see Library Recommendations below); now a standing citable artifact rather than something future reports need to re-derive.

**Artifact-library candidate identified but not yet submitted:** see Library Recommendations below.

## Library Recommendations (Alexandria — Closing)

**Candidate: "Named AGI Predictions — Frontier AI Leaders" fact-sheet.**
- **Category:** fact-sheet.
- **Why reusable beyond this report:** this engagement compiled, sourced, and confidence-rated ten individuals' dated AGI statements from scratch — exactly the kind of reference material future engagements (and future daily-report CIR matches to "AGI Arrival Timeline") will want to look up rather than re-research. Structured the same way `whos-who-in-frontier-ai.md` is (a living roster with an explicit shelf-life warning), it would give Nexus a standing, updatable ledger of who has said what, rather than re-deriving it inside a one-off report each time a leader makes a new statement.
- **Status:** Added to Library — [PR #18](https://github.com/raceBannon99/nexus-artifacts/pull/18) merged 2026-09-19. Final path: `fact-sheets/named-agi-predictions-frontier-ai-leaders.md` (nexus-artifacts).

**Companion image, added at Rick's direction (not an Alexandria recommendation at closing time):** the Tufte diagram from this report's own Visualizing the Landscape section — "What Frontier AI's Leaders Say About When AGI Arrives" — was separately submitted to the library as `images/agi-ceo-predictions-timeline.png`, pairing with the fact-sheet above the same way `whos-who-in-frontier-ai.png` pairs with its own fact-sheet.
- **Status:** Submitted — [PR #19](https://github.com/raceBannon99/nexus-artifacts/pull/19), awaiting merge.

**Also worth noting, not a separate library candidate:** the Jeff Dean/Oriol Vinyals August 2026 departure from Google DeepMind is a concrete, dated instance of `whos-who-in-frontier-ai.md`'s own shelf-life warning coming true within weeks of that fact-sheet's publication. This doesn't need its own artifact — it's a data point for whoever next updates that fact-sheet's roster, and is recorded here so it isn't lost.

**Pending artifact-library PRs:** [PR #19](https://github.com/raceBannon99/nexus-artifacts/pull/19) ("Add image: What Frontier AI's Leaders Say About When AGI Arrives (timeline)") is open as of this publish, awaiting Rick's review.

## Update Notes

- **2026-09-19, first revision (structural/presentational, per the `nexus-artifact-submit` skill):** Rick approved the "Named AGI Predictions — Frontier AI Leaders" fact-sheet candidate. Submitted the same day as [PR #18](https://github.com/raceBannon99/nexus-artifacts/pull/18) on `raceBannon99/nexus-artifacts`; this report's Library Recommendations status is updated above from "Recommended — awaiting decision" to "Submitted — PR #18, awaiting merge." No other section required a change.
- **2026-09-19, second revision (structural/presentational, per `Nexus Artifact Repository.md`'s "Closing the Loop on Reports That Recommended an Artifact"):** PR #18 merged the same day. This report's Library Recommendations status is updated above from "Submitted" to "Added to Library," and a new Sources entry cites the artifact directly. Separately, Rick asked that this report's own Tufte diagram also be added to the library; it was submitted as [PR #19](https://github.com/raceBannon99/nexus-artifacts/pull/19) and is recorded above pending Rick's review.
