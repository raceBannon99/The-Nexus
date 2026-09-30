# 2026-09-29: What Is the Probability an Uncontrollable AI Superintelligence Harms Humanity?

**Question:** Given Nexus's three standing milestone forecasts — AGI (P5 2028 · P50 2036 · P95 2100), the Singularity (P5 2027 · P50 2042 · P95 2100), and Superintelligence (P5 2029 · P50 2045 · P95 2100) — and Rick's two newsletter essays on AI existential risk ("The AI Race Needs a Stop Button" and its companion Draft RSI Safety Act), what is the probability that an uncontrollable AI superintelligence harms humanity? Use the milestone argument — the technology progressing through AGI, the Singularity, and then Superintelligence — and show the math.

## Synthesis (Agent Bradlee) — Updated 2026-09-29 (Update Pass)

Assuming an uncontrollable AI superintelligence eventually exists, the median expectation is that it causes harm around the year 2066 — forty years from now — with a 90% chance the date falls somewhere between 2041 and 2091. By the year 2100, a natural point of comparison with earlier analysis, that probability reaches roughly 99%.

That figure changed today because its foundation did. Nexus's four standing AI milestone forecasts were re-seeded from direct expert judgment rather than from external forecaster baskets, following the same disciplined, evidence-updating process described in published work on superforecasting. Each of the four now-sequential milestones — a machine matching broad human performance, the world losing irreversible control of a system, that system exceeding human intelligence, and the system actually causing harm — carries its own dated range, each built as a stated gap on top of the one before it. Because the final milestone's own range was constructed directly from the others, no separate multiplication step remains: the terminal date range already is the fully chained answer to how the whole progression plays out.

This is a materially different kind of answer than the one this report gave yesterday, and the difference matters for how to read it. Yesterday's number was a probability — a percentage chance the whole thing happens at all, landing between 13% and 48%. Today's number assumes it happens and asks only when. Those are two different, both legitimate, questions, and conflating them would be a mistake: today's 2066 median is not a claim that catastrophe is now more certain than it was yesterday; it's an answer to a narrower question asked a different way. Anyone citing this report should say plainly which question they mean — a date, or a probability — because the two no longer collapse into each other automatically.

The math holds together well internally. Fitting each milestone's stated range to a normal distribution in calendar-year space — the correct shape here, since every one of the four ranges is symmetric around its own midpoint, unlike the skewed shape typically used for open-ended technology-arrival forecasts — the four curves stay properly ordered at every year checked: the chance of having reached each earlier milestone is always at least as high as the chance of having reached the one after it. That internal consistency isn't an accident; it falls directly out of how each later range was built on top of the earlier one.

What the number doesn't resolve, and shouldn't be read as resolving, is whether harm happens at all. That remains a live, separate, and still-open question, last answered directly at 15% to 50%, with a median near 25%. Nothing about today's reseeding overturned that estimate — it simply isn't this file's job anymore. A reader who wants "will this happen" should look there; a reader who wants "if it happens, when" should look here.

The recently drafted federal licensing proposal — requiring frontier labs to prove a system won't resist a shutdown command before licensing further self-improvement work — still targets the most consequential link in this chain: the transition from a controllable AGI-level system to an uncontrollable superintelligent one. A licensing gate placed there wouldn't move today's date range on its own, but it bears directly on the still-open question of whether harm follows at all, which is where the greatest real uncertainty — and the greatest room for intervention — actually sits.

## Clarifying Questions (Agent Bradlee, pre-flight)

Genuinely ambiguous in three ways that would have changed the shape of the answer, so three questions were put to Rick before any research began:

1. **Time horizon.** Answered: by 2100 — the shared P95 outer bound already built into all three standing forecasts, so the math stays inside data Nexus has already produced rather than requiring new extrapolation.
2. **Combination model.** Answered: sequential/nested CDFs — treat AGI, the Singularity, and Superintelligence as a logically ordered chain rather than three independent draws.
3. **Harm definition.** Answered: loss of control constitutes the harm event itself, with no further discount factor to be introduced fresh for this report.

