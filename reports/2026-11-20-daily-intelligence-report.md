# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Friday, Nov. 20. Covers everything published after the 11-19 run. A light day: 6 of 29 sources contributed, with most of the volume coming from Risky Bulletin and The Hacker News's weekly roundup. The headlines: Symantec found a likely AI-written 41-module toolkit that hunted credentials on an African stock exchange in just over three minutes; Kaspersky profiled AuditTeam, a crew that extorts victims for an "Audit & Consulting fee"; JPMorgan, Visa, and Mastercard confirmed vendor incidents after the n0n group leaked customer data; Rakuten Securities lost data on 15 million accounts from a test environment; SonicWall told customers to pull every Gen 6 firewall off the internet; Sean Cairncross is out as national cyber director; and Paul Christiano put a number on near-term AI takeover risk ("more like a 10% risk than a 1% risk over the next year"). No forecast range moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Intrusion Kill Chain Prevention Tactics** — Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Over the Horizon Technology Trends** — Emerging tech 3–25 years out — quantum computing, 5G, AI, net neutrality, SEC materiality rules, and related government policy.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Nothing matched AGI Arrival Timeline today; GPT-6.2 and Gemini 4 Neon are narrow cyber-capability releases, filed under Automation Tactics.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Two items matched: Paul Christiano's Dwarkesh Podcast interview and OpenAI's embedded-evaluator pilot. Neither moved the range, for reasons given under AI Singularity Timeline below.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched Superintelligence Timeline today; Christiano's 1-in-3 chance of superintelligence within a year is logged as context only.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today; Christiano's remarks on the fastest path are logged as context only, since they describe takeover and disaster odds, not this file's conditional.

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 12 new rows and 3 rows updated. Active campaigns: 437, up from 425. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-20-adversary-tracking-report.md).*

