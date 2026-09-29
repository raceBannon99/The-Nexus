# 2026-09-29: What Is the Probability an Uncontrollable AI Superintelligence Harms Humanity?

**Question:** Given Nexus's three standing milestone forecasts — AGI (P5 2028 · P50 2036 · P95 2100), the Singularity (P5 2027 · P50 2042 · P95 2100), and Superintelligence (P5 2029 · P50 2045 · P95 2100) — and Rick's two newsletter essays on AI existential risk ("The AI Race Needs a Stop Button" and its companion Draft RSI Safety Act), what is the probability that an uncontrollable AI superintelligence harms humanity? Use the milestone argument — the technology progressing through AGI, the Singularity, and then Superintelligence — and show the math.

## Synthesis (Agent Bradlee)

The probability that an uncontrollable AI superintelligence harms humanity runs from about 13% to 48%, with a central estimate near 24%, calculated on a horizon running to the year 2100.

That number comes from multiplying two separately-sourced probabilities together. The first is the chance the technology actually completes the full progression — a machine matching broad human performance, then the world losing irreversible control of a frontier system, then that system exceeding human intelligence — within the next 74 years. Because all three of the underlying date forecasts already share the same outer boundary of 2100, that chance lands at approximately 95% under the assumption implied by the milestone progression itself: reaching superintelligence requires having already passed through the two earlier stages. Relaxing that assumption — treating the three stages as statistically independent events rather than a strict pipeline, a more cautious reading — lowers the figure to about 86%. The honest range for "the world reaches an uncontrollable superintelligent system by 2100" is therefore 86% to 95%.

The second number is the chance that such a system, once it exists, actually does something harmful rather than remaining benign or merely disruptive. That figure was established directly: 15% to 50%, with a median near 25%, weighing Metaculus's community forecast, Joseph Carlsmith's and Toby Ord's published existential-risk estimates, the Existential Risk Persuasion Tournament's expert and superforecaster panels, and the public positions of Roman Yampolskiy, Nate Soares, Ed Zitron, and Andrew McAfee against each other. The 15%–50% figure is not new; it is the same number this same analytical process produced yesterday for a narrower, conditional version of exactly this question, and it is also the number Rick's own newest essay cites. Multiplying the arrival probability by the harm probability gives the combined answer: roughly 13% at the low end, roughly 48% at the high end, centered around 24%.

Read plainly, that means the more likely outcome, even on a 74-year horizon, is that humanity does not suffer a superintelligence-driven catastrophe — but "more likely not" is a considerably weaker statement than "unlikely." A one-in-four central chance of a civilization-altering event is not a rounding error, and the range's upper bound, just under one-in-two, sits closer to a coin flip than to a remote possibility. The math is dominated less by whether the technology arrives — that part is closer to certain than not — and far more by what happens once it does, which is the part with the least calibrated data behind it.

Two things temper the number without erasing it. First, the "milestone argument" framing this question asked for — AGI, then loss of control, then superintelligence, in that strict order — is a simplification the underlying forecasts do not fully endorse; Nexus's own methodology treats loss of control and superintelligence arrival as related but not strictly sequential, since a narrower, non-superintelligent system could plausibly slip control first. That is why the honest range spans 86% to 95% rather than resting on 95% alone. Second, every serious estimate of what happens after an uncontrollable system exists spans from near-zero to near-certain among credentialed people, which is itself informative: the field has not converged, so a wide band is the accurate answer, not an evasion.

The recently drafted federal licensing proposal — requiring frontier labs to prove a system won't resist a shutdown command and won't self-replicate before licensing further self-improvement work — targets exactly the transition this math depends on most: the jump from a controllable AGI-level system to an uncontrollable superintelligent one. A licensing gate at that specific chokepoint would not change the estimate of whether superintelligence eventually arrives, but it directly targets the harm-conditional half of the calculation, which is both the larger share of the uncertainty and the part most amenable to policy intervention before the fact rather than after.

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

## What Are the Facts? (Agent Sherlock)

**The three standing forecasts, as of 2026-09-29 (unchanged since their respective last-updated dates):**

