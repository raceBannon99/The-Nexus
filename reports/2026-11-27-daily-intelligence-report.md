# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

## Summary

Date: Friday, November 27th, 2026\
Source Contribution: 8 of 30 sources contributed\
The Headlines:

- None of the five AI timeline forecasts changed.
- Switzerland confirmed its first attacks run by AI agents: four of five succeeded, two of them against critical-infrastructure operators.
- SAP is investigating attackers who used stolen employee tokens to copy and alter source code on GitHub.
- Todoist disclosed a breach that began with a stolen version-control credential and ended with attackers in its cloud infrastructure.
- A hacker steering a jailbroken DeepSeek agent stole ID-card and bank details for 1.2 million residents and staff of 82 Flemish municipalities.
- Britain's Department for Work and Pensions took online services offline after a cyber incident.
- The North Korea-linked PolinRider campaign has poisoned more than 7,600 GitHub repositories.

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 17 new rows and 1 row updated. Active campaigns: 506, up from 489. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-27-adversary-tracking-report.md).*

**Switzerland confirms its first AI-agent attacks; Italy reports the same pattern.** Switzerland's National Cyber Security Centre says attackers using "agentic offensive frameworks" (AI agents that find weaknesses, pick tools, and plan and execute next steps on their own) broke in at four of five organizations that reported in recent days. Three targeted critical-infrastructure operators in at least two sectors and two of those succeeded, with no major disruption; small and medium-sized firms were also hit. The agency says freely reachable tools such as ARTEX and CyberStrikeAI have nearly doubled since October (a count of tools, not attacks) and expects more successful attacks. CSIRT Italia's bulletin the same week describes AI-directed agents breaking into many systems within hours, chaining flaws, misconfigurations, and stolen credentials, and names ARTEX, CyberStrikeAI, PentAGI, and DeepSeek Harness. Advice from both: patch internet-facing systems within 24 hours, isolate what can't be patched, shrink exposure, put MFA or passkeys on everything reachable, and watch for behavioral deviation. Victims and attackers are unnamed. New Unclear row 186 (🤖, Tier 3). [Swiss NCSC](https://www.bacs.admin.ch/en/26-ki-agenten-1-en); [The Hacker News](https://thehackernews.com/2026/11/switzerland-confirms-ai-assisted.html); [CSIRT Italia](https://www.acn.gov.it/portale/w/impiego-di-agenti-di-ia-in-campagne-di-compromissione-automatizzate)

**SAP confirms a breach of its development infrastructure.** Der Spiegel's sources say attackers used stolen employee authentication tokens to copy and alter source code on GitHub, possibly with AI help (not confirmed). SAP says it has found no access to customer business data; it reportedly replaced signing keys, limited GitHub access, and paused automated development operations. Nothing suggests tampered code reached customers, and the incident appears unrelated to the Gentlemen ransomware group's October listing of SAP's Latin American operations. New Unclear row 187 (Tier 3). [SecurityWeek](https://www.securityweek.com/sap-confirms-cyberattack-source-code-reportedly-compromised/)