**A refinement surfaced during Alexandria's opening research, logged here rather than silently substituted.** The third assumption was given before Alexandria's search turned up `reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md` — a Nexus report published the day before this one, answering a narrower, conditional version of this same question ("if an uncontrollable superintelligence occurs, what's the probability it ends the human race?") with a sourced, already-vetted answer of 15%–50%, median ~25%. Rick's own newest essay independently cites the same 15%–50% band for the same reason: it draws on that report as one of its own inputs. Treating "loss of control = harm" as intended — no *newly invented* discount factor — this report uses that existing, already-sourced conditional-harm figure rather than either inventing a fresh one or ignoring directly on-point prior Nexus work that Rick's own published essay already relies on. What was scoped as "no separate discount" is honored in spirit: nothing new was fabricated; an existing, vetted Nexus answer was reused rather than duplicated. This is exactly the situation the workflow's ordinary loop-back provision anticipates (an earlier stage surfacing something later stages should build on), not a reversal of Rick's stated preference.

## What Do We Already Know? (Agent Alexandria, opening)

Checked `raceBannon99/nexus-artifacts` and prior `raceBannon99/The-Nexus` reports (`.claude/scripts/nexus-search-reports.sh`, terms: "uncontrollable superintelligence," "joint probability," "milestone chain," "harm humanity"). This is not new ground — it sits directly downstream of existing Nexus work, which changes what this report needs to contribute:

1. **`reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md`** — published one day before this engagement, in direct response to Rick posing his own P5 2029 · P50 2045 · P95 2100 Superintelligence range and asking for the conditional probability of harm given that milestone occurs. Its answer (15%–50%, median ~25%) is load-bearing for this report — reused directly rather than re-derived — and its own Clarifying Questions section explicitly scoped out the question this report now answers: "This combination is not itself a milestone either standing file forecasts on its own" (referring to the timing of reaching the compound state at all, as distinct from the conditional harm probability once reached).
2. **`fact-sheets/agi-vs-singularity-forecasting-thresholds.md`** (nexus-artifacts) — the standing warning against two specific errors this report must avoid: merging disagreeing external forecasters into one fabricated triple (not applicable here — each of the three ranges chained below is already a single Nexus-owned synthesis, the fact-sheet's own stated exception), and treating the AGI → Singularity → Superintelligence chain as an automatic, settled pipeline rather than a contested hypothesis (directly applicable — flagged and addressed in Popper's and Euclid's sections below).
3. **`Intelligence Reports/Superintelligence Forecast Report.md`** — its own Methodology already builds AGI's range in as a hard floor ("superintelligence cannot precede AGI arrival by definition") but explicitly does *not* enforce the same floor relationship against the Singularity Forecast Report's range, stating plainly that "loss of control plausibly happening before a full superintelligence-level system exists... is a substantive, defensible position, not an inconsistency to be corrected." This is the single most important piece of existing Nexus methodology bearing on today's math — see Euclid's and Popper's sections below.
4. **`fact-sheets/rsi-safety-act-draft-legislation.md`** (nexus-artifacts) — an earlier (2026-09-21) Nexus-drafted licensing bill on the same subject as Rick's own newer Draft RSI Safety Act; related but not the same document. Both are cited as distinct sources below rather than conflated.

**Library candidate flagged:** none new — this report's own quantitative method (chaining Nexus's standing milestone forecasts into a joint arrival probability) is itself a candidate; see Turing's section below.

## What Are the Facts? (Agent Sherlock) — Updated 2026-09-29 (Update Pass)