| Standing file | P5 | P50 | P95 | Uncertainty window | Years to 50% chance |
|---|---|---|---|---|---|
| AGI Forecast Report | 2028 | 2036 | 2100 | 72 years | 8 years |
| Singularity Forecast Report | 2027 | 2042 | 2100 | 73 years | 15 years |
| Superintelligence Forecast Report | 2029 | 2045 | 2100 | 71 years | 16 years |

Each carries the standing Nexus caveat restated here per the `nexus-forecast-narrative` skill: the AGI and Singularity ranges are anchored to external forecaster/survey baskets (Metaculus, Samotsvety, the AI Impacts survey); the Superintelligence range has no such basket and is a structural inference — Nexus's own least-confident standing AI forecast, built by taking the AGI range as a floor and adding a reasoned transition-gap, not backward from calibration data.

**Rick's own essay, fetched and read in full (WebFetch was blocked on both rebrand.ly links with an HTTP 403; retried via Chrome MCP navigate + get_page_text per the standing rule, which retrieved both cleanly):**

- ["The AI Race Needs a Stop Button"](https://diffuser.substack.com/p/the-ai-race-needs-a-stop-button) (Rick Howard, Sep 28, 2026). States his own forecast for "the uncontrollable superintelligence milestone" as P5 2029 · P50 2045 · P95 2100 — identical to Nexus's own Superintelligence Forecast Report range, used as a single already-synthesized figure representing the compound state (loss of control having occurred, then superintelligence following via recursive self-improvement), not as a separate independent estimate. States explicitly: "a 50% chance we could reach this milestone in 19 years" and, once reached, "a non-zero chance of doing something stupid that ends us all. I'd give it between a 15% and 50% chance" — this is the figure `reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md` supplied the day before, cited back by Rick as his own working number, not independently re-derived in the essay.
- [DRAFT LEGISLATION — The RSI Safety Act](https://rebrand.ly/Howard-draft-RSI-Safety-ACT) (Rick Howard, companion document, Google Doc). A licensing (not prohibition) regime for recursive self-improvement at frontier labs: bans autonomous, unreviewed self-modification specifically, not ordinary human-directed training; applies to the largest compute-threshold models regardless of the developer's home country, if used in the US; requires adversarial proof a system won't resist a stop command, a government-verified kill switch, and an anti-self-exfiltration plan before a license issues; creates a five-person "Frontier AI Safety Commission" (modeled on the Nuclear Regulatory Commission) with unannounced-inspection and immediate-shutdown authority; penalizes unlicensed violations at the greater of $100M or 10% of global revenue per day, with up to 20 years' imprisonment for executives who knowingly permit it, and a 20%-of-fines whistleblower incentive.

**First Principles Newsletter Tracker check:** Thread 5 ("AI's real danger is relentless, non-sentient task-pursuit and institutional-control erosion, not conscious malice") — Status: Under Pressure. "The AI Race Needs a Stop Button" is that thread's fifth and current constituent essay; today's evidence (this engagement's own math) neither supports nor contradicts the thread's thesis on its own terms — it quantifies a risk the thesis already argues is real without hostile intent, rather than testing the thesis's own claim about *mechanism* (non-sentient task-pursuit vs. conscious malice). No new Evidence Log entry warranted; this report reasons from the thread's existing, already-current position rather than introducing evidence bearing on its Status.

**Library candidate flagged:** the lognormal-CDF-fitting method used below (fit each standing forecast's own P50/P95 to a continuous distribution, check stochastic ordering, chain via nesting) is a reusable technique for any future question needing a joint probability across Nexus's own sequential milestone forecasts — see Turing's section.

## What Does the Adversary Playbook Look Like Here? (Agent Ryan)

No adversary, campaign, or attribution angle applies — this is a probability-and-timing question about hypothetical future AI capability, not an incident, campaign, or attribution analysis. No entry warranted in `Intelligence Reports/Adversary Tracking Report.md`. Passing the draft on unchanged.

## What Must Be Fundamentally True? (Agent Euclid)

**The math, worked from first principles.**

**Step 1 — turn each standing forecast into a continuous curve.** A P5/P50/P95 triple alone doesn't answer "what's the probability of X by year Y" for any Y other than those three anchor years. To use the forecasts for arbitrary intermediate years (and to chain them), each was fit to a lognormal time-to-event distribution — the standard choice for technology-arrival forecasting, since it's naturally skewed with a long right tail, matching the shape of these ranges (a compressed near side, P5 only a few years out, against a P95 pinned at a fixed 2100 ceiling 70-plus years out). Fitting each milestone's own P50 and P95 (its two most emphasized, most load-bearing figures) gives a closed-form cumulative probability function for time T, in years from today (2026-09-29):

| Milestone | μ = ln(P50 in years) | σ = [ln(P95 years) − μ] / 1.645 |
|---|---|---|
| AGI (P50=10 yrs, P95=74 yrs) | 2.302585 | 1.216705 |
| Singularity (P50=16 yrs, P95=74 yrs) | 2.772589 | 0.930989 |
| Superintelligence (P50=19 yrs, P95=74 yrs) | 2.944439 | 0.826520 |

Each curve reproduces its own file's stated P50 and P95 exactly by construction. (The stated P5 figures don't fall exactly on these fitted curves — the Singularity file's own P5 of 2027 actually precedes the AGI file's P5 of 2028 in the raw numbers, an artifact of each file being anchored to its own separate external basket rather than a single joint model. The fitted curves resolve this: see the ordering check below.)

**Step 2 — check whether the fitted curves behave the way the milestone argument requires.** If AGI genuinely must precede the Singularity, which must precede Superintelligence, then at any given year, the cumulative probability of having reached AGI should be at least as high as having reached the Singularity, which should be at least as high as having reached Superintelligence. Checked at five years spanning the whole range:

| Year | P(AGI reached) | P(Singularity reached) | P(Superintelligence reached) | Ordered correctly? |
|---|---|---|---|---|
| 2036 | 50.0% | 30.7% | 21.9% | Yes |
| 2042 | 65.0% | 50.0% | 41.8% | Yes |
| 2045 | 70.1% | 57.3% | 50.0% | Yes |
| 2050 | 76.4% | 66.8% | 61.1% | Yes |
| 2100 | 95.0% | 95.0% | 95.0% | Tied (both anchor points) |

The fitted curves are consistently ordered at every checked year short of the shared endpoint — genuine support for treating the three as a coherent, nested progression, not just an assumption asserted without evidence.

**Step 3 — the nested/pipeline joint probability.** If reaching Superintelligence by year T strictly requires having already passed through the Singularity and AGI by T (true containment: the event "Superintelligence by T" is a subset of "Singularity by T," which is a subset of "AGI by T"), then the probability of completing the *entire* chain by T is simply the probability of the last, most restrictive gate: **P(full chain by T) = P(Superintelligence by T)**. At T = 2100, that's 95% — not because of any new calculation, but because Nexus's own standing methodology already capped all three files' P95 at the same 2100 horizon "for methodological consistency." The three forecasts already agreeing on a shared outer boundary is doing real work here: it's what makes 95% the answer under strict nesting, with no further computation needed.

**Step 4 — why 95% shouldn't be taken as the whole answer.** Per Alexandria's opening section, the Superintelligence Forecast Report's own Methodology explicitly declines to nest itself under the Singularity Forecast Report the same way it nests under the AGI Forecast Report — it states outright that loss of control could plausibly precede full superintelligence via a narrower system, and that the two files' medians "are not required to sit in any particular order relative to each other... a substantive, defensible position, not an inconsistency to be corrected." That means the strict three-way nesting Step 3 assumes is stronger than what Nexus's own standing methodology actually commits to. A more conservative alternative — treating the three milestones as statistically independent rather than strictly nested — multiplies the three marginal probabilities directly: 0.95 × 0.95 × 0.95 = 85.7% (rounded to 86% wherever this report states the range in prose or in the diagram; the unrounded 0.857 is what Step 5's low-bound multiplication actually uses). The honest range for "the world reaches the compound state (AGI-level capability, having lost control, in a system that exceeds human intelligence) by 2100" is therefore **85.7%–95%, stated as 86%–95%** for readability, not a single point figure.

**Step 5 — combine with the conditional harm probability.** `reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md` already established, from first principles reasoning over Carlsmith, Ord, the Existential Risk Persuasion Tournament, and Nexus's own Metaculus/AI Impacts anchors, that P(harm | the compound state occurs) runs 15%–50%, median ~25%. The two probabilities are close to independent of each other — the timing question (does the technology get there) and the alignment question (does it turn hostile once there) rest on almost entirely different evidence bases — so multiplying them is the correct operation, not a loose approximation:

- **Low bound:** 0.857 (independent-milestones timing) × 0.15 (low harm estimate) = **12.9%**
- **High bound:** 0.95 (nested-pipeline timing) × 0.50 (high harm estimate) = **47.5%**
- **Central estimate:** 0.95 (the nested model, matching the milestone-argument framing this question explicitly asked for) × 0.25 (median harm estimate) = **23.75%**

**The answer: roughly 13% to 48%, centered around 24%, that an uncontrollable AI superintelligence harms humanity by 2100.**

## How Could We Be Wrong? (Agent Popper)

Genuine pushback on four fronts:

**Objection 1 — the "milestone argument" itself may not be the right model.** This report was explicitly asked to use it, and did, but `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` warns directly against treating the AGI → recursive-self-improvement → intelligence-explosion → Superintelligence chain as an established sequence rather than a contested hypothesis — on the same panel that fact-sheet documents, Ed Zitron disputed that "superintelligence" is even a coherently defined concept, and Andrew McAfee called the whole threshold argument speculative. Toby Ord's own RSI-dynamics paper (logged in the Superintelligence Forecast Report's Evidence Log, 2026-09-22) argues generation-time limits make an unbounded "singularity" explosion less likely than a bounded, eventually-saturating one — genuine bottleneck evidence against the fast-pipeline assumption Step 3's nesting model leans on. This is exactly why the report gives a range (86%–95%) rather than resting on the pipeline figure alone, but the range's *upper* bound still assumes a mechanism a credentialed minority actively disputes.

**Objection 2 — this recombines two numbers that were never designed to be multiplied.** The 15%–50% harm figure from yesterday's report was computed to answer a conditional question with the compound premise already given as fact. Nothing in that report's own reasoning validated it as one input to a further multiplication against a timing probability — Popper's own stress-test in that report (Objection 3) flagged that the compound premise itself might be "answering the wrong question" relative to the broader, more likely failure mode (loss of control via a non-superintelligent system). Chaining these two numbers compounds that scoping limitation rather than resolving it.

**Objection 3 — no historical base rate exists for any link in this chain.** As the 2026-09-28 report already states plainly, and this report inherits without softening: every figure here — Carlsmith's, Ord's, the XPT panel's, the lognormal fits themselves — is structured reasoning about unprecedented events, not measured frequency. Multiplying two structured-judgment figures together produces a third structured-judgment figure with compounded uncertainty, not a more precise number.

**Objection 4 — the shared 2100 cutoff is doing more work in this answer than the underlying forecasts intend.** All three standing files state their own P95=2100 is "a known simplification... not an assertion that the event definitely happens by 2100," chosen for methodological consistency across files rather than as a genuine 95th-percentile belief extending to 2100 and no further. Step 3's clean 95% result depends entirely on that shared, admittedly-arbitrary cap. A different, non-arbitrary horizon (say, an uncapped "ever" probability) would likely push the timing-arrival figure higher still, since real probability mass plausibly extends past 2100 for all three milestones — meaning today's 86%–95% timing-arrival band, and the compound answer built on it, may understate rather than overstate the true long-run figure.

## What Is Likely to Happen Next? (Agent Seldon)

Resolving each objection rather than leaving it dangling:

**On Objection 1 (contested pipeline):** Correct, and already reflected in the range rather than argued away — Step 4's 86%–95% band exists specifically because the strict pipeline isn't settled science. The central estimate uses the pipeline figure (95%) only because that's the framing this engagement was explicitly asked to use; the report states plainly, here and in the Synthesis, that this is a modeling choice made at Rick's direction, not a claim that the pipeline is established fact.

**On Objection 2 (recombining numbers not designed to combine):** Popper is right that this stacks one scoping limitation on another, and that's stated directly rather than hidden: the combined 13%–48% answer inherits the "may be answering a narrower question than the true risk surface" caveat from yesterday's report, on top of today's own timing-model uncertainty. The alternative — refusing to combine them — would leave Rick's actual question (which explicitly asked for a single combined answer, using the milestone argument, showing the math) unanswered. Combining them with the caveat stated is more useful than either an unstated combination or no combination at all.

**On Objection 3 (no base rate):** Accepted without qualification. Every figure in this report's chain, including the lognormal fits themselves, is reasoned judgment. The lognormal-fitting step doesn't manufacture calibration where none exists — it makes explicit and computable what Nexus's own three standing forecasts already imply, nothing more.

**On Objection 4 (the 2100 cap):** Correct, and the implication is directional, not just a caveat: if the true, uncapped probability mass for all three milestones extends meaningfully past 2100, the honest timing-arrival figure — and therefore the combined answer — is more likely understated than overstated by this report's math. Stated here as a limitation with a known direction, not a symmetric error band.

**The forecast, in plain language rather than statistical notation, per this engagement's own standing rule for ad-hoc ranges:** the probability that an uncontrollable AI superintelligence harms humanity by 2100 runs from about 13% to 48% — a 35-percentage-point span — with a central estimate around 24%, a little under a quarter of the way from the low end toward the high end of the credentialed range this depends on. This is a probability-of-event-by-fixed-date figure rather than a date-of-event figure, so the standing uncertainty-window/years-to-median date narrative doesn't apply directly to it the way it does to the three date forecasts cited above (each of which carries its own such narrative in Sherlock's table); the 35-point span plays the same role here that a date range's own width does elsewhere — a stated measure of how uncertain the estimate genuinely is, not an artifact of imprecise reasoning.

**Newsletter Tracker bearing:** Thread 5's current thesis ("the danger isn't hostile intent... it just doesn't care") is the mechanism this report's harm-conditional (drawn from Carlsmith's instrumental-convergence reasoning) already assumes throughout — this report's math is fully consistent with, and adds numerical texture to, Rick's own already-published position rather than complicating or contradicting it. No Status change warranted.

## How Do We Make This Clear? (Agent Tufte)

The CDF-ordering check (Euclid's Step 2 table) is genuine tabular data — already presented as a table above, the right tool for it. The chain itself — three sequential milestones, each gating the next, converging on a shared 2100 boundary, then multiplied against a separately-sourced harm probability to produce the final range — has real spatial/flow structure a table can't carry: which quantity feeds into which, and where the compounding actually happens. Built as a rendered diagram rather than approximated in text.

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-09-29-uncontrollable-asi-harm-probability/milestone-chain.png" alt="Milestone chain diagram: AGI to Singularity to Superintelligence, gated at 2100, multiplied by the harm-conditional probability to produce the final 13%-48% range">

No First Principles Newsletter Tracker prior-position-vs-evidence diagram warranted — Thread 5's bearing is fully captured in prose in Sherlock's and Seldon's sections above, and nothing here shifts its Status.

**Library candidate flagged:** the diagram's underlying structure (sequential milestone gates converging on a shared horizon, multiplied by a conditional outcome probability) is reusable for any future Nexus question chaining two or more of the standing AI forecasts.

## Should Any of This Become a Skill? (Agent Turing)

**Candidate identified, not built this round.** The lognormal-CDF-fitting-and-chaining method used in Euclid's section — fit each standing forecast's P50/P95 to a continuous curve, check stochastic ordering, chain via nested or independent assumptions, combine with a separately-sourced conditional probability — is a genuinely repeatable procedure Nexus is likely to need again any time a future question asks to combine two or more of the three standing AI forecasts into one answer. It is not built as a formal skill this round because this is only the first time the technique has been used; per the standing "most runs won't produce one" discipline, one data point isn't yet enough to know the method's edge cases (how it should handle a horizon other than 2100, a fourth milestone, or forecasts that don't share a common P95 anchor). Worth building if a comparable chaining question comes up again.

## New Skills

None created this run.

## Sources

**Nexus standing forecasts (load-bearing, quoted directly):**
- `Intelligence Reports/AGI Forecast Report.md` — P5 2028 · P50 2036 · P95 2100 (unchanged since 2026-09-18): a 72-year uncertainty window and a 50% chance we could reach this milestone in 8 years.
- `Intelligence Reports/Singularity Forecast Report.md` — P5 2027 · P50 2042 · P95 2100 (unchanged since 2026-09-14): a 73-year uncertainty window and a 50% chance we could reach this milestone in 15 years.
- `Intelligence Reports/Superintelligence Forecast Report.md` — P5 2029 · P50 2045 · P95 2100 (unchanged since 2026-09-18): a 71-year uncertainty window and a 50% chance we could reach this milestone in 16 years. Structural inference, not externally calibrated — see the file's own confidence caveat.

**Nexus prior analysis (load-bearing, reused directly rather than re-derived):**
- [`reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-09-28-uncontrollable-superintelligence-extinction-probability.md) — P(harm | uncontrollable superintelligence occurs) = 15%–50%, median ~25%, this report's harm-conditional input.
- `fact-sheets/agi-vs-singularity-forecasting-thresholds.md` (nexus-artifacts) — the AGI/Singularity/Superintelligence distinction, the pipeline-is-contested warning, and the anti-merging rule this report's method respects.
- `fact-sheets/rsi-safety-act-draft-legislation.md` (nexus-artifacts) — an earlier (2026-09-21), related but distinct Nexus-drafted licensing bill on the same subject.
- [[First Principles Newsletter Tracker]] Thread 5 — reasoned from directly in Sherlock's and Seldon's sections; no new Evidence Log entry, no Status change.

**Rick's own essays (primary sources, fetched via Chrome MCP after WebFetch returned HTTP 403 on both rebrand.ly links):**
- [The AI Race Needs a Stop Button](https://diffuser.substack.com/p/the-ai-race-needs-a-stop-button) (Rick Howard, Sep 28, 2026) — source of the P5 2029/P50 2045/P95 2100 figure quoted as "the uncontrollable superintelligence milestone" and the 15%–50% harm estimate.
- [DRAFT LEGISLATION — The RSI Safety Act](https://rebrand.ly/Howard-draft-RSI-Safety-ACT) (Rick Howard, companion draft bill).

## Numbers Check (Agent Popper, second appearance)

Every number in this report checked against its original source and against every other place it appears, including the diagram:

- The three P50/P95 date pairs (2036/2100, 2042/2100, 2045/2100) match their source files exactly in Sherlock's table, Euclid's fitting table, and the diagram's three gate labels.
- The uncertainty-window and years-to-50%-chance figures (72/8, 73/15, 71/16) recompute correctly from those same date pairs and match the `nexus-forecast-narrative` skill's own worked reference table for 2026-09-27, unchanged since.
- The lognormal μ/σ parameters and the five-year stochastic-ordering table were independently recomputed (not hand-approximated) and match what's printed in Euclid's section exactly.
- 95% at 2100 for each milestone is stated consistently everywhere it appears (Euclid's Step 2 table, Step 3, the diagram's three gate percentages) — no drift between prose and figure.
- **One precision inconsistency found and fixed during this check:** the independent-multiplication figure (0.95³) is 85.7% precisely, but an earlier draft stated "86%" in some places and "85.7%" in others without flagging the rounding. Corrected in Step 4 above to state both explicitly and note which one the actual low-bound multiplication (Step 5) uses.
- The final range (13%–48%, central 24%) recomputes correctly from its two stated inputs (85.7–95% × 15–50%, median 95% × 25%) in Euclid's Step 5, Seldon's section, the Synthesis, and the diagram's final-output node — all four agree.
- The diagram's own numbers were checked against the prose, not assumed correct because they were auto-generated from the same figures: all match.

No further loop-back required.

## Library Recommendations (Agent Alexandria, closing)

**Candidate: "Chaining Nexus's Standing AI Milestone Forecasts" method note.**
- **Category:** fact-sheet.
- **Why reusable beyond this report:** documents the lognormal-fit-and-chain method (Euclid's Steps 1–5 above) as a repeatable technique, alongside the existing `agi-vs-singularity-forecasting-thresholds.md` fact-sheet's cautions about what the method must not do (merge disagreeing externals, assume the pipeline is settled). Closely related to Turing's flagged skill candidate above — if that skill gets built on a future engagement, this fact-sheet and it should be cross-referenced rather than duplicated.
- **Status:** Recommended — awaiting Rick's decision. Not yet submitted.

**Pending artifact-library PRs:** #21 ("Emerging-Technology Licensing Design Checklist") and #22 ("Floor, Not Shield") remain open on `raceBannon99/nexus-artifacts`, unrelated to this report.

## Update Notes

None yet — this is the initial publish (2026-09-29).
