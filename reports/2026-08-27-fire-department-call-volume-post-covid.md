# Did Fire Department Call Volume Explode During COVID and Never Come Back Down?

**Question:** Is it true that during Covid, fire departments across the world saw an exponential increase in call volume, but after, the volume never went down? If it is true, assess why that might be true.

## Bradlee's Synthesis

Partly true, but not in the way the question assumes — and the "why" is more interesting than a simple pandemic-shock story.

The literal claim — an exponential rise in fire department call volume *during* COVID that then never reverted — doesn't hold up against the best available aggregate US data (NFPA's Fire Experience Survey, the national estimate covering all fire department call types). Total call volume actually *dipped* slightly in 2020, the most acute pandemic year (37.3M calls in 2019 to 36.4M in 2020), consistent with fewer car accidents under lockdown and documented public avoidance of calling 911 or going to hospitals early in the pandemic. That pattern shows up as a real decrease in some US regions, even as a few dense cities (New York) and other countries (Israel, Denmark) saw sharp spikes from COVID-specific respiratory calls. There was no broad-based exponential increase in 2020 itself.

What *did* happen — and this is the part of the premise that holds up, once corrected — is a large, durable step-up in total call volume that appeared in 2021–2022, after the acute pandemic phase, and has not receded through the most recent full year of data (2024): roughly 36–37 million calls/year pre-pandemic to roughly 42–43 million calls/year since 2022, a sustained ~15% increase with three full years now sitting on the new plateau. One data-quality note carried through this report: NFPA's own published 2021 total doesn't sum from its own published category breakdown — the true 2021 figure is probably closer to 39.6M than the 36.6M shown, meaning the ramp likely started a year earlier than the published headline number alone suggests (flagged transparently in Sources, not silently corrected). The UK's NHS ambulance data shows the same qualitative shape — record volumes in 2023–2024, meaningfully above pre-pandemic baselines — modest but real corroboration this isn't a US-only reporting artifact, while still falling well short of a literal worldwide claim (this report is scoped to the US, with UK corroboration, per Rick's own scoping decision below).

The "why it never went down" question has a more mundane answer than "COVID broke something." The increase is almost entirely in medical/EMS calls, not fires — and it sits on top of a four-decade secular trend (EMS's share of total fire department calls has climbed from 47% in 1980 to 66% today) driven by population aging, rising chronic disease burden, and growing EMS utilization by long-term care facilities. COVID's most likely role was as an accelerant and stress-test, not a root cause: it coincided with, and plausibly worsened, an opioid-overdose surge, a mental/behavioral-health crisis in call volume, and — critically — supply-side damage to the surrounding healthcare system (rural hospital and ER closures, primary-care access gaps, ER boarding) that pushes uninsured and underserved populations toward 911 as a default entry point to care. None of those demand- or supply-side drivers have reversed; several (aging, chronic disease, healthcare-access gaps) are structurally one-directional. A system whose downstream capacity to absorb demand didn't recover, sitting under a demand curve that was already rising before the pandemic, has no obvious mechanism to snap back to its old baseline — which is exactly what three years of flat, elevated data now show.

Genuine open uncertainty, addressed head-on below: how much of the specific 2021–2022 jump reflects real new 911 activity versus reporting or dispatch-protocol changes, and whether early declines in opioid-overdose deaths (2023–2024, per CDC) will be enough to offset continued aging-driven demand growth. Seldon's forecast treats a future reversion to pre-2022 call volumes as possible but not the base case.

## Clarifying Questions

Before research began, two scope questions were flagged as genuinely ambiguous in ways that would change the shape of the answer — Rick was asked and chose in both cases:

1. **Geographic scope.** "Across the world" implies a literal global claim, but detailed, systematically reported call-volume data exists for only a handful of countries. Rick chose to have Sherlock research the US as the primary evidentiary base (by far the best public data — NFPA, USFA), corroborate with other well-documented countries where possible, and frame the conclusion as broadly generalizable rather than a literal worldwide survey.
2. **Definition of "call volume."** Fire departments respond overwhelmingly to EMS/medical calls, not fires. Rick chose to treat "call volume" as total call volume across all incident types (fire, EMS/medical, rescue, hazmat, false alarm, mutual aid, other) — the metric fire departments and NFPA themselves report, and the one most likely to show the pattern described in the question.

Both choices shape everything below.

## What Do We Already Know? (Alexandria, opening)

Checked the artifact library (`raceBannon99/nexus-artifacts`) and prior Nexus reports (`raceBannon99/The-Nexus`) for anything on fire department call volumes, EMS utilization, or COVID-era public-safety-system strain. Nothing came back — no matching entries in the library's `fact-sheets/`, `essays/`, or `book-reviews/` indexes, and a full-text search of `reports/` for "fire department," "EMS call volume," "emergency medical services," and "call volume" returned no matches. This is a clean-slate topic for The Nexus; nothing here builds on prior work.

## The Facts (Sherlock)

**The core dataset.** NFPA's Fire Experience Survey publishes a national estimate of US fire department calls by year and category, back to 1980. Selected years (Total / Fires / Medical aid):

| Year | Total | Fires | Medical aid | False alarms | Mutual aid | Other |
|---|---|---|---|---|---|---|
| 2018 | 36,746,500 | 1,318,500 | 23,551,500 | 2,889,000 | 1,512,500 | 6,342,500 |
| 2019 | 37,272,000 | 1,291,500 | 24,481,000 | 2,893,000 | 1,487,000 | 5,936,000 |
| 2020 | 36,416,000 | 1,388,500 | 23,812,000 | 2,760,000 | 1,390,000 | 5,938,500 |
| 2021 | 36,624,000* | 1,353,500 | 26,291,000 | 2,904,500 | 1,550,000 | 6,403,500 |
| 2022 | 42,059,000 | 1,504,500 | 27,841,500 | 3,092,000 | 1,503,500 | 6,953,000 |
| 2023 | 42,412,500 | 1,388,500 | 28,405,000 | 3,140,000 | 1,590,500 | 6,745,500 |
| 2024 | 42,687,000 | 1,388,000 | 28,226,500 | 3,287,500 | 1,592,000 | 6,964,500 |

*\*Data-quality flag: NFPA's published 2021 total (36,624,000) does not sum from its own published category columns for that row — those columns sum to approximately 39,624,000. Every other year in the table (checked 2020, 2022 explicitly) sums correctly to its published total, so this looks like an isolated transcription error (a "9" rendered as "6") rather than a different accounting method. I could not independently confirm which figure is correct via a second NFPA source in the time available — flagging rather than silently correcting. If the ~39.6M figure is the accurate one, the step-up in call volume began a year earlier (2021) than the published total alone suggests, which is also consistent with numerous individual US fire departments (Des Moines, Reno, Appleton, Massena, and others) independently reporting "record number of calls" for 2021 in local news coverage — a pattern one would expect less strongly if the national total had been essentially flat at 36.6M that year.*

**2020 itself was mixed, not a broad spike.** International and US regional evidence on the acute pandemic period (2020) is genuinely mixed, not uniformly "exponential increase":
- NYC EMS call volume rose from a typical daily high of ~4,000 to over 7,000 calls at the pandemic's peak (>50% above pre-COVID highs).
- Israel's national EMS call volume rose ~1,900% in the first three months of 2020 (an extreme, short-lived spike tied to COVID screening/triage calls).
- Copenhagen, Denmark saw EMS calls rise ~24%.
- By contrast, a peer-reviewed study of the US Upper Midwest found emergent EMS call volume *fell* 28.7% in 2020 versus the 2015–2019 average — consistent with reduced trauma/vehicle-accident volume under lockdown and public avoidance of seeking emergency care.
- NFPA's national US total for all fire department calls (all types) fell slightly in 2020 versus 2019.

**EMS/medical aid, not fire, drives the long-run trend.** Structure/vehicle/wildland fire call volume has been roughly flat for a decade (1.29M in 2019, 1.39M in 2024). Medical aid's share of total fire department calls has grown continuously for over four decades: 46.6% of all calls in 1980, 66.1% in 2024. This is the pre-existing secular trend the pandemic-era numbers sit on top of.

**Drivers cited in current fire/EMS trade literature and research for sustained elevated demand:** an aging population (age is an independent risk factor for EMS utilization, and utilization from long-term care facilities specifically is called out as a growing driver); rising chronic-disease burden; the opioid epidemic (one fire-service source states more than half of medical calls in some jurisdictions are now overdose-related, dwarfing the ~9% attributable to vehicle crashes); a rise in behavioral/mental-health-related calls, associated in part with growth in the unhoused population; and economic/healthcare-access strain, with EMS increasingly used as a default entry point to care by people without reliable access to primary care or insurance.

**UK corroboration.** NHS England's ambulance statistics show the same qualitative shape in a completely different country and reporting system: 2024 was the busiest year on record for NHS emergency services (~8.9M incidents, up from ~8.35M in 2023); January 2024 999 call volume was 22% higher than January 2023; Category 1 (most urgent) calls in January 2023 were already 20% above the equivalent pre-pandemic month. This is corroboration of the *pattern* (record, sustained, non-reverting elevated demand) in a data-rich country outside the US — not proof of a literal worldwide phenomenon, per the scoping decision above.

**Library-candidate note (Sherlock):** the NFPA Fire Department Calls table itself is a live, continuously updated external data source (not static text), so it isn't a natural fit to archive verbatim in the library — better referenced by URL each time it's needed. No source flagged here for archiving.

## Adversary/Campaign Check (Ryan)

This question involves no named threat actor, attack campaign, or Adversary Playbook activity under the CIR taxonomy — it's a public-safety/health-systems question, not a cyber-intelligence one. No kill-chain, Diamond Model, or ATT&CK characterization applies. Passing the draft on unchanged; no update to `Intelligence Reports/Adversary Tracking Report.md` is warranted.

## First-Principles Answer (Euclid)

Start from what a "call volume never reverts" pattern actually requires, mechanically. A demand time series that spikes and then plateaus at a new, higher level — rather than spiking and decaying back to trend — requires one of two things to be true: either the shock permanently changed the underlying population's need for the service, or the shock permanently changed the system's capacity to meet that need through other channels, so that demand that used to go elsewhere now routes through this system instead. Both appear to be operating here, and neither is really "about COVID" as a disease event — COVID is better understood as a catalyst that pulled forward and accelerated trends already in motion, and as a stressor that damaged adjacent infrastructure that hasn't been rebuilt.

**Demand-side (need actually grew).** Three of the cited drivers are structural and were already trending upward well before 2020: population aging, chronic-disease prevalence, and EMS reliance among long-term-care facilities. None of these reverse on their own — an aging population keeps aging. The opioid epidemic is a partial exception (see Popper/Seldon below on recent overdose-death declines), but even there, non-fatal overdose calls and repeat "frequent flyer" utilization patterns tend to lag mortality trends. Mental/behavioral-health call growth reflects both rising incidence and a shrinking supply of dedicated behavioral-health response capacity, which pushes those calls onto 911 by default.

**Supply-side (the surrounding system's capacity shrank).** This is the more interesting first-principles mechanism, because it explains persistence better than demand growth alone. If rural hospitals close, primary-care access shrinks, and emergency rooms board patients for longer, the marginal person with a non-catastrophic but real medical need has fewer non-EMS paths to get seen. 911/EMS becomes the path of least resistance — not because more people are sicker, but because the alternative doors (a same-day PCP appointment, an urgent care, a functioning local ER) are harder to open than they used to be. Once that substitution habit forms and the alternative capacity hasn't been rebuilt, there's no automatic mechanism pulling volume back down — the system would need the *supply* side to recover, not merely the acute shock to pass.

**Why this predicts a step-change two years after the shock, not during it.** A pure "COVID makes people sick, so more 911 calls" story predicts the spike concentrated in 2020, when case counts and hospitalizations were highest — and the aggregate US data shows the opposite (a dip in 2020). A "COVID damaged the surrounding healthcare system, and healthcare workforce/capacity losses continued to compound after the acute phase" story predicts exactly what's observed: the level-shift lands in 2021–2022, once the initial lockdown-driven suppression of ordinary activity (fewer car trips, fewer public gatherings) ended and the underlying, now-larger unmet demand met a still-damaged healthcare system. On this view, "never went back down" isn't a mystery requiring a special explanation — it's the default expectation for a demand curve rising under a shrinking supply of alternatives, unless and until either side reverses.

**Library-candidate note (Euclid):** this demand-side/supply-side framework — distinguishing secular growth in need from structural loss of alternative-access capacity as two separate, compounding causes of sustained service-demand growth — looks reusable well beyond this report (hospital-system strain, police call volume, 911 dispatch center staffing, etc.). Flagging for Alexandria's library consideration below.

## Devil's Advocate (Popper)

Euclid's mechanism is plausible, but several parts of both the premise and the explanation deserve real pressure before this goes out under Rick's name.

**1. The premise itself is being repaired, not confirmed.** The question as posed — "exponential increase during COVID" — is not what the US aggregate data shows. Euclid's own framing concedes this and substitutes a different, more defensible claim (a step-change concentrated in 2021–2022). That's a legitimate correction, but it should be stated as a correction, not blended into the narrative as if it were the original claim all along. Readers relaying "the Nexus confirmed fire calls spiked during COVID" would be repeating something the data doesn't actually support.

**2. Is the 2021–2022 jump real demand, or partly a measurement artifact?** A 14.8% single-year jump in a national statistical estimate is a large move for any real-world demand series to make in one year. NFPA's Fire Experience Survey is itself an extrapolation from a sample of reporting departments to a national estimate — changes in survey response, sampling methodology, or department participation could produce a jump of this size without a matching real-world change in 911 activity. The "Other" category — the least well-defined bucket — grew 17.3% from 2019–2024, faster than the total, which is exactly the kind of catch-all growth you'd expect from either genuine new call types or reporting/classification drift. This needs to be treated as a live uncertainty, not resolved in Euclid's favor by default.

**3. Dispatch protocol changes could mechanically inflate fire department call counts without more emergencies occurring.** Many jurisdictions changed EMS dispatch protocols in and after the pandemic to send fire apparatus alongside ambulances on a wider range of call types (partly a fire-service trade-press-documented trend, partly a pandemic-era response to ambulance/EMS staffing shortages). If a fire engine is now dispatched to call types it previously wasn't, "fire department calls" rises mechanically even if total 911 call volume across all responders is flat. Euclid's supply-side story doesn't address this alternative, non-demand-driven mechanism.

**4. Three years of plateau isn't yet "permanent."** The report's language edges toward treating the 2022–2024 plateau as structurally locked in. Three years is a short base on which to declare a trend can't revert, especially since at least one major input — opioid-overdose mortality — has reportedly been declining since 2023, per CDC data not yet incorporated into this draft.

**5. The international evidence is thin, and it's the wrong kind of thin.** Sherlock verified the pattern in exactly two countries: the US and the UK. Both are wealthy, English-speaking, have aging populations, and have well-documented strain in their public healthcare systems (the UK's NHS crisis is its own well-known story). This is close to the least surprising pair of countries to find this pattern in — it's weak evidence for "broadly generalizable" precisely because it wasn't a random or even a deliberately diverse sample. The report should be explicit that this is corroboration in two similar countries, not a broad multi-country finding.

## Forecast and Resolution of Objections (Seldon)

Taking Popper's five objections in order, and resolving each rather than merely logging it:

**On (1), the premise repair:** Agreed, and applied — this report's own headline, Bradlee's synthesis, and every section above now state explicitly that the "exponential increase during COVID" framing is not supported by the aggregate US data, and substitute the corrected claim (a delayed, sustained step-change concentrated in 2021–2022, not the acute pandemic year itself). This is a resolved correction, not a caveat buried at the bottom.

**On (2) and (3), how much of the jump is real demand versus measurement/protocol artifact:** This cannot be fully resolved with the secondary sourcing available in this engagement — it would require access to NFPA's underlying survey methodology notes or a department-level NFIRS reporting-rate comparison across years, neither of which was pulled here. But an artifact-only explanation is hard to reconcile with two pieces of evidence: first, the growth is concentrated in medical aid specifically (not the vaguest "Other" bucket alone — medical aid rose from 24.5M to 28.2M, a "hard," well-defined call type less prone to reclassification gaming, though "Other's" faster relative growth rate is a genuine remaining flag); second, the UK's NHS 999 system — an entirely independent country, methodology, and reporting chain — shows the same qualitative pattern of sustained, record-breaking volume. Two independently measured systems converging on the same shape is inconsistent with a pure single-country measurement artifact, though it does not rule out artifacts contributing to the *size* of the US jump specifically. Net judgment: most of the increase is real demand growth, with dispatch-protocol changes and survey-methodology effects as real but likely secondary contributors to the magnitude of the 2021–2022 US jump in particular. This should be read as a moderately-held judgment, not a settled fact.

**On (4), permanence:** Agreed as a real limit, and the language throughout this report has been kept to "has not receded through the most recent data" rather than "is now permanent." The forecast below treats reversion as a live, rangeable question rather than declaring the plateau locked in.

**On (5), thin/non-representative international sample:** Agreed. This report is explicitly scoped as US-centered with UK corroboration in two similar wealthy countries with aging populations and documented healthcare-system strain — not a worldwide finding — consistent with the scoping decision Rick made at the outset. No stronger claim is made here.

**Forecast: will US fire-department call volume revert toward its pre-2022 range (roughly back below ~40M/year), or keep growing or holding at/above the current ~42–43M plateau?** The core demand-side drivers (population aging, chronic-disease burden, long-term-care-facility reliance on EMS) are structural and still moving upward, not reversing — that part of the demand curve has no plausible mechanism to fall in the foreseeable future. The supply-side driver (healthcare-access damage — rural hospital closures, ER boarding, primary-care shortages) also shows no broad sign of reversing as of 2026. The main variable working in the other direction is the opioid-overdose component, where mortality has reportedly declined since 2023; if non-fatal overdose call volume follows mortality down and behavioral-health-specific response capacity is meaningfully rebuilt, that could offset some of the plateau's height, though probably not overturn its direction, since it's one driver among several that are still rising. Putting this together as a range rather than a point estimate: the range of plausible time-until-a-sustained-multi-year-decline-back-toward-pre-2022-levels runs from about 3 years on the low end (if opioid and behavioral-health-driven call growth falls fast and dispatch protocols are pulled back) to well over 15 years on the high end, with a median guess landing around 8–10 years out — and that median is doing real work papering over a distribution that may not have a right tail at all, since the aging-population component alone is not expected to reverse within any planning horizon relevant to Rick. This is reasoned judgment built from partial, mixed-quality evidence, not a measured or modeled probability — treat it accordingly.

## Visualization (Tufte)

The core finding here is a *shape* — a slight dip, a plateau, then a sharp level-shift that holds — which a table of numbers alone under-communicates; this gets a rendered chart rather than only a table (the data table above still carries the full year-by-year figures for reference). Built with the `dataviz` skill's design system, rendered via headless Chrome CLI per standing convention, and embedded by URL:

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-08-27-fire-department-call-volume-post-covid/us-fire-department-call-volume-2015-2024.png" alt="Line chart of US fire department total call volume, 2015 through 2024, showing a slight dip in 2020, a flat-to-slightly-rising 2020-2021 period, a sharp level-shift upward in 2022, and a plateau at the new higher level through 2024. The published 2021 total is flagged as inconsistent with NFPA's own category breakdown.">

The chart deliberately surfaces the 2021 data-quality flag directly on the plot (not only in a footnote), since it materially affects when a reader should believe the increase actually started. No update to `Intelligence Reports/Adversary Tracking Report.md` was needed — this isn't a cyber/adversary report. No source flagged here for archiving beyond what Euclid and Sherlock already noted.

## New Skills (Turing)

No new skill built this run. One general practice worth naming even though it doesn't warrant a dedicated skill: cross-footing a published statistical table's own component columns against its stated totals caught a real, materially important data-quality issue (the likely 2021 NFPA transcription error) that a straight read of the page would have missed. This is a good habit for Sherlock to keep applying to any multi-column government/trade-association dataset going forward, but it's a research discipline, not a repeatable procedure with enough structure to script — saying so plainly rather than manufacturing a skill around it.

## Sources

**Primary data**
- [NFPA — Fire department calls (national statistics table, 1980–2024)](https://www.nfpa.org/education-and-research/research/nfpa-research/fire-statistical-reports/fire-department-calls) — core dataset for this report; total US fire department calls by year and category. **Data-quality flag:** the published 2021 row's category columns sum to ~39,624,000, not the published total of 36,624,000 — treated as a likely isolated transcription error, unconfirmed against a second source.
- [NHS England — Monthly Operational Statistics, October 2024](https://www.england.nhs.uk/long-read/monthly-operational-statistics-october-2024/) — UK ambulance/999 call volume data used for international corroboration.
- [BSW Together — Busiest year on record for NHS emergency services](https://bswtogether.org.uk/blog/triangle/busiest-year-on-record-for-nhs-emergency-services/) — 2024 UK ambulance incident totals vs. 2023.

**Pandemic-era (2020) call volume research**
- [PMC — Emergency Medical Services (EMS) Calls During COVID-19: Early Lessons Learned for Systems Planning](https://pmc.ncbi.nlm.nih.gov/articles/PMC8434918/) — NYC, Israel, and Copenhagen call-volume spikes during acute pandemic onset.
- [PMC — Impact of COVID-19 on emergency medical services utilization and severity in the U.S. Upper Midwest](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11444382/) — documents a 28.7% *decrease* in emergent EMS calls in 2020 vs. 2015–2019 average, evidence for the "mixed, not uniform spike" 2020 picture.
- [PMC — By Nature, We're Doers and Problem Solvers: Evolving Job Demands and Resources in Response to COVID-19 Among US-Based Fire Service Personnel (RAPID Study II)](https://pmc.ncbi.nlm.nih.gov/articles/PMC10090346/) — fire service personnel-reported workload and stress during the pandemic.

**Drivers of sustained elevated demand**
- [JEMS — Aging population, payment and liability issues drive increasing calls to long term care facilities](https://www.jems.com/ems-operations/ground-ambulance-operations/aging-population44-payment-and/) — long-term-care-facility reliance on EMS as a structural demand driver.
- [FireRescue1 — Q&A: Why the opioid epidemic is a fire service issue](https://www.firerescue1.com/combating-the-opioid-crisis/articles/qa-why-the-opioid-epidemic-is-a-fire-service-issue-4QnEWTcBJ1lQtv17/) — opioid overdose calls as a large share of medical call growth in some jurisdictions.

**General coverage (uncited claims, not independently verified — labeled per Nexus convention)**
- General fire/EMS trade coverage on rising economic strain, reduced primary-care access, and behavioral-health/homelessness-linked call growth was consistent across multiple secondary sources surfaced in search but not independently verified against a primary dataset in this engagement; treated as directionally supportive background, not as confirmed fact.

## New Skills

None this run — see Turing's section above for the general practice worth carrying forward without a dedicated skill.

## Library Recommendations (Alexandria, closing)

One candidate surfaced during this run, flagged by Euclid at the first-principles stage:

- **Candidate:** "Demand-Side vs. Supply-Side Drivers of Sustained Public-Service Demand Growth" — a short reusable framework distinguishing secular, demand-side growth in need (aging, chronic disease, population growth) from structural, supply-side loss of alternative-access capacity (hospital/clinic closures, staffing shortages, reduced primary-care access) as two separate, compounding causes of a service-demand curve that rises under a shock and then fails to revert.
- **Category:** fact-sheet.
- **Why reusable beyond this report:** the same two-axis framework applies directly to future Nexus questions about hospital-system strain, police call volume, 911/dispatch staffing, and other public-service capacity questions — anywhere a "why did X stay elevated after the shock passed" question comes up. It's a general diagnostic lens, not specific to fire departments.
- **My judgment:** worth archiving. It's genuinely reusable, distinct from the narrower Evidence Tier / attribution frameworks already in the library (which are cyber-specific), and cheap to write up as a one-page fact-sheet.
- **Status:** recommended, awaiting Rick's decision — not yet submitted. No PR has been opened against `nexus-artifacts`; per standing process, submission only happens if Rick says to proceed.

No other candidates were flagged at any stage (Sherlock, Ryan, Popper, Seldon, or Tufte) — the underlying data source (NFPA's table) is a live external resource better referenced by URL than archived, and no diagram-independent artifact stood out beyond the framework above.
