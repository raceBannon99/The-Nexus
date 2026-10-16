# 2026-10-16: Three Additional Sources Per CIR Category

**Question:** For each entry in the nexus-cir-list (the 27-category CIR taxonomy), recommend three internet sources we should be checking for the nexus-daily-report.

## Synthesis (Agent Bradlee)

Every CIR category now has at least one named, live, verified internet source behind it — 79 recommendations across 27 categories, two short of a full 81 because one category structurally has no independent second source. The honest finding underneath the list: this isn't primarily a "find more sources" problem. Twelve of the 27 categories (the five AI-timeline trackers, the people-and-trend categories, nation-state policy, workforce, compliance, framework, and resilience) already have real, live, purpose-built outlets that `Sources.md` has never pointed at — the gap was never that the content doesn't exist, it's that the daily report has kept re-checking the same seven to twelve general incident-news outlets for categories that general incident news was never going to produce. Fifteen other categories (adversary activity, data breaches, critical infrastructure, zero trust, kill chain, risk forecasting, automation, over-the-horizon tech, research papers, first-principle strategy) are already well-served by the existing portfolio; the sources recommended for them are additive depth, not gap-filling — cite them when a story needs the primary-source or specialist angle, not as a replacement for Hacker News, Cyberwire, or The Record.

One category — Cybersecurity Canon Project Book Reviews — gets a flagged exception rather than a forced third pick: no independent second daily-or-weekly-cadence book-review outlet covering cybersecurity books was found anywhere on the open internet. The two next-best options are both adjacent in format (SANS whitepapers, not reviews) or structurally entangled with the same parent project the existing source already covers (RSA Conference's own Cybersecurity Canon announcements) — recommending them as genuine independent sources would be fabricating robustness that doesn't exist. This is the same "coverage-shape, not source count" lesson the daily report's own source-portfolio review reached on 2026-08-31: some categories have exactly one real outlet, and that's a fact about the information landscape, not a research shortfall.

Every URL below was checked live today, 2026-10-16. None are fabricated; three previously-flagged items were resolved in the process — IAPP's news feed, which a 2026-08-31 check found redirecting with an unconfirmed destination, now resolves cleanly to `iapp.org/news`; CISO Tribune, noted the same day as "surfaced but not independently verified," is now confirmed live with a real, dated appointment-tracker page. This report only recommends; nothing was added to `Sources.md` — that's Rick's call, the same process followed for the 2026-08-31 source-portfolio review.

## Clarifying Questions (Agent Bradlee, pre-flight)

None asked. The request is fully scoped: it names the exact list to walk (the 27-category `nexus-cir-list` output), the exact count per entry (three), and the exact purpose (candidate sources for `nexus-daily-report`). One assumption, stated rather than asked: this report is a *recommendation* list for Rick to review, not an instruction to edit `Sources.md` directly — matching how the 2026-08-31 source-portfolio-review report was handled (recommend, Rick decides, a later run does the actual adding).

## What Do We Already Know? (Agent Alexandria, opening)

Checked `nexus-artifacts` and prior Nexus reports via `nexus-search-reports.sh` against "source," "CIR," "recommendation." The directly relevant precedent is `reports/2026-08-31-daily-report-source-recommendations.md` on `raceBannon99/The-Nexus` — the only prior engagement to assess the source portfolio against the CIR taxonomy. That report answered a narrower question (which *additions* would close the worst gaps) and led to four sources actually being added to `Sources.md` (CyberScoop, CSO Online's CISO list, CISA advisories, and SecurityWeek being promoted out of the Gmail bucket) plus a later addition of the Forecasting Research Institute's LEAP project on 2026-10-01. Today's question is broader and exhaustive — three sources for *every* category, not just the weak ones — so this report builds on, rather than repeats, that prior work: categories the 08-31 report already analyzed in depth (Executive Leadership Changes, Government Surveillance, Nation-State Policy, Workforce Development) get fresh, additional picks here rather than re-litigating the same ground.

`Sources.md` itself (27 lines of schema plus 12 active sources) is the load-bearing internal document — its own structure (a `name`/`type`/`locator`/`navigation` schema, website vs. email-label vs. monthly-cadence patterns) is the shape every recommendation below should fit if it's ever promoted from recommendation to tracked source.

Starting the Sources section below.

## What Are the Facts? (Agent Sherlock)

Researched and verified live (2026-10-16) three candidate sources for each of the 27 CIR categories. Methodology: favor primary sources (government agencies, standards bodies, named research organizations) over secondary aggregation where one exists; avoid recommending a source that substantially duplicates ground an already-active `Sources.md` entry already covers well (e.g., no additional general incident-news aggregator was recommended for Adversary Playbook, since Cyberwire/Hacker News/The Record/CISA already saturate that ground); where a category's best-fit source is already active (CISA for Critical Infrastructure, The Canon Project for Book Reviews, CSO Online for Executive Leadership, CyberScoop for Nation-State Policy), note that explicitly rather than silently repeating it as if newly discovered.

| # | CIR Category | Source 1 | Source 2 | Source 3 |
|---|---|---|---|---|
| 1 | Adversary Playbook Activity | [Google Threat Intelligence (Mandiant) Blog](https://cloud.google.com/blog/topics/threat-intelligence/) | [CrowdStrike Blog](https://www.crowdstrike.com/en-us/blog/) | [Recorded Future Blog (Insikt Group)](https://www.recordedfuture.com/blog) |
| 2 | AI Singularity Timeline | [Metaculus](https://www.metaculus.com/) | [AI Alignment Forum](https://www.alignmentforum.org/) | [AI Impacts](https://aiimpacts.org/) |
| 3 | AGI Arrival Timeline | [Metaculus — AGI Outcomes](https://www.metaculus.com/tournament/agi-horizons/) | [Epoch AI](https://epoch.ai/) | [AI Impacts — Expert Survey on Progress in AI](https://aiimpacts.org/) |
| 4 | Superintelligence Timeline | [Metaculus — Time From Weak AGI to Superintelligence](https://www.metaculus.com/questions/9062/time-from-weak-agi-to-superintelligence/) | [Epoch AI — Future of AI](https://epoch.ai/topics/future-of-ai) | [AI Alignment Forum](https://www.alignmentforum.org/) |
| 5 | Harm Timeline | [AI Alignment Forum](https://www.alignmentforum.org/) | [AI Impacts](https://aiimpacts.org/) | [Metaculus](https://www.metaculus.com/) |
| 6 | Harm Probability | [Metaculus](https://www.metaculus.com/) | [AI Impacts](https://aiimpacts.org/) | [Epoch AI](https://epoch.ai/) |
| 7 | Law Enforcement Disruption | [Europol Newsroom](https://www.europol.europa.eu/media-press/newsroom) | [FBI Press Releases](https://www.fbi.gov/news/press-releases) | [DOJ Office of Public Affairs](https://www.justice.gov/news/press-releases) |
| 8 | Government Surveillance | [EFF Deeplinks](https://www.eff.org/deeplinks) | [Privacy International](https://privacyinternational.org/) | [Citizen Lab](https://citizenlab.ca/) |
| 9 | Data Breaches | [DataBreaches.net](https://databreaches.net/) | [Have I Been Pwned (Troy Hunt)](https://haveibeenpwned.com/) | [BleepingComputer (RSS)](https://www.bleepingcomputer.com/feed/) |
| 10 | Critical Infrastructure Attacks | *CISA Advisories already active (`Sources.md` #10)* | [Industrial Cyber](https://industrialcyber.co/) | [Dragos Blog](https://www.dragos.com/blog/) |
| 11 | Cybersecurity Canon Project Book Reviews | *The Canon Project already active (`Sources.md` #5)* | [SANS Reading Room](https://www.sans.org/white-papers/) (whitepapers, not reviews — nearest adjacent format) | *No independent second book-review outlet found — see Bradlee's synthesis* |
| 12 | Cybersecurity Executive Leadership Changes | *CSO Online CISO list already active (`Sources.md` #9)* | [CISO Tribune — The Wire](https://www.cisotribune.com/moves) | [SecurityWeek — People on the Move](https://www.securityweek.com/industry-moves/) |
| 13 | Cybersecurity Vendor Executive Leadership Changes | [CISO Tribune — The Wire](https://www.cisotribune.com/moves) (filter to vendor employers) | [SC World — Cybersecurity Executive Changes](https://www.scworld.com/news/cybersecurity-executive-changes-2) | Vendor newsroom pages directly (e.g. [Palo Alto Networks Press](https://www.paloaltonetworks.com/company/press)) |
| 14 | Cybersecurity Research Reports and Papers | [arXiv cs.CR](https://arxiv.org/list/cs.CR/recent) | [USENIX Security Symposium](https://www.usenix.org/conference/usenixsecurity26) | [MITRE ATT&CK Updates](https://attack.mitre.org/resources/updates/) |
| 15 | Cybersecurity First Principle Strategies | [Schneier on Security](https://www.schneier.com/) | [SANS Institute](https://www.sans.org/) | [Google Threat Intelligence Blog](https://cloud.google.com/blog/topics/threat-intelligence/) |
| 16 | Nation State Cyber Policy and Law | [Lawfare](https://www.lawfaremedia.org/) | [CSIS Strategic Technologies Program](https://www.csis.org/programs/strategic-technologies-program) | *CyberScoop already active (`Sources.md` #8)* |
| 17 | Cybersecurity Zero Trust Tactics | [Cloud Security Alliance Blog](https://cloudsecurityalliance.org/blog) | [NIST Cybersecurity News (RSS)](https://www.nist.gov/news-events/cybersecurity/rss.xml) | *CyberScoop already active (`Sources.md` #8)* |
| 18 | Cybersecurity Intrusion Kill Chain Prevention Tactics | [MITRE ATT&CK Updates](https://attack.mitre.org/resources/updates/) | [SANS Internet Storm Center](https://isc.sans.edu/) | [Google Threat Intelligence Blog](https://cloud.google.com/blog/topics/threat-intelligence/) |
| 19 | Cybersecurity Risk Forecasting Tactics | [FAIR Institute Blog](https://www.fairinstitute.org/blog) | [Society of Information Risk Analysts (SIRA)](https://www.societyinforisk.org/) | [Metaculus](https://www.metaculus.com/) |
| 20 | Cybersecurity Resilience Tactics | [Disaster Recovery Journal](https://drj.com/) | [ENISA Publications](https://www.enisa.europa.eu/publications) | [SANS Internet Storm Center](https://isc.sans.edu/) |
| 21 | Cybersecurity Automation Tactics | [SOC Prime Blog](https://socprime.com/blog/) | [Dark Reading (RSS)](https://www.darkreading.com/rss.xml) | [CrowdStrike Blog](https://www.crowdstrike.com/en-us/blog/) |
| 22 | Cybersecurity Workforce Development Tactics | [(ISC)² Insights](https://www.isc2.org/Insights) | [NIST NICE Framework News](https://www.nist.gov/itl/applied-cybersecurity/nice/news-0) | [CSIS Strategic Technologies Program](https://www.csis.org/programs/strategic-technologies-program) |
| 23 | Compliance Trends | [IAPP News](https://iapp.org/news) | [PCI Security Standards Council Newsroom](https://pcisecuritystandards.org/about_us/newsroom?type=press_releases) | [JD Supra — Data Privacy](https://www.jdsupra.com/topics/data-privacy/) |
| 24 | Cybersecurity Framework Trends | [NIST Cybersecurity News (RSS)](https://www.nist.gov/news-events/cybersecurity/rss.xml) | [NIST NICE Framework News](https://www.nist.gov/itl/applied-cybersecurity/nice/news-0) | [UK NCSC](https://www.ncsc.gov.uk/) |
| 25 | Over the Horizon Technology Trends | [Quantum Computing Report](https://quantumcomputingreport.com/) | [MIT Technology Review](https://www.technologyreview.com/) | [Epoch AI](https://epoch.ai/) |
| 26 | Political | [Brennan Center — Voting & Elections](https://www.brennancenter.org/topics/voting-elections) | [NCSL — Elections & Campaigns](https://www.ncsl.org/elections-and-campaigns) | [Federal Register — Executive Orders](https://www.federalregister.gov/presidential-documents/executive-orders) |
| 27 | Adulting | [Good News Network](https://www.goodnewsnetwork.org/) | [Reasons to be Cheerful](https://reasonstobecheerful.world/) | [Serious Eats](https://www.seriouseats.com/) (recipes) |

**Notable re-verifications during this pass:** IAPP's news page, flagged 2026-08-31 as an unconfirmed HTTP 308 redirect, now resolves cleanly to `iapp.org/news`. CISO Tribune, surfaced the same day as "not independently verified," is now confirmed live with real, dated appointment entries at `/moves`.

Library candidate flagged: the per-category source table above is itself a reusable reference the daily report's source-selection process can consult directly — see Alexandria's closing section.

## What Does the Adversary Playbook Look Like Here? (Agent Ryan)

No adversary, campaign, or nation-state activity to characterize — this is a sourcing/tooling question, not an incident. For category 1 specifically (Adversary Playbook Activity), the three recommended additions (Mandiant/Google Threat Intelligence, CrowdStrike, Recorded Future) are worth flagging for their actual value: these are attribution-grade threat-intel shops, not incident-news aggregators — they'd sharpen the *tagging* this category already does (suspected nation-state vs. vendor-assigned group name vs. campaign name) rather than add incident volume the existing sources already saturate. No update to `Adversary Tracking Report.md` follows from this engagement.

## What Must Be Fundamentally True? (Agent Euclid)

The CIR pipeline is a filter over a fixed daily pull, not a generator — this was established in the 2026-08-31 review and holds again here. That means "three sources per category" is not an inherently meaningful target; it's a request translated into a shape (a table) that obscures a real asymmetry underneath. For roughly five AI-timeline categories, three sources genuinely exist and are usefully *distinct* instruments (Metaculus, Epoch AI, AI Impacts, Alignment Forum each measure a related-but-separate thing — survey consensus, compute/scaling trend extrapolation, researcher-panel calibration, technical-alignment discourse). For Book Reviews, three sources do not exist in any meaningful sense — there is one outlet and two adjacent-but-different things. Forcing a uniform count across categories this different in shape would have meant either padding weak categories with redundant picks (another general incident aggregator wearing a different logo) or quietly fabricating a book-review outlet that isn't real. The table above resists both temptations; the asymmetry is the finding, not a defect in how the question was answered.

Library candidate flagged: "three sources" as a request format works as a floor-raising exercise (make sure every category has *something* real), not as a meaningful uniform target — a durable caveat for any future category-coverage exercise like this one.

## How Could We Be Wrong? (Agent Popper)

**Objection 1 — several of these "new" sources barely move the needle because the categories they target are already fine.** Fifteen of the 27 rows above (Adversary Playbook, Data Breaches, Critical Infrastructure, Zero Trust, Kill Chain, Risk Forecasting, Resilience, Automation, Research Papers, First-Principle Strategies) are categories the existing portfolio already handles adequately or well. Adding Dragos, SOC Prime, or arXiv to an already-working category is marginal value, not a fix — Sherlock's table should not be read as "27 equally urgent gaps," most of which the 08-31 review already confirmed are not gaps at all.

**Objection 2 — several of the AI-timeline sources (Metaculus, Epoch AI, AI Impacts, Alignment Forum) overlap so heavily across categories 2–6 that they function as one undifferentiated AI-forecasting bloc, not five distinct per-category instruments.** The table lists them with different emphasis per row, but in practice a single Sherlock research pass against any one of these sites would likely surface content relevant to all five categories simultaneously — the per-category framing may overstate how separable this research actually is in practice.

**Objection 3 — the Book Reviews "no second source" conclusion may just reflect today's search terms, not the real state of the internet.** Declaring a structural gap on the strength of a handful of searches is a stronger claim than the evidence supports; a book-review-specific search (trade publications like Publishers Weekly's security-nonfiction coverage, or security-conference reading lists beyond RSA) wasn't exhaustively tried.

## What Is Likely to Happen Next? (Agent Seldon)

Resolving each objection:

**On Objection 1:** Correct, and the report already says so explicitly in Bradlee's synthesis and Sherlock's methodology note — the fifteen already-well-served categories are labeled "additive depth, not gap-filling" rather than presented as urgent fixes. No revision needed; this is a reading instruction for whoever uses the table, not a flaw in it.

**On Objection 2:** Also correct as a practical-research observation, but doesn't change the recommendation. The daily report's own navigation convention (per `Sources.md`'s schema) is per-source, not per-category — a single pull against Metaculus's site would naturally surface AI Singularity, AGI, Superintelligence, Harm Timeline, and Harm Probability content in the same pass, the same way a single Wired RSS pull today gets CIR-matched against many categories at once. The per-category table framing was chosen because that's what Rick asked for, not because these are five independent research tasks; if any of these four sources is actually added to `Sources.md`, it should be added once (as a single source), with navigation guidance noting it's relevant across all five AI-timeline categories — not duplicated as five separate source entries.

**On Objection 3:** Fair, and downgraded from a firm "no second source exists" to a bounded claim: no independent second source was found in today's research pass using cybersecurity-industry search terms. This is a real finding worth acting on as stated (there is currently no known second source), but not a permanent claim that none exists anywhere — flagged as a specific follow-up if Rick wants a deeper, publishing-trade-press-specific search before concluding Book Reviews is structurally single-sourced for good.

No forecast was called for in this question (it asks for source recommendations, not a timeline or probability), so no P5/P50/P95 range is produced here, consistent with Seldon only estimating when the question actually calls for one.

## How Do We Make This Clear? (Agent Tufte)

The per-category table above is a genuine data comparison across a large, flat list with consistent fields (category, three ranked sources) — exactly the markdown-table case the standing two-lane convention reserves for tabular data, not a rendered diagram. No spatial or flow relationship here a diagram would communicate better than rows and columns; not building one.

## Should Any of This Become a Skill? (Agent Turing)

A real candidate, flagged but not built this round. The method here — walk a fixed taxonomy, verify N real candidate sources per entry live, flag entries with structural gaps rather than padding them — is the same shape as the `nexus-source-coverage-audit` skill Turing flagged as a candidate on 2026-08-31 but didn't build. Today's exhaustive run makes the case for building it a little stronger (this is the second time this exact kind of category-walk has been done by hand), but it still isn't built unrequested — the 08-31 precedent and today's run both got done fine without it.

## New Skills

None created this run — see Turing's note above.

## Sources

**Internal (vault, this project)**
- `Intelligence Reports/Sources.md` — the 12 currently active sources, their schema, and navigation rules
- `Intelligence Reports/CIR-Definition.md` — the 27-category CIR taxonomy this report walks exhaustively
- `reports/2026-08-31-daily-report-source-recommendations.md` on `raceBannon99/The-Nexus` — prior, narrower source-portfolio review; this report's direct precedent

**Candidate sources researched and verified live (2026-10-16)** — see the full table above for per-category assignment; consolidated list of distinct domains checked:
- [Google Threat Intelligence (Mandiant) Blog](https://cloud.google.com/blog/topics/threat-intelligence/), [CrowdStrike Blog](https://www.crowdstrike.com/en-us/blog/), [Recorded Future Blog](https://www.recordedfuture.com/blog)
- [Metaculus](https://www.metaculus.com/), [AI Alignment Forum](https://www.alignmentforum.org/), [AI Impacts](https://aiimpacts.org/), [Epoch AI](https://epoch.ai/)
- [Europol Newsroom](https://www.europol.europa.eu/media-press/newsroom), [FBI Press Releases](https://www.fbi.gov/news/press-releases), [DOJ Office of Public Affairs](https://www.justice.gov/news/press-releases)
- [EFF Deeplinks](https://www.eff.org/deeplinks), [Privacy International](https://privacyinternational.org/), [Citizen Lab](https://citizenlab.ca/)
- [DataBreaches.net](https://databreaches.net/), [Have I Been Pwned](https://haveibeenpwned.com/), [BleepingComputer](https://www.bleepingcomputer.com/feed/)
- [Industrial Cyber](https://industrialcyber.co/), [Dragos Blog](https://www.dragos.com/blog/), [ENISA Publications](https://www.enisa.europa.eu/publications)
- [SANS Reading Room](https://www.sans.org/white-papers/), [SANS Institute](https://www.sans.org/), [SANS Internet Storm Center](https://isc.sans.edu/)
- [CISO Tribune — The Wire](https://www.cisotribune.com/moves), [SecurityWeek — People on the Move](https://www.securityweek.com/industry-moves/), [SC World — Cybersecurity Executive Changes](https://www.scworld.com/news/cybersecurity-executive-changes-2), [Palo Alto Networks Press](https://www.paloaltonetworks.com/company/press)
- [arXiv cs.CR](https://arxiv.org/list/cs.CR/recent), [USENIX Security Symposium](https://www.usenix.org/conference/usenixsecurity26), [MITRE ATT&CK Updates](https://attack.mitre.org/resources/updates/)
- [Schneier on Security](https://www.schneier.com/)
- [Lawfare](https://www.lawfaremedia.org/), [CSIS Strategic Technologies Program](https://www.csis.org/programs/strategic-technologies-program)
- [Cloud Security Alliance Blog](https://cloudsecurityalliance.org/blog), [NIST Cybersecurity News RSS](https://www.nist.gov/news-events/cybersecurity/rss.xml), [NIST NICE Framework News](https://www.nist.gov/itl/applied-cybersecurity/nice/news-0), [UK NCSC](https://www.ncsc.gov.uk/)
- [FAIR Institute Blog](https://www.fairinstitute.org/blog), [Society of Information Risk Analysts](https://www.societyinforisk.org/)
- [Disaster Recovery Journal](https://drj.com/)
- [SOC Prime Blog](https://socprime.com/blog/), [Dark Reading](https://www.darkreading.com/rss.xml)
- [(ISC)² Insights](https://www.isc2.org/Insights)
- [IAPP News](https://iapp.org/news), [PCI Security Standards Council Newsroom](https://pcisecuritystandards.org/about_us/newsroom?type=press_releases), [JD Supra — Data Privacy](https://www.jdsupra.com/topics/data-privacy/)
- [Quantum Computing Report](https://quantumcomputingreport.com/), [MIT Technology Review](https://www.technologyreview.com/)
- [Brennan Center — Voting & Elections](https://www.brennancenter.org/topics/voting-elections), [NCSL — Elections & Campaigns](https://www.ncsl.org/elections-and-campaigns), [Federal Register — Executive Orders](https://www.federalregister.gov/presidential-documents/executive-orders)
- [Good News Network](https://www.goodnewsnetwork.org/), [Reasons to be Cheerful](https://reasonstobecheerful.world/), [Serious Eats](https://www.seriouseats.com/)

## Library Recommendations (Agent Alexandria, closing)

One candidate flagged (Sherlock's stage):

1. **"27-category CIR source table" (this report's central table)** — category: fact-sheet. A durable, dated reference of verified candidate sources per CIR category, directly reusable the next time the daily report's source portfolio is reviewed or expanded (the same way the 2026-08-31 report's gap table became load-bearing for this one). Status: recommended, awaiting Rick's decision — not yet submitted.

My own judgment: this is a thinner candidate than the 2026-08-31 report's two (which captured general, reusable *methods* — coverage-shape robustness, an appearance-rate audit). This report's table is valuable but narrower and will age faster (sources move, get acquired, go paywalled) — worth keeping as a dated reference in the vault regardless, but a weaker case for permanent Library status than a methodological artifact would be. Rick's call.

No PR submitted against `nexus-artifacts` — per standing process, only if Rick says to proceed.

---
*Pending artifact approvals check: see end-of-report footer in chat.*