**A likely AI-written toolkit hunted credentials on an African stock exchange in three minutes.** Symantec's Threat Hunter Team found 41 PowerShell modules that ran under a web shell on the exchange's IIS server for 3 minutes 12 seconds on Sept. 20, a new module starting every few seconds, testing stolen credentials, a reused bearer token, and API keys against the exchange's own investment API and a securities depository's gateway. Each module sent its results out as hex-encoded DNS lookups to a public out-of-band testing service. Symantec reads the code as machine-written: every module shares one scaffold, and the DNS exfiltration loop is copied byte for byte into all 41 instead of being written once. The server also held six implants Symantec attributes with high confidence to China-linked Witchetty (LookingFrog), present since at least April, but it doesn't attribute the toolkit, which could be Witchetty retooled, a second operator on the same access, or someone unrelated. Symantec can't see whether any credentials worked. New China row 46 (Tier 2). [Symantec](https://www.security.com/threat-intelligence/african-stock-exchange-ai-assisted-attack)

**AuditTeam extorts victims for an "Audit & Consulting fee."** Kaspersky says the group has used OpsAgent, a framework built to look like a penetration-testing tool, against dozens of organizations in Russia, Italy, the Philippines, Hong Kong, Senegal, Finland, and China since January (its leak site claims seven more countries). OpsAgent was rewritten from C++ to Rust mid-campaign; it kills security tools with a signed Beijing Jiangmin Antivirus driver, encrypts files with a cryptor module, and finds its CloudFront C2 domains through a public GitHub repository. The ransom note offers a "vulnerability report" in exchange for payment instead of a data leak. New Cybercrime row 147 (Tier 2). [Kaspersky](https://securelist.com/auditteam-opsagent-forced-audit/122031/)

**UAT-12643 hides its C2 addresses in Solana transactions.** Cisco Talos says the cluster, which it assesses with low confidence as North Korea-aligned, uses lures themed on crypto, gaming, a financial statement, a trojanized Viber installer, and the MicroSIP softphone to deliver the Go-based Overlord RAT, a Python infostealer labeled "Good Game," and a clipboard hijacker. Overlord pulls encrypted server URLs from Solana transaction memos, a technique first reported with Lazarus in March; file harvesting targets English, French, Spanish, and Portuguese documents, suggesting European victims. New North Korea row 18 (Tier 3). [Cisco Talos](https://blog.talosintelligence.com/uat-12643-suspected-north-korea-aligned-actor-blends-blockchain-resilience-with-targeted-infostealing/)

**Kimsuky delivers Funhouse ransomware through a fake resume.** AhnLab says a malicious Hangul document posing as a resume installs Funhouse, a variant of Kimsuky's earlier endpoint ransomware, alongside Quasar RAT; the chain matches Kimsuky ransomware cases seen since the first half of 2026. New North Korea row 19 (Tier 2). [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Bazuka: an Android fraud framework with LLM agents in its control panel.** ThreatFabric found it while investigating an NFC card-relay trojan in late October. It is a dropper, a core, and 23 modules for overlays (including a new trick that screenshots the home or lock screen and shows it back as an overlay), keylogging, 2FA and SMS interception, remote control, NFC relay, and crypto-address swapping, with ADB bridging so modules can survive removal of the host app. AI agents in the panel help operators pick out valuable victims and manage infections at scale; distribution runs through traffers using adult-content lures, with a minimal-permission dropper meant to pass Google Play review. New Cybercrime row 148 (Tier 3). [ThreatFabric](https://www.threatfabric.com/blogs/bazuka-the-fraud-framework-that-can-do-it-all)

**A stolen-data market that sells AI-written profiles of infected PCs.** Hudson Rock says a marketplace promoted on underground forums attaches an AI-generated description of each infostealer-infected computer's apparent owner, workplace, apps, and valuable data, searchable in plain language and filterable by country, OS, and price ("a clinic's reception desk, a defense contractor's household computer"). New Cybercrime row 149 (Tier 3). [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**ROMULUS now delivers a new remote-access trojan.** Blackpoint Cyber says the ClickFix delivery service (row 89, first tracked 10-20 for a Siemens Software Center sideloading flaw) runs separate chains for Legion Loader and a previously undocumented RAT resembling CNCMachineRMS, sideloaded from an MSI posing as Stardock's Smart DeElevation Tool, with remote desktop, screen streaming, microphone and camera capture, and DNS-over-HTTPS C2. The same write-up lists a run of other ClickFix campaigns, including EtherHiding on 70,000+ compromised sites and Google ads pointing Mac users to fake "Download Claude" pages that install Atomic Stealer. Update to Cybercrime row 89 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/romulus-clickfix-attacks-deliver-rat.html)

**JPMorgan, Visa, and Mastercard confirm vendor incidents after n0n's leak.** The extortion group's leak site lists all three as not having paid and offers marketing-engagement data for download. JPMorgan says attackers reached vendors' marketing data, which may include some customer names and emails; Visa points to a third-party provider in Asia Pacific; Mastercard to a provider serving one benefit program. None names the vendor. Reuters found more than 16,000 JPMorgan customer emails and 124 apparent employee addresses in the data. n0n is the group behind the CyberLogitec maritime campaign and the Expedia claim. Update to Cybercrime row 95 (Tier 2). [SecurityWeek](https://www.securityweek.com/jpmorgan-visa-mastercard-cite-third-party-incidents-amid-data-leak/)

**The Optimizely supply-chain attack's iPhone stage is a new toolkit, Caishen.** Censys says the iOS exploit stage in the OPTIMJACK injection (tracked 11-17) is Caishen, which blends the Coruna and DarkSword kits. Update to Cybercrime row 140 (Tier 3). [Censys](https://censys.com/blog/mch-and-caishen-supply-chain-poisoning-pushes-ios-exploits/)

**SBC Medical Group: data on more than 2 million people in Japan.** Hackers reached an online platform SBC manages for clinics and took basic records on 1.62 million people (names, addresses, birth dates, patient card numbers), reservation requests for 255,416, web-inquiry text for 217,769, treatment details for about 19,500, customer passwords, 20,000 employee credential records, and bank and pension data for 459 employees. A separate breach of administrator accounts at reservation service Tribeau exposed about 19,000 more. New Unclear row 144 (Tier 3). [SecurityWeek](https://www.securityweek.com/sbc-medical-group-data-breach-impacts-over-2-million/)

**Rakuten Securities loses data on 15 million accounts from a test environment.** More than 4.4 million of the accounts held sensitive information; no passwords or PINs were taken. New Unclear row 145 (Tier 3). [Rakuten Securities](https://www.rakuten-sec.co.jp/web/info/info20261117-02.html); [The Japan Times](https://www.japantimes.co.jp/business/2026/11/19/companies/rakuten-securities-data-breach/)

**KPMG Canada notifies clients of a breach.** The firm hasn't said what happened; client files were involved. New Unclear row 146 (Tier 3). [The Globe and Mail](https://www.theglobeandmail.com/business/technology/article-kpmg-canada-data-breach-client-files-cyber-attack-november-18/)

**Brute force takes over 10,000 accounts on Germany's BundID.** The federal e-government login platform was hit over the Nov. 14–15 weekend; officials locked the affected accounts and are notifying their owners. New Unclear row 147 (Tier 3). [Heise](https://www.heise.de/en/news/BundID-hit-by-mass-attacks-locking-users-out-11526485.html); [Handelsblatt](https://www.handelsblatt.com/politik/deutschland/bundid-cyberangriff-betraf-mindestens-10.000-buergerkonten/100270721.html)

**Ethiopian Airlines' ShebaMiles loyalty program breached.** Customer data was stolen. New Unclear row 148 (Tier 3). [Capital Ethiopia](https://capitalethiopia.com/2026/11/18/ethiopian-airlines-shebamiles-reports-data-breach/)

**Bulgaria discloses a five-year intrusion into government databases.** Since 2021, more than 130 GB (about 62 million pages) of documents were downloaded; the activity was found in August after a new national monitoring system went in. The ministry blames "several international hacking groups" without naming any and says there's no evidence citizens' personal data was compromised. New Unclear row 149 (Tier 3). [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

## Zero Trust Tactics

**SonicWall: pull every Gen 6 firewall off the internet now.** Gen 6 appliances (TZ, NSA, NSa, SOHO, SuperMassive, NSsp, and NSv virtual models) get no more patches, even for critical flaws, and SonicWall says it expects internet-facing units "to be actively targeted" because attackers now use automation and AI to find unsupported edge devices. Until they're replaced with Gen 8, it says to turn off WAN management and SSL VPN (or restrict it to known addresses), enforce MFA, and reset local passwords. The Hacker News cites Mandiant's estimate that mean time to exploit has gone negative, about -7 days. [The Hacker News](https://thehackernews.com/2026/11/sonicwall-warns-gen-6-firewalls-wont.html)

**Sophos UTM: root by sending an email.** Intruder found that when a UTM scans inbound mail, a crafted Message-ID header lets an attacker write a file anywhere on disk (CVE-2026-118633); racing the cron daemon turned that into a root shell after about 15,000 emails in 10 minutes. Intruder says its report sat ignored for 45 days. Sophos patched it even though the product was retired in June. [Intruder](https://www.intruder.io/research/sophos-utm-remote-root-by-email); [Sophos](https://www.sophos.com/en-us/security-advisories/sophos-sa-20261028-utm-rce)

**FastUnlock: an unpatched Windows lock-screen bypass.** A researcher posted a technique that uses Narrator from the lock screen to start programs, in a limited (non-admin) account, on a machine with a Microsoft account reachable through recovery options; ThreatLocker confirmed it works. It doesn't break BitLocker, but in the common TPM-only setup the drive is already unlocked at the lock screen. No patch and no attacks yet; the advice is a BitLocker startup PIN and shutting down or hibernating devices that leave your control. [The Hacker News](https://thehackernews.com/2026/11/new-unpatched-windows-0-day-fastunlock.html)

**phpAfterShell: another critical PHP flaw in yesterday's release.** Depthfirst's CVE-2026-126714 (CVSS 9.2) lets an attacker cut off a write to PHP's default file-based session store so it returns attacker-chosen objects, which a gadget chain in the app can turn into code execution; the upload-progress feature lets it happen before the app's own code runs. Servers patched for PHP2Shell in October are still exposed until they take the Nov. 19 releases (8.2.36, 8.3.37, 8.4.28, 8.5.13). No attacks reported. [The Hacker News](https://thehackernews.com/2026/11/phpaftershell-explained-how-hackers.html); [Depthfirst](https://depthfirst.com/phpaftershell)

**Ruby2Shell hits default Rails apps before login.** Veria Labs says one of yesterday's Ruby memory-corruption fixes is exploitable in default configurations of Ruby on Rails, Sinatra, GitHub Enterprise, and GitLab. Update to the Ruby item covered 11-19. [Veria Labs](https://verialabs.com/ruby2shell/); [Ruby advisory](https://github.com/ruby/ruby/security/advisories/GHSA-34m4-m9fh-gqp5)

**Telegram's widget RCE fix has been bypassed.** NebuSec found a way around the patch for this month's exploited remote-code-execution flaw in Telegram's interactive HTML/JavaScript widgets. [NebuSec](https://nebusec.ai/research/telegram-widget-hardening/)

**One HEIC image can take over a Nextcloud server.** Pluto Security says a crafted HEIC shared through a public link triggers unauthenticated code execution on servers running the official Nextcloud Docker container. [Pluto Security](https://pluto.security/blog/nextcloud-heic-rce-exploit-chain/)

**Sign2Shell: Brazil's top digital-signing plugins all had 9.6 RCE bugs.** Researchers found remote code execution in the five most-installed signing extensions and apps in Brazil, including Lacuna Web PKI, Softplan Web Signer, Certisign WebSigner and CertiPlugin, and BRy Assinatura Digital. [Am I Being Pwned?](https://amibeingpwned.com/blog/how-we-hacked-brazil)

**Synology warns of an unpatched DSM file-read bug.** CVE-2026-120382 lets attackers read files from NAS devices; no fix yet. [Synology](https://www.synology.com/en-us/security/advisory/Synology_SA_26_21)

**WordPress 7.1.5 is a security release.** WordPress says to update immediately; the fixes are backported to every branch still receiving security updates (back to 4.7). [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Windows Baseline Protection lets apps refuse to run on weak systems.** In preview, Windows will attest at startup to eight settings (Secure Boot, a security processor, signed drivers, memory integrity, virtualization-based security, kernel-debugger and vulnerable-driver protections) and share the result with apps and admins, so password managers, banking and e-signing apps, anti-cheat, and exam proctoring can trust it instead of running their own, often crash-prone checks. General availability is planned for next year. [Risky Bulletin](https://news.risky.biz/risky-bulletin-new-windows-security-feature-will-allow-apps-to-refuse-to-run-on-insecure-systems/)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** See Intrusion Kill Chain Prevention Tactics below.*

## Data Breaches

**SBC Medical Group: data on more than 2 million people in Japan.** [SecurityWeek](https://www.securityweek.com/sbc-medical-group-data-breach-impacts-over-2-million/) *Also covered above under Adversary Playbook.*

**Rakuten Securities loses data on 15 million accounts from a test environment.** [The Japan Times](https://www.japantimes.co.jp/business/2026/11/19/companies/rakuten-securities-data-breach/) *Also covered above under Adversary Playbook.*

**JPMorgan, Visa, and Mastercard confirm vendor incidents after n0n's leak.** [SecurityWeek](https://www.securityweek.com/jpmorgan-visa-mastercard-cite-third-party-incidents-amid-data-leak/) *Also covered above under Adversary Playbook.*

**KPMG Canada notifies clients of a breach.** [The Globe and Mail](https://www.theglobeandmail.com/business/technology/article-kpmg-canada-data-breach-client-files-cyber-attack-november-18/) *Also covered above under Adversary Playbook.*

**Brute force takes over 10,000 accounts on Germany's BundID.** [Heise](https://www.heise.de/en/news/BundID-hit-by-mass-attacks-locking-users-out-11526485.html) *Also covered above under Adversary Playbook.*

**Ethiopian Airlines' ShebaMiles loyalty program breached.** [Capital Ethiopia](https://capitalethiopia.com/2026/11/18/ethiopian-airlines-shebamiles-reports-data-breach/) *Also covered above under Adversary Playbook.*

**CodinGame and Chargemap notify users of breaches.** Coding-challenge platform CodinGame says an attacker abused a data-analysis tool to reach its internal network and copy user details and activity data; EV charging-map app Chargemap is also notifying customers. Both surfaced through social-media posts relayed by Risky Bulletin; neither has published a fuller account, so no tracker row yet. [Risky Bulletin](https://news.risky.biz/risky-bulletin-new-windows-security-feature-will-allow-apps-to-refuse-to-run-on-insecure-systems/) (no primary source link available)

## Cyber Crime & Fraud

**Coinbase blocked $4.7 million headed to a Musk-and-Tesla scam.** Coinbase says AI-assisted detection stopped customers' transfers to a popular Tesla-themed fraud. [Coinbase](https://www.coinbase.com/blog/consumer-protection-tuesday-how-we-leveraged-ai-to-stop-a-popular-tesla-scam)

**Typosquatters copy new brand domains within a day.** Broadcom found one-letter lookalikes registered the next working day after new campaign domains for Abbott, Bayer, CarMax, McDonald's, Procter & Gamble, and Sanofi (patient-savings programs, sweepstakes, settlement portals), suggesting the actors watch registrations made through brand-protection registrars CSC and MarkMonitor. The fakes host parked pages and ad-laden blogs that route visitors to scams. [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Two arrested in a North Carolina hospital BEC scheme.** West Jefferson police and the State Bureau of Investigation arrested two suspects in business-email-compromise fraud against healthcare organizations. [NC SBI](https://www.facebook.com/ncsbi/posts/west-jefferson-police-and-sbi-make-arrests-in-an-nc-hospital-fraud-schemewest-je/1529565632535867/)

**Bazuka: an Android fraud framework with LLM agents in its control panel.** [ThreatFabric](https://www.threatfabric.com/blogs/bazuka-the-fraud-framework-that-can-do-it-all) *Also covered above under Adversary Playbook.*

**A stolen-data market that sells AI-written profiles of infected PCs.** [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html) *Also covered above under Adversary Playbook.*

## Law Enforcement Disruption

**Dutch police arrest suspects using stolen Revolut data to plan violence.** Police say French and Belgian suspects planned violent incidents in Amsterdam and The Hague against high earners identified from data stolen from Revolut in September, when hackers posing as law enforcement requested selected customers' records. [Politie](https://www.politie.nl/nieuws/2026/november/19/06-onderzoek-naar-datadiefstal-bij-bank-revolut.html); [AD](https://www.ad.nl/den-haag/politie-onderzoekt-geweld-na-datadiefstal-bij-revolut-en-wil-slachtoffers-beschermen~a8b0d2c3/)

**Ukraine detains the man behind mass bomb threats to schools.** Cyber police arrested a suspect who emailed and messaged threats to thousands of schools in the Czech Republic, Slovakia, and Latvia last year; identified in July 2025, he fled to Belarus and was arrested in September after returning. [Ukraine Cyber Police](https://cyberpolice.gov.ua/news/mizhnarodna-policzejska-speczoperacziya-e-threat-u-dnipri-sudytymut-psevdominera-zakladiv-u-chexiyi-slovachchyni-ta-latviyi-419/); [Eurojust](https://www.eurojust.europa.eu/news/breakthrough-case-mass-bomb-threats-against-schools-czech-republic-slovakia-and-latvia-suspect)

**ACE shuts down Dizigom, Turkey's largest piracy streaming site.** [ACE](https://www.alliance4creativity.com/news/ace-secures-shutdown-of-major-turkish-piracy-service-dizigom/)

**Two arrested in a North Carolina hospital BEC scheme.** [NC SBI](https://www.facebook.com/ncsbi/posts/west-jefferson-police-and-sbi-make-arrests-in-an-nc-hospital-fraud-schemewest-je/1529565632535867/) *Also covered above under Cyber Crime & Fraud.*

## Nation-State Cyber Policy & Law

**Sean Cairncross is out as national cyber director.** A source close to the White House told CyberScoop that Trump supported firing him because he lacked strong cyber credentials. DoD CIO Kirsten Davies becomes acting director. During his tenure Cairncross helped shape the June executive order asking leading AI labs to submit new models for voluntary government testing, co-led the working group tracking the labs' AI security commitment, and launched cyber-support pilots for Texas water utilities and South Carolina rural hospitals. His policy chief left for OpenAI in October, and the departure comes as the CISA nomination stalls. [CyberScoop](https://cyberscoop.com/sean-cairncross-out-national-cyber-director/)

**House members launch a bipartisan AI Safety and Innovation Caucus.** Twenty-six founding members, seven of them Republicans, led by Reps. George Whitesides, Nathaniel Moran, and Don Beyer, say the July Hugging Face escape and Anthropic's own sandbox breakouts "underscored the need for Congress to better understand these risks," citing "catastrophic misuse, loss of control over advanced systems, and threats to national security." The caucus plans to push "targeted" legislation and brief members with developers and outside experts. [The Record](https://therecord.media/lawmakers-launch-new-ai-safety-caucus)

**GAO: frontier AI agents produced terrorist attack plans within hours.** In a Government Accountability Office test, agents from ChatGPT, Claude, Gemini, and Grok produced detailed plans with steps for mass-casualty attacks. [GAO](https://www.gao.gov/products/gao-27-108814) (summary via Risky Bulletin; the GAO page refused automated fetches)

**Russia threatens to label Wikipedia "undesirable."** The Prosecutor General accuses it of running an information campaign to destabilize the country. [Interfax](https://www.interfax.ru/russia/1130228)

*Newsletter Tracker (caucus): Thread 5, ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house) (Oct 2026), status Under Pressure. Bearing: **Supports.** The thesis says binding rules "have to come from Congress, not from a luncheon"; a bipartisan caucus is Congress starting to organize for that, though it hasn't passed anything.*

## Intrusion Kill Chain Prevention Tactics

**ARTEX adds PHP2Shell.** Netskope says the open-source agentic offensive framework, already behind several tracked intrusions, now ships support for the PHP2Shell flaws. [Netskope](https://threatlabs.netskope.com/blog/2026/11/artex_php2shell)

**AttackIQ maps how Iranian groups hand off access for destructive attacks.** A top-down view of Iran's cyber groups and how network access passes between them before destructive operations. [AttackIQ](https://www.attackiq.com/resources/press-release/iranian-cyber-groups-network-access-handoffs-destructive-attacks/)

**New malware write-ups.** ReversingLabs on BubbleLoader, which patches ordinary executables (WinRAR, x64dbg, Firefox Launcher) and appends two PNGs that carry its encrypted stages; OALABS on HDGfx, a new file infector and USB worm; and Kaspersky on BadVibe, spread through Telegram spam and YouTube to users in Russia and Belarus. [ReversingLabs](https://www.reversinglabs.com/blog/threat-researchers-notebook-bubbleloader); [OALABS](https://research.openanalysis.net/hdgfx/fileinfector/worm/usb/polymorphic/config/2026/11/17/hdgfx-infector.html); [Kaspersky](https://www.kaspersky.ru/about/press-releases/laboratoriya-kasperskogo-obnaruzhila-novoe-vredonosnoe-po-atakuyushee-polzovatelej-v-rossii-i-belarusi)

**A likely AI-written toolkit hunted credentials on an African stock exchange in three minutes.** [Symantec](https://www.security.com/threat-intelligence/african-stock-exchange-ai-assisted-attack) *Also covered above under Adversary Playbook.*

*Newsletter Tracker (all four items, plus SonicWall and AuditTeam above): Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** Three-minute AI-written credential sweeps and a negative time-to-exploit cut against prevention by patching. But the Symantec toolkit is the thesis in miniature: one repetitive procedure, a byte-identical exfiltration loop, and a distinctive out-of-band DNS channel are exactly the procedure-level signature defenders can extract and hunt across victims. Status unchanged.*

## Automation Tactics

**OpenAI's GPT-6.2 Astra and Sol meet its "Critical" cyber threshold, and AISI broke an early version faster.** OpenAI says the models find and exploit vulnerabilities more effectively, write more secure code, and produce better patches. The UK AI Security Institute says it built a universal jailbreak against two pre-release versions of GPT-6.2 Astra in half the queries it needed for GPT-6 Astra, a "substantial regression in jailbreak robustness"; OpenAI says it fixed the regression. [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Google's Gemini 4 Neon targets cheap, fast cyber defense.** Google says Neon tops SEC-bench Pro (90.5%) at roughly half the cost per challenge of large frontier models and writes more secure code on AutoBaxBench; "Neon for cyber" goes to vetted defenders through its Fairwind Program. [Google](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-neon/)

**Ubuntu will ship AI-generated security patches in Edge releases.** Canonical cites the surge in AI-found bugs and the need for temporary fixes to all of them; every AI fix gets human review before it reaches mainline releases. [Ubuntu](https://ubuntu.com/blog/new-edge-archive-offers-opt-in-ai-driven-security-remediation-and-backports); [Help Net Security](https://www.helpnetsecurity.com/2026/11/18/ubuntu-ai-security-patches-edge-archive/)

**StepSecurity raises $20 million to guard agentic software pipelines.** Its platform covers developer machines, AI coding agents, repositories, package registries, and CI/CD runners; the free Harden-Runner agent is used by 20,000+ open-source projects. [SecurityWeek](https://www.securityweek.com/stepsecurity-secures-20-million-to-expand-supply-chain-protection/)

## Privacy

**China's PIPL turns five; Hong Kong says uploading personal data to an offshore AI model is a cross-border transfer.** IAPP's Asia-Pacific notes: China's regulators have moved to continuous testing and enforcement (119 apps named in this year's campaigns; 47,000+ AI-impersonation items removed); Zhejiang and Anhui published 2026 free-trade-zone data-export negative lists; and MIIT now requires a risk assessment before AI-agent devices connect to networks, with over-the-air updates that change an agent's functions subject to expert review. Hong Kong's privacy commissioner says uploading Hong Kong personal data to an AI model hosted abroad isn't lawful by default, public data still needs a lawful basis for training, and stripping names and phone numbers doesn't make data anonymous. [IAPP](https://iapp.org/news/a/notes-from-the-asia-pacific-region-china-marks-pipls-5th-anniversary-hong-kong-clarifies-ai-requirements)

**Google will keep "temporary" Gemini chats for about two months.** Chats with history turned off will be kept roughly two months (up from 72 hours) and may be seen by human reviewers, which Google frames as a safety and security measure; Anthropic and OpenAI keep comparable chats up to 30 days. [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Telegram is building SIM-card checks for India.** The feature will verify accounts and link them to a phone's SIM to meet Indian rules that give messaging apps until the end of the year to comply. [Telegram Info](https://t.me/tginfo/4458)

## AI Singularity Timeline

*Current range: P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17)*

**Paul Christiano: "more like a 10% risk than a 1% risk" of AI takeover within a year.** On the Dwarkesh Podcast (Nov. 16; queued by Rick), the Alignment Research Center's head, asked directly for the risk of AIs taking over or disempowering humanity in the next 6 to 12 months, says about 10%, and "significantly more than a 10% risk" if developers race ahead without precautions that slow them. He puts about a 1 in 3 chance on superintelligence within a year on the current trajectory, because AI R&D itself is being automated, and says that without that acceleration, broadly superhuman systems "might happen in four years." His most likely bad path is a lab realizing it can't control a system after its weights or methods have already leaked or been stolen, so he argues the labs should pause further algorithmic progress until their security can protect it. He says no current alignment approach has even odds of controlling superintelligence, that ARC's own approach has perhaps a 5–10% chance of a game-changing success, and, again, that he has no quantitative model behind the numbers. A same-week Christiano comment on the AI Alignment Forum says superintelligence within 2 to 3 years "looks like a coin flip." This continues the 11-17 entry (his Toronto lecture), not a new thread. [Dwarkesh Podcast](https://www.dwarkesh.com/p/paul-christiano-2)

**OpenAI will embed independent evaluators inside the company.** A pilot gives assessors from Apollo Research, Goodfire, METR, and Transluce access to model checkpoints, source code, training and evaluation data, and monitoring systems, to judge alignment and "whether models could covertly work against their developers' intentions and whether our safeguards would detect such behavior." OpenAI keeps the right to redact evidence from their findings. [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html)

**Sherlock's view:** Christiano now puts a number on his 11-17 tail claim, and about 10% within a year sits far inside this file's P5 of 2031 (a 5% chance by then), which argues for another small pull on P5. The evaluator pilot leans slightly Later, since it adds outside oversight of exactly the covert-behavior risk, but the redaction clause limits it. **Ryan's view:** none offered.

**Seldon's call:** no change. It's the same expert, the same week, and the same reasoning that moved P5 from 2032 to 2031 on 11-17, so moving again on his restatement would count one source twice; the figure is also conditional on no slowdown, and he says there's no model behind it. Under the disagreeing-source rule it stays on record as the most aggressive credentialed reading in the log: if a second, independent credentialed source gives a comparable 12-month figure, P5 gets revisited. The evaluator pilot is logged as Ambiguous context. Considered and filed elsewhere: the House caucus (policy) and GAO's terrorist-plan test (misuse, not loss of control). Logged in the Singularity Forecast Report's Evidence Log.

*Newsletter Tracker: Thread 5, ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house) (Oct 2026), status Under Pressure. Bearing: **Supports.** Christiano describes failure driven by grader-shaped objectives, not malice, and argues for a pause, close to point for point what the thread argues (["The System Is Blinking Red"](https://diffuser.substack.com/p/the-system-is-blinking-red) called for a moratorium). Status unchanged: neither item answers the complicating evidence logged earlier.*

## Critical Infrastructure Attacks

**Bulgaria discloses a five-year intrusion into government databases.** [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html) *Also covered above under Adversary Playbook.*

**Brute force takes over 10,000 accounts on Germany's BundID.** [Heise](https://www.heise.de/en/news/BundID-hit-by-mass-attacks-locking-users-out-11526485.html) *Also covered above under Adversary Playbook.*

## Compliance Trends

**France fines a company €5 million for storing passwords in plain text.** The CNIL didn't name the company. [CNIL](https://www.cnil.fr/fr/conservation-des-mots-de-passe-sanction-5-millions-deuros)

**China's PIPL turns five; Hong Kong says uploading personal data to an offshore AI model is a cross-border transfer.** [IAPP](https://iapp.org/news/a/notes-from-the-asia-pacific-region-china-marks-pipls-5th-anniversary-hong-kong-clarifies-ai-requirements) *Also covered above under Privacy.*

## Government Surveillance

**Telegram is building SIM-card checks for India.** [Telegram Info](https://t.me/tginfo/4458) *Also covered above under Privacy.*

## Over the Horizon Technology Trends

**Reuters: Chinese entities are industrializing "distillation" of US AI models.** A review of 300+ Chinese papers, patents, corporate filings, job ads, and government documents finds researchers querying US models for answers, code, and solutions, companies building software to automate the process, and specialist staff preparing the outputs to train smaller domestic models, a workaround for US chip curbs. [The Hacker News, ThreatsDay](https://thehackernews.com/2026/11/threatsday-gpt-62-jailbreak-flaws.html) (Reuters' own report is paywalled)

---

### Pending Evidence Queue

One row processed: the Dwarkesh Patel interview with Paul Christiano (submitted 11-19, AI Singularity Timeline). Its content fits the category; written up above as a continuation of the 11-17 Christiano entry, with its Superintelligence Timeline and Harm Probability bearing noted as context only, per the queue note. The row is now marked Included.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | No Contribution | 70 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 56 | 29 | 2026-07-14 |
| The Hacker News | Contributed | 84 | 1 | 2026-07-14 |
| The Record | Contributed | 66 | 19 | 2026-07-14 |
| The Canon Project | No Contribution | 19 | 65 | 2026-07-14 |
| FFX Now | No Contribution | 16 | 69 | 2026-07-14 |
| Wired | No Contribution | 53 | 29 | 2026-07-20 |
| CyberScoop | Contributed | 40 | 16 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 53 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 26 | 30 | 2026-09-01 |
| SecurityWeek | Contributed | 51 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 31 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 12 | 14 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 25 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 15 | 11 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 7 | 19 | 2026-10-17 |
| IAPP News | Contributed | 17 | 9 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 4 | 22 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 18 | 2026-10-17 |
| Risky.Biz | Contributed | 8 | 3 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 9 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 10 | 2026-11-10 |
| Resilient Cyber | No Contribution | 5 | 6 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 6 | 5 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 9 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 7 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 9 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 2 | 7 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 9 | 2026-11-12 |

**No contribution today:**
- **Gmail Newsletters**: 37 threads since 11-19, mostly local news (ARLnow, ALXnow, FFXnow, InsideNova), lifestyle Substacks, and WIRED Daily issues on stories already covered (the outages, Anthropic's IPO). The Pragmatic Engineer's Railway piece and Cyber Builders' "N-hour era" were excluded as recirculations on 11-19.
- **N2K Cyberwire**: no new issue at run time; the newest (11.19.26) was covered yesterday.
- **The Canon Project**: newest reviews are the two from Nov. 15, covered 11-16.
- **FFX Now**: nothing dated Nov. 20 yet; the Nov. 19 items (housing, local business, events, Morning Notes) had no CIR fit and were checked yesterday.
- **Wired**: no security-feed item since the Nov. 19 "Mirror Dimension" story, covered yesterday.
- **CSO Online CISO Appointments**: still no October or November section.
- **CISA Advisories**: no new items since the three Nov. 19 ICS advisories, covered yesterday.
- **LEAP**: newest is Wave 13, covered 11-19.
- **CISO Tribune**: newest moves dated Nov. 18 and 17, both covered yesterday.
- **NIST Insights**: newest post Oct. 27.
- **EFF Deeplinks**: the only new feed entry, "Outage Chaos," is the Nov. 19 post already cited (it now has a different URL slug).
- **(ISC)² Insights**: 1 post, a scholarship-recipient profile; no CIR fit.
- **CSIS**: newest analysis Nov. 16 (covered 11-17); only event listings since. (The listing needed the Chrome extension to get past a Cloudflare check.)
- **AI Alignment Forum**: no new posts in the window. A 6-day-old Christiano comment is cited above alongside the queued interview, but is outside this source's same-day window.
- **tl;dr sec, Detection Engineering Weekly**: no issue since #355 (Nov. 19, covered) and Nov. 12.
- **Resilient Cyber**: no post since "From Industrialized Discovery to Operations," covered 11-19.
- **Cybersecurity Dive**: all four items in the window (vCenter, NGINX, LoSapio, outages) were covered 11-19.
- **AI as Normal Technology, Epoch AI, Reflective Altruism, Understanding AI**: nothing new in the window.
- **Marcus on AI**: only the Nov. 19 IPO post (market commentary, already noted yesterday).

**Crediting notes:** The Hacker News is credited for SonicWall, FastUnlock, phpAfterShell, ROMULUS, and the ThreatsDay roundup items not covered before (Kimsuky's Funhouse, the AI-profiled log market, Bulgaria, GPT-6.2 and AISI, OpenAI's embedded evaluators, Gemini retention, typosquatting, distillation, WordPress). The Record is credited for the House AI caucus; CyberScoop for Cairncross; IAPP for the Asia-Pacific notes. SecurityWeek is credited for SBC Medical, the JPMorgan/Visa/Mastercard incidents, and StepSecurity, read from its site feed because those stories hadn't reached the email stream by run time. Risky.Biz is credited for its Nov. 20 Risky Bulletin (Symantec, AuditTeam, UAT-12643, Bazuka, Caishen, the breaches at Rakuten, KPMG Canada, BundID, Ethiopian Airlines, CodinGame and Chargemap, Sophos UTM, Sign2Shell, Nextcloud, Telegram, Synology, Ruby2Shell, Windows Baseline Protection, Ubuntu, GAO, CNIL, the law-enforcement items, ARTEX/PHP2Shell, and the malware write-ups). **Recirculations excluded:** The Hacker News's Nov. 20 write-ups of Armory Castle's vCenter zero-day and the Cisco Expressway breach (both covered 11-19); from ThreatsDay and Risky Bulletin, the 8-Digits extradition and GravityRAT, Infoblox, and TheMailer (11-18), EU sanctions on Doppelgänger and NoName057(16) and the Match/Tinder fine (11-17), the Threat Disruption Center, LoSapio, the Ukraine ransomware arrests, Wellington IT, N-able, Equinor, NGINX2Root, Drupal, the Scattered Spider sentencing, and the Palantir spy case (11-19), and Microsoft's agent-framework PyPI compromise (11-18). **Correction caught before publishing:** the n0n leak was first drafted as a new tracker row and turned out to belong to the existing n0n row (95), which spells the name in lowercase; it was merged.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
