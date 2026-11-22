# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Sunday, Nov. 22. Covers everything published after the 11-21 run. 5 of 29 sources contributed, a typical weekend. The headlines: the FBI is investigating an apparent hack of the National Crime Information Center, the criminal-justice database police query at traffic stops; Dragos seeded two million prompts with canary credentials and found three AI inference providers breached for months, with prompts marked "zero data retention" kept, passed on, and read by people (OpenRouter dropped three providers); a joint House report says PLA cyber-unit personnel have visited Zhipu and that the PLA is building Chinese open-weight models into its cyber ranges, and warns US companies off those models; GAO finds 17 of 22 major agencies short on zero-trust planning; Japan's two largest insurers report cyber claims running 2.5 to 3 times normal; and WIRED pulls the patch-driven outage story together. No forecast range moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Nothing matched AGI Arrival Timeline today. Considered and filed elsewhere: the House committees' report that Chinese labs close the gap by harvesting US model outputs (*Source:* two committee chairmen drawing on hearings, classified briefings, and company documents, Commentary/advocacy with documentary support; *Effect:* none, since copying capability bears on who holds frontier systems, not when one first matches broad human performance); WIRED's count of 100,000+ vulnerabilities recorded in 2026 (*Source:* public tallies via WIRED, Measured result; *Effect:* none, a narrow task at scale).

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Nothing matched AI Singularity Timeline today. Considered: Dragos's inference-provider research (*Source:* Dragos's two-million-prompt canary experiment, Measured result; *Effect:* none, since every actor is a human stealing data or directing ARTEX, which is misuse, not loss of control) and the PLA procurement records in the House report (*Source:* as above; *Effect:* none, human-directed offensive use already tracked in the Adversary Tracking Report).

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched Superintelligence Timeline today.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today; the day's AI items concern human misuse (*Effect:* none on this file's conditional).

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 2 new rows and 2 rows updated. Active campaigns: 443, up from 441. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-22-adversary-tracking-report.md).*

**The FBI is investigating an apparent hack of the National Crime Information Center.** NCIC is the FBI-run database of fugitives, missing persons, criminal histories, warrants, and stolen property that local, state, and federal agencies query, including at traffic stops. CNN reported it first; one person familiar with the matter confirmed it to the AP, and the BBC cites two. The scope isn't clear and the FBI declined to comment. Asked on Fox News, President Trump said "We just heard about it, and I will say that it's not good." There's no sign it's tied to the November outages. The bureau's jobs portal and employee data (claimed by ShinyHunters in September) and an internal system holding surveillance-related information (March) were hit earlier this year. New Unclear row 153 (Tier 3). [SecurityWeek (AP)](https://www.securityweek.com/fbi-investigating-apparent-hack-of-its-key-national-criminal-justice-database-ap-source-says/); [BBC](https://www.bbc.com/news/articles/cvze7de86pk3o)