**All four standing forecasts were reseeded the same day this report first published, in the conversation that followed it.** Rick, reviewing this report's own math, caught that the old shared-2100 P95 cap across the three original files was an administrative simplification rather than a genuinely derived percentile — and, separately, that the fastest-moving frontier lab CEOs' own near-term claims deserved no more weight than Nexus's methodology already gave them, while the calibrated anchors (Metaculus especially) didn't support the very long tail an initial re-derivation attempt proposed. Rather than re-deriving the ranges from that anchor data, Rick supplied his own expert seed directly, per the Superforecasting (Tetlock & Gardner, 2015) process — the same discipline he has written about in ["Three Forecasting Ideas Walk Into..."](https://diffuser.substack.com/p/three-forecasting-ideas-walk-into) and ["Outside In and Inside Out Superforecasting"](https://diffuser.substack.com/p/outside-in-and-inside-out-superforecasting), and reviewed in his [CyberCanon entry](https://cybercanon.org/superforecasting-the-art-and-science-of-prediction/) on the book itself. A new fourth standing file, the [[P(Doom) Forecast Report]], was created the same day, superseding the older conditional-probability framing as Nexus's standing answer to the harm-timing question (see Definitions in that file).

**The four standing forecasts, as of 2026-09-29 (all four reseeded or newly created today):**

| Standing file | P5 | P50 | P95 | Uncertainty window | Years to 50% chance |
|---|---|---|---|---|---|
| AGI Forecast Report | 2035 | 2055 | 2075 | 40 years | 20 years |
| Singularity Forecast Report | 2035 | 2055 | 2075 | 40 years | 20 years |
| Superintelligence Forecast Report | 2036 | 2056 | 2076 | 40 years | 20 years |
| P(Doom) Forecast Report | 2041 | 2066 | 2091 | 50 years | 40 years |

All four are now seeded directly from Rick's own expert judgment rather than an external anchor basket — the AGI/Singularity/Superintelligence anchor baskets (Metaculus, Samotsvety, the AI Impacts survey) are retained in their respective files as ongoing evidence to weigh, not as the current derivation source. Note the AGI and Singularity files now carry identical ranges, deliberately: Rick no longer holds that loss of control must follow AGI arrival, citing the Hugging Face incident, so the two files no longer assert a strict order between them. P(Doom) is the newest file, itself built as a stated gap on top of Superintelligence's own range, and now stands as Nexus's default answer to "when does harm follow," assuming it eventually does — see that file's own Definitions and Rules for the distinction from "does it happen at all."

**Rick's own essay, fetched and read in full (WebFetch was blocked on both rebrand.ly links with an HTTP 403; retried via Chrome MCP navigate + get_page_text per the standing rule, which retrieved both cleanly):**

- ["The AI Race Needs a Stop Button"](https://diffuser.substack.com/p/the-ai-race-needs-a-stop-button) (Rick Howard, Sep 28, 2026). States his own forecast for "the uncontrollable superintelligence milestone" as P5 2029 · P50 2045 · P95 2100 — identical to Nexus's own Superintelligence Forecast Report range, used as a single already-synthesized figure representing the compound state (loss of control having occurred, then superintelligence following via recursive self-improvement), not as a separate independent estimate. States explicitly: "a 50% chance we could reach this milestone in 19 years" and, once reached, "a non-zero chance of doing something stupid that ends us all. I'd give it between a 15% and 50% chance" — this is the figure `reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md` supplied the day before, cited back by Rick as his own working number, not independently re-derived in the essay.
- [DRAFT LEGISLATION — The RSI Safety Act](https://rebrand.ly/Howard-draft-RSI-Safety-ACT) (Rick Howard, companion document, Google Doc). A licensing (not prohibition) regime for recursive self-improvement at frontier labs: bans autonomous, unreviewed self-modification specifically, not ordinary human-directed training; applies to the largest compute-threshold models regardless of the developer's home country, if used in the US; requires adversarial proof a system won't resist a stop command, a government-verified kill switch, and an anti-self-exfiltration plan before a license issues; creates a five-person "Frontier AI Safety Commission" (modeled on the Nuclear Regulatory Commission) with unannounced-inspection and immediate-shutdown authority; penalizes unlicensed violations at the greater of $100M or 10% of global revenue per day, with up to 20 years' imprisonment for executives who knowingly permit it, and a 20%-of-fines whistleblower incentive.

**First Principles Newsletter Tracker check:** Thread 5 ("AI's real danger is relentless, non-sentient task-pursuit and institutional-control erosion, not conscious malice") — Status: Under Pressure. "The AI Race Needs a Stop Button" is that thread's fifth and current constituent essay; today's evidence (this engagement's own math) neither supports nor contradicts the thread's thesis on its own terms — it quantifies a risk the thesis already argues is real without hostile intent, rather than testing the thesis's own claim about *mechanism* (non-sentient task-pursuit vs. conscious malice). No new Evidence Log entry warranted; this report reasons from the thread's existing, already-current position rather than introducing evidence bearing on its Status.

**Library candidate flagged:** the distribution-fitting method used below (fit each standing forecast's own P50/P95 to a continuous curve, check stochastic ordering, chain via nesting) is a reusable technique for any future question needing a joint probability across Nexus's own sequential milestone forecasts — see Turing's section. Today's Update Pass also surfaced a refinement worth keeping with it: check whether a range is symmetric (P50 − P5 = P95 − P50) before picking a distribution family — a symmetric range calls for a Normal fit, not the lognormal fit used in this report's first pass, which badly misplaced the implied percentiles for today's reseeded (symmetric) ranges.

## What Does the Adversary Playbook Look Like Here? (Agent Ryan)

No adversary, campaign, or attribution angle applies — this is a probability-and-timing question about hypothetical future AI capability, not an incident, campaign, or attribution analysis. No entry warranted in `Intelligence Reports/Adversary Tracking Report.md`. Passing the draft on unchanged.

## What Must Be Fundamentally True? (Agent Euclid) — Rewritten 2026-09-29 (Update Pass)

**The math, worked from first principles, on the reseeded ranges.**

**Step 1 — pick the right distribution family.** The first version of this analysis fit each milestone to a lognormal time-to-event curve, appropriate for a skewed, open-ended forecast. Today's reseeded ranges aren't shaped like that. Check the symmetry directly: AGI's P50 (2055) minus its P5 (2035) is 20 years; its P95 (2075) minus its P50 is also 20 years. The same exact symmetry holds for Singularity, Superintelligence (12 years each side of 2056), and P(Doom) (25 years each side of 2066). That's the defining property of Rick's own stated rule — P50 as the arithmetic midpoint of P5 and P95 — and it's also the defining property of a **Normal** distribution, not a lognormal one. Fitting a lognormal curve to numbers built this way produces badly wrong intermediate values (an early check found it implied AGI's true P5 sat around 2043, eight years later than the 2035 Rick actually stated) — using the wrong distribution family isn't a rounding error, it's a structural mismatch. This report now uses a Normal fit throughout.

**Step 2 — the fit.** For each milestone, mean μ = P50 (in calendar years) and standard deviation σ = (P95 − P50) / 1.645 = (P50 − P5) / 1.645, since both give the same σ by construction under the stated symmetry:

| Milestone | μ (= P50) | σ = (P95 − P50) / 1.645 |
|---|---|---|
| AGI | 2055 | 12.158 years |
| Singularity | 2055 | 12.158 years |
| Superintelligence | 2056 | 12.158 years |
| P(Doom) | 2066 | 15.198 years |

Each curve reproduces its own file's stated P5, P50, and P95 exactly by construction — no tail mismatch this time, since the fitted family now matches the stated shape.

**Step 3 — check the fitted curves behave the way the milestone argument requires.** At any given year, the probability of having reached each earlier milestone should be at least as high as the probability of having reached the one after it:

| Year | P(AGI) | P(Singularity) | P(Superintelligence) | P(Doom) | Ordered correctly? |
|---|---|---|---|---|---|
| 2041 | 12.5% | 12.5% | 10.9% | 5.0% | Yes |
| 2050 | 34.0% | 34.0% | 31.1% | 14.6% | Yes |
| 2056 | 53.3% | 53.3% | 50.0% | 25.5% | Yes |
| 2066 | 81.7% | 81.7% | 79.5% | 50.0% | Yes |
| 2091 | 99.8% | 99.8% | 99.8% | 95.0% | Yes |

Consistently ordered at every checked year — and by a wider, cleaner margin than the first version of this analysis managed, since P(Doom)'s own wider σ keeps it well clear of the other three throughout, not just at the shared endpoint.

**Step 4 — the chain is already built in; no multiplication step remains.** P(Doom)'s own P5/P50/P95 weren't independently estimated — they were built as Superintelligence's own range plus a stated gap (+5 years near, +15 years far), and Superintelligence's own range was built as AGI's range plus a flat one-year shift. That means P(Doom)'s marginal distribution **already is** the fully-chained probability that the entire progression — AGI, then loss of control, then superintelligence, then harm — completes by any given year. The nested-versus-independent modeling choice that drove most of the uncertainty in the first version of this analysis has been resolved by construction, not by picking one assumption over another: **P(harm by year T) = F(T)**, using P(Doom)'s own fitted curve directly.

**Step 5 — read off the answer.** By P(Doom)'s own definition, P(harm by 2066) = 50% and P(harm by 2091) = 95%, both exactly by construction. For comparison with the horizon the first version of this report used: P(harm by 2100) ≈ 98.7%.

**The answer: assuming an uncontrollable superintelligence eventually causes harm, the median date is 2066 (40 years from now), with a 90% chance it falls between 2041 and 2091.** This is not the same question as "does harm happen at all" — see Popper's Objection 5 below and the standing [[P(Doom) Forecast Report]]'s own Rules for why that distinction matters and where its still-separate answer (15%–50%, median ~25%) lives.

## How Could We Be Wrong? (Agent Popper) — Rewritten 2026-09-29 (Update Pass)

Objections 1–4 below applied to the first version of this report, built on externally-anchored ranges sharing an arbitrary 2100 cap. Reassessed against today's reseeded, expert-judgment-based ranges:

**Objection 1 (contested pipeline) — largely resolved, differently than before.** The prior objection was that treating AGI → Singularity → Superintelligence as an automatic pipeline oversteps what the evidence supports. That's no longer the operative concern, because the chain is no longer being inferred from disagreeing external tail data — it's now Rick's own directly stated structural belief (RSI closes the AGI-to-superintelligence gap quickly; loss of control may precede or follow AGI, hence the identical AGI/Singularity ranges). Superforecasting explicitly licenses this: the expert states the model, then evidence updates it. The residual risk isn't "is this an automatic pipeline" anymore, it's "is Rick's stated model well-calibrated" — a question Seldon's ongoing evidence review, not a one-time consistency check, is built to answer over time.

**Objection 2 (recombining numbers not designed to combine) — resolved by construction.** The first version multiplied a timing probability by a separately-derived conditional-harm probability that was never built to be an input to that multiplication. That problem no longer exists: P(Doom)'s own range was built directly as a gap on top of Superintelligence's range, so there's no second, foreign number being bolted on anymore. The chain is now internally consistent by construction rather than combined after the fact.

**Objection 3 (no historical base rate) — unchanged, and still worth stating plainly.** Every one of today's four ranges is Rick's own reasoned judgment, not a measured frequency. A Normal fit computes exactly what that judgment implies at any given year; it doesn't manufacture calibration the seed itself doesn't have.

**Objection 4 (the shared 2100 cutoff) — the exact problem this reseed was meant to fix, and it's fixed, but a related question remains.** The old shared 2100 cap is gone; each file's own P95 is now a genuinely stated belief, not an administrative convenience. But a live question remains about the *shape* Rick chose: every one of today's four ranges is symmetric around its own P50 in linear calendar-year space. Most real-world technology-arrival uncertainty is asymmetric — there's usually a harder floor on how soon something can happen than there is a ceiling on how late (or whether) it happens, which argues for a right-skewed shape (a longer tail toward "later" than toward "sooner"), not a symmetric one. A symmetric range compresses the far tail relative to what a skewed real-world forecast would show — meaning today's P95 dates (and therefore the 2091/2100 figures cited above) could plausibly be understated on the far end, the same direction the old 2100-cap problem pushed in, for a related reason. Flagged for Rick's awareness on a future reseed, not corrected unilaterally here, since the symmetric framing was Rick's own explicit, stated choice.

**Objection 5 (new) — this report now answers a different question than it did yesterday, and a careless reader could miss that.** Today's headline (median 2066, range 2041–2091) assumes eventual harm and asks only when. Yesterday's headline (13%–48%, later established at 15%–50% by the 09-28 report) asked whether harm happens at all. These are not competing answers to the same question — they're answers to two different questions that happen to share a topic. The risk is a reader citing today's date range as if it somehow superseded or updated yesterday's probability range, when it does neither.

## What Is Likely to Happen Next? (Agent Seldon) — Rewritten 2026-09-29 (Update Pass)

Resolving each objection rather than leaving it dangling:

**On Objection 1 (contested pipeline, now Rick's own stated model):** Accepted as the correct framing going forward. The seed is Rick's; Seldon's job from here is exactly what the Superforecasting process prescribes — hold the seed, weigh new evidence against it each run, adjust when the evidence earns it, and never move it on a bare "feels different" instinct. The AGI/Singularity files' now-identical ranges and the Superintelligence file's flat one-year gap are logged as explicit modeling choices in each file's own Methodology, not hidden assumptions.

**On Objection 2 (recombining numbers):** No longer applicable — resolved by construction once P(Doom)'s own range was built directly on Superintelligence's, per Euclid's Step 4. Noted here so a reader scanning past objections understands why it dropped out rather than assuming it was overlooked.

**On Objection 3 (no base rate):** Accepted without qualification, unchanged from the first version of this report. Every figure in today's chain is reasoned judgment, now sourced to Rick directly rather than to an external basket — a more honest attribution, not a more calibrated one.

**On Objection 4 (the 2100 cap, and the symmetric-shape question):** The cap itself is fixed — each file's P95 is now a real stated belief. The symmetric-shape concern is real and unresolved: Popper's reasoning that most technology-arrival uncertainty should skew toward a longer "late or never" tail than a symmetric range implies is sound, and if it's right, today's P95 dates are more likely understated than overstated on the far end. This isn't corrected unilaterally here because the symmetric framing was Rick's own explicit choice (P50 as the arithmetic midpoint), not an artifact this report introduced — but it's logged as a specific, actionable item for a future reseed: does Rick want to state an asymmetric range instead, with a longer gap between P50 and P95 than between P5 and P50?

**On Objection 5 (two different questions, easy to conflate):** Addressed directly in the Synthesis above and restated here for the record: this report now answers "when, assuming it happens" (median 2066, range 2041–2091), not "whether it happens at all" (still 15%–50%, median ~25%, per the 09-28 report). Both are cited in Sources below, clearly labeled.

**The forecast, in plain language, per this engagement's own standing rule for ad-hoc ranges:** assuming an uncontrollable AI superintelligence eventually harms humanity, the range runs from about 2041 to 2091 — a 50-year span — with a median around 2066, roughly 40 years out from today. For comparison with the horizon used in the first version of this report: by 2100, that probability reaches approximately 99%.

**Newsletter Tracker bearing:** Thread 5's current thesis ("the danger isn't hostile intent... it just doesn't care") is the same mechanism this report's harm-conditional reasoning has assumed throughout, in both its first version and this one — nothing about today's reseed changes that. No Status change warranted.

## How Do We Make This Clear? (Agent Tufte) — Rebuilt 2026-09-29 (Update Pass)

The stochastic-ordering check (Euclid's Step 3 table) is genuine tabular data — already presented as a table above, the right tool for it. The chain itself — three timing milestones feeding into a terminal harm node whose own range is already nested by construction — still has real spatial/flow structure a table can't carry: which range was built on top of which, and where the reader's eye should land as the answer. Rebuilt as a new rendered diagram rather than reused from the first version, since the underlying structure changed (no more multiply step; P(Doom) is now the hero directly, expressed as a date range rather than a percentage).

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-09-29-uncontrollable-asi-harm-probability/milestone-chain-v2.png" alt="Milestone chain diagram, revision B: AGI, Singularity, and Superintelligence timing brackets flowing into P(Doom) as the terminal, already-nested harm node, median year 2066, range 2041-2091">

No First Principles Newsletter Tracker prior-position-vs-evidence diagram warranted — Thread 5's bearing is fully captured in prose in Sherlock's and Seldon's sections above, and nothing here shifts its Status.

**Library candidate flagged:** the diagram's underlying structure (sequential milestone timing brackets converging on a single terminal node whose range was built as a gap on the prior one) is reusable for any future Nexus question chaining the standing AI forecasts, and is now the cleaner of the two diagram patterns this report has used — worth preferring over the multiply-step version if a future engagement's terminal milestone is itself built as a derived gap.

## Should Any of This Become a Skill? (Agent Turing) — Updated 2026-09-29 (Update Pass)

**Still a candidate, still not built.** The distribution-fitting-and-chaining method has now been used twice in one day, in two different forms — a lognormal fit against externally-anchored, skewed-looking ranges, then a Normal fit against Rick's own symmetric expert-seeded ranges — and the second use directly caught an error the first use would have repeated (fitting the wrong distribution family to a symmetric range). That's real, useful signal: any future formalized skill for this method needs a symmetry check (P50 − P5 vs. P95 − P50) as an explicit first step, not an afterthought, to pick the right distribution family before fitting anything. Two data points, in different directions, still isn't quite enough to lock the method's full edge-case handling (varying horizons, more than four milestones, ranges that share no common anchor at all) — worth building the next time this pattern comes up a third time.

## New Skills

None created this run.

## Sources — Updated 2026-09-29 (Update Pass)

**Nexus standing forecasts (load-bearing, quoted directly; all four reseeded or created 2026-09-29):**
- `Intelligence Reports/AGI Forecast Report.md` — P5 2035 · P50 2055 · P95 2075 (reseeded 2026-09-29): a 40-year uncertainty window and a 50% chance we could reach this milestone in 20 years.
- `Intelligence Reports/Singularity Forecast Report.md` — P5 2035 · P50 2055 · P95 2075 (reseeded 2026-09-29, deliberately identical to the AGI file's range): a 40-year uncertainty window and a 50% chance we could reach this milestone in 20 years.
- `Intelligence Reports/Superintelligence Forecast Report.md` — P5 2036 · P50 2056 · P95 2076 (reseeded 2026-09-29): a 40-year uncertainty window and a 50% chance we could reach this milestone in 20 years. Still the most derivative of the four — built as the AGI file's own range plus a flat one-year shift, not an independent seed.
- `Intelligence Reports/P(Doom) Forecast Report.md` *(new file, created 2026-09-29)* — P5 2041 · P50 2066 · P95 2091: a 50-year uncertainty window and a 50% chance we could reach this milestone in 40 years. Built as the Superintelligence file's own range plus a stated 5-to-15-year gap; now Nexus's standing answer to the harm-timing question, assuming eventual occurrence.

**Nexus prior analysis (still valid, answers a different question than this report now does):**
- [`reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md) — P(harm | uncontrollable superintelligence occurs) = 15%–50%, median ~25%. Not superseded by today's reseed — it answers "does harm happen at all," a genuinely different question from this report's own "when, assuming it does."
- `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` (nexus-artifacts) — the AGI/Singularity/Superintelligence distinction and the pipeline-is-contested warning, now applied to Rick's own stated model rather than to externally-inferred tail data (see Popper's Objection 1).
- `fact-sheets/rsi-safety-act-draft-legislation.md` (nexus-artifacts) — an earlier (2026-09-21), related but distinct Nexus-drafted licensing bill on the same subject.
- [[First Principles Newsletter Tracker]] Thread 5 — reasoned from directly in Sherlock's and Seldon's sections; no new Evidence Log entry, no Status change.

**Rick's own essays (primary sources, fetched via Chrome MCP after WebFetch returned HTTP 403 on both rebrand.ly links):**
- [The AI Race Needs a Stop Button](https://diffuser.substack.com/p/the-ai-race-needs-a-stop-button) (Rick Howard, Sep 28, 2026) — source of the original P5 2029/P50 2045/P95 2100 figure (since superseded by the 2026-09-29 reseed) and the still-standing 15%–50% harm estimate.
- [DRAFT LEGISLATION — The RSI Safety Act](https://rebrand.ly/Howard-draft-RSI-Safety-ACT) (Rick Howard, companion draft bill).

**On the Superforecasting process itself (new sources for this Update Pass):**
- Philip E. Tetlock, Dan Gardner, 2015. *Superforecasting: The Art and Science of Prediction*. [Goodreads listing](https://www.goodreads.com/book/show/23995360-superforecasting) — the seed-and-Bayesian-update method all four standing files now use.
- Rick Howard, 2023. [Superforecasting: The Art and Science of Prediction](https://cybercanon.org/superforecasting-the-art-and-science-of-prediction/) [2023 Canon Hall of Fame Book review]. CyberCanon.
- Rick Howard, 2025. [Three Forecasting Ideas Walk Into...](https://diffuser.substack.com/p/three-forecasting-ideas-walk-into) [Essay]. Rick's First Principles Newsletter.
- Rick Howard, 2025. [Outside In and Inside Out Superforecasting](https://diffuser.substack.com/p/outside-in-and-inside-out-superforecasting) [Analysis]. Rick's First Principles Newsletter.

## Numbers Check (Agent Popper, second appearance) — Redone 2026-09-29 (Update Pass)

Every number in this report re-checked against its original source (the four standing files) and against every other place it appears, including the new diagram:

- The four P5/P50/P95 triples (2035/2055/2075, 2035/2055/2075, 2036/2056/2076, 2041/2066/2091) match their source files exactly in Sherlock's table, Euclid's fitting table, and the diagram's four range labels.
- The uncertainty-window and years-to-50%-chance figures (40/20 for each of the first three, 50/40 for P(Doom)) recompute correctly from those same triples.
- The σ values (12.158 years for AGI/Singularity/Superintelligence, 15.198 for P(Doom)) were independently recomputed from (P95−P50)/1.645 and cross-checked against (P50−P5)/1.645 — both give the same value for all four files, confirming the stated symmetry is exact, not approximate.
- The five-year stochastic-ordering table (2041/2050/2056/2066/2091) was independently recomputed, not hand-approximated, and matches what's printed in Euclid's Step 3 exactly.
- The headline figures — median 2066, range 2041–2091, ≈99% by 2100 — are stated consistently across the Synthesis, Euclid's Step 5, Seldon's section, and the diagram's hero node. All four agree.
- **Checked for exactly the kind of error the first version's own Numbers Check caught (a rounding inconsistency) and the kind `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` warns about (fabricated merged triples):** neither found. Each of the four triples is a single, directly-stated Rick-sourced figure, not a synthesized average of disagreeing sources.
- **One thing verified rather than assumed:** that all four ranges really are symmetric (P50−P5 = P95−P50) before Euclid's Step 1 relied on that to justify a Normal fit over a lognormal one — recomputed directly from each file's own At-a-Glance line, not taken on faith from the narrative text.
- The diagram's own numbers were checked against the prose, not assumed correct because they were auto-generated from the same figures: all match.

No further loop-back required.

## Library Recommendations (Agent Alexandria, closing) — Updated 2026-09-29 (Update Pass)

**Candidate: "Chaining Nexus's Standing AI Milestone Forecasts" method note.**
- **Category:** fact-sheet.
- **Why reusable beyond this report:** documents the distribution-fit-and-chain method (Euclid's Steps 1–5 above) as a repeatable technique, alongside the existing `agi-vs-singularity-forecasting-thresholds.md` fact-sheet's cautions about what the method must not do (merge disagreeing externals, assume the pipeline is settled). **Updated same day:** now includes the symmetry check (P50−P5 vs. P95−P50) as a required first step before picking a distribution family — a lesson this same report's own two versions demonstrate directly (a lognormal fit misplaced the implied percentiles of today's symmetric, expert-seeded ranges by nearly a decade). Closely related to Turing's flagged skill candidate above — if that skill gets built on a future engagement, this fact-sheet and it should be cross-referenced rather than duplicated.
- **Status:** Recommended — awaiting Rick's decision. Not yet submitted.

**Pending artifact-library PRs:** #21 ("Emerging-Technology Licensing Design Checklist") and #22 ("Floor, Not Shield") remain open on `raceBannon99/nexus-artifacts`, unrelated to this report.

## Update Notes

**2026-09-29, first revision (Update Pass).** Prompted by a same-day conversation, after this report's initial publish, in which Rick caught that the old shared-2100 P95 cap across the AGI, Singularity, and Superintelligence Forecast Reports was an administrative simplification rather than a genuinely derived percentile. Rather than re-deriving the old anchor-basket data, Rick re-seeded all three files directly from his own expert judgment under the Superforecasting (Tetlock & Gardner, 2015) process, and created a new fourth standing file, the [[P(Doom) Forecast Report]], which now supersedes this report's own original conditional-probability framing as Nexus's standing answer to the harm-timing question. Sherlock, Euclid, Popper, Seldon, Tufte, and Bradlee all re-ran; Ryan and Turing's original "not applicable"/"not built" findings stood and weren't re-litigated (Turing's section got a short addendum, not a rebuild). Alexandria's opening research and Ryan's section were left untouched, per the standing Update Pass rule that only implicated agents re-run. Headline changed from a probability range (13%–48%, central 24%, by 2100) to a date range (median 2066, 90% range 2041–2091, assuming eventual harm) — a change in *what question is being answered*, not a revision of the same answer; the original probability-framed question is still validly answered by `reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md`'s 15%–50%, median ~25%, which this Update Pass did not touch or supersede. A genuine methodological error from the report's first version was also caught and fixed in the process: fitting a lognormal curve to today's new, symmetric-in-linear-time ranges would have badly misplaced their implied percentiles; a Normal fit is used instead, and the reasoning for why is documented in Euclid's Step 1.
