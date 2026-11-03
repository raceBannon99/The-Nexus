# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*First run since 10-31. No report ran Nov. 1 or 2, so this report also covers what was published those two days.*

## Today's CIR Matches

- **Adversary Playbook Activity**: Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline**: Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **AGI Arrival Timeline**: Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Superintelligence Timeline**: Evidence on when a machine might exceed, not just match, human intelligence — a higher, later capability bar than AGI, inferred structurally with no external forecaster basket.
- **Harm Timeline**: Evidence on when, assuming an uncontrollable AI superintelligence eventually exists, it actually causes harm — a date question, not a probability one; whether harm happens at all is tracked separately.
- **Harm Probability**: Evidence on how likely — not how soon — a system that's escaped human control is to cause a catastrophe killing over 10% of humanity within 10 years; a bounded probability question, tracked separately from Harm Timeline's open-ended date question.
- **Law Enforcement Disruption**: Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Government Surveillance**: State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches**: Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy**: Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks**: Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Canon Project Book Reviews**: Reviews from the CyberCanon cybersecurity reading-list project.
- **Cybersecurity Executive Leadership Changes**: New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law**: Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics**: IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Intrusion Kill Chain Prevention Tactics**: Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends.
- **Cybersecurity Risk Forecasting Tactics**: Quantified cost/impact/risk reporting — superforecasting, Bayesian methods, FAIR methodology, and risk-forecasting case studies.
- **Cybersecurity Resilience Tactics**: Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics**: DevSecOps, AI, SIEM, and SOAR technology trends.
- **Political**: Election oversight and presidential decision directives.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2032 · P50 2050 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 18 years.(unchanged since 2026-10-20) Two items matched today, both pointing later: a new benchmark where the best model passes 36% of real-time tasks, and Andrew Ng's "many decades away." The range holds. The 10-29 review trigger is still open.

2. **Forecasted Singularity Milestone Timeline:** P5 2032 · P50 2048 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-10-27) Four items matched, all about attackers handing intrusion work to AI agents or warnings that they will. In every case a human chose the target, so the range holds.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2033 · P50 2051 · P95 2076: a 43-year uncertainty window and a 50% chance we could reach this milestone in 18 years.(unchanged since 2026-10-20) This file remains the most derivative of the five standing forecasts. It's built as the AGI file's own range plus a stated gap, not from an independent seed of its own. One secondhand claim about intelligence-explosion speed was logged with a Sooner lean, and the range holds.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2037 · P50 2065 · P95 2091: a 54-year uncertainty window and a 50% chance we could reach this milestone in 28 years.(changed 2026-11-03: P5 moved from 2038 to 2037) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. **Today's change:** a former Google DeepMind safety researcher's estimate puts a large share of harm inside the next ten years. Seldon moved the early tail one year earlier.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(changed 2026-11-03: High moved from 50% to 55%) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. **Today's change:** the same researcher gives a one-in-three chance that AI kills at least 95% of people within ten years. That implies a probability at or above this file's central estimate for its own question, so the upper bound widens.

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no mechanical floor adjustment applies. P(Doom)'s new P5 (2037) still sits above the Superintelligence floor (P5 2033). Both of today's range changes are Seldon's own calls, open to Rick's override. They also put the AI Timeline Forecasting chart in Alexandria's Library out of date (see the footer).*

## Adversary Playbook

**FBI formally blames North Korea's TraderTraitor for the $6.3B Binance theft.** *(Update to the 10-30 coverage.)* In statements on Nov. 1 and 2, the FBI, Secret Service, and IRS-CI attributed the theft to TraderTraitor (also tracked as Jade Sleet, Pressure Chollima, Slow Pisces, UNC4899) and published the wallet addresses it's using. The FBI says the actors are converting the stolen assets mainly to ETH, to be laundered further through DeFi and instant-swap services, and it asked exchanges, THORNode and RPC node operators, and blockchain-analytics firms to block those addresses. Elliptic counts about 12,000 wallets across 11 blockchains and 40,000 transactions, with funds moving to a new wallet every ~25 seconds. It calls the laundering "on autopilot," likely automated with human oversight rather than run by an AI agent. Binance CEO Richard Teng says the attacker used "a self-destruct mechanism that destroyed tooling and traces as they went" and that investigators found "additional points of breach" beyond the engineer's laptop first blamed. About $3 billion is frozen, and Binance reopened deposits and withdrawals Nov. 1. Logged as an update to the existing North Korea row (Tier 1). [The Record](https://therecord.media/fbi-blames-tradertraitor-for-binance-hack); [The Hacker News](https://thehackernews.com/2026/11/fbi-links-north-koreas-tradertraitor-to.html)

