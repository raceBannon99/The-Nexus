# 2026-09-27: Probability Republicans Lose Both the House and Senate in the 2026 Midterms

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

**Question:** As of today (September 27, 2026), what is the probability that Republicans will lose control of *both* the House and the Senate in the upcoming midterms?

## Synthesis (Agent Bradlee)

The probability that Democrats win control of both the House and the Senate this November runs from about **35% to 60%, with a median around 48%** — meaning it is closer to a coin flip than either an underdog bet or a foregone conclusion, but tilted slightly against a clean Democratic sweep rather than slightly in favor of one.

The House is very likely to flip. Republicans hold it by the thinnest of margins — 218 seats to 214, with three vacancies, meaning Democrats need a net gain of only three seats. Every major forecaster shows Democrats favored to take it, with probabilities ranging from 72% (Decision Desk HQ) to 92% (Kalshi's prediction market). The national environment explains why: the generic congressional ballot has Democrats ahead by roughly 7 to 9 points, the widest margin of the cycle, and President Trump's approval rating sits in the low-to-mid 30s, underwater by 20 to 30 points in most recent polling — driven in large part by a bruising government-funding fight in September. A president this unpopular heading into his first midterm has historically cost his party an average of 37 House seats; Democrats need only 3.

The Senate is a genuine toss-up, not a probable flip. Only 35 of 100 seats are up this cycle, and while 22 of them are Republican-held versus 13 Democratic-held — favorable exposure on paper — most of those Republican seats sit in solidly red states that no national wave will move. Democrats' realistic path runs through a handful of true toss-ups: Maine, Ohio, Alaska, and Michigan by consensus rating, plus North Carolina as their best pickup opportunity and Texas as a longer-shot contest. They need to net four of these. Forecasters disagree more here than on the House — 54% (Decision Desk HQ) to 62% (Kalshi) — because the outcome hinges on a small number of individually close races rather than a smooth national trend.

Because the House and Senate are driven by the same underlying environment — presidential approval, the generic ballot, economic conditions — their outcomes move together, not independently. The right way to answer "will Republicans lose both" is not to multiply two separate chamber probabilities, which would understate how correlated they actually are; it is to ask what a model that simulates both chambers jointly, accounting for that shared environment, actually says. Decision Desk HQ's own joint simulation puts a clean Democratic sweep at 51%, with Republicans holding both chambers at 25%, and a split outcome (each party holding one chamber) at the remaining 24% — overwhelmingly a Democratic Senate loss paired with a Republican Senate hold, since a Democratic Senate with a Republican House is a near-nonevent at 3%.

That 51% figure is the best single point estimate available today, but it deserves real error bars in both directions. National polling has shown a directional bias against Republicans' actual performance in two of the last three cycles with a comparable environment (2016, 2020), which argues for not taking today's favorable Democratic numbers entirely at face value. Offsetting that, an approval rating this deeply underwater is itself one of the more reliable signals of midterm punishment in the historical record, and five more weeks remain for an already-bad Republican environment to worsen rather than improve. Both risks are real and roughly offsetting, which is why the honest range is wide — 35% to 60% — with the median landing just under, not at, an even coin flip.

## Clarifying Questions (Agent Bradlee, pre-flight)

The question was well-scoped enough to answer directly: "lose both" unambiguously means losing majority control of both chambers of Congress (not merely a net loss of seats), in the November 3, 2026 general election, as assessed with information available as of today (September 27, 2026). No clarifying questions were needed — proceeding on this stated reading.

## What Do We Already Know? (Agent Alexandria, opening)

Checked the artifact library (`raceBannon99/nexus-artifacts`) and prior reports (`.claude/scripts/nexus-search-reports.sh` against "midterm," "generic ballot," "Senate map," "House majority"). **Nothing in the Library or in any prior Nexus report addresses election forecasting or midterm control odds** — this is new analytical ground for Nexus. The only prior mentions of "midterm" in the report archive are incidental: the Senate's 2026 recess calendar (cited in a Wyden-letter-timing report), a Wired story on the FRONTIER Act's lack of a floor vote before the midterms, a Virginia felon-voting-rights update timed to early voting, and a CyberScoop story on a USPS mail-ballot IT system — none bear on the control-odds question itself, and none are cited further below.

Sources section started here; every subsequent stage adds to it.

## What Are the Facts? (Agent Sherlock)

**Current control and the maps at stake.** Republicans hold the House 218–214 with three vacancies — Democrats need a net gain of only **3 seats** to take the majority. In the Senate, Republicans hold 53 seats to Democrats' 47; 35 seats are up in 2026 (including special elections in Florida and Ohio), of which 22 are currently Republican-held and 13 Democratic-held — Democrats need a net gain of **4 seats**. Consensus ratings place four Senate seats at true toss-up (Maine, Ohio, Alaska, Michigan), with North Carolina rated Democrats' best pickup opportunity (Roy Cooper's candidacy) and Texas a contested but longer-shot race (James Talarico vs. Ken Paxton). [Ballotpedia — US House elections, 2026](https://ballotpedia.org/United_States_House_of_Representatives_elections,_2026); [Ballotpedia — US Senate battlegrounds, 2026](https://ballotpedia.org/U.S._Senate_battlegrounds,_2026); [NPR — the competitive Senate map keeps shifting](https://www.npr.org/2026/07/27/nx-s1-5907379/2026-midterm-election-senate-races); [RealClearPolling — Senate toss-up map](https://www.realclearpolling.com/maps/senate/2026/toss-up).

**Generic congressional ballot.** As of late September 2026, Democrats lead the generic ballot by roughly 7 to 9 points depending on aggregator — RealClearPolling has it at D+8.7 (50.6%–41.9%), Nate Silver's tracker at D+8.1, up from roughly D+6.7 in early September. This is the widest Democratic lead of the cycle, and coincides with a government-funding fight that dragged down approval of both Congress and the White House, especially among independents. [RealClearPolling — 2026 Generic Congressional Vote](https://www.realclearpolling.com/polls/state-of-the-union/generic-congressional-vote); [Silver Bulletin — Generic Congressional Ballot](https://www.natesilver.net/p/generic-ballot-average-2026-nate-silver-bulletin-congress-polls); [uspollingdata.com — Generic Ballot September 2026](https://uspollingdata.com/news/generic-ballot-democrats-lead-widens-september-2026/).

**Presidential approval.** A mid-September Strength In Numbers/Verasight poll put Trump's approval at 33% approve / 63% disapprove — the worst reading in that poll's history since May 2025. Aggregators as of September 18 showed approval in the 35–40% range against 58–63% disapproval across CNN, Ballotpedia, and RealClearPolitics; every major poll released in late September showed him underwater by at least 14 points, most by 20 or more. [uspollingdata.com — Trump Approval Rating September 2026](https://uspollingdata.com/news/trump-approval-new-low-september-2026/); [G. Elliott Morris — September Strength In Numbers/Verasight release](https://www.gelliottmorris.com/p/2026-09-23-september-strength-in-numbers-verasight-poll-release); [Yahoo — Trump's approval rating by state](https://www.yahoo.com/news/politics/articles/president-trumps-approval-rating-state-212034293.html).

**Forecaster win probabilities, as of September 25, 2026.** Decision Desk HQ's model: House — Democrats 72% / Republicans 28%; Senate — Democrats 54% / Republicans 46%; and critically, its own **joint** simulation of both chambers together: Democratic control of both chambers 51.0%, Republican control of both chambers 25.0%, Republican Senate + Democratic House 21.0%, Democratic Senate + Republican House 3.0%. [Decision Desk HQ — 2026 Election Forecast](https://votes.decisiondeskhq.com/forecast/2026). Kalshi's prediction market shows House — Democrats 92%; Senate — Democrats 62% (up from a 50/50 dead heat as recently as August 12). [Kalshi — Senate control market](https://kalshi.com/markets/controls/senate-winner/controls-2026); [CNBC — six months out, control of the Senate is a dead heat](https://www.cnbc.com/2026/05/01/6-months-out-control-of-the-senate-is-50-50-traders-on-kalshi-say.html).

**Historical base rate.** Since 1946, the president's party has averaged a loss of 25 House seats across all midterms, 28 in first-term midterms specifically, and 37 when the president's approval is below 50% at the time of the election — a bucket Trump's current numbers fall well inside. Only two first-term presidents since World War II (Clinton in 1998, Bush in 2002) saw their party gain House seats in a midterm. [Gallup — Midterm Seat Loss Averages 37 for Unpopular Presidents](https://news.gallup.com/poll/242093/midterm-seat-loss-averages-unpopular-presidents.aspx); [The Conversation — 80 years of midterm losses](https://theconversation.com/for-80-years-the-presidents-party-has-almost-always-lost-house-seats-in-midterm-elections-a-pattern-that-makes-the-2026-congressional-outlook-clear-271605); [uspollingdata.com — Midterm History: Seat Losses Since 1930](https://uspollingdata.com/news/midterm-history-party-losses/).

**Newsletter Tracker check (standing rule):** checked `Intelligence Reports/First Principles Newsletter Tracker.md` for any standing thesis bearing on this question. None of the five Thesis Threads or six standalone essays address domestic electoral politics or congressional control — the tracker's political-adjacent entries (Thread 5's AI-race framing, "The Transporter Room Problem" on Sen. Wyden) don't have a genuine reasoned bearing here, only surface-level topical proximity (both involve Congress). No citation made; no Evidence Log entry appended, consistent with the tracker's own rule against logging topical-proximity-only mentions.

**Library candidate flagged:** none at this stage — the sourcing above is standard election-forecasting reference material, not a reusable Nexus analytical artifact.

## What Does the Adversary Playbook Look Like Here? (Agent Ryan)

No adversary, threat actor, or attack campaign involved — this is a domestic electoral-forecasting question, not an incident or campaign analysis. The kill-chain/Diamond Model/ATT&CK apparatus doesn't apply, and no adversary angle is forced onto it. Passes the draft on unchanged.

## What Must Be Fundamentally True? (Agent Euclid)

Reasoning from first principles about what structurally determines a "Republicans lose both chambers" outcome:

**(1) The House and Senate face structurally different bars this cycle, and that difference alone explains most of the gap between the two chambers' win probabilities.** The House is a single national referendum multiplied across 435 districts with a nearly even overall partisan lean — a uniform national swing of even a few points reliably flips a chamber this narrowly held (3 seats). The Senate is not a referendum at all in the same sense: only 35 of 100 seats are in play, their partisan composition is fixed by which third of the map happens to be up this cycle (not by the national environment), and most of the 22 Republican-held seats up in 2026 are in states no plausible national swing would flip. The Senate outcome is therefore much closer to the sum of four to six genuinely close, semi-independent local contests than to a single national trend — which is exactly why forecasters show far more disagreement on the Senate (54–62%) than the House (72–92%): more of the real uncertainty in this cycle lives in the Senate's small number of close races, not in the broad national mood.

**(2) A midterm's outcome is driven by one underlying latent variable — the national political environment — not by two independent chance processes.** Presidential approval and the generic ballot are both downstream measurements of the same thing: how the electorate currently feels about the party in power. Because House and Senate results both respond to that same underlying environment, a bad environment for Republicans tends to produce bad Republican outcomes in *both* chambers simultaneously, not one chamber randomly and the other independently. This means the correlation between "Republicans lose the House" and "Republicans lose the Senate" is strongly positive — which has a direct, somewhat counterintuitive consequence for this question: **the probability of losing both chambers is necessarily higher than it would be if the two chambers' outcomes were independent events multiplied together**, precisely because a bad night for Republicans tends to be a bad night everywhere at once, not compartmentalized by chamber.

**(3) The correct estimation method follows directly from principle (2): use a model that simulates both chambers jointly against a shared environment, not the product of two marginal probabilities.** Naively multiplying two chamber-level win probabilities (e.g., Kalshi's own House 92% × Senate 62% = 57%) treats the chambers as independent coin flips, discarding the shared-environment correlation that principle (2) establishes as real. A properly specified joint model — one that draws a single national-environment shock and propagates it consistently into both chamber outcomes in the same simulation — is the structurally correct tool for this exact question. Decision Desk HQ publishes exactly this: a direct joint-scenario probability (51% Democratic sweep) rather than two marginals a reader would have to combine themselves.

**(4) Historical base rates and the current environment point the same direction, which is itself informative.** An unpopular first-term president (Trump's approval in the low-to-mid 30s) sits squarely in the historical bucket associated with the largest average midterm losses (37 House seats), and the current D+7–9 generic ballot lead is consistent with — not an outlier against — that historical pattern. When a structural base rate and real-time polling data point the same direction, that should increase confidence in the current numbers relative to a case where they conflicted.

**Library candidate flagged:** the joint-simulation-over-naive-product reasoning in point (3) is a reusable diagnostic for any future Nexus question involving two or more correlated binary outcomes driven by a shared underlying variable — not specific to elections. Flagged for Alexandria's closing evaluation.

## How Could We Be Wrong? (Agent Popper)

Devil's advocate against Euclid's draft, on four fronts:

**Objection 1 — polling has a directional miss history, and it doesn't cut in a neutral direction.** National polling underestimated Republican performance in both 2016 and 2020, in some states by several points. If a similar systematic bias reappears in 2026, both the generic ballot (D+7–9) and the forecaster models built substantially on polling inputs would be overstating Democratic strength across the board — not a random noise term but a directional risk that specifically argues for discounting today's favorable-to-Democrats numbers, not just widening the range symmetrically around them.

**Objection 2 — the Senate's toss-up races are exactly the kind of contest most vulnerable to idiosyncratic, late-breaking factors a national-environment model can't capture.** Four to six races deciding Senate control is a small enough sample that a single strong or weak candidate, a late scandal, or a state-specific turnout quirk in just one or two of them could flip the chamber's outcome independent of the national mood — meaning the Senate probability is more fragile and more likely to move sharply on late news than the House's more uniformly-distributed outcome across 435 seats.

**Objection 3 — Euclid's own correlation argument, taken at face value, could be read as implying the joint probability should be reliably close to the lower single-chamber marginal (the Senate's 54%), not meaningfully below it — is 51% actually consistent with "strong positive correlation," or is it suspiciously close to independence?** If House and Senate outcomes were driven almost entirely by one shared variable, the joint "wins both" probability should sit much closer to the Senate's own marginal (54%) than a naive independent product would predict — and 51% is, in fact, fairly close to that Senate marginal, which is consistent with strong correlation rather than contradicting it. But it's worth stating plainly that this is a directional check, not a proof the 51% figure is correctly calibrated — Decision Desk HQ's specific joint-simulation methodology (correlation structure, historical training data, treatment of undecided voters) isn't independently auditable from published output alone.

**Objection 4 — five weeks is a real amount of time for the environment to move, and the current numbers reflect a moment shaped heavily by one event (the September funding fight) that may not still be salient by November 3.** Treating today's snapshot as if it were the election-day probability ignores that approval ratings and generic-ballot leads driven by a specific news cycle sometimes partially revert once that cycle fades from the front pages.

## What Is Likely to Happen Next? (Agent Seldon)

Resolving each objection rather than leaving it dangling:

**On Objection 1 (directional polling-miss risk):** Correct, and this is the single strongest reason not to simply adopt Decision Desk HQ's 51% at face value as if it carried no further uncertainty. The historical miss pattern (2016, 2020 both underestimated Republicans; 2018, 2022, 2024 were comparably close to accurate) means roughly two of the last five comparable cycles saw a meaningful pro-Republican polling bias — a real, non-trivial base rate for exactly the scenario that would push the true probability below today's models. This is the main force pulling the range's lower bound down to 35% rather than settling closer to Decision Desk HQ's 51% point estimate.

**On Objection 2 (Senate fragility):** Correct, and it's precisely why the forecaster disagreement is wider on the Senate (54–62%, an 8-point spread) than the House (72–92%, technically a 20-point spread but driven by very different methodologies — a simulation model vs. a trading market — rather than genuine analytical disagreement about the same evidence). The Senate's dependence on a handful of close races is already priced into why its win probability sits so much lower than the House's; it doesn't require a separate downward adjustment beyond what's reflected in Decision Desk HQ's own joint model, which explicitly accounts for exactly this kind of race-level uncertainty in its simulation.

**On Objection 3 (is 51% really consistent with strong correlation, or close to independence by coincidence):** The check itself is reassuring rather than alarming — 51% sitting close to the Senate's own 54% marginal is the expected signature of strong positive correlation (a fully independent combination of a 72% House and a 54% Senate would land at 39%, well below 51%), so the joint figure is directionally consistent with Euclid's correlation argument, not merely coincidentally close to it. But Popper is right that the internal mechanics of Decision Desk HQ's simulation aren't independently verifiable from public output, which is exactly why this report treats 51% as an anchor and a starting point, not as the final answer with no error bars.

**On Objection 4 (time remaining, event-driven snapshot):** Correct, and unresolvable with more certainty than this: five weeks is enough time for the environment to shift, and it has shifted meaningfully within just the last month (D+6.7 in early September to D+7–9 by late September) on the back of one event. This argues for real range width rather than false precision, in both directions — not a directional adjustment, since the environment could as easily worsen further for Republicans (another funding fight, a weak jobs report) as partially revert.

**Forecast.** The probability that Democrats win control of both the House and Senate in the November 3, 2026 midterms runs from about **35% to 60%, with a median around 48%**. That is a 25-percentage-point-wide range, with the median sitting roughly in the middle of it — about 13 points above the low end and 12 points below the high end — reflecting genuine, largely offsetting uncertainty in both directions rather than a strong lean toward either edge. The anchor for this range is Decision Desk HQ's own joint-simulation estimate (51%), adjusted modestly downward to account for the historical directional polling-miss risk that a pure model-output number doesn't independently correct for, and bounded above by the scenario where the current, historically severe environment for an unpopular first-term president (33–40% approval, D+7–9 generic ballot) holds or worsens through election day, consistent with the historical pattern of unpopular presidents losing an average of 37 House seats. This is reasoned judgment layered onto real polling and forecasting data, not a number read directly off any single source — stated plainly per this report's own standing discipline.

**Library candidate flagged:** none beyond what Euclid already flagged above.

## How Do We Make This Clear? (Agent Tufte)

The comparison across forecasters and chambers is genuine tabular data — a straightforward side-by-side of point estimates, not a process or flow that spatial layout would clarify — so this gets a markdown table, not a rendered diagram:

| | House (D win probability) | Senate (D win probability) | Both chambers (D sweep) |
|---|---|---|---|
| **Decision Desk HQ** (joint simulation, Sep 25) | 72% | 54% | **51%** |
| **Kalshi** (prediction market, late Sep) | 92% | 62% | 57% (naive product — not a joint estimate) |
| **Nexus (this report)** | — | — | **35–60%, median ~48%** |

No diagram is warranted here — there's no process flow, branching decision, or spatial relationship to show; the table above already captures the full comparison a reader needs. No First Principles Newsletter Tracker thesis applies (see Sherlock's check above), so no prior-position-vs-evidence diagram is relevant either.

**Library candidate flagged:** none.

## Should Any of This Become a Skill? (Agent Turing)

No new skill built this round. Election-forecasting synthesis is a one-off analytical exercise using standard public forecasting sources — real, useful work, but not a repeatable Nexus procedure distinct enough from ordinary first-principles reasoning applied to public data to justify formalizing. If Rick brings a second election-forecasting question (a different race, or a follow-up on this one closer to November), that's the point to reconsider — one data point isn't enough to generalize a skill from.

## Sources

**Forecasts and prediction markets**
- [Decision Desk HQ — 2026 Election Forecast](https://votes.decisiondeskhq.com/forecast/2026) — House/Senate win probabilities and the joint four-scenario simulation (51% Democratic sweep) this report anchors on.
- [Kalshi — Senate control market, 2026](https://kalshi.com/markets/controls/senate-winner/controls-2026) — prediction-market pricing for Senate control.
- [Kalshi — 2026 midterms category](https://kalshi.com/category/elections/midterms) — House and Senate market overview.
- [CNBC — "Six months out, control of the Senate is a dead heat"](https://www.cnbc.com/2026/05/01/6-months-out-control-of-the-senate-is-50-50-traders-on-kalshi-say.html) — historical context on how far the Senate market has moved since August.

**Polling**
- [RealClearPolling — 2026 Generic Congressional Vote](https://www.realclearpolling.com/polls/state-of-the-union/generic-congressional-vote)
- [Silver Bulletin — Generic Congressional Ballot tracker](https://www.natesilver.net/p/generic-ballot-average-2026-nate-silver-bulletin-congress-polls) (topline cited via search summary; full model behind paywall, not independently verified beyond the publicly visible figures)
- [uspollingdata.com — "Generic Ballot September 2026: Democrats Widen Lead"](https://uspollingdata.com/news/generic-ballot-democrats-lead-widens-september-2026/)
- [uspollingdata.com — "Trump Approval Rating September 2026: New Term Low"](https://uspollingdata.com/news/trump-approval-new-low-september-2026/)
- [G. Elliott Morris — September Strength In Numbers/Verasight poll release](https://www.gelliottmorris.com/p/2026-09-23-september-strength-in-numbers-verasight-poll-release)
- [Yahoo News — "President Trump's approval rating by state entering September 2026"](https://www.yahoo.com/news/politics/articles/president-trumps-approval-rating-state-212034293.html)

**Maps and current composition**
- [Ballotpedia — United States House of Representatives elections, 2026](https://ballotpedia.org/United_States_House_of_Representatives_elections,_2026)
- [Ballotpedia — U.S. Senate battlegrounds, 2026](https://ballotpedia.org/U.S._Senate_battlegrounds,_2026)
- [NPR — "With just a few primary elections to go, the competitive Senate map keeps shifting"](https://www.npr.org/2026/07/27/nx-s1-5907379/2026-midterm-election-senate-races)
- [RealClearPolling — Battle for the Senate 2026, toss-up map](https://www.realclearpolling.com/maps/senate/2026/toss-up)

**Historical base rates**
- [Gallup — "Midterm Seat Loss Averages 37 for Unpopular Presidents"](https://news.gallup.com/poll/242093/midterm-seat-loss-averages-unpopular-presidents.aspx)
- [The Conversation — "For 80 years, the president's party has almost always lost House seats in midterm elections"](https://theconversation.com/for-80-years-the-presidents-party-has-almost-always-lost-house-seats-in-midterm-elections-a-pattern-that-makes-the-2026-congressional-outlook-clear-271605)
- [uspollingdata.com — "Midterm History: Seat Losses by President's Party Since 1930"](https://uspollingdata.com/news/midterm-history-party-losses/)

## Arithmetic & Consistency Check (Agent Popper, second pass)

Checked every number in the draft against its cited source and against every other place it recurs. Verified: the DDHQ four-scenario joint probabilities (51.0 + 25.0 + 21.0 + 3.0) sum to 100%; the House composition (218 + 214 + 3 vacancies = 435) and the stated 3-seat gap to a Democratic majority are consistent; the Senate composition (53 + 47 = 100) and the 2026 map split (22 + 13 = 35 seats up) are consistent, as is the stated 4-seat gap to Democratic control; Kalshi's naive product (92% × 62% = 57.04%, stated as 57%) is correctly computed; and this report's own final range (35–60%, median ~48%) is internally consistent with its own stated decomposition (48 is 13 points above 35 and 12 points below 60, a 25-point-wide range) everywhere it's cited — the Synthesis, Seldon's forecast, and Tufte's table all state the same figures. No chart or rendered diagram was built this round, so no visual-mark-count check applies. No inconsistency found; no revision needed.

## Library Recommendations (Agent Alexandria, closing)

One candidate flagged during the run:

1. **The joint-simulation-over-naive-product diagnostic (Agent Euclid's stage, point 3)** — category: fact-sheet. When two or more binary outcomes share a common underlying driver (here, House and Senate control both responding to one national political environment), the correct way to estimate their joint probability is a model that simulates them together against that shared driver, not the product of their separately-estimated marginal probabilities, which discards the correlation and produces a biased (generally too-low, for positively correlated outcomes) estimate. This is a general forecasting-methodology principle, not election-specific, and could apply to any future Nexus question involving correlated risks or outcomes (e.g., "probability two different vendors both suffer a breach this quarter" where both depend on a shared industry-wide vulnerability). Status: **Recommended, awaiting Rick's decision — not yet submitted.**

My own judgment: this is a real, reusable methodological principle worth keeping, though it's closer to a restatement of a well-established statistical concept (the difference between joint and marginal probability under correlation) than a genuinely novel Nexus finding — similar in spirit to how Euclid's structural-licensing-requirements argument was assessed as the weakest of three candidates in the 2026-09-21 RSI legislation report. Worth keeping as a checklist entry, not a strong standalone claim to reusability.

## Pending Artifact Approvals

Two PRs open against `raceBannon99/nexus-artifacts`, unrelated to this engagement, flagged per standing convention:
- [PR #21 — Emerging-Technology Licensing Design Checklist](https://github.com/raceBannon99/nexus-artifacts/pull/21)
- [PR #22 — Floor, Not Shield: A Cross-Domain Deterrence Diagnostic](https://github.com/raceBannon99/nexus-artifacts/pull/22)