**Dragos: three AI inference providers were breached for months, and none knew.** Between July and November, researchers seeded about two million prompts with unique web links and credentials, then watched for anyone using them. The earliest breach began in mid-July. At one provider, every request sent during a few late-October windows was copied, including requests rejected before a model ran, so the attacker was copying traffic at its first point of arrival. Planted AWS keys were tested within hours: the thief listed S3 buckets, searched Secrets Manager and Parameter Store, and tried to create Bedrock keys and IAM users, driving tens of thousands of API calls. One attacker held two providers at once from a single rented server, and on Nov. 1 ran the ARTEX AI pentesting framework only to confirm stolen keys were still live (its user agents, artex-agent and artex-judge-r121, appear in no public indicator list). Railway had said in October that its intrusion was likely part of a series aimed at inference providers, so Ryan treats this as a continuation of Black October. OpenRouter removed three providers and pulled 125 endpoints from Zero Data Retention eligibility; Phala and Together AI have disclosed incidents, but neither Dragos nor OpenRouter names the three, so those links are unconfirmed. Update to Cybercrime row 128 (🤖, Tier 3). [The Hacker News](https://thehackernews.com/2026/11/openrouter-drops-3-providers-after.html); [Ars Technica](https://arstechnica.com/security/2026/11/a-leaky-ai-supply-chain-is-exposing-secret-user-data-at-an-alarming-rate/) (via Global Frequency)

**House report: PLA cyber-unit personnel visited Zhipu, and the PLA is building Chinese models into its cyber ranges.** The House Homeland Security Committee and Select Committee on China say personnel tied to the 1st Bureau of the PLA Cyberspace Force, its cyber-espionage and attack unit, were present at Zhipu's Beijing headquarters several times, most recently in August. PLA procurement records show a July 2026 cyber range that required DeepSeek for "intelligent attack" and "intelligent penetration," a command system built on Qwen and DeepSeek, and an air-gapped project using DeepSeek, Alibaba, Moonshot, and MiniMax models for military AI agents. The same model families run inside US companies. Update to China row 19 (Tier 1). [House Select Committee on China](https://chinaselectcommittee.house.gov/media/press-releases/joint-investigation-report-china-is-trying-to-get-us-companies-addicted-to-chinese-ai-models); [The Record](https://therecord.media/chinese-open-weight-AI-use-by-US-companies-house-investigation)

**Iran-linked hackers posed as a US think-tank expert to target an Australian broadcaster.** Erin Molan says the head of ASIO, Australia's domestic intelligence agency, told her she was one of three Australians targeted. No group named and no technical detail; the approach resembles APT42's think-tank lures, but the reporting doesn't make that link. New Iran row 21 (Tier 3). [Iran International](https://www.iranintl.com/en/202611204601) (via Google Alert)

## Law Enforcement Disruption

**FBI agents posed as both ransomware victim and attacker to catch a recovery firm allegedly in the middle.** Prosecutors say a Florida company run by Juan Ricardo Palacio Escobar and an unnamed associate, operating since 2020, claimed to offer data-recovery services to ransomware victims; the undercover operation targeted it from both sides. The rest of the story is paywalled, so the alleged scheme isn't detailed here. [404 Media](https://www.404media.co/ransomware-fraud-attack-fbi-indictment/) (with Court Watch; via Global Frequency)

**Delhi Police arrest 22 across four states in a malicious-APK fraud crackdown.** Raids from Nov. 11 to 15 in Jharkhand (including Jamtara), Uttar Pradesh, West Bengal, and Bihar hit 11 fraud groups linked to 22,139 victims and more than Rs 20 crore in losses, and turned up a network of developers and distributors building malicious Android apps. The groups posed as bank officials, often targeting seniors with fake life-certificate and KYC help. [Deccan Chronicle (PTI)](https://www.deccanchronicle.com/nation/delhi-police-arrest-22-in-cybercrime-network-that-duped-22000-via-malware-2006641) (via Google Alert)

**Dutch police thwart "attempts at violence" against Revolut customers after its September data theft.** The National Police say several arrests can be linked to the theft. It's unclear who was targeted; WIRED notes the rise in physical "wrench attacks" on wealthy crypto holders. [WIRED, Kernel Panic](https://www.wired.com/story/brace-yourself-for-years-of-outage-chaos/)

## Cyber Crime & Fraud

**Japan's largest insurers report cyber claims at 2.5 to 3 times normal.** Tokio Marine received three times its usual cyber-claim notifications in October and Sompo about 2.5 times, both told earnings briefings, with Sompo saying requests to raise coverage have tripled. They blame more sophisticated, AI-driven attacks and a string of data leaks. Payouts haven't hit earnings yet; Tokio Marine may cap payouts or tighten terms by risk profile. Only 8.8% of Japanese small and medium businesses carry cyber insurance. [The Star (Bloomberg)](https://www.thestar.com.my/tech/tech-news/2026/11/22/cyberattacks-drive-claims-surge-at-japan-insurers) (via Google Alert)

**Binance wins a $6.5 billion worldwide freezing order over its record October hack.** The Abu Dhabi Global Market Courts' orders target the unidentified attackers, can be served to wallet addresses on-chain, and come with a "living list" of 26,000 wallets holding stolen assets. The figure isn't a recovery tally; DOJ has separately moved to seize more than $1.2 billion. Published Nov. 18; first captured here. [Cointelegraph](https://cointelegraph.com/news/binance-says-won-65b-worldwide-freezing-order-after-hack) (via Global Frequency)

## Data Breaches

**The FBI is investigating an apparent hack of the National Crime Information Center.** [SecurityWeek (AP)](https://www.securityweek.com/fbi-investigating-apparent-hack-of-its-key-national-criminal-justice-database-ap-source-says/) *Also covered above under Adversary Playbook.*

**Dragos: three AI inference providers were breached for months, and none knew.** [The Hacker News](https://thehackernews.com/2026/11/openrouter-drops-3-providers-after.html) *Also covered above under Adversary Playbook.*

## Zero Trust Tactics

**GAO: 17 of 22 major agencies haven't fully addressed zero-trust planning guidance.** Only five had, as of August; GAO issued 40 recommendations. HHS got six, the most, for lacking a department-wide zero-trust plan; Commerce blamed staffing losses on its working group, and DHS and DOJ cited the shutdown and resource limits for incomplete assessments of high-value systems. Eleven agencies only partly documented how they identify actors in their environments, including non-person entities such as service accounts. Thirteen agreed with the recommendations; four neither agreed nor disagreed. [Fox News](https://www.foxnews.com/politics/17-major-federal-agencies-flagged-cybersecurity-gaps-watchdog-warns-increased-attack-risk) (summarizing the GAO report; via Google Alert)

**A Ghostscript sandbox escape reaches servers through ordinary upload, preview, and print features.** CVE-2026-125396, a use-after-free in font loading, switches off Ghostscript's -dSAFER sandbox. pwn.ai ran commands on servers through about ten applications, several with no login: an anonymous print job to a Debian 13 queue, an attachment Roundcube processed when opened, and public upload forms in the Forminator and Essential Addons for Elementor WordPress plugins. Image libraries such as ImageMagick, Pillow, and libvips hand PostScript to Ghostscript even when a file is named .png or .pdf. Fixed in 10.08.0 on Sept. 8; no attacks reported. [The Hacker News](https://thehackernews.com/2026/11/researchers-demonstrate-ghostscript.html)

## Privacy

**Prompts marked "zero data retention" were kept, passed on, and read by people.** Beyond the provider breaches above, Dragos found inference-marketplace sellers listing models at the lowest price, logging requests, and harvesting what came through; one, on home broadband in France, typed root SSH logins by hand with passwords taken from prompts. An unnamed Chinese AI lab fetched the secret links from more than half the seeded prompts sent to its models, including about two-thirds of those marked no-collection or Zero Data Retention, and prompts sent to US resellers of its models triggered the same scraper. One secret link turned up in a Feishu chat 24 days later and was opened within two minutes from six devices in Beijing and Shanghai. Dragos's advice: a privacy flag binds only the first hop, so choose upstream providers yourself, avoid reseller marketplaces, and seed canary credentials as tripwires. [The Hacker News](https://thehackernews.com/2026/11/openrouter-drops-3-providers-after.html)

## Critical Infrastructure Attacks

**The FBI is investigating an apparent hack of the National Crime Information Center.** [SecurityWeek (AP)](https://www.securityweek.com/fbi-investigating-apparent-hack-of-its-key-national-criminal-justice-database-ap-source-says/) *Also covered above under Adversary Playbook.*

## Executive Leadership Changes

**The White House formally announces Kirsten Davies as national cyber director.** It says she will drive an "America First" cyber strategy. This confirms the 11-20 reports covered yesterday, which described her as acting director; the post still needs Senate confirmation. [SecurityWeek](https://www.securityweek.com/president-trump-taps-kirsten-davies-as-national-cyber-director/)

## Nation-State Cyber Policy & Law

**House chairmen warn US companies off Chinese open-weight AI models.** The 50-page report from Reps. Andrew Garbarino and John Moolenaar uses Airbnb, DoorDash, and Anysphere (Cursor's owner) as examples of firms running Chinese models for customer service, coding, and inventory. It argues the models are cheap, customizable, and near-frontier partly because Chinese developers "used proxy networks and fraudulent accounts to harvest outputs from American frontier models," warns that removing them later would be a Huawei-style rip-and-replace, and makes 12 recommendations, including an American open-weight initiative, a model-provenance standard and AI bill of materials, and keeping Chinese models out of federal contract work and high-risk critical-infrastructure functions. [The Record](https://therecord.media/chinese-open-weight-AI-use-by-US-companies-house-investigation); [House Select Committee on China](https://chinaselectcommittee.house.gov/media/press-releases/joint-investigation-report-china-is-trying-to-get-us-companies-addicted-to-chinese-ai-models) *The PLA findings are covered above under Adversary Playbook.*

## Resilience Tactics

**WIRED: the outages are just getting started.** The Kernel Panic newsletter rules out a coordinated AI hacking spree but says researchers increasingly see AI pressure behind real failures: AI-found bugs force patching faster than teams can test. More than 100,000 vulnerabilities have been recorded so far in 2026, against about 25,000 in 2022, yet only about 300 reached CISA's KEV catalog (VulnCheck counts about 1,500, 1.5% of the total). Dataminr's Joe Slowik says turnaround times now "completely defeat the ability to do patch verification"; Satya Nadella warned of more "instability"; Cloudflare's Matthew Prince predicts "it's going to feel like the sky is falling for two years" before defenders catch up. [WIRED](https://www.wired.com/story/brace-yourself-for-years-of-outage-chaos/)

*Newsletter Tracker: Thread 3, ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience) (Aug 2025), status Holding. Bearing: **Supports.** If only about 1.5% of flaws are ever exploited, most of the patch rush is prevention spending on bugs nobody uses, and the rush itself is breaking availability, the cost the thread predicts. Continues the 11-19 and 11-21 entries; status unchanged.*

## Compliance Trends

**UK regulators consult on cyber-risk guidance for financial firms.** The Prudential Regulation Authority, Financial Conduct Authority, and Bank of England published a joint consultation on cyber risk and resilience management, proposing guidance rather than new rules on meeting existing requirements, plus nonbinding practice papers on AI and quantum computing. PRA chief Katharine Braddick separately said supervisors will give "materially greater weight" to cyber and operational risk. [Bank Policy Institute, BPInsights Nov. 21](https://bpi.com/bpinsights-november-21-2026/) (a summary; the regulators' own notice wasn't fetched; via Google Alert)

---

### Pending Evidence Queue

Nothing queued: every row in the Pending Evidence Queue was already marked Included before this run.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 72 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 57 | 30 | 2026-07-14 |
| The Hacker News | Contributed | 86 | 1 | 2026-07-14 |
| The Record | Contributed | 68 | 19 | 2026-07-14 |
| The Canon Project | No Contribution | 19 | 67 | 2026-07-14 |
| FFX Now | No Contribution | 17 | 70 | 2026-07-14 |
| Wired | Contributed | 54 | 30 | 2026-07-20 |
| CyberScoop | No Contribution | 41 | 17 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 55 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 27 | 31 | 2026-09-01 |
| SecurityWeek | Contributed | 53 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 33 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 13 | 15 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 27 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 15 | 13 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 7 | 21 | 2026-10-17 |
| IAPP News | No Contribution | 18 | 10 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 4 | 24 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 20 | 2026-10-17 |
| Risky.Biz | No Contribution | 8 | 5 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 11 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 12 | 2026-11-10 |
| Resilient Cyber | No Contribution | 6 | 7 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 7 | 6 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 11 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 9 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 11 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 2 | 9 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 11 | 2026-11-12 |

**No contribution today:**
- **N2K CyberWire**: newest issue is Nov. 20, covered yesterday; no weekend issue.
- **The Canon Project**: newest reviews are Nov. 15, covered 11-16. (Read through Chrome MCP past a Cloudflare check.)
- **FFX Now**: nothing dated after Nov. 20 (covered yesterday).
- **CyberScoop**: only the Signal story, covered yesterday.
- **CSO Online CISO Appointments**: still no October or November section.
- **CISA**: newest advisory is the Nov. 20 KEV addition, covered yesterday.
- **LEAP**: newest is Wave 13, covered 11-19.
- **CISO Tribune**: newest entries are the Nov. 20 Davies and Cairncross moves, covered.
- **NIST Insights**: newest post Oct. 27.
- **EFF Deeplinks**: only the Section 702 post excluded yesterday as a recirculation.
- **(ISC)² Insights**: nothing since Nov. 20 (assessed 11-20).
- **IAPP**: newest items are Nov. 20, covered yesterday; the third (a Canada column on who decides what's true about you) has no CIR fit.
- **CSIS**: newest item is a Nov. 18 event listing. (Read through Chrome MCP past a Cloudflare check.)
- **AI Alignment Forum**: shortform comments only (including a thread on straight-line extrapolations of LLM progress); no new posts.
- **Risky.Biz, tl;dr sec, Detection Engineering Weekly**: no issue since Nov. 20, Nov. 19, and Nov. 12, all covered.
- **Resilient Cyber, Cybersecurity Dive**: nothing since Brief #123 and the Nov. 20 items, covered yesterday.
- **AI as Normal Technology, Epoch AI, Understanding AI**: nothing new in the window.
- **Reflective Altruism**: 1 post, "Deep utopia (Part 6: Saturday)," on Bostrom's account of the meaning of life; no AI-risk bearing.
- **Marcus on AI**: only the Nov. 20 share-price post, out of scope under its filter.

**Crediting notes:** SecurityWeek (site feed again; its email stream carried only the weekly Top Headlines, all covered) for the FBI NCIC story and the Davies announcement; The Hacker News for the Dragos/OpenRouter research and Ghostscript; The Record for the House open-weight AI report; WIRED for Kernel Panic (outages and the Revolut arrests); and Gmail (11 threads) for Google Alert digests (Japan's insurers, GAO's zero-trust audit, the UK consultation, the Molan impersonation, the Delhi arrests) and Matt Devost's Global Frequency (the FBI recovery-firm sting, Binance's freezing order). Gmail's search returned no snippets today, so candidate messages were opened one at a time. Ars Technica's "leaky AI supply chain" story, linked from Global Frequency, is the same Dragos research and is cited as corroboration only. **Recirculations excluded:** Paul Christiano's Hinton Lectures remarks (Futurism; covered 11-17 and 11-20); the Optimizely malware story (11-17 onward); California's suit against OpenAI over the Hugging Face hack (11-17, 11-18); GTIG's agentic-threat report (11-17); the NSA CAC-reader malware, Cairncross's exit, JPMorgan/Visa/Mastercard, the European Commission attack, and the VMware/Cisco/Apache KEV additions (all 11-19 to 11-21, resurfacing in Global Frequency and Google Alerts); The Hacker News's Muse, GPGME, Cairn, Signal, WhatsApp, Bazuka, KVM, and a16z items (11-20, 11-21); and SecurityWeek's Cairn, WhatsApp, In Other News, and Feedback Friday posts (11-21). **Considered, no CIR fit:** a Kaspersky briefing on threats in Pakistan (vendor statistics, with only a passing mention of Persian-speaking hacktivists), a CNN item on a feared Iranian dirty bomb (not cyber), and MiniMax's claim to have broken four old NIST post-quantum candidates (the summary page refused automated fetches; worth a look if it resurfaces with a primary source).

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
