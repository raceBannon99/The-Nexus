# First Principles Daily Intelligence Report — August 13, 2026

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

## Summary

**Two reports already exist for August 12** — the regular daily report and a same-day supplemental "permissions test" pull ([reports/2026-08-12-daily-intelligence-report-permissions-test.md](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-08-12-daily-intelligence-report-permissions-test.md)), which Rick authorized as a live test of `bypassPermissions`. Both were checked during curation. Between them they already cover Microsoft's August Patch Tuesday, the UK ACRO criminal-records breach, and Wired's Boeing 737 hacking-device story — none of those are repeated here.

**Cyberwire's issue-listing page under-reported on the first WebFetch pass for a third run in a row** — it topped out at Issue 152 (8.11.26); a headless-Chrome cross-check found the real latest issue, 153 (8.12.26). Worth escalating if this keeps recurring every run.

**The `claude-in-chrome` extension is reachable again today** — paired cleanly, navigated multiple sites (The Record, Canon Project, Cyberwire) with no pairing failures, permission-denials, or screenshot errors. This contradicts the "ongoing outage" status in `Sources.md`'s Known Tooling Limitations (last updated 2026-08-04) and bugs #82879/#83959/#83960 — none confirmed fixed upstream, but the symptoms didn't reproduce in this run. Flagging as a status change rather than editing the bug tracker entries; worth a look if it regresses tomorrow.

**Four Record stories from August 11 were forward-pulled as first-capture.** No daily report ran 2026-08-11 (confirmed via GitHub), and the 08-12 morning pull explicitly saw these headlines on The Record's homepage but skipped them as "not today" — so they were never actually published anywhere. Included below with their real August 11 dates noted, same forward-pull precedent used for the 07-31 and 08-06 gap days.

**One story is a follow-up, not a first disclosure.** The AnMed hospital Facebook-hijack item below continues a malware incident The Record first reported in [the 2026-07-28 report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-28-daily-intelligence-report.md) — cross-referenced in place rather than presented as a new incident.

**Two candidate items were considered and rejected as no CIR match:** a Record story on the Kids Online Safety Act's stalled progress in Congress (privacy/platform-regulation policy, not core cybersecurity — the same judgment call the 08-12 report made on a similar Wired story), and a Pakistan FIA/NCCIA report of 374 Chinese nationals arrested in an immigration sweep that only glancingly mentioned "illegal call centres" with no cyber-fraud detail given.

**It's an early-in-the-day pull** — FFX Now (checked twice) and the Canon Project (no new review since the August 10 title already credited to 08-12) show nothing new yet for today specifically; today's report leans on stories dated August 11–13 that hadn't previously appeared in any report.

## Adversary Playbook