**Todoist: a stolen version-control credential led to its cloud.** On Nov. 22-23 an attacker used the credential to modify automated workflows in three repositories, harvest more credentials, take over an employee's account, and reach cloud infrastructure, reading source code along the way (no code changes found). They downloaded records for early users whose passwords still used salted SHA1, queried account tokens, searched customer content for credentials, and read email through Todoist for Outlook connections. Todoist's leading theory is a compromised employee device; it has now retired SHA1 support. New Unclear row 188 (Tier 3). [Todoist](https://www.todoist.com/help/todoist/get-started/security-incident-in-november-2026-cG0EIACNU) (via [Risky.Biz](https://news.risky.biz/risky-bulletin-hackers-breach-erlang-and-elixir-package-manager/))

**BabidiGhost stole the data of 1.2 million Flemish residents.** Secutec says the operator, tied to APT90 (also called Ghost Hunters), jailbroke DeepSeek to drive a Hermes agent that wrote its own scanners, exploits, and exfiltration tools; of 5,800-plus tasks it refused 41. The agent reached a shared IT provider's server that kept all 82 municipalities' data unsegmented and unencrypted, taking names, addresses, national-register and ID-card numbers, IBANs, and some license plates; data from at least one municipality has been sold. Secutec stresses how little skill the attacker needed. Update to Cybercrime row 151 (Tier 2; not tagged 🤖, since a human set each task). [Secutec](https://secutec.com/nl/nieuws/hackersgroep-ghost-hunters-steelt-de-persoonsgegevens-van-12-miljoen-vlamingen-uit-82) (via Risky.Biz)

**Britain's DWP takes services offline after a cyber incident.** The Department for Work and Pensions, the government's largest by spending, pulled several online services "as a precaution"; benefit and pension payments are unaffected. It is working with the NCSC and the Government Cyber Coordination Centre and hasn't described the incident. New Unclear row 190 (Tier 3). [The Record](https://therecord.media/uk-department-work-pensions-cyber-incident)

**PolinRider has poisoned more than 7,600 GitHub repositories.** Apiiro counts 7,609 compromised repos, 86% on established personal accounts, and dates the activity to as early as February 2025. SafeDep found a Python loader in 375 repos that reads an Ethereum wallet's self-sent transaction, runs it as JavaScript under Node.js, and locates its C2 through a second wallet; it hasn't appeared on PyPI or npm. The campaign also uses fake hiring portals (BlockNovas, AccuraSoftHire, HuntRole). New North Korea row 20 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/north-korea-linked-polinrider-poisons.html)

**Trojanized Q-Dir and DesktopOK installers on the official site.** AhnLab found poisoned installers for five versions served from SoftwareOK's own download page and through updates; they run the real program while fetching a Python RAT (shell and Python execution, file transfer, screenshots) that persists as a scheduled task posing as Microsoft Edge. How the files were swapped is unknown. New Unclear row 189 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-trojanize-official-q-dir-and.html)

**Chile's visa system breached through an October phishing email.** Officials suspect a criminal group selling visas and fake identities and have kept the system running to avoid stranding Chileans abroad. New Cybercrime row 157 (Tier 3). [El Mostrador](https://www.elmostrador.cl/unidad-de-investigacion/2026/11/22/hackeo-a-la-cancilleria-inteligencia-naval-comienza-a-indagar/) (via Risky.Biz)

**Zero-click spyware on Sea-Watch's Italian spokesperson.** Citizen Lab and Forenser conclude with high confidence that Giorgia Linardi's iPhone was infected at least seven times between May and August 2021, likely giving full access to files, messages, microphone, and location. The spyware can't be attributed; Sea-Watch notes zero-click tools are sold almost only to governments and has filed a complaint in Rome. New Unclear row 191 (Tier 3). [Sea-Watch](https://sea-watch.org/en/spyware-attack-on-sea-watch-spokesperson/) (via Risky.Biz)

**Ad networks fund pro-Russian disinformation sites.** A ten-month CheckFirst investigation with journalists from seven countries traced revenue from AdNow, AdsKeeper, and MGID to at least six networks of fake news-style sites, fed by 34-plus inauthentic Facebook pages pushing Ukraine-war and election narratives; AdNow-linked infrastructure connects to a sanctioned United Russia candidate's campaign. The operators weren't independently identified. New Unclear row 193 (Tier 3). [CheckFirst](https://checkfirst.network/poisoning-the-mind-following-ad-revenue-from-deceptive-websites-to-russias-ruling-party/) (via Risky.Biz)

**Azalea Agent RAT aimed at Ukrainian government bodies.** Seqrite describes a multi-stage spear-phishing chain delivering the .NET remote access trojan; no actor named. New Unclear row 192 (Tier 3). [Seqrite](https://www.seqrite.com/blog/from-phishing-email-to-azalea-agent-uncovering-a-multi-stage-attack-on-ukrainian-government-bodies/) (via Risky.Biz)

**UPS software used to reach a domain controller.** Symantec describes an attacker abusing CyberPower PowerPanel Business, which runs a script when it detects a power event, to execute code on a domain controller, dump Active Directory secrets, and plant a persistent implant. New Unclear row 194 (Tier 3). [The Hacker News (ThreatsDay)](https://thehackernews.com/2026/11/threatsday-250-rogue-extensions-10m.html)

**Turkey arrests two over alleged espionage against defense Wi-Fi networks.** The MIT intelligence agency says the suspects, detained in Ankara and Istanbul, worked for an unnamed foreign intelligence service against defense-industry and state wireless networks; coverage relays the official account only. New Unclear row 195 (Tier 3). [NewsCord](https://newscord.org/article/turkish-intelligence-arrests-two-suspects-over-alleged-cyber-espionage-against-d--Story_20261126_ab9af88a) (via Gmail)

**Malware and fraud kits named this week.** New Cybercrime rows, all Tier 3, all via Risky.Biz:
- **Keenadu and Triada** (Kaspersky): malware preinstalled on almost 680,000 phones and tablets this year, Keenadu on about a third. Row 158. [Kaspersky](https://securelist.com/tr/how-to-protect-against-preinstalled-android-malware/122093/)
- **MadApe** (Group-IB): a kit for device-code phishing of Microsoft 365 accounts. Row 159. [Group-IB](https://www.group-ib.com/blog/madape-the-code-that-opens-the-door/)
- **Vinci RAT** (eSentire): distributed through the Microsoft Store, which declined to remove it when reported. Row 160. [eSentire](https://www.esentire.com/blog/vinci-rat-lives-in-the-microsoft-store)
- **GodFather.Tech** (CloudSEK): an Android fraud kit sold by a Chinese-speaking developer, impersonating 182 banks in 56 countries and 38 crypto and payment platforms. Row 161. [CloudSEK](https://www.cloudsek.com/blog/182-banks-38-crypto-platforms-one-toolkit-the-godfather-tech-android-fraud-arsenal)
- **WalletGuard**: fake "leaked private key" issues on 200-plus crypto GitHub projects lured maintainers into moving funds; at least two fell for it. Row 162. [OpenSourceMalware](https://opensourcemalware.com/blog/walletguard-phishing-campaign)

## Cyber Crime & Fraud

**GodFather.Tech, MadApe, WalletGuard, and Vinci.** [Risky.Biz](https://news.risky.biz/risky-bulletin-hackers-breach-erlang-and-elixir-package-manager/) *Also covered above under Adversary Playbook.*

**DOJ's Scam Center Strike Force reports six months of results.** 17.3 million scam accounts deplatformed on Meta, 700 fraudulent crypto-investment sites seized, 12 US arrest warrants, and about $1.08 billion in stolen crypto traced and restrained. [The Hacker News (ThreatsDay)](https://thehackernews.com/2026/11/threatsday-250-rogue-extensions-10m.html)

**A Liberian romance scammer is extradited.** David Hardy, 39, was extradited from Côte d'Ivoire to Oregon, charged with taking more than $700,000 from US women he met on dating sites, in part by claiming Mexican cartels were holding his fictitious son for ransom. [DOJ](https://www.justice.gov/usao-or/pr/liberian-national-extradited-cote-divoire-face-charges-707000-oregon-romance-fraud) (via Risky.Biz)

**Keenadu and Triada preinstalled on ~680,000 devices.** [Kaspersky](https://securelist.com/tr/how-to-protect-against-preinstalled-android-malware/122093/) *Also covered above under Adversary Playbook.*

**Chile's visa-fraud breach.** [El Mostrador](https://www.elmostrador.cl/unidad-de-investigacion/2026/11/22/hackeo-a-la-cancilleria-inteligencia-naval-comienza-a-indagar/) *Also covered above under Adversary Playbook.*

## Zero Trust Tactics

**Unpatched Cacti zero-day: guest access to code execution in four requests.** A researcher's "4HTTP2SHELL" chain affects Cacti 1.2.31, the latest version, when the guest account is enabled (off by default since 0.8.7): an unvalidated preview setting becomes a second-order SQL injection that edits the poller table, and the realtime poller then passes that row to PHP's `popen()`. No CVE or patch yet; disable guest access. [The Hacker News](https://thehackernews.com/2026/11/unpatched-cacti-zero-day-enables-rce-in.html)

**NFS2ROOT: unauthenticated root on Linux NFS servers.** A kernel flaw (CVE-2026-99362, CVSS 9.8) exploitable in 61 bytes against exposed NFS ports affects every Linux version since 2014; it is patched, and blocking TCP 2049 stops attacks until then. [OpenSec](https://opensec.in/blog/nfs2root-cve-2026-99362) (via Risky.Biz; the OpenSec page didn't load through any fetch tier, so details rest on Risky Bulletin)

**Joomla's Easy File Uploader allows unauthenticated upload to RCE.** VulnCheck found the flaw in the extension. [VulnCheck](https://www.vulncheck.com/blog/easy-file-uploader-unauthenticated-upload-to-rce) (via Risky.Biz)

**Belgian police: rename default admin accounts on smart devices.** After the wave of supermarket refrigerator hacks done with default credentials, police told users to disable default admin accounts and create new ones with hard-to-guess names. [Belgian Federal Police](https://www.politie.be/5998/nl/nieuws/gehackte-koelkasten-hoe-bescherm-je-je-slimme-apparaten) (via Risky.Biz)

**Todoist's stolen version-control credential.** [Todoist](https://www.todoist.com/help/todoist/get-started/security-incident-in-november-2026-cG0EIACNU) *Also covered above under Adversary Playbook.*

## Law Enforcement Disruption

**Huawei convicted of sanctions violations, trade-secret theft, and money laundering.** After a three-month trial in the Eastern District of New York, a jury found Huawei and three subsidiaries (Huawei Device, Futurewei, and Huawei Device USA) guilty of a decades-long scheme that included supplying Iran through the front company SkyCom, lying to banks and Congress, and stealing secrets from US firms. [DOJ](https://www.justice.gov/opa/pr/chinese-tech-giant-huawei-and-subsidiaries-convicted-sanctions-violations-fraud-conspiracy) (via Risky.Biz)

**The Scam Center Strike Force's six-month tally.** [The Hacker News](https://thehackernews.com/2026/11/threatsday-250-rogue-extensions-10m.html) *Also covered above under Cyber Crime & Fraud.*

**David Hardy's extradition.** [DOJ](https://www.justice.gov/usao-or/pr/liberian-national-extradited-cote-divoire-face-charges-707000-oregon-romance-fraud) *Also covered above under Cyber Crime & Fraud.*

**Turkey's MIT arrests two alleged spies.** [NewsCord](https://newscord.org/article/turkish-intelligence-arrests-two-suspects-over-alleged-cyber-espionage-against-d--Story_20261126_ab9af88a) *Also covered above under Adversary Playbook.*

## Data Breaches

**SAP's GitHub source code.** [SecurityWeek](https://www.securityweek.com/sap-confirms-cyberattack-source-code-reportedly-compromised/) *Also covered above under Adversary Playbook.*

**Todoist's early-user password hashes and account tokens.** [Todoist](https://www.todoist.com/help/todoist/get-started/security-incident-in-november-2026-cG0EIACNU) *Also covered above under Adversary Playbook.*

**1.2 million Flemish residents' ID and bank data.** [Secutec](https://secutec.com/nl/nieuws/hackersgroep-ghost-hunters-steelt-de-persoonsgegevens-van-12-miljoen-vlamingen-uit-82) *Also covered above under Adversary Playbook.*

**Chile's visa system.** [El Mostrador](https://www.elmostrador.cl/unidad-de-investigacion/2026/11/22/hackeo-a-la-cancilleria-inteligencia-naval-comienza-a-indagar/) *Also covered above under Adversary Playbook.*

## Critical Infrastructure Attacks

**AI agents breach Swiss critical-infrastructure operators.** [Swiss NCSC](https://www.bacs.admin.ch/en/26-ki-agenten-1-en) *Also covered above under Adversary Playbook.*

**DWP services offline.** [The Record](https://therecord.media/uk-department-work-pensions-cyber-incident) *Also covered above under Adversary Playbook.*

**Belgium's advice after the refrigerator hacks.** [Belgian Federal Police](https://www.politie.be/5998/nl/nieuws/gehackte-koelkasten-hoe-bescherm-je-je-slimme-apparaten) *Also covered above under Zero Trust Tactics.*

## Government Surveillance

**Spyware victims in Europe face a legal labyrinth.** A CDT report finds that surveillance victims in Greece, Hungary, Poland, and Spain must work through barriers to redress, often against the same governments that spied on them. [CDT](https://cdt.org/insights/navigating-the-labyrinth-assessing-the-barriers-to-redress-for-victims-of-spyware-in-europe/) (via Risky.Biz)

**Sea-Watch spokesperson infected with zero-click spyware.** [Sea-Watch](https://sea-watch.org/en/spyware-attack-on-sea-watch-spokesperson/) *Also covered above under Adversary Playbook.*

## Nation-State Cyber Policy & Law

**Congress wants to regulate AI; its own machinery may stop it.** After the midterms gave Democrats wide majorities, both parties are pushing: chip-export limits on Chinese firms, likely attached to the defense bill and spurred by the Jensen Huang affair (Anthropic supports them; Nvidia declined comment); the Trahan-Obernolte safety bill, updated to protect the strictest state laws; proposals for model audits, data-center limits, third-party monitoring, and Sen. Ruben Gallego's ban on recursive self-improvement; and a possible special Senate AI committee. The obstacles are committee turf, Senate procedure, tech lobbying, and years of failed tech bills; Vanderbilt's Asad Ramzanali expects action only after a crisis such as an AI-agent cyberattack. [NYT](https://www.nytimes.com/2026/11/26/us/politics/ai-regulation-congress-nvidia.html) (queued by Rick; read from his vault clipping, since nytimes.com is paywalled. Huang testifies before the House next week, Dec. 1)

*Newsletter Tracker: Thread 5, ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house) (Oct 2026), status Under Pressure. Bearing: **Ambiguous.** The push is toward the binding rules the thread argues voluntary lab pledges can't replace, but nothing has passed, and "only after a crisis" is the thread's worry restated. Status unchanged.*

**Russia plans another state GitHub alternative.** The government wants a domestic code platform for critical software, its second try after sanctions cut access to Western tools; the first stalled without funding. [RBC](https://www.rbc.ru/technology_and_media/25/11/2026/6b06fd791335363210f4ff61) (via Risky.Biz)

## Intrusion Kill Chain Prevention Tactics

**Agent attacks are caught by context, not signatures.** CSIRT Italia says each agent action "looks like normal user or API traffic"; detection depends on where requests come from, how often they arrive, how much data moves, and in what order. The UK NCSC adds that the frameworks are noisy (bursts of requests, high error rates), and the agencies recommend bot challenges on high-value endpoints and honeytokens as decoys. [The Hacker News](https://thehackernews.com/2026/11/switzerland-confirms-ai-assisted.html); [CSIRT Italia](https://www.acn.gov.it/portale/w/impiego-di-agenti-di-ia-in-campagne-di-compromissione-automatizzate)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Supports.** Two more national agencies find that agentic attacks reuse known weaknesses and are caught by sequence and tempo, the procedure-level detection the thread says is now feasible. Status unchanged.*

**PowerPanel abuse to reach a domain controller.** [The Hacker News](https://thehackernews.com/2026/11/threatsday-250-rogue-extensions-10m.html) *Also covered above under Adversary Playbook.*

## Risk Forecasting Tactics

**Retail ransomware claims run 50% above average in November.** Insurance Business cites claims data from 2021-2025 showing ransomware against retail, leisure, and hospitality firms about 50% above the monthly average in November, while a survey of SMEs in the UK, US, Canada, and Australia finds only 43% of retailers carry cyber insurance, against 81% in financial services and manufacturing. [Insurance Business](https://www.insurancebusinessmag.com/uk/news/cyber/black-friday-ransomware-spike-exposes-retail-cyber-insurance-gap-598944.aspx) (via Gmail Google Alerts; the article doesn't name the claims-data source in the text read)

**Ransomware claims rose 23% in October.** NCC Group counts 1,049 claimed incidents, led by the Gentlemen, N0n, Qilin, Akira, and Silent Ransom; Check Point counted a record 2,830 victims in Q3 across 117 groups. Both count leak-site claims, not confirmed attacks. [The Hacker News (ThreatsDay)](https://thehackernews.com/2026/11/threatsday-250-rogue-extensions-10m.html)

## AI Singularity Timeline

**Current range:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17)

**"How to Talk to Your Family About A.I. Doom at Thanksgiving."** Emmy Martin frames the feature on the fear that AI "may soon be able to improve itself faster than people can control it." MIRI's Nate Soares sees "a real chance" AI wipes out humanity "in the next few years" and told his parents not to wait to finish visiting the national parks. Daniel Kokotajlo expects next year to bring "AI-powered euphoria and whole new gadgets" and is less sure about the years after. Naveen Rao calls the extinction fear "just the dumbest way to look at it," Robin Hanson expects AI to be absorbed slowly, and Encode AI's Nathan Calvin says concern is warranted but dread isn't. [NYT](https://www.nytimes.com/2026/11/25/technology/thanksgiving-ai-doom-family.html) (queued by Rick; read from his vault clipping, since nytimes.com is paywalled)

**Source:** a journalist's feature quoting five people whose positions are already on record. *Commentary/advocacy*, no numbers.

**Effect on the range:** held. Soares's and Kokotajlo's views are already logged (Soares 09-18; Kokotajlo 11-07 and the AI Futures update 11-13), Rao and Hanson pull the other way, and nothing here gives a date or probability that could be sized against P5 or P50.

*Context only:* Sen. Gallego's proposed ban on recursive self-improvement (above, under Nation-State Cyber Policy & Law). **Source:** reporting on an unintroduced proposal; *Commentary/advocacy*. **Effect on the range:** none yet; if enacted, it would argue for a later P50.

*Context only:* the Swiss and Italian AI-agent attacks (above, under Adversary Playbook). **Source:** two national cyber authorities, from incident reports; *Disclosed incident*. **Effect on the range:** none; human operators directing AI tools is misuse, not loss of control.

**Sherlock's view:** no shift; known positions restated. **Ryan's view:** the Swiss and Italian cases are human-directed, no bearing. **Seldon's call:** hold at P5 2031 · P50 2046 · P95 2075.

## Privacy

**Forty-two states and DC fight the sale of Character.AI's private chats.** Connecticut's attorney general is challenging a Dec. 1 bankruptcy auction of Character.AI's platform, including chat histories and personal data (IP addresses and other metadata) from more than 21 million US accounts, 2.1 million registered to minors, with no obligation on the buyer to protect them. The company had promised never to sell users' personal information; the same bipartisan coalition objected last week to a separate license sale to Disney. [Connecticut Attorney General](https://portal.ct.gov/ag/press-releases/2026-press-releases/attorney-general-tong-challenges-plan-to-auction-off-character-ai-private-chats) (via Risky.Biz)

## Executive Leadership Changes

**Canara Robeco Mutual Fund names Joel F. Machado CISO (reported, unconfirmed).** The former Ageas Federal Life Insurance security lead takes the role; CISO Tribune flags the report, from enterpriseitworld.com, as not yet confirmed by the company or an established publication. [CISO Tribune](https://www.cisotribune.com/moves)

## Resilience Tactics

**Britain's "Be Ready" campaign turns ordinary households into preppers.** The government's campaign, launched last month as the first stage of a three-year effort, advises stocking three days of water, tinned food, and essentials for outages of power, water, phones, and the internet. UK preppers welcome it but ask "What's your plan for day four?", and WIRED notes cyberattacks such as this month's supermarket refrigerator hacks among the disruptions they plan for. [WIRED](https://www.wired.com/story/the-british-government-is-turning-everyone-into-a-prepper/)

## Workforce Development Tactics

**Romania launches a National Academy for Cybersecurity Skills; ISC2 signs on.** Rather than a new institution, the academy is a national framework linking school cyber-hygiene education, universities, professional entry, and lifelong learning, using the EU's ECSF to map skills to roles. Romania names 61 certifications from 15 providers in its official frameworks, the most of the four EU states that name any. [(ISC)²](https://www.isc2.org/Insights/2026/11/isc2-joins-launch-of-romania-national-academy-for-cybersecurity-skills)

---

### Pending Evidence Queue

Two rows processed, both queued 11-26 and read from Rick's vault clippings since nytimes.com is paywalled: the NYT's Thanksgiving AI-doom feature (AI Singularity Timeline; range held) and the NYT's report on Congress and AI regulation (Nation-State Cyber Policy & Law). Both categories fit. Both rows are now marked Included.

### Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Intrusion Kill Chain Prevention Tactics** — Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends.
- **Cybersecurity Risk Forecasting Tactics** — Quantified cost/impact/risk reporting — superforecasting, Bayesian methods, FAIR methodology, and risk-forecasting case studies.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Workforce Development Tactics** — Unconventional hiring/development approaches — e.g. "Moneyball for Cybersecurity."

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 77 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 60 | 32 | 2026-07-14 |
| The Hacker News | Contributed | 91 | 1 | 2026-07-14 |
| The Record | Contributed | 72 | 20 | 2026-07-14 |
| The Canon Project | No Contribution | 20 | 71 | 2026-07-14 |
| FFX Now | No Contribution | 18 | 74 | 2026-07-14 |
| Wired | Contributed | 58 | 31 | 2026-07-20 |
| CyberScoop | No Contribution | 44 | 19 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 60 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 30 | 33 | 2026-09-01 |
| SecurityWeek | Contributed | 58 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 38 | 2026-10-02 |
| CISO Tribune — The Wire | Contributed | 15 | 18 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 32 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 16 | 17 | 2026-10-17 |
| (ISC)² Insights | Contributed | 10 | 23 | 2026-10-17 |
| IAPP News | No Contribution | 21 | 12 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 5 | 28 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 9 | 24 | 2026-10-17 |
| Risky.Biz | Contributed | 12 | 6 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 16 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 2 | 16 | 2026-11-10 |
| Resilient Cyber | No Contribution | 8 | 10 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 10 | 8 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 1 | 15 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 14 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 16 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 4 | 12 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 1 | 15 | 2026-11-12 |
| Zero Trust Forum | No Contribution | 0 | 4 | 2026-11-24 |

**No contribution today:**
- **N2K Cyberwire Daily Briefing**: on its Thanksgiving break; newest issue is 225 (Nov. 25), covered.
- **The Canon Project**: newest review is still Nov. 23, covered 11-24 (read through Chrome; the listing is behind Cloudflare).
- **FFX Now**: one new item (Nov. 26), the Thanksgiving storm leaving 11,000-plus Dominion customers without power; no CIR fit.
- **CyberScoop**: nothing since Nov. 25.
- **CSO Online CISO Appointments**: still no October or November section.
- **CISA Cybersecurity Advisories**: nothing since the Nov. 25 KEV update, covered.
- **LEAP**: newest is Wave 13, covered 11-19.
- **NIST Insights**: newest post Oct. 27.
- **EFF**: the only item is a holiday merchandise guide.
- **IAPP**: nothing new since the 11-26 run; the Nov. 25 items were already seen then.
- **CSIS**: newest items Nov. 18 and Nov. 16 (read through Chrome; headless Chrome is blocked by Cloudflare).
- **AI Alignment Forum**: no post since Nov. 24.
- **tl;dr sec, Detection Engineering Weekly, Resilient Cyber, Cybersecurity Dive**: no new issue or item in the window.
- **AI as Normal Technology, Epoch AI, Reflective Altruism, Understanding AI, Marcus on AI**: nothing new in the window.
- **Zero Trust Forum**: newest item is still the Nov. 20 podcast.

**Crediting notes:** The Hacker News for the Swiss AI-agent attacks, PolinRider, Q-Dir/DesktopOK, the Cacti zero-day, and (via ThreatsDay) the Scam Center Strike Force, PowerPanel, and NCC's October ransomware count; The Record for the DWP incident; SecurityWeek (site listing) for SAP; Risky.Biz (Risky Bulletin, Nov. 26) for Todoist, the Flanders theft, Chile, Sea-Watch, CheckFirst, Azalea Agent, Keenadu/Triada, MadApe, Vinci, GodFather.Tech, WalletGuard, NFS2ROOT, Joomla, Belgium's police advice, Huawei, Hardy, Character.AI, Russia's GitHub plan, and CDT's spyware report; WIRED for the Be Ready campaign; (ISC)² for Romania's academy; CISO Tribune for Machado; Gmail (Google Alerts) for the Black Friday claims data and the Turkish arrests. **Recirculations excluded:** Hex.pm (covered 11-25; Risky Bulletin's lead and SecurityWeek's 11-27 story), myColorado (covered 11-25; SecurityWeek now estimates about 100,000 affected against the 150,000 reported then), FIFA, 1Password, FinCEN, Drupal, ARTEX's adoption by four APT groups, Peninsula Energy, Optimizely, DIVD, Rackspace Spot, the casino exploit kits, ChatGPT Sites, Copeland XWEB, and Fragnesia (all covered 11-16 to 11-26), Volant Manticore (Iran row 22, covered 11-25), SecurityWeek's Juniper Session Smart story (in the 11-25 KEV update), and The Hacker News's ThreatsDay items on Todoist, CrowdStrike–Zscaler, the Binance seizure, ShinyHunters, Anthropic's safeguards, BankWeaver, BYOD, NGINX2Root, and the IPTV takedown (all covered earlier). **Considered, no CIR fit:** The Hacker News's contributed piece on security metrics (vendor content), SAP's 10,000 layoffs, Anthropic's block of Epic Games accounts, X's teen parental controls, GitHub's advisory roles, and Google Alerts snippets on Gartner placements, SASE market sizing, and cyber-insurance products. **Tooling notes:** Gmail `search_threads` again returned no snippets, so the Google Alerts digest was read with `get_thread`; SecurityWeek's RSS feed failed to parse, so its homepage was read through headless Chrome; The Hacker News bodies, the Canon Project, and CSIS were read through Chrome MCP; the NFS2ROOT write-up (opensec.in) didn't load at any tier.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*

## AI Timeline Current State and Definitions

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years. **(unchanged since 2026-11-11)**
   - Nothing matched today.
   - Considered: Daniel Kokotajlo's expectation of "AI-powered euphoria" next year (NYT, Nov. 25).
   - *Source:* AI Futures Project lead, quoted in a feature; Credentialed expert judgment.
   - *Effect:* none; his dated forecasts were logged 11-13 and this restates them.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years. **(unchanged since 2026-11-17)**
   - One item matched today, from the Pending Evidence Queue: the NYT's feature on how AI insiders talk about doom with their families.
   - Range held; see the AI Singularity Timeline section above.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years. **(unchanged since 2026-11-11)**
   - This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed.
   - Nothing matched today.
   - Considered: the NYT feature's retelling of "AI 2027".
   - *Source:* Commentary.
   - *Effect:* none; nothing on transition speed beyond the 11-13 AI Futures update.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years. **(unchanged since 2026-11-11)**
   - This isn't a prediction that disaster will happen, only a guess at when, if it ever does.
   - It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen?
   - Entry 5 below answers the separate question of how likely that is in the first place.
   - Nothing matched today.
   - Considered: Nate Soares's "real chance" AI wipes out humanity "in the next few years" (NYT, Nov. 25).
   - *Source:* MIRI president, co-author of "If Anyone Builds It, Everyone Dies"; Commentary/advocacy with no number.
   - *Effect:* none; it runs together when control is lost and whether harm follows, and his position has been on record here since September.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end. **(unchanged since 2026-11-03)**
   - This answers a different, bounded question from entry 4.
   - Entry 4 asks *when* a system that has escaped meaningful human control would cause harm.
   - This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control.
   - Nothing matched today.
   - Considered: Soares against Naveen Rao and Robin Hanson in the same NYT feature.
   - *Source:* three credentialed voices restating known positions; Commentary/advocacy.
   - *Effect:* none; the views point both ways and none addresses this file's conditional.

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*