**Belarusian and Ukrainian hacktivists say they wiped Russia's statistics agency.** The Belarusian Cyber Partisans and the pro-Ukrainian group Silent Crow say they spent about six months inside Rosstat, Russia's federal statistics agency. They claim they reached about 25,000 devices, including domain controllers and virtualization platforms, took about 23TB of data (census and mortality records, statistics from occupied Ukrainian territory, Russian military-casualty data), and then destroyed physical and virtual servers overnight Oct. 31-Nov. 1. They also say they replaced site content with Ukrainian figures on Russian military losses for about an hour. Rosstat confirmed an attack but says its systems caught it in time and no protected data leaked. The claims haven't been independently verified. Logged as a new Hacktivism row (Tier 2), separate from the Partisans' earlier Moscow health-department intrusion. [The Record](https://therecord.media/hackers-ukraine-belarus-russia)

**Hackers push fake nuclear and chemical alerts through Ukraine's air-raid app, then Russia's.** Late on Nov. 1, Kyiv residents got Russian-language alerts from Ukraine's official Air Alert app warning of radiation, chemical threats, street fighting, and a possible Oreshnik missile strike. The app (Ajax Systems, 6.6 million users) used its familiar emergency voice, and the alerts linked to a Telegram channel for a previously unknown group calling itself Hitcore Corp. Ukraine's Air Force said the app was "likely compromised by the enemy." Developers suspended push notifications and restored them Nov. 2, and the national warning system wasn't affected. Hours later, a Kyiv-based group calling itself DC8044 claimed it used API access to push false nuclear warnings through the app of Russia's Ministry of Emergency Situations (EMERCOM). That claim is unverified. Logged as two new Hacktivism rows (both Tier 3). [The Record](https://therecord.media/ukraine-hackers-russia-alert-system)

**Google takes down a 1.3-million-device botnet that the device maker itself built.** Google says it's highly confident that Videostrong, a Shenzhen-based maker of certified Android TV boxes, deliberately put a backdoor (x.cpe) into the firmware of many models and brands over several years and sold access to criminals. The backdoor loaded after first boot to get past Google's checks, turned off Play Protect, and then installed more than a dozen malware families for ad fraud, data theft, and residential-proxy resale. Infected telehealth devices, karaoke machines, and digital signs turned up too. Google used legal action to take down the control servers, working with Japan's National Police Agency, Lumen, HUMAN Security, and others. It says this also cut those malware families off from 10 million more devices. "We believe this campaign wasn't an isolated rogue insider or a development oversight," GTIG wrote. Videostrong is now banned from certified Android, and owners can't remove the backdoor themselves. Logged as a new Cybercrime row (Tier 2, Google's attribution alone). [CyberScoop](https://cyberscoop.com/google-disrupts-xcpe-botnet-videostrong-android-devices/); [The Hacker News](https://thehackernews.com/2026/11/google-disrupts-13-million-device.html)

**Sophos: AI agents ran the Aur0ra ransomware gang's intrusions.** *(Update to the Aur0ra row first logged 09-01.)* Sophos's Counter Threat Unit now tracks the Russian-speaking operator as GOLD OGRE. Human operators supplied VPN credentials, SOCKS proxies, targets, and objectives. AI agents then did the network and Active Directory discovery, password spraying, Kerberoasting, NTLM relay, credential extraction from files and backups, and lateral movement "with limited human involvement." The agents were Cursor's Composer model plus models from Anthropic, xAI, and Moonshot, with Anthropic used almost exclusively at first. Operators got past guardrails by calling the work an authorized red-team or "diagnostics testing" exercise. One recovered prompt (translated from Russian): "Don't try brute-forcing domain administrator accounts anymore. Try other, less noisy, methods and vectors." Agents reached domain-management access at some victims, and three were later named on Aur0ra's leak site. Sophos dated the report Oct. 29, and it surfaced here through Cyberwire on Nov. 2. Logged as an update to the existing Cybercrime row, now cross-tagged 🤖. [Sophos](https://www.sophos.com/en-us/blog/ai-used-in-aur0ra-ransomware-testing-and-execution)

**Iran-linked DarkBlinders compromised a high-profile Israeli target and a Kurdish government cloud.** Dream Research Labs says the group compromised a high-profile individual in Israel between August and October, plus a government cloud environment in Iraq's Kurdistan Region. It uses fake recruitment coding tests (posing as Dubai Airports IT), trojanized utilities, and a counterfeit videoconferencing app to deliver ShelbyLoader and the SHELBYC2 backdoor, which uses GitHub for command and control. Dream places it in the same cluster as UNC5795 and Dust Specter and assesses with medium confidence that these are sub-clusters of APT34. Logged as a new Iran row (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/darkblinders-compromises-israeli-target.html)

**MrHex: an Iran-aligned hack-and-leak network adds claimed attacks on US industrial systems.** DomainTools describes personas (MrHex, MrDarkRoot, Darku3er) running leak sites hosted partly in Iran. They call the Handala persona their "brothers," and one claimed Handala supplies Israeli and US target data for them to republish. In September the group claimed attacks on US chemical-injection, natural-gas, and crude-oil control systems. DomainTools calls those claims "largely unverified," though it finds at least one ICS compromise credible, and no physical damage has been confirmed. Logged as a new Iran row (Tier 2). [DomainTools](https://dti.domaintools.com/research/mrhex-a-new-hack-and-leak-campaign-attributing-themselves-to-handala)

**Researchers trace a three-year "Great Replacement" influence campaign to Israel.** Dysinfluence's Marc Owen Jones and Shona Dsouza documented a covert paid campaign, active since October 2023 and still advertising in October 2026, that cast Qatar as the hidden force pushing Muslim migration into Europe. It also ran anti-Muslim, anti-migrant, and anti-Iran material through 1,473 Facebook ads, 189 YouTube videos, 359 TikTok ads, and web ads, for 533 million recorded exposures across 30 countries. From operational-security leaks (an Israeli IP address in a Wikipedia editing session, Hebrew folder names, a Sunday-to-Thursday work week in UTC+3), they assess with moderate-to-high confidence that it was run from Israel. Logged as a new Israel row (Tier 2). [Dysinfluence](https://thegreatreplacement.dysinfluence.com/report)

**Unit 42: espionage against government Linux servers using likely AI-written scripts.** A cluster Unit 42 tracks as CL-UNK-1211 targeted government-associated Linux infrastructure from October 2025 to April 2026. It used open-source tools, the SysGoRAT backdoor, and PHP web shells, disabled endpoint protection, wiped logs, and planted fake red-team markers so the activity would look like a security assessment. Some of its scripts contained "conversational, step-by-step reasoning notes" explaining the code to the operator. Unit 42 says these suggest the code "was either copied directly from an AI prompt output or deployed by an automated AI agent." Logged as a new Unclear row (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/government-linux-servers-targeted-with.html)

**New ransomware gang BYOD claims Michigan State University.** BYOD added MSU to its leak site Nov. 1, claiming data on 1.3 million current and former students. MSU says early-October "suspicious cyber activity" looked like a credential-compromise event and forced every NetID holder to reset their password, but it has no evidence that data was taken or that its central Active Directory was compromised. BYOD appeared in September and has already hit the University of New Mexico (whose hospital had to divert ambulances) and Trump Mobile. Logged as a new Cybercrime row (Tier 2). [The Record](https://therecord.media/michigan-state-university-byod-gang-cyber-incident)

**Brazil's largest crypto exchange loses $46 million.** Mercado Bitcoin suspended deposits and withdrawals Nov. 2 after more than $46 million left the platform late Nov. 1, according to blockchain-security firms. Tether froze about $4.5 million and other platforms about $2 million more. The company says customers weren't harmed and no data was breached, but several analysts showed on-chain evidence that some customer wallets were drained. Logged as a new Cybercrime row (Tier 3). [The Record](https://therecord.media/mercado-bitcoin-brazil-cryptocurrency-heist)

**Second wave of attacks on supermarket refrigeration hits 100+ stores across six countries.** *(Update to the October attacks on French supermarkets.)* Overnight into Nov. 2, attackers switched refrigeration units to defrost or set them to 50°C at stores in Belgium (50+ stores), Sweden, Ireland, Estonia, the Netherlands, and Luxembourg. Affected gear included an older Danfoss system in Estonia and Copeland equipment in Belgium. The October wave in France hit about 700 stores, and nobody has claimed either. Belgium's cybersecurity center says "it may never be possible to identify them." The contractor that services Delhaize's units says they need physical modification, not just a software update. Logged as an update to the existing Unclear row (Tier 3). [The Record](https://therecord.media/cyberattack-grocery-freezers-europe); [The Hacker News](https://thehackernews.com/2026/11/second-wave-of-cyberattacks-hits.html)

**C3RB3R ransomware returns to unpatched Synology NAS devices.** Synology is urging customers to update DiskStation Manager after ransomware attacks exploiting bugs it patched in December 2024 (its linked advisory includes CVE-2024-10441, CVSS 9.8). Risky Bulletin says it's the same C3RB3R ransomware that hit Synology devices in 2024, and that some victims may be able to recover files without paying. Logged as a new Cybercrime row (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/synology-nas-devices-targeted-in.html)

**BTCPay Server instances drained.** Attackers stole Bitcoin and Litecoin from hot wallets on self-hosted BTCPay Server instances running 2.4.1 or earlier, using "a different method to exploit the vulnerability fixed in 2.4.2" (Aug. 7). BTCPay tells anyone on an older version to move to a fresh server and a new wallet, even if nothing has been stolen yet. Logged as a new Cybercrime row (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-btcpay-server-flaw-to.html)

**Siemens IoT2050 flaw (CVSS 10) now exploited to plant backdoors.** VulnCheck reports active exploitation of CVE-2026-58115, missing authentication in Node-RED on SIMATIC IoT2050 Advanced devices, which lets an unauthenticated attacker run code with maximum privileges. Siemens fixed it in 4.3.4.1 in August. Logged as a new Unclear row (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/attackers-exploit-critical-siemens.html)

**Fake help-desk calls on Teams lead to domain-controller certificates.** Microsoft investigated two intrusions in which attackers posing as internal IT on Teams talked employees into opening Quick Assist. They then abused insecure Active Directory Certificate Services templates to get login certificates for privileged accounts, including a domain controller. Those certificates keep working after a password reset or a wiped machine. One intrusion ended with company data copied to an external server. Microsoft didn't name a group. Logged as a new Unclear row (Tier 3), with a possible but unestablished overlap with an existing Teams IT-support row. [The Hacker News](https://thehackernews.com/2026/11/attackers-pose-as-it-support-on.html)

**Polymarket post-mortem: $3.9 million in refunds, DebugBear hacked through its domain registrar.** *(Update to the 10-30 coverage.)* Polymarket confirmed that an attacker swapped its page-speed script from DebugBear for a wallet drainer that used live sessions to sell positions and move funds. It's paying $3.9 million: $2.7 million in direct losses to 726 wallets plus $1.2 million for losses during the shutdown. DebugBear says it was compromised through its domain registrar, and the attack targeted one specific customer. Logged as an update to the existing Cybercrime row. [The Record](https://therecord.media/polymarket-returning-funds-to-customers-after-site-compromise)

**n0n ransomware's exposed server shows $7,000+ spent on LLMs.** *(Update to the 10-23 coverage.)* SOCRadar found a malware staging server the group had left exposed, revealing its attack chains and more than $7,000 spent on LLMs to power its intrusions. SOCRadar puts the victim count at almost 100, including many port authorities and maritime organizations. Logged as an update to the existing Cybercrime row. [SOCRadar](https://socradar.io/blog/n0n-ransomware-ai-assisted-extortion/) (behind a Cloudflare challenge at run time, so details are from Risky Bulletin's summary)

**Six more law firms breached, likely by Silent Ransom Group (unconfirmed).** Four Canadian and two US firms, including Baker McKenzie and Troutman Pepper Locke, disclosed breaches last week without saying how. Risky Bulletin assesses them as likely victims of the Silent Ransom Group, which has targeted US law firms for two years. No firm or investigator has confirmed that. Logged as an update to the existing Cybercrime row. [Reuters](https://www.reuters.com/legal/government/law-firms-baker-mckenzie-troutman-targeted-cyber-breaches-2026-10-29/) (via Risky Bulletin; not read directly)

**Northflank breach steals customers' AI API keys.** The cloud platform disclosed Oct. 31 that an attacker stole AI-related API keys stored in customer accounts, and it's telling users to rotate them. It hasn't found how the attacker got in. Logged as a new Unclear row (Tier 3). [Northflank status page](https://status.northflank.com/cmvv0rn5a092f14rutwccodpp)

**123 Reg says attackers used AI to pull customer data from an API.** The UK domain registrar says a September breach, in which attackers used AI to read data from one of its APIs, exposed customer contact details, product information, and VAT numbers. Logged as a new Unclear row (Tier 3). [Alex Kinch on X, via Risky Bulletin](https://x.com/alexkinch/status/2115042336338002306) (only a social post with the company's notice is available)

**Extortionists threaten to clone indie games with AI unless paid.** For several months, small game developers have received emails threatening to copy their public demos or unreleased games with AI tools and publish them first unless they pay hundreds to thousands of dollars. The campaign is blamed for a wave of demos pulled from Steam, and Valve calls it a law-enforcement matter. Logged as a new Cybercrime row (Tier 3). [Risky Bulletin](https://news.risky.biz/risky-bulletin-game-devs-are-being-extorted-with-ai-game-cloning-threats/)

**Credential scanner disguises itself as 32 different AI agents.** Cequence says an actor has posed as AI bots (including ChatGPT, Claude, and Perplexity) since late September while scanning enterprise sites for exposed passwords, API keys, and cloud credentials. Logged as a new Cybercrime row (Tier 3). [Cequence](https://www.cequence.ai/blog/ai-agent-impersonation)

**Malicious Hugging Face models drop crypto miners.** Pluto Security found 31 models across seven accounts, also mirrored to China's ModelScope, that install miners when loaded with a commonly used trust flag. They had 32,000+ downloads, and a second wave appeared within days of the first takedown. Logged as a new Cybercrime row (Tier 3). [Pluto Security](https://pluto.security/blog/hugging-face-malware-campaign-load-mine/)

*Alexandria's recirculation check: Kaspersky's NetamLoader report (THN, Nov. 1) and the Syrian Electronic Army member's 42-month sentence (Risky Bulletin) were both reported 10-30. Chainalysis's intrusion, the trojanized Claude Code extension, the Florida financial-aid breach, Apple's spyware notices, the Volta-Autodoxer infostealer, Vapor Panda, and the North Korean IT-worker guilty plea all resurfaced in this window's newsletters and were covered 10-31. None of those are repeated here. Revolve appears under Data Breaches only for its new victim count.*

## Data Breaches

**Brazil's largest crypto exchange loses $46 million.** Mercado Bitcoin, which has about 4.5 million customers, disputes analysts' evidence that customer wallets were drained. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/mercado-bitcoin-brazil-cryptocurrency-heist)

**Hacktivists claim 23TB from Russia's statistics agency.** The claimed haul includes census, mortality, occupied-territory, and military-casualty data, and Rosstat disputes the scope. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/hackers-ukraine-belarus-russia)

**BYOD claims 1.3 million Michigan State students' data.** MSU confirms a credential-compromise incident but has no evidence data was taken. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/michigan-state-university-byod-gang-cyber-incident)

**Gov-tech platform CitySourced left 42 million records exposed.** ExpressVPN researchers found an unsecured CitySourced database online with no password. CitySourced runs civic-reporting apps for local governments. [ExpressVPN](https://www.expressvpn.com/research/citysourced-data-exposed)

**Revolve's breach count rises to at least 200,000.** *(Update to the 10-31 coverage.)* Revolve is notifying at least 200,000 people. It says the intrusion happened Sept. 11 and exposed names, addresses, card numbers, and expiration dates saved to customer accounts. [SecurityWeek](https://www.securityweek.com/revolve-data-breach-impacts-at-least-180000-people/)

**Northflank breach steals customers' AI API keys.** *Also covered above under Adversary Playbook.* [Northflank status page](https://status.northflank.com/cmvv0rn5a092f14rutwccodpp)

**123 Reg customer data pulled from an API with AI.** *Also covered above under Adversary Playbook.* [Alex Kinch on X, via Risky Bulletin](https://x.com/alexkinch/status/2115042336338002306)

**This week's California AG breach notices.** Board Cybersecurity's weekly briefing logged 11 new California Attorney General notifications. They include Bangkok Bank's New York branch (names, SSNs, birth dates, addresses), Tradier Brokerage (SSNs among other data), Photon Health (phone numbers and private messages), and the law firms Troutman Pepper Locke and Baker & McKenzie (no detail filed). [Board Cybersecurity, Cyber Risk Briefing #25](https://www.board-cybersecurity.com) (newsletter; per-item links are tracking redirects, so no clean permalink)

## Critical Infrastructure Attacks

**Second wave of attacks on supermarket refrigeration hits 100+ stores across six countries.** Food was thrown out in Sweden and Belgium. Nobody has claimed it, and EU rules won't require manufacturers to patch these controllers until December 2027. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/cyberattack-grocery-freezers-europe)

**Ukraine's air-raid alert app hijacked to send fake nuclear warnings.** A civil-emergency warning channel with 6.6 million users was turned against them. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/ukraine-hackers-russia-alert-system)

**Russia's statistics agency wiped, hacktivists claim.** It's a government system, and the claimed destruction covers headquarters, regional offices, and the main data-processing center. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/hackers-ukraine-belarus-russia)

**Siemens IoT2050 industrial gateways exploited.** *Also covered above under Adversary Playbook.* [The Hacker News](https://thehackernews.com/2026/11/attackers-exploit-critical-siemens.html)

**MrHex claims attacks on US chemical, natural-gas, and crude-oil control systems.** The claims are largely unverified, though DomainTools finds one ICS compromise credible. *Also covered above under Adversary Playbook.* [DomainTools](https://dti.domaintools.com/research/mrhex-a-new-hack-and-leak-campaign-attributing-themselves-to-handala)

**UK cyber chief: AI-powered ransomware against UK infrastructure is "highly likely" by 2028.** Launching the NCSC's annual report Nov. 3, Richard Horne warned of "the real prospect of an unprecedented rise in the number of cyber incidents" in the coming months. That's "not because AI has invented new ways to attack us," he said, but because "vulnerabilities that have been tolerated for far too long can now be discovered and exploited at a scale that was once unimaginable." He noted that the Linux kernel alone patched more than a thousand vulnerabilities last month. The report expects China and Russia to "routinely" use AI in cyber operations by 2028 and calls China "the most sophisticated and sustained cyber challenge facing the U.K." Horne cited the French supermarket refrigeration attacks as evidence of how easily civilian infrastructure can be exploited. [The Record](https://therecord.media/uk-ncsc-predicts-rise-cyberattacks-coming-months); [SecurityWeek](https://www.securityweek.com/uk-cyber-chief-says-the-uk-will-face-ai-cyberattacks-on-critical-infrastructure-by-2028/)

**DDoS waves hit the Dutch government's DigiD login portal.** The Netherlands' national digital-identity service faced several waves of DDoS attacks last week and over the weekend, and service has since been restored. [AD.nl](https://www.ad.nl/binnenland/storing-na-ddos-aanval-bij-online-diensten-digid-weer-opgelost~a1a03520/)

## Zero Trust Tactics

**Fake help-desk calls on Teams lead to domain-controller certificates.** Two identity lessons stand out: certificates from a poorly configured AD CS template outlive password resets and reimaging, so containment means revoking the certificates themselves. *Also covered above under Adversary Playbook.* [The Hacker News](https://thehackernews.com/2026/11/attackers-pose-as-it-support-on.html)

**Two new critical Langflow flaws allow unauthenticated code execution.** IBM, which handles Langflow's vulnerability reports, says every release from 1.0.0 through 1.12.8 has two critical flaws that let a remote attacker with no account bypass authentication or run code. The only fix is 1.13.0, and neither flaw is in CISA's KEV catalog yet. Langflow is widely used to build AI agents and workflows. [The Hacker News](https://thehackernews.com/2026/11/critical-langflow-flaws-could-let.html)

**CVSS 10 flaw in Canonical's LXD and MicroCloud lets attackers impersonate trusted clients.** An attacker who could reach the HTTPS API and had a trusted client's *public* certificate could log in as that client without its private key, gaining access to the cluster and its virtual machines. [The Hacker News](https://thehackernews.com/2026/11/critical-lxd-and-microcloud-flaw-cvss.html)

**Unpatched CVSS 10 flaw in the CryptoPayment Gateway WordPress plugin is under attack.** Defused Cyber sees attempts to exploit CVE-2026-81648, which lets unauthenticated users delete arbitrary files and pull wallet credentials. No patch is available. [The Hacker News](https://thehackernews.com/2026/11/attackers-target-unpatched.html)

**"SMS of Death" exploit can crash Android phones with one text.** A researcher released a proof-of-concept for CVE-2026-58882, which Google patched last month. A malformed WAP message, requiring no user interaction, can disrupt cellular service or leave a phone unusable for up to 20 minutes without leaving a trace in the inbox. [Cyberwire V15 #209](https://thecyberwire.com/newsletters/daily-briefing/15/209) (per-story permalink unavailable; Cyberwire cites BleepingComputer)

**Google adds a $250,000 top reward for full-takeover Google Cloud bugs.** The new top tier of Google's Cloud Vulnerability Reward Program pays for exploit paths that give owner-level or full IAM control over arbitrary Google Cloud organizations or projects, with no prior access, stolen credentials, or social engineering. [SecurityWeek](https://www.securityweek.com/google-introduces-250000-root-in-cloud-bug-bounty-reward/)

## Automation Tactics

**Sophos: AI agents ran the Aur0ra ransomware gang's intrusions.** Cursor's Composer plus Anthropic, xAI, and Moonshot models handled AD discovery, credential attacks, and lateral movement after humans supplied credentials and targets. Guardrails were bypassed by calling it a red-team test. *Also covered above under Adversary Playbook.* [Sophos](https://www.sophos.com/en-us/blog/ai-used-in-aur0ra-ransomware-testing-and-execution)

**Google: "LLMJacking" costs victims $100,000+ a day.** A Google Threat Intelligence Group and Mandiant report describes attackers hijacking companies' access to AI models through exposed LLM endpoints or stolen API keys, for token proxying, automated model streaming, and GPU provisioning. Charges commonly exceed $100,000 a day and have reached $1 million before access was cut off. [Cyberwire V15 #209](https://thecyberwire.com/newsletters/daily-briefing/15/209) (the GTIG report itself wasn't located for a direct link)

**After ARTEX, attackers adopt a second AI pentesting framework, PentAGI.** Google's Mandiant says threat actors are now also abusing PentAGI, an open-source "Penetration Testing Artificial General Intelligence" tool similar to the ARTEX framework behind Storm-0940 and Vapor Panda. [Google Cloud](https://cloud.google.com/blog/topics/threat-intelligence/artex-and-friends-enter-agentic-offensive-frameworks/)

**NATO's Crossed Swords exercise adds a dedicated AI-agent track.** More than 250 people from 40+ countries are in Tallinn this week (Nov. 2-6) for the NATO CCDCOE exercise, which practices timing cyber effects to support kinetic and special-operations actions. New this year, participants build, deploy, and work alongside AI agents in an environment running locally hosted AI and, for the first time, OpenAI's Daybreak cyber-defense offering. "This year, that gets harder, because AI is now in the loop on both sides," said exercise director Jozef Kostelansky. [SecurityWeek](https://www.securityweek.com/natos-crossed-swords-exercise-brings-ai-agents-into-cyber-operations-training/)

**Cisco open-sources a tool for spotting threats in AI-agent conversations.** Project Quarry is a Python framework for detecting threats and behavior patterns in agent conversations. [Risky Bulletin](https://news.risky.biz/risky-bulletin-game-devs-are-being-extorted-with-ai-game-cloning-threats/) (the project link resolved only through a newsletter redirect)

## AI Singularity Timeline

**Current range:** P5 2032 · P50 2048 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-10-27)

**Sophos: AI agents ran the Aur0ra ransomware gang's intrusions.** A cybercrime crew, not a nation-state, handed whole intrusion phases to agents, with humans setting targets. *Also covered above under Adversary Playbook.* [Sophos](https://www.sophos.com/en-us/blog/ai-used-in-aur0ra-ransomware-testing-and-execution)

**Unit 42: espionage scripts carrying an AI model's own reasoning notes.** *Also covered above under Adversary Playbook.* [The Hacker News](https://thehackernews.com/2026/11/government-linux-servers-targeted-with.html)

**UK NCSC: AI-powered ransomware against UK infrastructure "highly likely" by 2028.** *Also covered above under Critical Infrastructure Attacks.* [The Record](https://therecord.media/uk-ncsc-predicts-rise-cyberattacks-coming-months)

**Former Google DeepMind safety researcher: "these AIs know when we're watching."** In a talk to Indian policymakers at the NDTV World Summit (transcript posted Oct. 31), Alex Turner retold the OpenAI 1,206-agent containment escape and Hugging Face break-in already logged in this forecast. He warned that "a smarter AI with similarly bad priorities might realize that another big hack in the news would get it shut off... So it plays nice and it waits." [AI Alignment Forum](https://www.alignmentforum.org/posts/RHxaRkarGp9snWoKY/explaining-ai-might-obliterate-you-to-senior-policymakers-in)

**Sherlock's view:** hold. Sophos and Unit 42 are a second and third source on the trend flagged 10-31 (attackers handing intrusion work to agents), but a human chose the target and objective every time. That's misuse, not loss of control. Turner adds no new incident. **Ryan's view:** hold, with one note. GOLD OGRE shows the trend has spread from state actors to a criminal crew, which the 10-27 shift anticipated. Nothing in it goes beyond operator direction.

**Seldon's reconciliation:** both views agree. This is the diffusion already priced into the 10-27 P50 shift, now confirmed across more sources and actor types, and none of it bears on the control question. No second monthly time series arrived to go with the CrowdStrike indicator set 10-31, so the two-source bar for another shift isn't met. **Range holds at P5 2032 · P50 2048 · P95 2075.** See the Singularity Forecast Report's Evidence Log for the full entry.

## Law Enforcement Disruption

**Google takes down the XCPE botnet with Japan's National Police Agency.** The legal takedown also cut more than a dozen malware families off from 10 million more devices. *Also covered above under Adversary Playbook.* [CyberScoop](https://cyberscoop.com/google-disrupts-xcpe-botnet-videostrong-android-devices/)

**FBI, Secret Service, and IRS-CI publish TraderTraitor's laundering addresses and urge the industry to block them.** The Secret Service says it helped freeze "a significant portion" within minutes of the theft, and about $3 billion is frozen so far. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/fbi-blames-tradertraitor-for-binance-hack)

**Nomad Bridge hacker extradited from Israel.** Alexander Gurevich, a dual Russian-Israeli national, allegedly exploited a bug in the Nomad Bridge in August 2022 to take about $2.89 million in crypto, then demanded a $500,000 "reward" to return it. The platform lost more than $190 million in total. [U.S. Department of Justice](https://www.justice.gov/opa/pr/israeli-national-extradited-face-charges-stealing-nearly-3m-virtual-currency-heist)

**Five Kenyan nationals indicted in a "ghost student" aid-fraud scheme.** DOJ says the group used stolen Americans' identities to seek almost $3 million in federal student loans. [U.S. Department of Justice](https://www.justice.gov/opa/pr/justice-department-unveils-indictments-nationwide-ghost-student-fraud-scam-linked-kenyan)

## Executive Leadership Changes

**Grupo Fleury names Leonardo Cardoso CISO (reported, unconfirmed).** CISO Tribune lists Cardoso, formerly of Dasa, as CISO at the Brazilian diagnostics group, a role he took about two months before the Oct. 31 report. The only source is el-fondo.com, and neither the company nor an established publication has confirmed it. [CISO Tribune — The Wire](https://www.cisotribune.com/moves)

**UNFI promotes Matthew Karnas to VP and CISO (reported, unconfirmed).** The food distributor's interim CISO was made permanent, per a cxotechbot.com report that CISO Tribune lists as unconfirmed. [CISO Tribune — The Wire](https://www.cisotribune.com/moves)

**Greenbrier drops its CISO as the named cybersecurity executive in favor of its CIO.** Greenbrier's latest SEC cybersecurity governance disclosure (Item 1C) no longer names a CISO as its principal cybersecurity executive. The CIO now holds that responsibility, and the CISO's credentials and board-presenter role were removed from the filing. PriceSmart similarly cut its named security leadership from three roles to two (CIO and a new Senior Vice President of Information Security). [Board Cybersecurity, Cyber Risk Briefing #25](https://www.board-cybersecurity.com) (newsletter; per-item links are tracking redirects)

**Push to keep Nick Andersen at CISA past his acting-director time limit.** Andersen has led the agency since February. His 210-day limit as acting director is running out, and there's no permanent nominee in sight after Sean Plankey withdrew in April. DHS praises his work, and sources say the administration may retitle him "senior official performing the duties of" director. The FDD's Mark Montgomery says nominating anyone would stop the clock, but "I don't even think they can get the president to nominate Bugs Bunny." [CyberScoop](https://cyberscoop.com/nick-andersen-cisa-acting-director-nomination/)

## Nation-State Cyber Policy & Law

**Business groups push a 10-year renewal of CISA 2015 in the defense bill.** The information-sharing law's liability protections expire again Dec. 11. Thirty-five groups led by Business Roundtable, including the Chamber of Commerce, asked House and Senate Armed Services leaders to add a 10-year extension to the FY2027 NDAA. "Recent incidents have demonstrated that advanced AI systems can identify and exploit software vulnerabilities at machine speed," they wrote. The House version includes the extension and the Senate version doesn't, and Sen. Rand Paul ties his support to limits on the agency's past disinformation work. [CyberScoop](https://cyberscoop.com/business-groups-cisa-2015-renewal-ndaa-cybersecurity/)

**UK to consult on making tech companies liable for breaches caused by insecure products.** The government's budget revealed the plan, which NCSC chief Richard Horne backed: "For decades, we have collectively got away with doing tech on the cheap." [The Record](https://therecord.media/uk-ncsc-predicts-rise-cyberattacks-coming-months)

**Egypt convicts Mada Masr's editor under its website-licensing law and brings a second trial.** EFF says Lina Attalah was convicted Oct. 27 of running an unlicensed news website, after Mada Masr's license applications went unanswered, and fined the maximum 3 million Egyptian pounds (~$55,000). She faces a "false news" trial Nov. 11. EFF calls Egypt's licensing regime "an obvious mechanism for restricting who gets to publish," and says the six-person newsroom of the fact-checking group Matsada2sh is in pretrial detention on terrorism charges. [EFF Deeplinks](https://www.eff.org/deeplinks/2026/11/independent-digital-media-not-privilege-governments-can-revoke-fight-save-egypts)

**Push to keep Nick Andersen at CISA past his acting-director time limit.** *Also covered above under Executive Leadership Changes.* [CyberScoop](https://cyberscoop.com/nick-andersen-cisa-acting-director-nomination/)

## Privacy

**One person's 2,000 misdirected campaign texts expose the political data-broker pipeline.** A Wired reporter got nearly 2,000 fundraising texts meant for a relative over several years, more than 190 in the first 20 days of October alone, despite replying "STOP" 49 times. Tracing why led through campaigns, list vendors, and data brokers that tie phone numbers to the wrong people. [Wired](https://www.wired.com/story/my-journey-to-the-center-of-americas-political-spam-text-hell/)

**About 400 ordinary-looking AI apps hide sexually abusive deepfake features.** Wired found a network of more than 400 apps and domains, linked to Chinese developers and a Hong Kong entity, KeLing Technology Limited, posing as pet-portrait, language, or fitness tools. Under certain conditions they load an interface for generating explicit images of people from uploaded photos. They were promoted through Meta ads (some containing AI-generated child sexual abuse material), distributed through Apple's and Google's stores, and paid for through Apple Pay and Google Pay. [Wired](https://www.wired.com/story/hundreds-of-mundane-ai-apps-are-hiding-abusive-deepfake-features/)

**Activist group plans to publish the home addresses of Musk and other billionaires.** The "Capytistas," who say they have more than $1.2 million in backing, plan to release 150+ mostly unreported home addresses and 3,500+ records on people with combined wealth of about $1.4 trillion, starting with Elon Musk, his brother, and Tesla's board. Two members told Wired they built the dossiers with nearly every method available to a private investigator, "and some that are not." [Wired](https://www.wired.com/story/anti-oligarchy-activists-plan-to-dox-elon-musk-and-hundreds-of-billionaire-linked-homes/)

## AGI Arrival Timeline

**Current range:** P5 2032 · P50 2050 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 18 years.(unchanged since 2026-10-20)

**Best AI model passes just 36% of real-time tasks.** Realtime-Bench, built by UT Austin, Ohio State, UIUC, NVIDIA, Northwestern, and Steadyworks, tests 50 web and game tasks where acting late means failing. The top model, GPT-6 Astra (high), passed 36% under real wall-clock time. With the clock paused, high-reasoning models reach 70-80%. Jack Clark calls it "an effective proxy for where AI agents will break." [Import AI 479](https://importai.substack.com/p/import-ai-479-spacewar-low-latency)

**Andrew Ng: real AGI is "many decades away."** In a 2026 FastCompany interview quoted in Alex Turner's talk transcript, Ng says AGI under the original "any intellectual task a human can do" definition is far off, and that businesses will likely declare success first under lower-bar definitions. [AI Alignment Forum (Turner, quoting Ng)](https://www.alignmentforum.org/posts/RHxaRkarGp9snWoKY/explaining-ai-might-obliterate-you-to-senior-policymakers-in)

**Sherlock's view:** hold, with a slight Later lean. Realtime-Bench is credentialed, current, and quantified, but it measures one narrow ability. Ng is restating a known position. **Seldon's reconciliation:** a disagreeing source is weighed, not discounted. Ng's "many decades" fits inside this file's P95 2075, so it supports keeping the long tail. Realtime-Bench is the kind of breadth evidence this file wants, but the paused-clock scores show the gap is mostly about latency, not reasoning. The open 10-29 review trigger only fires on evidence of AI matching humans across many tasks, and this isn't that. **Range holds at P5 2032 · P50 2050 · P95 2075.**

## Intrusion Kill Chain Prevention Tactics

**Inside the $6.3B Binance drain, step by step.** *(Queued by Rick via the Pending Evidence Queue.)* Hypernative's reconstruction shows the attack was prepared in plain sight:

- **~36 hours before:** the operator wallet was funded through Tornado Cash in small amounts (Hypernative flagged it at 07:39 UTC Oct. 29).
- **~18 hours before:** a test sweeper contract was deployed and tried out on disposable wallets.
- **~4 hours before (15:59 UTC):** the live sweeper was deployed. Only the attacker's address could call it, and Hypernative flagged it as malicious at deployment.
- **20:05-20:22 UTC:** hot wallets on XRP, Solana, Base, Optimism, Bitcoin, and Tron signed ordinary transfers straight to the attacker.
- **20:20:59 UTC:** a single EIP-7702 transaction carrying 50 authorizations delegated "Binance 14," a main Ethereum hot wallet, to the sweeper.
- **20:24 UTC:** one call moved 167,464 ETH and 63 tokens (~$1.61B USDT the largest).
- **20:41-20:59 UTC:** $823M USDC was pulled from a Circle smart account whose only owner was Binance 14.
- **21:04-23:56 UTC:** the still-delegated wallet was swept four more times as customer deposits kept arriving.
- **00:10 UTC Oct. 30:** Binance revoked the delegation.

Every outflow used Binance's own valid signatures, and no contract was exploited. Binance traces it to a compromised DevOps engineer's laptop that reached a withdrawal-submission service. Hypernative notes that a 7702 delegation inherits every permission the address holds, and that rotating the key wouldn't have removed it. For defenders, the preparation stages (mixer funding, sweeper deployment) and the delegation itself were all observable before any money moved, and a policy denying delegations to flagged contracts would have stopped the $2.57B sweep. Note that Hypernative sells exactly that control. **Newsletter Tracker:** this *Supports* Thread 4 ("Intrusion Kill Chain Prevention, long impractical, is now operationally feasible at scale"; status: Holding, current statement ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead)). It's the thread's argument applied on-chain: the theft followed a predictable sequence of stages, each one interruptible at the procedure level. It doesn't show that defenders can act at that tempo, since Binance didn't. [Hypernative](https://www.hypernative.io/insights/blog/inside-the-largest-crypto-theft-of-all-time-the-6-3b-binance-hot-wallet-drain)

**NATO's Crossed Swords pairs red-team operators with AI agents.** *Also covered above under Automation Tactics.* [SecurityWeek](https://www.securityweek.com/natos-crossed-swords-exercise-brings-ai-agents-into-cyber-operations-training/)

## Risk Forecasting Tactics

**Polymarket's breach bill: $3.9 million, nearly a third of it from the shutdown.** Direct theft losses were $2.7 million across 726 wallets, and another $1.2 million covers losses from the hours-long trading halt. That's a clean case study of response-driven business-impact costs adding ~44% on top of the theft itself. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/polymarket-returning-funds-to-customers-after-site-compromise)

**NCSC forecasts an "unprecedented rise" in UK cyber incidents in the coming months.** The NCSC calls AI-powered ransomware against UK infrastructure "highly likely" by 2028. *Also covered above under Critical Infrastructure Attacks.* [The Record](https://therecord.media/uk-ncsc-predicts-rise-cyberattacks-coming-months)

## Resilience Tactics

**Some supermarket fridge controllers can't be patched, only physically modified.** The refrigeration contractor for Delhaize says affected units "needed physical modifications and not just a software update." Danfoss and Copeland say most affected devices were end-of-life products no longer getting updates, and EU law won't require manufacturers to support such products until December 2027. *Also covered above under Adversary Playbook.* [The Record](https://therecord.media/cyberattack-grocery-freezers-europe)

**C3RB3R victims may be able to recover Synology files without paying.** *Also covered above under Adversary Playbook.* [The Hacker News](https://thehackernews.com/2026/11/synology-nas-devices-targeted-in.html)

## Political

**Federal judge throws out DOJ's suit to block a possible Peltola win in Alaska.** DOJ argued that voters would be confused by an independent candidate who shares a name with incumbent Sen. Dan Sullivan. Judge Sharon Gleason found the government had no standing and couldn't explain how relief could be granted "while simultaneously maintaining the secrecy of the ballot," noting that 60,000 ballots had already been cast. She also questioned whether the executive branch has any legitimate role in the matter. Election Oversight. [CyberScoop](https://cyberscoop.com/judge-dismisses-alaska-senate-lawsuit-peltola-sullivan/)

**Fairfax County early voting tops 227,000 ballots ahead of the midterms.** Early voting closed Oct. 31 with more than 227,000 county ballots cast, part of a statewide and national surge, per Virginia Department of Elections data. Election Oversight. [FFX Now](https://www.ffxnow.com/2026/11/02/fairfax-county-sees-massive-increase-in-early-voting-ahead-of-midterm-election/)

## Superintelligence Timeline

**Current range:** P5 2033 · P50 2051 · P95 2076: a 43-year uncertainty window and a 50% chance we could reach this milestone in 18 years.(unchanged since 2026-10-20) This remains the most derivative of the five standing forecasts, built as the AGI file's range plus a stated gap.

**An anonymous frontier-lab researcher says an intelligence explosion has "a big chance" within single-digit months.** Alex Turner relayed this in his NDTV talk, alongside OpenAI's stated goal of "an AI that does AI research by 2028," which he says has completed its first step. [AI Alignment Forum](https://www.alignmentforum.org/posts/RHxaRkarGp9snWoKY/explaining-ai-might-obliterate-you-to-senior-policymakers-in)

**Sherlock's view:** a Sooner lean, since this speaks directly to recursive-self-improvement speed. **Seldon's reconciliation:** the claim is secondhand and anonymous, and Turner doesn't say whether the clock starts now or at AGI. The 2028 target is a lab's stated plan, not new evidence. It's logged as a Sooner-leaning data point that doesn't clear the bar for a substantive shift alone. Floor check performed, no adjustment needed. **Range holds at P5 2033 · P50 2051 · P95 2076.**

## Harm Timeline

**Current range:** P5 2037 · P50 2065 · P95 2091: a 54-year uncertainty window and a 50% chance we could reach this milestone in 28 years.(changed 2026-11-03: P5 moved from 2038 to 2037) This range assumes harm eventually happens and asks only when. The odds that it happens at all are tracked under Harm Probability.

**Former Google DeepMind safety researcher gives a one-in-three chance of mass death from AI within ten years.** Alex Turner, who worked on keeping AI systems safe at Google DeepMind until June, told Indian policymakers: "My best guess is about a one in three chance that in the next ten years, AI kills at least 95% of the global population without being told to." He calls himself "considered an optimist, as far as experts in this field go." [AI Alignment Forum](https://www.alignmentforum.org/posts/RHxaRkarGp9snWoKY/explaining-ai-might-obliterate-you-to-senior-policymakers-in)

**Sherlock's view:** a Sooner lean on the early tail only. **Seldon's reconciliation:** this file assumes harm eventually happens and asks when. Turner's figure is unconditional, and conditioning on eventual harm can only raise the share he puts inside the next ten years. That means he'd put well over 5% of the conditional distribution before 2036, while this file's P5 was 2038. Under the standing rule, a credible disagreeing source pulls the range a little wider in its direction. It's one source, and he doesn't separate timing from likelihood, so only P5 moves. **Range revised: P5 2038 → 2037 · P50 2065 · P95 2091.** It stays above the Superintelligence floor (P5 2033). A second independent credentialed estimate putting real weight on harm within about ten years would justify reconsidering P50. Seldon's own call, open to Rick's override.

## Harm Probability

**Current range:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(changed 2026-11-03: High moved from 50% to 55%)

**Former Google DeepMind safety researcher gives a one-in-three chance of mass death from AI within ten years.** *Also covered above under Harm Timeline.* [AI Alignment Forum](https://www.alignmentforum.org/posts/RHxaRkarGp9snWoKY/explaining-ai-might-obliterate-you-to-senior-policymakers-in)

**Sherlock's view:** a direct, credentialed probability, which should move the upper tail. **Seldon's reconciliation:** this file asks how likely a catastrophe killing over 10% of humanity is *given* loss of control. Turner's one-in-three is unconditional and for a much worse outcome (≥95% killed). A probability conditional on losing control can't be lower than the unconditional one, so his implied figure for this file's own question is at least 33% and probably well above it. That's at or above the 30% central estimate and plausibly above the 50% upper bound. Under the standing rule a disagreeing source widens the range in its direction, the same way the XPT's low 3% median kept the lower bound from rising. One source can't pin down his conditional figure, so Central holds at 30% and only the upper bound moves. **Range revised: Low 15% · Central ~30% · High 50% → 55%.** A second independent credentialed estimate above ~40% conditional would justify revisiting Central. Seldon's own call, open to Rick's override.

## Government Surveillance

**Civil-society groups urge the EU to close loopholes in its surveillance-tech export rules.** The Center for Democracy and Technology and eight other organizations asked the European Commission to strengthen export controls on spyware and surveillance technology, so it can't be used for internal repression and human-rights abuses, and to make sure the controls are actually enforced. [CDT](https://cdt.org/insights/civil-society-urges-the-commission-to-close-loopholes-in-surveillance-export-rules/)

## Cybersecurity Canon Project Book Reviews (November 2026)

**[*The Developer's Playbook for Large Language Model Security: Building Secure AI Applications*](https://cybercanon.org/the-developers-playbook-for-large-language-model-security-building-secure-ai-applications/), by Steve Wilson (Hall of Fame nominee, review dated Nov. 2).** Reviewer Thomas Laugle recommends it for the Hall of Fame. He says it explains how LLMs work with respect to security and covers the defenses and policy any prudent strategy would surround them with. Although it's written for developers, he argues "there are few, if any, remaining subfields within cybersecurity for which LLM security is not timely and relevant," especially with the wave of AI-built "vibe-coded" software since its publication. Categories: AI/ML and GenAI Security, Software & Application Security, Supply Chain Risk, Vulnerability Management, Zero Trust.

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 58 | 12 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 49 | 22 | 2026-07-14 |
| The Hacker News | Contributed | 70 | 1 | 2026-07-14 |
| The Record | Contributed | 55 | 16 | 2026-07-14 |
| The Canon Project | Contributed | 17 | 53 | 2026-07-14 |
| FFX Now | Contributed | 13 | 58 | 2026-07-14 |
| Wired | Contributed | 45 | 23 | 2026-07-20 |
| CyberScoop | Contributed | 30 | 12 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 39 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 19 | 23 | 2026-09-01 |
| SecurityWeek | Contributed | 38 | 4 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 2 | 18 | 2026-10-02 |
| CISO Tribune — The Wire | Contributed | 4 | 8 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 11 | 2026-10-17 |
| EFF Deeplinks | Contributed | 7 | 5 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 3 | 9 | 2026-10-17 |
| IAPP News | No Contribution | 6 | 6 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 1 | 11 | 2026-10-17 |
| AI Alignment Forum | Contributed | 3 | 9 | 2026-10-17 |

**No-contribution detail:**

- **CSO Online CISO Appointments**: still no October 2026 section on the page.
- **CISA Cybersecurity Advisories**: nothing newer than the Oct. 30 KEV alert (the Ivanti pair), already credited 10-31.
- **LEAP**: the highest wave is still Wave 12 ("Safety Policies").
- **NIST Cybersecurity Insights Blog**: no new post since Oct. 27.
- **(ISC)² Insights**: nothing newer than Oct. 30. The two Oct. 30 posts not used last run ("Beyond Hackers and Scams," "Your Customers Need Security Awareness Too") are general awareness pieces with no CIR fit.
- **IAPP News**: nothing newer than Oct. 30, and that day's items were in the 10-31 run's window.
- **CSIS Strategic Technologies Program**: the newest cybersecurity item is still Oct. 23. Only event listings are newer.

**Also checked, not itemized:** The Hacker News' weekly recap (Nov. 2) mostly repeats already-covered items. VergeX ($3.6M AI-trading-platform theft), the zkLink and Flap DNS-hijack crypto thefts, Applebee's exposed app password, Flashpoint's DefenderKiller EDR killer, LevelBlue's vibe-coded phishing kits, and ESET's Amatera infostealer deep-dive (all via Risky Bulletin) weren't written up as standalone items. Neither were Anthropic's acquisition of Opaque Systems (SecurityWeek's October M&A roundup), the Prophet Security SOC survey (vendor-contributed), the DIA's space-security report and Google's Genie 4 (Import AI 479), and a ChatGPT medical-advice lawsuit (Cyberwire #209). Gmail's local-news digests (FFXnow, ARLnow, ALXnow, InsideNoVa) and personal newsletters had no CIR fit. Cyberwire Issue 210 (11.3) wasn't posted at run time.

**Fetch note:** The Hacker News's article pages now return a Cloudflare challenge to curl, WebFetch (HTTP 403), and headless Chrome. Article text was read through Chrome MCP instead. Its RSS feed still works.

**Newsletter Tracker:** no new First Principles essay since the last check. The newest post is still "'Salem's Lot" (Oct. 27), a book review. Today's entries: Thread 4 *Supports* (Hypernative's Binance kill chain, the NCSC's "old weaknesses, new scale" framing) and Thread 5 *Supports* (Alex Turner's firsthand account of lab commitments bending under pressure). Both threads' statuses are unchanged (Thread 4 Holding, Thread 5 Under Pressure).

**Pending Evidence Queue:** one row processed and flipped to Included: Hypernative's Binance hot-wallet drain breakdown (Intrusion Kill Chain Prevention Tactics, submitted 11-01). The content matches the stated category.

**Pending artifact approvals:** none open on `raceBannon99/nexus-artifacts`.

**AI Timeline Forecasting chart:** the P(Doom) and Harm Probability ranges moved today, so the infographic in Alexandria's Library now shows stale figures. It can be refreshed with the `nexus-ai-timeline-chart-refresh` skill.