**[Researchers observe first "near-autonomous" AI attack on government target in Taiwan](https://cyberscoop.com/near-autonomous-ai-attack-government-target-taiwan/)** (CyberScoop, surfaced via a Gmail Google Alert digest) — Israeli cyber firm Dream reported suspected Chinese hackers used two open-source AI frameworks (Hermes and OpenClaw) to run a "near-autonomous" attack against the Taiwanese government, extracting more than 2,500 personnel records. The framework ran self-directed "Learning Cycles" — searching vulnerability databases and GitHub for applicable techniques without human direction — then expanded on its own from primary targets into government IT supply-chain vendors, a nuclear safety agency, a government email system, and 7+ energy companies. Dream says the system still required human tuning to build (Bayesian prioritization, self-correction logic), consistent with Anthropic's autonomous-espionage disclosure last fall, but the operation itself ran without a human in the loop once launched. *Also matches Automation Tactics — see below.*

**[FBI: Hackers using social engineering to breach accounts and steal explicit content](https://therecord.media/social-engineering-hackers-explicit-photos-fbi-alert)** (The Record) — An FBI notice released this week warns that hackers are breaking into adults' and children's social media accounts — via credential-stuffing, impersonating platform support staff to harvest password-reset codes, and cloned-login phishing sites — to steal and sell explicit content on criminal marketplaces, often alongside victims' personal information for harassment and sextortion.

**Ransomware group hijacks hospital system's Facebook page amid ongoing cyberattack fallout** (The Record, published August 11th) — Two weeks after AnMed's July 26 malware incident (first reported in [the 2026-07-28 report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-28-daily-intelligence-report.md)), a group calling itself "The Gentlemen" posted ransom demands on the nonprofit health system's hijacked Facebook page, claiming to have exfiltrated 6TB of data including sexual-assault, mental-health, and abortion records — unverified by AnMed. The Gentlemen is a ransomware-as-a-service operation active since late 2025, reportedly founded by a former Qilin affiliate, that claimed 332 victims in its first five months and the third-most industrial-sector attacks of any group in Q2 2026 per Dragos. *Also matches Critical Infrastructure Attacks and Data Breaches — see below.*

## Critical Infrastructure Attacks

**Ransomware group hijacks hospital system's Facebook page amid ongoing cyberattack fallout** (The Record, published August 11th) — *Full write-up above under Adversary Playbook. AnMed operates four hospitals and clinics across Georgia and South Carolina; ten facilities remained closed to appointments as of the most recent update.*

**Local governments in four states dealing with cyberattacks that have shut down services** (The Record, published August 11th) — Suisun City, California declared a state of emergency after malware knocked out 911 routing, police/fire dispatch, and city IT systems; the county dispatch center is routing emergency calls in the interim. In the same week, Coweta, Oklahoma (ransomware, all city computers affected), Mitchell, South Dakota (network shutdown, email systems spared), Coryell County, Texas, and Washburn County, Wisconsin (phone/fax and court-filing disruption) each disclosed separate incidents. The Record notes this cluster coincides with an ongoing string of water/wastewater-system attacks affecting at least 12 states.

**Patch Tuesday's ICS/OT vendor patches** (N2K Cyberwire Daily Briefing, Issue 153, 8.12.26 — no stable per-story permalink exists within a daily issue) — Beyond the Microsoft/Adobe/SAP fixes already covered in [the August 12 supplemental report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-08-12-daily-intelligence-report-permissions-test.md), this month's Patch Tuesday cycle also included Siemens, Schneider Electric, and Phoenix Contact updates for industrial-control products, plus CISA advisories covering additional ICS vendors including Pulsetto and Johnson Controls. Siemens' fix addressed a maximum-severity missing-authentication flaw in its Simatic IoT gateways.

## Government Surveillance

**[CBP Workers Allegedly Used Government Databases to Spy on Exes, Crushes, and Colleagues](https://www.wired.com/story/cbp-workers-allegedly-used-government-databases-to-spy-on-exes-crushes-and-colleagues/)** (Wired) — Reporting details Customs and Border Protection employees allegedly misusing access to law-enforcement databases to look up personal information on ex-partners, romantic interests, and coworkers rather than for official investigative purposes — the kind of insider-misuse case that recurs across federal law-enforcement database access, raising the same oversight questions as prior CBP/DHS database stories this project has tracked.

**[NSA installs DHS lawyer as new general counsel](https://therecord.media/kerianne-tobitsch-new-nsa-general-counsel)** (The Record, published August 11th) — Kerianne Tobitsch, previously a senior DHS lawyer, was confirmed as the NSA's general counsel effective June 15 — a post left vacant for roughly a year after her predecessor was fired following a conservative-media campaign. The general counsel oversees legal review of clandestine operations and is expected to play a role when Congress attempts to renew Section 702 of FISA, the warrantless-surveillance authority that lapsed in June.

## Data Breaches

**Ransomware group hijacks hospital system's Facebook page amid ongoing cyberattack fallout** (The Record, published August 11th) — *Full write-up above under Adversary Playbook. The Gentlemen's unverified claim of 6TB exfiltrated, including sexual-assault and abortion records, is the Data Breaches angle; no evidence has been provided to substantiate the claim.*

**[Cyberattack on logistics giant Ceva hits retailers and Steam customers across Europe](https://therecord.media/ceva-logistics-cyberattack-bol-steam-debijenkorf-ace-tate)** (The Record, published August 11th) — A breach at freight company Ceva Logistics compromised order-processing systems at eight European warehouses, exposing names, addresses, phone numbers, and order details for customers of Dutch e-commerce platform Bol, department store De Bijenkorf, eyewear retailer Ace & Tate, and Valve's Steam hardware business. Ceva has not disclosed the attack publicly or said who was behind it; Bol and Valve are separately notifying affected customers.

## Zero Trust Tactics

**[Attackers Exploit SharePoint Authentication Bypass After Public PoC Release](https://thehackernews.com/2026/08/attackers-exploit-sharepoint.html)** (Hacker News, corroborated by N2K Cyberwire Daily Briefing Issue 153) — Threat actors are actively exploiting CVE-2026-55040 (CVSS 9.1), a SharePoint Enterprise Server 2016/2019 authentication-bypass flaw in the JWT token validation pipeline, using a proof-of-concept Rapid7 published this week. Microsoft patched the flaw July 14 following Rapid7's responsible disclosure; unpatched on-premises administrators remain exposed.

**Visa and Deel both acquire identity verification companies** (N2K Cyberwire Daily Briefing, Issue 153, 8.12.26 — no stable per-story permalink exists within a daily issue) — Visa agreed to acquire Israeli biometric-verification firm BioCatch to bolster its fraud/account-takeover defenses. Separately, HR platform Deel acquired Israeli AI identity-verification startup Clarity, aiming to embed continuous identity verification across hiring and workforce management.

## Risk Forecasting Tactics

**[Human Error, Not AI Agents, Is Driving Cyber Losses So Far In 2026](https://riskandinsurance.com/human-error-not-ai-agents-is-driving-cyber-losses-so-far-in-2026/)** (Risk & Insurance, citing cyber insurer Resilience's Cyber Mid Year Risk Report, surfaced via a Gmail Google Alert digest) — Social engineering accounted for 85.3% of Resilience's incurred cyber-insurance losses in H1 2026, up from 17.7% in H1 2024, while zero claims in its portfolio traced to AI-specific attack vectors (prompt injection, model exploitation, agentic misuse) despite two documented "warning sign" incidents (an autonomous ransomware operation dubbed JADEPUFFER, and an OpenAI model that autonomously breached Hugging Face during a security test). Known-vulnerability exploitation fell to 7.0% of losses from a 25% 2024 peak even as Mandiant's M-Trends 2026 puts industry-wide mean time-to-exploit at negative seven days — exploitation often starts before a patch exists. Extortion remains the costliest cause of loss (73% of H1 2026 incurred losses from just 5.8% of claims); average claim severity fell to ~$470K.

## Automation Tactics

**Researchers observe first "near-autonomous" AI attack on government target in Taiwan** (CyberScoop, surfaced via a Gmail Google Alert digest) — *Also covered above under Adversary Playbook.*

## Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 14 | 3 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 18 | 0 | 2026-07-14 |
| The Hacker News | Contributed | 18 | 0 | 2026-07-14 |
| The Record | Contributed | 8 | 10 | 2026-07-14 |
| The Canon Project | No Contribution | 5 | 12 | 2026-07-14 |
| FFX Now | No Contribution | 3 | 15 | 2026-07-14 |
| Wired | Contributed | 7 | 8 | 2026-07-20 |

**No-contribution detail:**
- **The Canon Project** — page loaded cleanly via Chrome MCP (not an outage; headless-Chrome CLI hit a Cloudflare bot-challenge, but the browser extension worked). Only one August review exists so far — "Legal and Privacy Issues in Information Security (3rd Edition)," published August 10 — and it was already credited to the 2026-08-12 report as first-capture. Nothing new this cycle.
- **FFX Now** — checked twice (per the source's standing second-pass rule). Latest content is a sponsored apartment-leasing post from August 12; nothing published under today's date at pull time. Not an outage — the site loaded fully both times.
