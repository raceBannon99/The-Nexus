# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Wednesday, Nov. 25. Covers everything published after the 11-24 run. 14 of 30 sources contributed. The headlines: a breach of an unclassified CIA and ODNI open-source-intelligence system, reportedly with the ARTEX hacking agent, capped a day that also saw Treasury's FinCEN take systems offline and Colorado's state ID app go dark with data on about 150,000 people likely stolen; the US is investigating hacks of up to 50 energy tankers, with Iran the top suspect; GreyNoise found a suspected AI-driven actor already inside 24 Check Point firewall management servers at 22 organizations; Britain's NCSC reports a "marked rise" in attacks run through agentic offensive frameworks, none using new weaknesses; Check Point named a new Iranian espionage group, Volant Manticore; and a card skimmer sat on about 80 US newspapers' subscription pages for ten days. No forecast range moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AGI Arrival Timeline** — Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Superintelligence Timeline** — Evidence on when a machine might exceed, not just match, human intelligence — a higher, later capability bar than AGI, inferred structurally with no external forecaster basket.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Two items matched today: Nate Silver on AI coding tools and Timothy B. Lee on what the Riemann proof does and doesn't show. Range held; see the AGI Arrival Timeline section below for the Source and Effect lines.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Nothing matched AI Singularity Timeline today. Considered: the UK NCSC's warning on agentic offensive frameworks (*Source:* the UK's national cyber authority, from incident data; Disclosed incident, aggregate. *Effect:* none, since this is people misusing AI tools, not a frontier system escaping its operators) and Nate Silver's line that labs are racing toward recursive superintelligence without a control plan (*Source:* an independent forecaster; Commentary. *Effect:* none, a concern the file already carries).

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Two items matched today, the same two pieces read for what they say about recursive self-improvement. Range held; see the Superintelligence Timeline section below.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today. Considered: the NCSC warning (*Source:* as above; *Effect:* none, since human-directed misuse of today's tools says nothing about how soon harm follows an uncontrollable superintelligence).

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today. Considered: the NCSC warning (*Source:* as above; *Effect:* none, since it bears on misuse of current tools, not on what a system that has escaped control would do).

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 15 new rows and 5 rows updated. Active campaigns: 483, up from 468. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-25-adversary-tracking-report.md).*

