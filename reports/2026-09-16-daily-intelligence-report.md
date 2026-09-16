# First Principles Daily Intelligence Report — September 16, 2026

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

**AI Singularity Timeline: P5 2027 · P50 2042 · P95 2100 (unchanged since 2026-09-14).**

## Government Surveillance

**[Hackers got inside a Flock camera. Its data shows how the system really works](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/)** (Wired, joint investigation with 404 Media) — A hacktivist collective calling itself **stegan0gram** physically removed a Flock Safety automated license-plate-reader camera from a roadway, extracted its on-device encryption key, and published roughly 21 days of the camera's logs and media — 1.6 million images, ~50,200 vehicles, and 27,321 video clips. Analysis of the dump confirmed the camera's software explicitly detects and logs people, not just license plates or vehicles, contradicting Flock's own public claims about what the device does and retains. Flock called the camera's removal "illegal" and disputed that the group has enough detail to properly assess its claimed vulnerability. *Also relevant to Adversary Playbook, below.*

**[County Board votes to end Arlington's use of Flock cameras](https://www.arlnow.com/2026/09/15/breaking-county-board-votes-to-end-arlingtons-use-of-flock-cameras/)** (ARLnow, via Gmail) — The Arlington County Board voted in closed session on September 15 to discontinue the county's use of Flock Safety automated license-plate-reader cameras, per sources cited by ARLnow — no public rationale had been given as of publication. Arlington joins a wave of jurisdictions (Florida, Texas, Los Angeles, Atlanta, and others, tracked in this report since 09-09) that have cut ties with Flock over the past several weeks.

**[Police are hiding their use of Flock surveillance cameras](https://www.schneier.com/blog/archives/2026/08/police-are-hiding-their-use-of-flock-surveillance-cameras.html)** (Schneier on Security, citing 404 Media; surfaced via Gmail's Crypto-Gram digest — originally published 08-18 and not previously captured in a daily report) — A Wapello County, Iowa police department's Flock ALPR usage policy instructs officers: "Do not mention ALPR usage to the occupants of the vehicle. Do not mention ALPR usage in your report or complaint unless absolutely necessary." The directive is part of a broader pattern 404 Media has documented of law-enforcement agencies deliberately concealing their reliance on automated license-plate-reader technology from the people it's used against.

**[Norway opens investigations into telecom Telenor's work with Myanmar's military junta](https://therecord.media/norway-investigations-telenor-telecom-myanmar-regime)** (The Record) — Norwegian police and the domestic security service PST opened crimes-against-humanity and sanctions-violation investigations into Telenor over the company's handling of customer data during its 2021–2022 exit from Myanmar, after the military junta seized power; Telenor's Oslo headquarters has been raided. The investigations focus on whether Telenor's compliance with junta data-handling demands facilitated surveillance or targeting of the company's Myanmar subscribers.

## Adversary Playbook

**Hacktivist collective "stegan0gram" physically extracts and publishes a Flock Safety camera's surveillance data** — *Full write-up above under Government Surveillance. The adversary angle: actor type Hacktivism, no nation-state affiliation claimed or evident; group name stegan0gram; no named ongoing campaign (a one-off device-level breach and disclosure); no malware (physical hardware compromise and firmware key extraction, not malware deployment); motivation privacy-activism/hacktivism; victim Flock Safety and the unnamed municipality operating the camera; disclosed 2026-09-16; attribution confidence Tier 1 (actors identified themselves directly, on the record, to the reporters).*

**[Iranian cyber spies used fake MRI scan results to hack an "enemy of the regime"](https://therecord.media/iran-cyber-spies-use-fake-mri-scans-as-lure)** (The Record, citing a joint UK NCSC/FBI/Dutch AIVD advisory) — A joint advisory describes **CHOSEN BRICK**, a Windows-only spyware implant with per-victim bot IDs and Telegram-based command-and-control, delivered via social-engineering lures including fake MRI scan results and fake Norton, Adobe, KeePass, and Telegram installers, deployed against dissidents, journalists, and activists in the UK, US, and Netherlands since 2025. The advisory's tradecraft description ties the operation to Iran's Ministry of Intelligence (MOIS) and the "Handala Hack" persona previously associated with "Homeland Justice"-branded activity, without formally naming a specific unit. Filed as a new Adversary Tracking Report row: actor type Nation-State-Affiliated (Iran); suspected group unattributed, tradecraft-linked to MOIS/Handala Hack; malware CHOSEN BRICK; motivation espionage; attribution confidence Tier 2.

**Leaked GRU recruitment-pipeline documents add institutional detail to the tracked Sandworm campaign** ([GBHackers](https://gbhackers.com/leaked-university-files/), surfaced via Schneier's Crypto-Gram digest) — Leaked documents from Bauman Moscow State Technical University describe a formal recruitment pipeline run by the GRU's General Staff Main Operational Directorate — specifically its 8th Directorate and a component called "Department No. 4" — funneling students into cyber and intelligence roles. The leak, reviewed by an international consortium including The Insider, The Guardian, and Le Monde, names a 2024 graduate, Aleksei Kondrashov, as linked to Military Unit 74455 — **Sandworm**, tracked in this report since 08-12. The disclosure adds institutional-recruitment context to the existing Sandworm row rather than a new technical campaign fact.

## AI Singularity Timeline

**AI Singularity Timeline: P5 2027 · P50 2042 · P95 2100 (unchanged since 2026-09-14).**

**["There's Now a Cyber Weapon Index"](https://www.defendersinitiative.com/p/theres-now-a-cyber-weapon-index)** (Defenders Initiative Substack, via Gmail) — Booz Allen has released the **Cyber Weapon Index (CWI)**, a two-part benchmark — a Vulnerability Research Score and a Kill Chain Attainment Score — tracking frontier AI models' progress toward autonomous, full-network-compromise capability with no human in the loop. The first test run had one model (Mythos) fully achieve domain-admin-level compromise; a second run less than a week later saw two models achieve full marks (adding GPT-6 Astra) and three more partially complete it, including China's open-weight GLM-5.2. The report's authors estimate all tested models will ace both benchmarks within six months.

**[China's spy chief warns of US AI models as a cyber threat](https://therecord.media/china-spy-chief-warns-of-us-ai-models)** (The Record) — Chen Yixin, head of China's Ministry of State Security, names Anthropic's Claude Mythos and OpenAI's GPT-5.5-Cyber as cyber risks to Chinese infrastructure in an essay published in a Cyberspace Administration of China journal — coming days after Anthropic's own threat report described a Chinese group ("undergraduates at a Hunan university") running autonomous vulnerability research using Claude. *Also relevant to Nation-State Cyber Policy & Law, below.*

**No range change today.** Neither item independently earns a shift. The Cyber Weapon Index is a genuinely new instrument — the first purpose-built benchmark in the Singularity Forecast Report's Evidence Log quantifying month-over-month progress toward autonomous full-network compromise — but its own six-month full-capability estimate lands inside the window Amodei's 6-12-month capability claim already priced into the 09-14 P5 shift to 2027, so it corroborates rather than extends that shift. Chen Yixin's essay is a policy and attribution statement about how a rival government characterizes US frontier models' risk, not new information about the models' own capability trajectory — logged for the record but not treated as forecast-moving evidence. Range holds at P5 2027 · P50 2042 · P95 2100. Full reasoning in the Singularity Forecast Report's Evidence Log.

## Data Breaches

**[CenterPoint Energy warns of data breach after dark-web post](https://therecord.media/centerpoint-energy-data-breach)** (The Record) — Texas utility CenterPoint Energy, which serves roughly 7 million customers, filed an SEC Form 8-K confirming a data breach after a dark-web actor claimed to be selling approximately 7.5 million records — names, partial Social Security numbers, and billing information — stolen via an external-facing system. CenterPoint says the breach caused no service impact and has not named the responsible actor. *Also relevant to Critical Infrastructure Attacks, below.*

## Critical Infrastructure Attacks

**CenterPoint Energy discloses breach of ~7.5 million customer records** — *Full write-up above under Data Breaches. The critical-infrastructure angle: CenterPoint is a major Texas electric and natural-gas utility; the breach was confined to a customer-data system and caused no disruption to grid or gas-delivery operations, but adds to this report's running count of utility-sector intrusions.*

## Cybersecurity Executive Leadership Changes

**[Zelensky appoints former police chief to lead Ukraine's cyber coordination center](https://therecord.media/ukraine-cyber-coordination-center-ihor-klymenko)** (The Record) — Ukrainian President Volodymyr Zelensky named Ihor Klymenko — formerly head of Ukraine's National Police and a former interior minister — to lead the country's National Cybersecurity Coordination Center, replacing Rustem Umerov, as part of a broader reshuffle of Ukraine's security leadership.

## Nation-State Cyber Policy & Law

**China's Ministry of State Security chief publicly names US frontier AI models as cyber threats** — *Full write-up above under AI Singularity Timeline. The policy angle: Chen Yixin's essay marks a rare public Chinese-government characterization of specific named US AI systems (Claude Mythos, GPT-5.5-Cyber) as offensive-cyber risks, coming as the two governments separately spar over Amodei's "Pace the Frontier" slowdown proposal and the joint NSA/CISA/FBI model-distillation advisory already tracked in the Adversary Tracking Report's China table.*

## Zero Trust Tactics

**[Attackers exploit WooCommerce Wholesale Lead Capture flaw to plant PHP web shells](https://thehackernews.com/2026/09/attackers-exploit-woocommerce-wholesale.html)** (The Hacker News) — A critical flaw (CVE-2026-27540, CVSS 9.8) in the WooCommerce Wholesale Lead Capture plugin, installed on 6,000+ WordPress sites, lets unauthenticated attackers upload PHP web shells for remote code execution. Wordfence has blocked over 100,000 exploitation attempts since June, including 99 in the past 24 hours. No adversary or campaign has been identified, so this does not get an Adversary Tracking Report row per that table's own no-identifiable-campaign rule.

## Cybersecurity Framework Trends

**[What's next for CISA's CDM program that gives cybersecurity tools to federal agencies](https://cyberscoop.com/whats-next-for-cisas-cdm-program-that-gives-cybersecurity-tools-to-federal-agencies/)** (CyberScoop) — Federal officials speaking at an Elastic Federal Cyber Defense Breakfast event discussed the future of CISA's Continuous Diagnostics and Mitigation (CDM) program, which supplies cybersecurity tooling to federal civilian agencies, amid ongoing questions about the program's funding and scope under the current administration.

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 33 | 7 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 34 | 7 | 2026-07-14 |
| The Hacker News | Contributed | 40 | 1 | 2026-07-14 |
| The Record | Contributed | 28 | 13 | 2026-07-14 |
| The Canon Project | No Contribution | 10 | 30 | 2026-07-14 |
| FFX Now | No Contribution | 4 | 37 | 2026-07-14 |
| Wired | Contributed | 23 | 15 | 2026-07-20 |
| CyberScoop | Contributed | 9 | 3 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 9 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 4 | 8 | 2026-09-01 |
| SecurityWeek | No Contribution | 10 | 2 | 2026-09-01 |

**No-contribution detail:**

- **N2K Cyberwire Daily Briefing** — Latest available issue, V15 Issue 175 (9.14.26), unchanged since yesterday's pull. All three of its stories (Amodei's "Pace the Frontier" essay, the OpenAI/RubyGems swarm attribution, the NSA five-mission-center reorganization) are already fully tracked in the Singularity Forecast Report and prior daily reports; no new issue has posted.
- **The Canon Project** — The two reviews published Sept 14 were already credited in the 09-15 report; nothing new published this week.
- **FFX Now** — Homepage still showing Sept 15 content (Daily Debrief, event listings) at pull time; nothing published yet for Sept 16.
- **CSO Online CISO Appointments** — September's running list unchanged since 09-07; all six listed appointments already credited.
- **CISA Cybersecurity Advisories** — All 8 items in the feed dated Sept 15 (a best-practices token-forgery resource document plus 7 routine ICS advisories); none carry an identifiable adversary or campaign link.
- **SecurityWeek** — Its two emails today were a recirculation of yesterday's already-credited Cisco Secure Email Gateway story and a promotional webinar invite; no exclusive SecurityWeek-sourced story had arrived at pull time.

*Pending artifact-repository approvals: none open at time of publishing (`gh pr list --repo raceBannon99/nexus-artifacts --state open` returned no results).*