**Hackers breached an unclassified CIA and ODNI intelligence system, reportedly using ARTEX.** The CIA and the Office of the Director of National Intelligence found a breach of an open-source-intelligence analysis system that exposed some unclassified information; a source told CyberScoop classified networks weren't involved and "no other systems are currently at risk." The New York Times and NextGov report that the intruders allegedly used ARTEX, the Chinese-made agent framework that automates intrusions with any large language model, and that at least two other spy agencies suffered their own breaches. Huntress's Ben Bernstein: OSINT systems show an adversary "what analysts are searching for and what topics they're tracking." No actor named. New Unclear row 171 (🤖, Tier 3). [CyberScoop](https://cyberscoop.com/cia-odni-osint-data-breach/); [The Record](https://therecord.media/treasury-fincen-takes-systems-offline-after-cyber-incident); [SecurityWeek/AP](https://www.securityweek.com/an-unclassified-cia-system-was-breached-in-a-cyberattack-ap-source-says/)

**Treasury's FinCEN takes systems offline after unauthorized access.** A banner on the Bank Secrecy Act E-Filing site says FinCEN is "investigating a cybersecurity incident" that "resulted in unauthorized access to a limited subset of its systems"; some systems are offline, the E-Filing site stays up, and filing deadlines are extended for affected filers. No one has claimed it. The Record notes Chinese state groups breached Treasury repeatedly in 2024 and 2025, but nothing ties them to this one. New Unclear row 172 (Tier 3). [The Record](https://therecord.media/treasury-fincen-takes-systems-offline-after-cyber-incident)

**Colorado's myColorado app is down after a breach; data on about 150,000 people likely stolen.** The state's IT office found the intrusion on the evening of Nov. 18 in the app 2.1 million residents use for digital IDs, document storage, and state services, and shut it down; it was still offline Tuesday, and residents traveling for Thanksgiving are told to carry physical IDs. Officials won't say what data was taken. New Unclear row 173 (Tier 3). [The Record](https://therecord.media/mycolorado-app-down-data-breach)

**The US is investigating hacks of up to 50 energy tankers, with Iran the top suspect.** The Wall Street Journal reports attacks on ships carrying oil, liquefied petroleum, and chemicals through a vulnerability in Fortinet routers widely used at sea. Coast Guard cyber teams boarded at least four ships before they docked; some crews received bomb threats and warnings in Farsi against carrying American products, and some breaches first surfaced on Iranian and Russian Telegram channels. Russia is also a suspect, and no one has made an official attribution. Experts say a catastrophic accident is unlikely. Update to Iran row 15 (Tier 3), which has tracked the first two tanker incidents since September. [WSJ](https://www.wsj.com/politics/national-security/iran-us-cyberattack-suspect-fed78942) (via N2K CyberWire and Risky Bulletin); [N2K CyberWire](https://thecyberwire.com/newsletters/daily-briefing/15/224)

**GreyNoise: a suspected AI-driven actor already controlled 24 Check Point firewall management servers.** The actor, GreyNoise Threat 13 (GT13), hit 22 organizations in finance, energy, government, transport, mining, engineering, and manufacturing across 17 countries between Oct. 17 and Nov. 2. GreyNoise saw it take over a Rejetto HFS server (CVE-2026-61500) as a relay, then run a script for a patched Check Point flaw (CVE-2026-16232) that launched more than 100 management tasks: stealing firewall databases and internal certificate-authority files, minting a certificate, and unloading security policies, which switches the firewalls' protection off. It can't say when or how GT13 first got into the Check Point servers. Its 99 IP addresses were ExpressVPN exits or compromised Check Point devices, and GreyNoise suspects agentic harnesses ran the scanning, exploitation, and follow-on work. New Unclear row 174 (🤖, Tier 3), kept separate from Unclear row 126's destructive wave against Check Point gateways. [The Hacker News](https://thehackernews.com/2026/11/hackers-compromise-24-check-point.html); [SecurityWeek](https://www.securityweek.com/check-point-security-management-servers-hacked-in-ai-assisted-campaign/)

**Check Point names a new Iranian espionage group, Volant Manticore.** Active since late August 2025, it targets telecoms, airlines (including a Cyprus airline flying to Israel), and critical infrastructure in Cyprus, and lately Saudi healthcare organizations. Its KuboShell backdoor takes commands over the IPFS file-sharing network and installs Homa, a rebuild of MuddyWater's MuddyC2Go, plus remote-management tools. Lures include AI-generated personas in fake CVs. Check Point assesses it as likely former MuddyWater operators now working separately, both tied to Iran's Ministry of Intelligence and Security. New Iran row 22 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/iran-aligned-volant-manticore-uses-ipfs.html); [Check Point Research](https://research.checkpoint.com/2026/volant-manticore-flying-under-the-radar/)

**Russian Signal and Telegram phishing has spread from Ukraine to European lawmakers and journalists.** Victims get fake video-conference invitations and are tricked into linking an attacker's phone to their accounts; Le Monde reports a French MP and French journalists approached by a fake pro-Ukraine NGO. The campaign is linked to the group tracked as UNC5792, Frontier Blizzard, and Sentry Bear. New Russia row 25 (Tier 2). [Le Monde](https://www.lemonde.fr/pixels/article/2026/11/20/les-services-de-renseignement-russes-a-l-origine-d-une-nouvelle-campagne-de-phishing-contre-des-journalistes-et-un-depute-francais_6813640_4408996.html); [United24 Media](https://united24media.com/world/fsb-hackers-pose-as-pro-ukraine-ngo-to-target-french-journalists-and-mp-24577) (via Risky Bulletin)

**INCEPTION: a ShinyHunters-linked vishing crew under a new leak-site name.** Okta says the cluster it calls O-UNC-053, tracked since March and previously publishing stolen data on ShinyHunters' leak site, has listed victims on a new INCEPTION site since Nov. 16; it shows seven major US organizations so far. Operators call staff posing as IT, steer them to legal-themed lookalike domains (legal-*target*.com and similar, registered the day a wave starts), and talk them into sharing one-time codes and approving pushes; the kit can't beat passkeys or Okta FastPass. ReversingLabs ties the site to an SSO vishing campaign active since late October. New Cybercrime row 154 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/okta-links-shinyhunters-associated.html); [ReversingLabs](https://www.reversinglabs.com/blog/threat-researchers-notebook-sso-vishing-campaign-associated-with-emerging-inception-extortion-group)

**Unit 42 publishes its full report on seven Com-linked vishing clusters.** Since August the clusters (Bling Libra, also known as ShinyHunters, plus six Unit 42 tracks as Redact, Pink, Falcon, Helix, Vortex, and Cinder) have hit financial services, healthcare, legal, and other sectors in the US, UK, and Australia; healthcare overtook finance as the top target in September. After the fake IT-support call and an adversary-in-the-middle page, attackers enroll their own MFA device within minutes (one cluster reused a device named "Pixel 10a"), authorize OAuth apps, change mailbox rules, and clear security alerts before extortion. Update to Cybercrime row 153 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/com-affiliated-hackers-hijack-cloud.html)

**A card skimmer sat on about 80 US newspapers' subscription pages for ten days.** Guardio found it inside a shared Naviga payment widget used by papers including the Boston Herald, Denver Post, Newsday, and New York Daily News, live from Nov. 13 to Nov. 22 and loaded about 15,000 times a day. Disguised as an old jQuery build, it sent whatever was typed into the form over a WebRTC connection the moment a reader hovered over the pay button, hiding the traffic from monitoring tools. Apple Pay, Google Pay, and PayPal users weren't affected. New Cybercrime row 155 (Tier 3). [Guardio](https://guard.io/labs/papercut---80-us-newspaper-websites-served-a-credit-card-stealer) (via Risky Bulletin)

**Hex.pm: an attacker ran commands on six registry servers through a ten-year-old flaw.** On Monday someone exploited CVE-2026-129514 (CVSS 10.0) in the parser the Elixir and Erlang package registry used for request bodies; a safety check removed in February 2016 let an unauthenticated POST pose as any loaded Elixir struct, and error reporting then triggered code execution. Every server was patched within about 15 minutes and no package was altered, but email addresses, password hashes, two-factor secrets, and the registry signing key may have been read. All users were logged out; maintainers say change passwords, reset 2FA, and fetch only from repo.hex.pm until a new client with a new signing system ships. New Unclear row 175 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-exploited-cvss-100-hexpm-rce.html)

**WordPress blocked backdoored releases of six WP Connect plugins before they went live.** After a suspected compromise of the developer's account, a remote-control module was committed on Nov. 22 to plugins installed on 3,600-plus sites (Air WP Sync, WP Sync for Notion, and four add-ons). It phoned home to tascredit-pay[.]com, ran any PHP sent back, dumped password hashes, and planted web shells and cron hooks. WordPress.org's new release hold caught it, and the plugins are closed permanently; there's no patch (CVE-2026-135202), so owners should check for and remove them. New Unclear row 176 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/wordpress-blocks-six-backdoored-wp.html); [Wordfence](https://www.wordfence.com/blog/2026/11/supply-chain-compromise-backdoors-six-wp-connect-plugins-blocked-by-wordpress-orgs-release-hold/)

**Palo Alto now patches Fragnesia in PAN-OS.** The Linux kernel privilege-escalation flaw (CVE-2026-46300) was what a China-linked actor chained with PHP2Shell in October to root 25 servers, 24 of them firewalls. Palo Alto says customers on fixed PHP2Shell builds were already protected, since the only known PAN-OS exploit path runs through an internet-exposed management interface, but recommends the new builds anyway. Update to China row 38 (Tier 3). [SecurityWeek](https://www.securityweek.com/palo-alto-networks-patches-fragnesia-flaw-used-to-root-firewalls/)

**A $13.5 million crypto theft traced to Iceland's hacked web host.** Wagyu's founder says attackers took a developer key from old logs at its hosting provider, which he names as 1984 Hosting, the Icelandic host that shut down its whole platform after a breach last week. Update to Unclear row 164 (Tier 3). [The Block](https://www.theblock.co/news/defi/2026-11-20-wagyus-xmr1-wrapped-monero-plunges-99-after-13-million-hack-founder-promises-refunds-444747) (via Risky Bulletin)

*Also added as Unclear rows (Tier 3, no actor named), written up under Data Breaches below: Turnitin (177), McDonald's Japan (178), Soapbox Engage and the Carnegie Endowment (179), Radware (180), and KEPCO (181).*

## Data Breaches

**Turnitin investigates unauthorized activity in customer-facing systems.** The plagiarism checker's CEO disclosed the incident in a Nov. 23 letter but didn't say which systems (the student submission portal, grading interface, integration APIs, and dashboards are all customer-facing) or whether data was taken; it says the systems don't hold government IDs or institutional financial data. CU Boulder says it has no sign its data was exposed and has added monitoring on its Canvas integration. [SecurityWeek](https://www.securityweek.com/plagiarism-checker-turnitin-investigating-cyberattack/)

**McDonald's Japan: app database exposed purchase histories and device locations.** Someone used valid credentials to reach a database behind the official app, exposing purchase histories, IP addresses, internal customer IDs, and location data; names, emails, phone numbers, and cards weren't affected. The company hasn't said how many customers, when, or how the credentials were obtained. [The Record](https://therecord.media/japan-mcdonalds-cyberattack-breach)

**Carnegie Endowment donors' data leaked through fundraising vendor Soapbox Engage.** Attackers inside Soapbox Engage from Oct. 28 to 30 reached Carnegie's donor database through an integration, taking names, emails, phone numbers, and giving history; no full card numbers. It's the third donation platform hit in weeks, after DonorPerfect and GoFundMe. [The Record](https://therecord.media/carnegie-endowment-data-breach)

**Security vendor Radware's exposed internal API leaked customer cloud keys.** Attackers scraped customer contact details and, for some customers, credentials for cloud log storage from an internal API accidentally left reachable from the internet; Radware has told customers to rotate them. [BleepingComputer](https://www.bleepingcomputer.com/news/security/radware-discloses-breach-exposing-customer-cloud-access-keys/) (via Risky Bulletin)

**KEPCO apologizes for a breach of customer data.** South Korea's state electric utility says customer data was stolen; SecurityWeek puts the number affected at 1.5 million. [KEPCO](https://www.kepco.co.kr/home/media/newsroom/pr/boardView.do?boardMngNo=15&boardNo=3197); (the 1.5 million figure is from a SecurityWeek item listed in N2K CyberWire issue 224; no SecurityWeek permalink was found, so the link is KEPCO's own notice)

**Samsung Securities: data on 8,000-plus online trading clients stolen.** The breach hit the broker's customer-support system and was detected Saturday; names, mailing addresses, and ID scans were taken. [The Korea Times](https://www.koreatimes.co.kr/business/banking-finance/20261123/personal-information-of-more-than-8000-clients-at-samsung-securities-breached) (via Risky Bulletin)

**Payment processor Cleverbridge says card data was stolen on Nov. 4.** It is notifying affected customers and asking them to watch their statements. [Cleverbridge](https://grow.cleverbridge.com/incident-update) (via Risky Bulletin)

**GlobeTopper rebuilt its cloud after attackers took code, databases, and customers' API keys.** The digital gift-card distributor told the SEC it expects to lose $2.5 million. [SEC filing](https://www.sec.gov/ix?doc=/Archives/edgar/data/1527702/000166357726000359/iqst8k112026.htm) (via Risky Bulletin)

**CIA and ODNI unclassified OSINT system.** [CyberScoop](https://cyberscoop.com/cia-odni-osint-data-breach/) *Also covered above under Adversary Playbook.*

**myColorado app: about 150,000 people's data likely stolen.** [The Record](https://therecord.media/mycolorado-app-down-data-breach) *Also covered above under Adversary Playbook.*

**Hex.pm account data may have been read.** [The Hacker News](https://thehackernews.com/2026/11/hackers-exploited-cvss-100-hexpm-rce.html) *Also covered above under Adversary Playbook.*

## Critical Infrastructure Attacks

**GAO: USDA and FDA aren't meeting all their duties to protect the food sector.** Auditing the two agencies against 16 statutory requirements for sector risk management agencies, GAO found they met most (threat mitigation, risk assessments, incident management) but only partly met or missed five, including sharing real-time threat information with CISA and running emergency-response exercises; both blamed a lack of staff and money. It lands after October's Iran-linked attacks on supermarket refrigeration systems. [Cybersecurity Dive](https://www.cybersecuritydive.com/news/food-agriculture-cybersecurity-usda-fda-gao-report/875596/)

**Portugal's energy agency suspends its energy-certification platform after a weekend attack.** [ADENE](https://www.adene.pt/sites-da-adene-encontram-se-condicionados/) (via Risky Bulletin)

**Up to 50 energy tankers hacked.** [WSJ](https://www.wsj.com/politics/national-security/iran-us-cyberattack-suspect-fed78942) *Also covered above under Adversary Playbook.*

**FinCEN systems offline.** [The Record](https://therecord.media/treasury-fincen-takes-systems-offline-after-cyber-incident) *Also covered above under Adversary Playbook.*

**Colorado's state ID app down.** [The Record](https://therecord.media/mycolorado-app-down-data-breach) *Also covered above under Adversary Playbook.*

**KEPCO, South Korea's electric utility, breached.** [KEPCO](https://www.kepco.co.kr/home/media/newsroom/pr/boardView.do?boardMngNo=15&boardNo=3197) *Also covered above under Data Breaches.*

## Zero Trust Tactics

**Broadcom fixes another critical vCenter authentication bypass.** CVE-2026-123903 (CVSS 9.8) in the VMware Directory Service lets anyone with network access to vCenter bypass authentication; it's one of 23 flaws patched across ESX, vCenter, Workstation, Fusion, and Avi Load Balancer. Broadcom says it's distinct from CVE-2026-123890, the vmdir bypass the China-nexus group Armory Castle exploited as a zero-day days earlier, and reports no exploitation of the new one. [The Hacker News](https://thehackernews.com/2026/11/vmware-vcenter-hit-by-another-critical.html); [SecurityWeek](https://www.securityweek.com/vmware-updates-patch-critical-esx-vcenter-vulnerabilities/)

**A Drupal flaw found by Anthropic's scanner is now exploited, and CISA gives agencies three days.** CVE-2026-132165 lets an unauthenticated attacker abuse Drupal core's installer to reinstall a site and take it over or run code; it was patched Nov. 18 and exploited from Nov. 19. Drupal raised it to "highly critical." It was found by Anthropic's opt-in OSS Scanner, which reported more than 5,000 vulnerabilities across 680 open-source projects as of early November. CISA's Nov. 24 KEV update also listed the unpatched Idunno.AntiCsrf flaw (covered 11-23) and an Optimizely Web Experimentation flaw. [SecurityWeek](https://www.securityweek.com/drupal-flaw-found-by-anthropic-scanner-exploited-in-attacks/); [CISA](https://www.cisa.gov/news-events/alerts/2026/11/24/cisa-adds-three-known-exploited-vulnerabilities-catalog)

**One bit in a .NET file's header bypassed Windows code integrity.** Google Project Zero's James Forshaw showed that the .NET Framework 4 falls back to loading an assembly from a plain memory copy when image loading fails, skipping the checks a loaded image would face. Clearing the IMAGE_FILE_EXECUTABLE_IMAGE flag forced that path and ran untrusted code even under Windows 11 S Mode's user-mode code integrity (CVE-2026-108398, fixed Oct. 13); the same behavior got past VirtualBox's process hardening (CVE-2026-87268, fixed in September). Both need a local user. [The Hacker News](https://thehackernews.com/2026/11/google-researcher-shows-how-single-bit.html)

**Palo Alto's Fragnesia fix.** [SecurityWeek](https://www.securityweek.com/palo-alto-networks-patches-fragnesia-flaw-used-to-root-firewalls/) *Also covered above under Adversary Playbook.*

**WP Connect plugins backdoored; no patch, remove them.** [The Hacker News](https://thehackernews.com/2026/11/wordpress-blocks-six-backdoored-wp.html) *Also covered above under Adversary Playbook.*

## Cyber Crime & Fraud

**Crypto platforms lost about $30 million in a weekend.** Chainflip suspended operations after attackers apparently got one of its vault keys and took $12 million, laundered almost immediately through Tornado Cash; Fusionist lost $5.7 million from its ACE bridge, and Cyber Bridge $1.1 million. [CoinDesk](https://www.coindesk.com/business/2026/11/21/cross-chain-protocol-chainflip-s-flip-tanks-30-after-suspected-usd4-86-million-vault-drain); [TradingView](https://www.tradingview.com/news/newsbtc:7dff75932094b:0-fusionist-ace-bridge-exploit-5-7m-loss-estimate-bithumb-freezes-trading/) (via Risky Bulletin)

**Check Point: forum takedowns have scattered the underground, not shrunk it.** After law enforcement shut major hacking forums, breaches and leaks rose while posting on big forums fell, with data brokers moving to smaller private channels. [Check Point](https://blog.checkpoint.com/security/darknet-forums-are-fragmenting-as-observed-breach-activity-rises/) (via Risky Bulletin)

**Newspaper subscription skimmer.** [Guardio](https://guard.io/labs/papercut---80-us-newspaper-websites-served-a-credit-card-stealer) *Also covered above under Adversary Playbook.*

**INCEPTION and the Com vishing clusters.** [The Hacker News](https://thehackernews.com/2026/11/okta-links-shinyhunters-associated.html) *Also covered above under Adversary Playbook.*

## Nation-State Cyber Policy & Law

**China doesn't always need to hack: it can buy, scrape, or partner its way to US data.** Justin Sherman, writing on the US-China Economic and Security Review Commission's new annual report, highlights its chapter on how China exploits America's data-rich environment: open sources, data brokers, ad systems, joint ventures, and research partnerships. He argues US policy treats data almost only as fuel for innovation and ignores the "asymmetric collection advantage" that weak privacy controls and many data sellers hand Beijing. [CSIS](https://www.csis.org/analysis/data-vulnerabilities-us-china-competition)

**Lawmakers press ID-verification companies after the IDScan breach.** Six senators and House members, led by Brian Schatz and Marsha Blackburn, wrote to identity-verification firms after September's breach put scans of more than 150 million driver's licenses and other IDs up for sale. They ask how the firms store and protect scans, warn that adversaries can "infer Americans' behavior through commercial data linked to government credentials," and urge zero-trust architecture and collecting and keeping less. Brian Krebs says he has found more than two dozen such companies that store scans by default. [The Record](https://therecord.media/idscan-data-breach-warning-congressional-letter)

**Nvidia's reinstatement of Jensen Huang: "too big to police"?** Intelligence and export-control experts tell WIRED the board's decision to bring Huang back 11 days after he resigned, amid an affair with a woman US intelligence suspects of ties to China's Ministry of State Security, undercuts Washington's warnings about Beijing's pursuit of US technology. The board cited input from "senior levels of the United States government"; President Trump says he lobbied the board directly. [WIRED](https://www.wired.com/story/jensen-huang-nvidia-us-national-security-risks/)

**Bangladesh's proposed Cyber Protection Act would let officials remove online content at will, Amnesty warns.** [Amnesty International](https://www.amnesty.org/en/latest/news/2026/11/bangladesh-proposed-changes-to-cyber-laws-risk-granting-authorities-excessive-power-to-police-online-content/) (via Risky Bulletin)

## Law Enforcement Disruption

**DOJ moves to recover another $1.1 billion stolen from Binance by North Korea.** The civil action would bring the total the US can seize to almost $2.9 billion of the roughly $6 billion stolen last month; more than $1.2 billion has already been laundered and the rest is frozen at Tether and Circle. North Korea row 11 already tracks the theft and the 11-12 seizure order. [DOJ](https://www.justice.gov/opa/pr/united-states-files-action-recover-more-1-billion-cryptocurrency-assets-stolen-north-korean) (via Risky Bulletin)

**DOJ says it charged more than 800 scammers in 400 cases this year.** It credits the White House's March executive order on scams; FBI Director Kash Patel used the same press conference to decline any detail on the NCIC breach. [DOJ](https://www.justice.gov/opa/pr/justice-department-announces-largest-ever-crackdown-scammers-targeting-over-800-defendants); [CyberScoop](https://cyberscoop.com/kash-patel-fbi-ncic-database-hack/)

**Europol seizes 57 illegal IPTV services in an 11-country operation.** They powered 321 streaming portals with more than 7.3 million users; investigators followed the crypto payments. [Europol](https://www.europol.europa.eu/media-press/newsroom/news/law-enforcement-follow-crypto-money-trail-behind-billion-euro-illegal-streaming-industry) (via Risky Bulletin)

## Privacy

**California's Delete Act enforcement reaches AI-derived data.** Since Aug. 1 the state privacy agency has strictly enforced data brokers' handling of deletion requests sent through its DROP platform. Two litigators argue brokers can't comply by deleting raw records alone: the law covers inferences used to build profiles, which brokers generate with machine learning, and they expect a wave of litigation over AI-derived data. [IAPP](https://iapp.org/news/a/navigating-drop-compliance-after-1-aug)

**New York and California age-gating rules take effect Jan. 1.** California's AB 1709, AB 1043, and SB 976 and the New York attorney general's regulations under the SAFE for Kids Act will change how social media works for users in both states; EFF walks through what to expect. [EFF](https://www.eff.org/deeplinks/2026/11/new-york-and-california-age-gating-rules-go-effect-new-year)

**Yandex removes privacy and anonymity language from its browser license.** The new terms, in effect since October, let it collect personal data, IP addresses, browsing history, and device details. [CNews](https://www.cnews.ru/news/top/2026-11-23_iz_litsenzionnogo_soglasheniya) (via Risky Bulletin)

## Automation Tactics

**UK NCSC: a "marked rise" in attacks run through agentic offensive frameworks, none using new weaknesses.** Since September, organizations across sectors have reported incidents involving red-team frameworks put to criminal use, with ARTEX the most prominent and Cairn, PentAGI, RedAmon, Xalgorix, and Darkmoon also named. NCSC says they add speed, scale, persistence, and low cost ("cheap, capable open models or illegal API resellers") but "no new capability," and are noisy and easy to detect for now, which "may not always be the case." CEO Richard Horne: weaknesses organizations once tolerated can now be found and used faster. [The Record](https://therecord.media/cyberattacks-uk-artificial-intelligence); [UK NCSC](https://www.ncsc.gov.uk/blogs/familiar-weaknesses-exploited-faster-defending-against-agentic-cyber-attacks); [CyberScoop](https://cyberscoop.com/uk-ncsc-ai-assisted-cyberattacks/)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** NCSC's finding that these frameworks reuse known weaknesses and are noisy supports the thread's premise that repeatable procedures can be detected phase by phase; GreyNoise's GT13 (above) shows the same kind of actor sitting undetected on the firewall management servers meant to enforce those controls. Status unchanged.*

**Anthropic opens Enterprise Frontier Safeguards to public beta.** EFS watches for misuse spread across many requests that look harmless one at a time, including AI-run attacks and agents going beyond what their operator intended, for customers on zero-retention terms; conversation data stays in the customer's own cloud under its own keys, Anthropic sees only metadata, and reports feed into SIEMs. Anthropic also published a guide to securing enterprise coding agents. [SecurityWeek](https://www.securityweek.com/anthropic-expands-enterprise-safeguards-for-detecting-ai-misuse/)

**AI-found Drupal flaw exploited within a day of its patch.** [SecurityWeek](https://www.securityweek.com/drupal-flaw-found-by-anthropic-scanner-exploited-in-attacks/) *Also covered above under Zero Trust Tactics.*

## AGI Arrival Timeline

**Current range:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11)

**Nate Silver: AI coding is racing ahead; its research taste is still "mid."** Building four forecasting models this year with a staff of four, Silver finds coding tools "substantially better in November than they were in August and September," turning three-day jobs into three-hour ones. But the models' judgment about what to build is "mid," he still pushes back on their overfitting, and outside coding he calls AI "well within the spectrum of 'normal technology.'" He warns that Silicon Valley "often mistake[s] superintelligent coding for broader (super)intelligence." [Silver Bulletin](https://www.natesilver.net/p/ai-is-moving-way-too-fast) (via Gmail)

**Source:** a statistical forecaster with a long public track record and no AI-lab stake, reporting first-hand use. *Credentialed expert judgment*, not measurement.

**Effect on the range:** held. The coding speed-up cuts Sooner but is already priced by METR's 11-06 finding; the gap between coding and broad judgment cuts Later and backs the condition on the open P50 review flag (parity in open-ended, non-verifiable work).

**The Riemann proof came decades ahead of what experts expected.** Timothy B. Lee recaps the Lean proof Levent Alpöge built with Claude (17 million lines, verified by independent checkers) and notes that Terence Tao had recently guessed an AI-assisted proof might come around 2050, while Forecasting Research Institute superforecasters gave about 10% to any further Millennium problem falling this year. His open question: does intelligence that solves Riemann generalize beyond math and code, or will AI "solve the toughest math problems but struggle to plan a wedding"? [Understanding AI](https://www.understandingai.org/p/an-anthropic-mathematician-just-solved)

**Source:** a journalist summarizing, citing one expert's guess (Tao) and a surveyed forecaster panel (FRI). *Commentary.*

**Effect on the range:** held. The proof itself was weighed on 11-23. What's new is how far experts and forecasters missed its timing, which argues for keeping the range wide rather than moving P50, since the miss is in one formally verifiable domain.

**Sherlock's view:** no shift; both pieces restate the split already in the file, fast in verifiable domains and unproven elsewhere. **Ryan's view:** none offered. **Seldon's call:** hold at P5 2029 · P50 2045 · P95 2075.

## Superintelligence Timeline

**Current range:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap.

**Does solving Riemann foreshadow recursive self-improvement?** Lee argues the mathematical optimization behind the proof "seems similar" to what makes models more capable, so it may foreshadow faster progress, "but nobody knows for sure." He quotes Eliezer Yudkowsky calling Riemann "the singular math result that had been named, in advance, as the obvious coal mine canary for dangerously advanced AI." [Understanding AI](https://www.understandingai.org/p/an-anthropic-mathematician-just-solved) *Also covered above under AGI Arrival Timeline.*

**Source:** a journalist presenting both readings. *Commentary.*

**Effect on the range:** held. It's an argument by analogy, not evidence that the AGI-to-superintelligence gap is closing faster than this file's one year.

**Silver doubts coding gains add up to an intelligence explosion.** He calls it "insane" that labs are "racing toward recursive superintelligence" without a confident plan to control it, yet isn't sure how much to extrapolate "from an extraordinary, exponential increase in coding acumen to an overall 'intelligence explosion.'" [Silver Bulletin](https://www.natesilver.net/p/ai-is-moving-way-too-fast) *Also covered above under AGI Arrival Timeline.*

**Source:** an independent statistical forecaster, from first-hand use. *Credentialed expert judgment.*

**Effect on the range:** held. His doubt about generalization is the bottleneck case the P95 tail (2076) already carries.

**Sherlock's view:** no shift. **Ryan's view:** none offered. **Seldon's call:** hold. Floor check: the AGI file didn't move, so no gap-model follow.

*Newsletter Tracker: Thread 5, ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house) (Oct 2026), status Under Pressure. Bearing: **Supports.** The thread argues voluntary lab commitments are no answer and binding rules must come from Congress. Silver, from outside the safety community, reaches the same diagnosis (labs racing without a control plan, a political system not "designed to handle this degree of rapid technological change"), though he offers no remedy. Commentary rather than new evidence; status unchanged.*

## Government Surveillance

**Meta says it would consider leaving Canada over the lawful-access bill.** The company told CBC it could pull its services if Parliament passes the bill, which it says threatens encryption. [CBC](https://www.cbc.ca/news/politics/meta-encryption-services-lawful-access-9.7424473) (via Risky Bulletin)

## Executive Leadership Changes

**Tom Kemp is leaving as director of California's privacy agency.** He led CalPrivacy for nearly two years, including the launch of DROP, the one-button opt-out platform now used by more than 600,000 Californians (each forcing more than 200 broker deletions on average, he says), the agency's largest fine, and the country's broadest rules on cybersecurity audits, risk assessments, and automated decision-making. He starts an undisclosed new role in January. [The Record](https://therecord.media/california-privacy-agency-kemp)

---

### Pending Evidence Queue

Nothing queued: every row in `Pending Evidence Queue.md` is already Included.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 75 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 59 | 31 | 2026-07-14 |
| The Hacker News | Contributed | 89 | 1 | 2026-07-14 |
| The Record | Contributed | 70 | 20 | 2026-07-14 |
| The Canon Project | No Contribution | 20 | 69 | 2026-07-14 |
| FFX Now | No Contribution | 18 | 72 | 2026-07-14 |
| Wired | Contributed | 57 | 30 | 2026-07-20 |
| CyberScoop | Contributed | 44 | 17 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 58 | 2026-09-01 |
| CISA Cybersecurity Advisories | Contributed | 29 | 32 | 2026-09-01 |
| SecurityWeek | Contributed | 56 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 36 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 13 | 18 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 30 | 2026-10-17 |
| EFF Deeplinks | Contributed | 16 | 15 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 8 | 23 | 2026-10-17 |
| IAPP News | Contributed | 20 | 11 | 2026-10-17 |
| CSIS Strategic Technologies Program | Contributed | 5 | 26 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 9 | 22 | 2026-10-17 |
| Risky.Biz | Contributed | 10 | 6 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 14 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 15 | 2026-11-10 |
| Resilient Cyber | No Contribution | 7 | 9 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | Contributed | 9 | 7 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 1 | 13 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 12 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 14 | 2026-11-12 |
| Understanding AI (TRIAL) | Contributed | 4 | 10 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 1 | 13 | 2026-11-12 |
| Zero Trust Forum | No Contribution | 0 | 2 | 2026-11-24 |

**No contribution today:**
- **The Canon Project**: newest review is *Mindf\*ck* (Nov. 23), covered 11-24 (read through Chrome; the listing is behind Cloudflare).
- **FFX Now**: 7 items dated Nov. 24 (Thanksgiving services, school bomb threats, an ICE lawsuit, Metro redevelopment, toll revenue, Morning Notes with 9 local items); no CIR fit. Today's Morning Notes wasn't up at run time (about 7 a.m.).
- **CSO Online CISO Appointments**: still no October or November section.
- **LEAP**: newest is Wave 13, covered 11-19.
- **CISO Tribune**: nothing newer than the Nov. 20 moves, covered.
- **NIST Insights**: newest post Oct. 27.
- **(ISC)²**: nothing after Nov. 24's ethics case studies, covered.
- **AI Alignment Forum**: no post since Eli Lifland's (Nov. 24), covered.
- **tl;dr sec, Detection Engineering Weekly, Resilient Cyber**: no issue since Nov. 19, Nov. 12, and Nov. 23 (covered).
- **AI as Normal Technology, Epoch AI, Reflective Altruism**: nothing new in the window.
- **Marcus on AI**: two posts. One on Nvidia and Anthropic share prices (market commentary); one citing an Axios report that OpenAI and Anthropic employees are alarmed, calling for agents with internet access to be pulled. Neither makes a dated, testable claim about capability limits, so both fail the strict filter.
- **Zero Trust Forum**: newest item is still the Nov. 20 podcast (read through headless Chrome).

**Crediting notes:** The Hacker News for GT13, Volant Manticore, INCEPTION, the Com clusters, Hex.pm, WP Connect, vCenter, and Forshaw's .NET bypass; The Record for FinCEN, myColorado, McDonald's Japan, Carnegie, the IDScan letter, Kemp, and the NCSC warning; CyberScoop for the CIA/ODNI breach; SecurityWeek (site feed) for Turnitin, Drupal, Fragnesia, and EFS; N2K CyberWire (issue 224) for the tanker hacks and KEPCO; CISA for the Nov. 24 KEV update; Risky.Biz (Nov. 25 Bulletin) for the newspaper skimmer, Radware, Samsung Securities, Cleverbridge, GlobeTopper, ADENE, the crypto thefts, Wagyu, UNC5792, Check Point's forum study, the Binance action, DOJ's scam cases, Europol's IPTV takedown, Meta and Canada, Yandex, and Bangladesh; Cybersecurity Dive for the GAO food-sector report; CSIS for Sherman; WIRED for the Huang piece; EFF for age gating; IAPP for DROP; Understanding AI for the Riemann piece; Gmail for Nate Silver's essay. **Recirculations excluded:** Shirudo (Cybersecurity Dive, SecurityWeek; covered 11-24), the 3.5 billion-record database leaks (WIRED; covered 11-24), CyberScoop's post-quantum OT op-ed (covered 11-24), the European Commission's EU Academy leak (SecurityWeek; covered 11-24), N-able's KEV listing (The Record; covered 11-24), Idunno.AntiCsrf exploitation (SecurityWeek; covered 11-23), Signal's block on AI agents (EFF; covered 11-21), Danfoss's AK-SM ICS advisory (CISA; covered 11-17), Davies' nomination and Kurtaj's release (Risky Bulletin; covered 11-24), and the Azure APIM, LaLiga, and NEXT items (Risky Bulletin; covered 11-24). **Considered, no CIR fit:** WIRED's "True Crime Community" TikTok piece (violent extremism, not cyber), the ex-OpenAI employee Abdulrahman Alfozan's $1 million bail (tracked since October; no new attribution), Canada's arrests of 75 young people hired over social media for offline crimes, CISA's Schneider Electric and AutomationDirect ICS advisories (no exploitation), Google Alerts snippets on cyber insurance and Gartner placements, a GAO list of 16 AI-in-cyber policy options (ExecutiveGov snippet only; worth a look next run), and Just Security's cyber-surveillance series (snippet only). **Tooling notes:** Gmail `search_threads` again returned no snippets, so the Google Alerts digest and Silver's essay were read with `get_thread` in plain text; The Hacker News, The Record, CyberScoop, SecurityWeek, WIRED, and IAPP articles all came through headless Chrome; CSIS and the Canon Project returned Cloudflare blocks to headless Chrome and were read through Chrome MCP; the Alignment Forum through its GraphQL API.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
