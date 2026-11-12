# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Thursday, Nov. 12. Covers everything published after the 11-11 run; an early-morning pull, so several daily sources had nothing for today yet. The headlines: an attacker used 4,837 hijacked GitHub accounts to plant a CI secret stealer that ran in at least 1,806 repositories; rogue ScreenConnect clients spread worm-like through managed-service technicians to 48 organizations; and Epoch AI showed an open-weight model building working Firefox exploits from unreleased patches for about $1,000 each. This is the first run with the five AI-timeline skeptic sources added 11-11. None of the five forecast ranges moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **AGI Arrival Timeline** — Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Superintelligence Timeline** — Evidence on when a machine might exceed, not just match, human intelligence — a higher, later capability bar than AGI, inferred structurally with no external forecaster basket.
- **Harm Probability** — Evidence on how likely — not how soon — a system that's escaped human control is to cause a catastrophe killing over 10% of humanity within 10 years; a bounded probability question, tracked separately from Harm Timeline's open-ended date question.
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Cybersecurity Workforce Development Tactics** — Unconventional hiring/development approaches — e.g. "Moneyball for Cybersecurity."
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Epoch's capabilities index puts Claude Fable 5.2 at a record, above trend, but that's the acceleration METR already measured, so counting it again would double-count.

2. **Forecasted Singularity Milestone Timeline:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06) An open-weight model building browser exploits on its own and another ARTEX-based agent platform in live attacks are diffusion evidence of the kind already priced in.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Epoch's data show compute additions growing more slowly than in 2023, a weak argument against shortening that gap.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. WIRED's ten-expert panel leans skeptical of extinction, but it doesn't address this conditional question.

*Seldon's floor checks: neither the AGI nor the Superintelligence range moved, so no floor or gap-model follow applied. No range moved today, so the AI Timeline Forecasting chart in Alexandria's Library needs no refresh beyond what 11-11 already flagged (see the footer).*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 7 new Active rows and 1 row updated. Active campaigns: 390, up from 383. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-12-adversary-tracking-report.md).*

**An attacker used 4,837 hijacked GitHub accounts to plant a CI secret stealer that ran in at least 1,806 repositories.** Starting Tuesday, the attacker opened test pull requests titled "docs: dependency audit notes" from `wfx-docs` branches in 61,764 repositories to see which accounts could write, then pushed a stealer into existing workflows or, in 771 repositories, an npm postinstall hook that also runs on developers' machines. The stealer takes Actions secrets, the workflow's `GITHUB_TOKEN`, OIDC and runtime tokens, cloud roles, and AI-provider keys, sends them out over HTTP or Telegram, and the attacker usually reverts the change and deletes the run logs within minutes. SafeDep counted 8,093 repositories with malicious commits, counting only public repositories' default branches. Aikido says any account that opened one of the test pull requests is compromised, and neither firm knows how the credentials were stolen. New pull requests with the same title were still appearing early today. Rotate every secret a hit repository can read, and treat any machine that ran `npm install` on an affected commit as compromised. New Cybercrime row (Tier 3); kept separate from the Gheist row because the tradecraft differs. [The Hacker News](https://thehackernews.com/2026/11/4837-hijacked-github-accounts-ran-ci.html)

**SCKit: rogue ScreenConnect clients spread from compromised panels to at least 288 endpoints at 48 organizations.** Huntress first saw the activity at 17:47 UTC on Nov. 11. Attackers use a cloud-hosted ScreenConnect panel's Run Command feature to install their own ScreenConnect client on every endpoint it manages. When a technician later connects to an infected machine, the malware can spread back to the technician's workstation, steal browser sessions and tokens, and move on to every other panel that technician can reach. ConnectWise disabled five third-party extensions (Labtech Plus, RMM Plus, RMM+, and two Password Link extensions) in about 400 partner environments and says it has found no flaw in ScreenConnect itself; Huntress points to stolen credentials or hijacked sessions, while SecurityWeek reports a flaw in a legitimate extension was used to bypass authentication. New Unclear row (Tier 3), separate from September's social-engineering ScreenConnect worm. [The Hacker News](https://thehackernews.com/2026/11/screenconnect-attacks-target-at-least.html); [SecurityWeek](https://www.securityweek.com/hackers-deploy-malware-in-fresh-screenconnect-campaign/)

**🤖 AntiFox: an open-source AI pentesting platform built on ARTEX went from web shells to AWS production secrets.** Arctic Wolf Labs tied several intrusions to Alibaba Cloud systems hosting AntiFox, a planner/worker multi-agent platform on GitHub (251 forks) whose README promises to run "the full engagement." In one chain, a compromised IIS application led to an ASPX web shell, which read `web.config` files and database connection strings. In others, valid AWS credentials were used to enumerate more than 20 services, including Bedrock, and in at least one case to pull a production secret from Secrets Manager. "Agentic frameworks such as these make penetration testing techniques more accessible to threat actors," Arctic Wolf says. New Unclear row (Tier 3), cross-tagged 🤖. [The Hacker News](https://thehackernews.com/2026/11/antifox-ai-pentesting-platform-linked.html)

**Attackers are probing N-central with a researcher's public zero-day exploits.** Sean Bales published more than 30 N-central flaws he calls Able2Shell, with proof-of-concept code and no coordinated disclosure. N-able took its hosted platform offline, has now patched every flaw that works without logging in (including CVE-2026-125883 and CVE-2026-125881, CVSS 9.3) in N-central 2026.4 HF2, and says the authenticated ones will follow. It reports scanning that opens anonymous agent sessions, pulls appliance configurations, and hits the remote-control endpoint without authentication, but no compromise of its hosted servers. Update on-premises N-central now. New Unclear row (Tier 3). [SecurityWeek](https://www.securityweek.com/hackers-target-n-central-zero-days-as-n-able-rushes-patches/)

**Qlik Sense servers hit with reverse-shell attempts resembling 2023's CACTUS intrusions.** Cynet blocked a one-line PowerShell reverse shell, run through Qlik's `scheduler.exe`, against several EU customers in a three-minute window in October; testing showed it would have installed a Go reverse shell for persistence. The exploited flaw is unknown, but the pattern matches 2023 CACTUS ransomware attacks on the DoubleQlik flaws. New Cybercrime row (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-target-qlik-sense-servers-with.html)

**Maersk confirms data theft as WhiteArmor demands $5 million.** The shipping company says hackers took data from a system it inherited through an acquisition, that the incident is isolated, and that its findings "strongly suggest no sensitive data has been disclosed." WhiteArmor, which listed Maersk on its leak site Nov. 7, claims 100GB from an LF Logistics platform (acquired 2022), including about 29,000 driver records (16,093 with plaintext passwords) and 16,123 staff accounts. Maersk hasn't confirmed the group's involvement. New Cybercrime row (Tier 2). [SecurityWeek](https://www.securityweek.com/maersk-confirms-data-theft-amid-5-million-extortion-attempt/)

**Poland takes its national e-government platform offline after a cyberattack.** ePUAP, which citizens and businesses use to file official documents and correspond with agencies, was attacked; Digital Affairs Minister Krzysztof Gawkowski says the attack was "detected and stopped," and a ministry spokesperson says the shutdown was a precaution, not damage. Officials haven't said how it happened or who did it, and the Trusted Profile digital-identity system may also be affected. New Unclear row (Tier 3). [The Record](https://therecord.media/poland-shuts-down-government-services-platform-cyberattack)

**US prosecutors say an IRGC-backed network directed European attacks live over FaceTime.** A superseding indictment unsealed Nov. 10 charges an alleged Kataib Hezbollah commander jailed in New York, an IRGC operative, and an Iraqi formerly living in Britain with orchestrating about 18 attacks and attempted attacks claimed by the front group HAYI, including synagogue arsons in London and a plot against RAF Fairford. Much of the evidence came from recordings on the commander's seized iPhone, since FaceTime calls themselves are end-to-end encrypted. This is terrorism, not a cyber campaign, so it gets no tracker row; it's here as US-Israel-Iran war context. [The Record](https://therecord.media/iran-backed-network-directed-london-attacks-over-facetime)

**Srsly Risky Biz: the French fridge attacks "felt very Russian."** Tom Uren says that if forced to bet, Risky Business would have picked Russia, noting that Turla hijacked Iranian tools in 2019 and that attacking Europe doesn't fit Iran's US-focused campaign this year. Analysis, not new evidence: Ryan logged the dissent on the Shahid Kaveh row (Iran row 20), which stays at Tier 2 under France's attribution. [Risky.Biz](https://news.risky.biz/srsly-risky-biz-iranian-hacks-with-russian-characteristics/)

## Zero Trust Tactics

**Attackers are probing N-central with a researcher's public zero-day exploits.** N-central 2026.4 HF2 fixes every flaw exploitable without authentication; scanning against on-premises servers began Monday. [SecurityWeek](https://www.securityweek.com/hackers-target-n-central-zero-days-as-n-able-rushes-patches/) *Also covered above under Adversary Playbook.*

**A critical Apache HTTP/2 flaw could let unauthenticated attackers run code.** CVE-2026-119618 in `mod_http2` affects Apache HTTP Server 2.4.55 through 2.4.70 and is fixed in 2.4.71; only servers with HTTP/2 turned on (the `h2`/`h2c` Protocols directive, server-wide or per virtual host) are exposed. Red Hat rates it 9.8 and says "public research has demonstrated a reliable exploit," without naming it; Wiz says no exploit is available and no attacks have been seen. Red Hat Enterprise Linux 9 and 10 are fixed and rated Important rather than Critical because of how their builds allocate memory. [The Hacker News](https://thehackernews.com/2026/11/critical-apache-http2-flaw-could-let.html)

**Node.js fixes 16 flaws, including HTTP/2 bugs that crash servers or leak other users' data.** CVE-2026-123863 lets an unauthenticated client crash a default HTTP/2 server on the 24.x and 26.x lines, and CVE-2026-123866 can send a client pieces of memory, including responses meant for other connections. A separate HTTPS flaw, CVE-2026-123864, can leak "TLS private keys and other users' requests" under specific handler patterns. Update to 22.23.5, 24.22.3, or 26.13.1. [The Hacker News](https://thehackernews.com/2026/11/nodejs-fixes-16-flaws-including-http2.html)

**A critical MongoDB flaw lets an unauthenticated attacker plant a crash that fires on failover.** CVE-2026-118383 (CVSS 4.0 score 9.5) is a use-after-free: two requests to a lagging replica-set member crash it if it's later elected primary, and turning on authentication doesn't stop them. MongoDB found it itself and knows of no attacks; Atlas clusters patch during maintenance, but self-managed deployments need the fix on every member. The end-of-life 8.2 branch won't be patched, and a public proof of concept says 8.2.12 still crashes in a lab test. [The Hacker News](https://thehackernews.com/2026/11/critical-pre-auth-mongodb-flaw-cve-2026.html)

**A critical Red Hat Quay flaw lets an attacker take over registry token signing.** CVE-2026-123710 (CVSS 9.8) lets an anonymous user, or any valid account, install their own signing key and mint tokens with read and write access to every repository, which means stealing private images and overwriting ones that other systems pull. The rogue key survives restarts, and changing passwords or robot tokens doesn't remove it. Red Hat says to restrict access to the key-management service and audit for unauthorized keys until the fix ships. [SecurityWeek](https://www.securityweek.com/critical-red-hat-quay-vulnerability-could-expose-private-container-images/)

**Zoom patches a critical privilege-escalation flaw in Zoom Workplace for Windows.** CVE-2026-108186 (CVSS 9.6) lets an unauthenticated user escalate privileges over the network in versions 7.1.0 through 7.1.7; a second flaw, CVE-2026-108187 (8.1), affects versions before 7.1.5. No exploitation reported. [The Hacker News](https://thehackernews.com/2026/11/critical-zoom-workplace-flaw-could.html)

**eMudhra revokes eight more certificate authorities it had called unaffected.** The certificate authority's full incident report says the in-house Python script that cut eight ECDSA keys down to a single byte in October also pulled the RSA keys of eight other intermediate CAs out of its hardware security modules at an April 2025 key ceremony, and it can't show those keys were handled by its own rules. It had told Mozilla on Oct. 19 that the RSA issuers were "not impacted." Six of the newly revoked CAs issued website certificates and two code-signing certificates; 195 certificates are listed. The weak keys passed linting and two WebTrust audits unnoticed. [The Hacker News](https://thehackernews.com/2026/11/emudhra-revokes-8-more-cas-it.html)

**October's CVE flood, fact-checked: publication quadrupled, known exploitation didn't.** Laurent Hausermann counts 17,052 CVEs published in October 2026 alone, about four times 2025's weekly rate, and projects about 128,000 for the year; NIST now enriches only CVEs in CISA's KEV catalog. Yet KEV additions are up only about 16% (285 so far this year). His leading explanation is that AI-driven attackers increasingly use unreported "sibling" bugs rather than the published CVE, so CVE-based accounting will understate real exploitation. He cites a16z's survey of 100 CISOs: 87% expect bigger budgets in 2027, but only 36% are comfortable letting AI agents act alone even on low-risk tasks. [Cyber Builders](https://cyberbuilders.substack.com/p/october-was-cybersecurity-awareness). **Newsletter Tracker:** this *Supports* Thread 3 ("Resilience, not prevention, is the affordable strategy for most organizations"; status: Holding, current statement ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience)). If the patch queue grows faster than any team can work it, and attacks stop mapping to the CVEs being patched, prevention-by-patching gets less affordable. It corroborates Chris Hughes's 11-10 argument with independent numbers.

## Workforce Development Tactics

**(ISC)² on staffing critical infrastructure security as IT and OT converge.** A webinar recap argues that "technology is advancing faster than the governance, funding and workforce models built around it," and that protecting power, water, and health systems requires professionals with the operational context to keep services running during an incident, not just tool skills. [(ISC)² Insights](https://www.isc2.org/Insights/2026/11/preparing-cybersecurity-workforce-to-protect-critical-national-infrastructure)

**(ISC)² creates an Academic Advisory Council to align degree programs with industry.** Chair Brian Callahan of Monmouth University wants to "produce future generations that meet industry needs faster with less on-the-job training," including training students directly on the tools industry uses; he had all his students earn the CC certification as part of class. [(ISC)² Insights](https://www.isc2.org/Insights/2026/11/preparing-tomorrows-cybersecurity-leaders)

**NVIDIA's Mark Weatherford on the CISO role in the AI era.** At (ISC)² Security Congress, Weatherford said "every month is a new month" and laid out what CISOs need now: aligning with CEO goals, reshaping the security agenda around AI's value, and upskilling for an "AI agentic workforce." [(ISC)² Insights](https://www.isc2.org/Insights/2026/11/evolving-the-ciso-role-in-the-age-of-ai)

## AI Singularity Timeline

**Current range:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06)

**An open-weight model built working Firefox exploits from unreleased patches for about $1,000 each.** In Epoch AI's offline sandbox, GLM 5.3 reverse-engineered security fixes that hadn't yet reached users and compromised six recent Firefox versions with no human input, building webpages that read files from a visitor's computer and send them to the attacker. It couldn't do the same against Chrome, though Epoch says better prompting or a stronger model might. Epoch calls the "patch gap" a known weakness that used to require significant expertise or frontier-model access, and expects such attacks to grow as open-weight models improve. [Epoch AI](https://epochai.substack.com/p/the-epoch-brief-november-11-2026)

**🤖 AntiFox: an open-source AI pentesting platform built on ARTEX went from web shells to AWS production secrets.** Arctic Wolf ties live intrusions to the multi-agent platform, which pulled a production secret from AWS Secrets Manager in at least one case. [The Hacker News](https://thehackernews.com/2026/11/antifox-ai-pentesting-platform-linked.html) *Also covered above under Adversary Playbook.*

**Sherlock's view:** slight Sooner on diffusion. Capability that needed frontier-model access months ago now runs on an open-weight model for $1,000. **Ryan's view:** AntiFox is the third ARTEX-derived framework in live attacks this month, after Storm-3358 and Vapor Panda, and Operation Snowball (11-11) ran on a jailbroken open model. It's a trend, not a single data point.

**Seldon's reconciliation:** both items are the same diffusion evidence that moved P50 on 11-06 and that Snowball added to on 11-11, and neither shows an agent escaping its operator's control. Diffusion raises the number of actors who could lose control, which this file already prices. **No change.** Cross-ref: [Adversary Tracking Report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-12-adversary-tracking-report.md) (new Unclear row 124, AntiFox).

## AGI Arrival Timeline

**Current range:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11)

**Epoch: Claude Fable 5.2 sets a record on its Capabilities Index, above the trend.** Fable 5.2 scored 174 on the Epoch Capabilities Index, which combines many benchmarks into one general-capability score, ahead of GPT-6 Astra's 169 and above what the post-2024 reasoning-model trend predicted. Epoch notes the debate over AI speeding up AI research, but says the score is "just one data point." It also switched ECI to a Bayesian method that gives probabilities: Astra has a 72% chance of being more capable than Claude Opus 5.5. [Epoch AI](https://epochai.substack.com/p/the-epoch-brief-november-11-2026)

**SRE-Bench: frontier models reverse-engineered only about a third of unseen programs.** Researchers at Columbia and elsewhere built 19 new programs averaging 17,000 lines each, so models couldn't have seen the answers in training. GPT-6 Sol and Claude Fable 5.1 reversed about a third of them; GPT-6 Astra did much better with unlimited tokens and time. [SRE-Bench](https://sre-bench.lol/) (via WIRED's AI Lab newsletter)

**Sherlock's view:** slight Sooner on the ECI record, since an independent, multi-benchmark index running above trend is the kind of breadth measurement this file prefers. SRE-Bench cuts slightly the other way: a third is far from expert parity at a demanding task. **Ryan's view:** none on arrival timing.

**Seldon's reconciliation:** a model scoring above trend is what the acceleration METR measured predicts, and that acceleration already moved this file on 11-06 and 11-11, so counting it again would double-count. SRE-Bench is too narrow to move a breadth forecast. **No change.**

## Data Breaches

**Maersk confirms data theft as WhiteArmor demands $5 million.** The group claims 100GB from an LF Logistics platform, including about 29,000 driver records, 16,093 with plaintext passwords; Maersk says the incident is isolated to a local system it inherited through an acquisition. [SecurityWeek](https://www.securityweek.com/maersk-confirms-data-theft-amid-5-million-extortion-attempt/) *Also covered above under Adversary Playbook.*

**More than 35,000 Grok-built apps are open to anyone, including some built by X and SpaceXSI staff.** Claroc found 37,571 apps built with Grok's chat app builder and 35,578 that open without a sign-in. About one in ten held internal business or personal data, and about 2% held material rated high or critical: a hospital group's list of 3,500+ employees, an ICU briefing on a single patient, a fire department's live shift board, and a timesheet whose code held every employee's password in plain text. The 24 staff apps included a confidential X advertising proposal to a US federal agency. "Anyone with the link" was the preselected sharing setting in the researchers' paid account, and app addresses show up in searchable passive-DNS records. SpaceXSI took down the 24 staff apps and says apps stay private until creators choose to share them. [The Hacker News](https://thehackernews.com/2026/11/over-35000-grok-built-apps-exposed.html)

## Privacy

**The European Commission proposes the Digital Fairness Act, banning dark patterns and extending limits on targeted ads.** The proposal, which Commissioner Michael McGrath calls "the most significant reform of EU consumer protection rules in more than 20 years," bans manipulative design, lets consumers turn off endless scrolling and autoplay, makes subscriptions easier to cancel, and requires human customer service rather than chatbots alone. It extends the Digital Services Act's bans on targeting minors with personalized ads and on ad targeting based on sensitive data from the largest platforms to all websites and apps. The Commission could fine up to 6% of global profits in large cross-border cases. Industry groups pushed back on the ad limits. [IAPP](https://iapp.org/news/a/european-commission-releases-draft-proposal-for-digital-fairness-act)

**EU data-protection authorities will review automated decision-making in hiring.** The EDPB's sixth coordinated enforcement action asks member authorities to check compliance with GDPR's right not to be subject to decisions based solely on automated processing (Article 22), and the right of access, in AI-driven candidate screening. The board hasn't addressed automated decision-making specifically since 2018. [IAPP](https://iapp.org/news/a/edpb-puts-admt-based-recruitment-in-focus-under-coordinated-enforcement-framework)

## Nation-State Cyber Policy & Law

**Fourteen governments adopt the first guidelines for commercial hacking firms.** At the Pall Mall Process's third conference, attended by 43 countries, fewer than half endorsed the guidelines, among them the UK, France, US, Germany, Italy, and Japan. Firms that build, sell, or finance commercial intrusion tools are asked to vet customers, build safeguards against misuse, monitor and report abuse, halt sales when serious misuse is a credible risk, and "consider" remedies for victims. The code is voluntary, with no penalties; pressure is expected to come from governments that buy the tools and license their export. "A voluntary code is not, however, an optional code," France's foreign ministry said. [The Record](https://therecord.media/britain-france-set-out-guidelines-for-commercial-hacking-firms)

**CISA's acting director sets the agency's 2027 priorities in an internal memo.** Nick Andersen's Nov. 2 memo, obtained by Cybersecurity Dive, lists three top-line priorities: leading national cyber defense, securing key infrastructure, and overseeing national resilience. It sets six operational focus areas, six critical information requirements, and seven priority intelligence requirements, including adversaries' targeting of operational technology and critical supply chains. A consistent theme is triaging CISA's support toward the most systemically important organizations. The memo arrives as CISA enters a third year without a Senate-confirmed director. [Cybersecurity Dive](https://www.cybersecuritydive.com/news/cisa-priorities-memo-risks-partnerships/874381/)

## Compliance Trends

**The European Commission proposes the Digital Fairness Act.** The Commission could fine up to 6% of a company's global profits in large cross-border cases, under a revised Consumer Protection Cooperation Regulation that gives it more power to investigate. [IAPP](https://iapp.org/news/a/european-commission-releases-draft-proposal-for-digital-fairness-act) *Also covered above under Privacy.*

**EU data-protection authorities will review automated decision-making in hiring.** The EDPB's coordinated enforcement action will check GDPR Article 22 compliance in AI-driven candidate screening. [IAPP](https://iapp.org/news/a/edpb-puts-admt-based-recruitment-in-focus-under-coordinated-enforcement-framework) *Also covered above under Privacy.*

## Superintelligence Timeline

**Current range:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) *This remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed.*

**Epoch: new AI computing capacity is doubling every nine months, but growth has slowed since 2023.** Quarterly additions have grown about 2.5x a year since 2024, down from about 6x in 2023. Broadcom doubled its TPU compute shipments in one quarter, to nearly 2 million H100-equivalents. Epoch says any further slowdown isn't statistically significant and may be a lull between chip generations. Separately, its new AI Chip Imports explorer finds 72% of the AI compute delivered worldwide since 2022 landed in the US and about 10% in China. [Epoch AI](https://epochai.substack.com/p/the-epoch-brief-november-11-2026)

**Sherlock's view:** slight Later on the gap, since the growth rate of compute additions has fallen by more than half since 2023. **Ryan's view:** none.

**Seldon's reconciliation:** floor check first. The AGI range didn't move, so there's no mechanical follow. A nine-month doubling is still very fast, and the slowdown is from an exceptional 2023 surge rather than a plateau. It argues modestly against shortening the gap below a year, which this file wasn't doing. **Gap holds at one year; no change.**

## Harm Probability

**Current range:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03)

**WIRED asked ten AI-safety experts for their real nightmares; few put weight on extinction.** Stanford's Rob Reich finds human extinction "pretty implausible," though catastrophe is "imaginable." Heidy Khlaaf of the AI Now Institute, a former OpenAI safety engineer, says safety engineering doesn't engage with extinction percentages "because there are no numbers to back it." Yoshua Bengio, on extinction: "I don't know about that. But, you know, we shouldn't take a chance." He lists rogue misaligned AI, misuse by terrorists and states, and concentration of power as the main risks. A RAND biosecurity researcher calls an AI-enabled biological attack one of the clearest catastrophic pathways. Most panelists doubt a development pause would last. [WIRED](https://www.wired.com/story/the-ai-safety-debate-has-lost-the-plot-we-asked-10-experts-what-the-real-nightmares-are/) *(published Nov. 10; surfaced through WIRED's AI Lab newsletter and not covered before)* **Newsletter Tracker:** this *Supports* Thread 5 ("AI's real danger is relentless, non-sentient task-pursuit and institutional-control erosion, not conscious malice"; status: Under Pressure, current statements ["The Doomsday Talk Isn't Over"](https://diffuser.substack.com/p/the-doomsday-talk-isnt-over) and ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house)). A credentialed panel puts the most plausible harms in misuse, power concentration, and dynamics where "nobody intended to do something bad," which is the thread's own framing. It doesn't settle why the thread is Under Pressure, and Bengio still lists rogue AI first.

**Sherlock's view:** slight Lower lean. A broad, credentialed panel is more skeptical of mass-casualty outcomes than this file's 30% central estimate implies. **Ryan's view:** none.

**Seldon's reconciliation:** under the disagreeing-source rule this is weighed, not discounted, but it doesn't answer this file's question. The panel speaks to unconditional extinction risk. This file asks about a catastrophe killing more than 10% of humanity within ten years *given* that control is already lost, a conditional most panelists didn't address. Khlaaf's objection echoes the Narayanan and Kapoor critique logged 11-11 and argues for humility about the whole range, not for a lower number. If a credentialed source gives a reasoned low estimate for this conditional question, the Low end should widen. **No change.**

## Government Surveillance

**Fourteen governments adopt the first guidelines for commercial hacking firms.** The Pall Mall Process's voluntary code asks spyware and intrusion-tool vendors to vet customers and halt sales when serious misuse is a credible risk; France's foreign ministry notes such tools "have also been implicated in surveillance campaigns targeting journalists, political officials, activists or businesses." [The Record](https://therecord.media/britain-france-set-out-guidelines-for-commercial-hacking-firms) *Also covered above under Nation-State Cyber Policy & Law.*

## Critical Infrastructure Attacks

**Poland takes its national e-government platform offline after a cyberattack.** ePUAP, used to file official documents and reach government agencies, was shut down as a precaution; officials haven't said how the attack worked or who was behind it. [The Record](https://therecord.media/poland-shuts-down-government-services-platform-cyberattack) *Also covered above under Adversary Playbook.*

## Resilience Tactics

**Japan's language barrier was a security control nobody owned, and AI wore it away.** Brandon Karpf argues that for decades, attacking Japanese companies meant phishing in fluent Japanese, which most crews couldn't do. Generative AI removed that friction: Proofpoint found in May 2025 that 81.4% of 240 million scam emails targeted Japanese speakers. By the end of September 2026, Japan had seen more public breach disclosures than in all of 2025, per Trend Micro, including a parcel carrier's 53 million records and a disaster-alert service used to send 1.4 million phishing emails. His advice: list every place your security depends on something being hard for attackers (a language, an obscure protocol, an internal app nobody knows about), give each an owner and a recheck date, and add fresh friction through deception, such as decoy logins and files wired to alarms, changed often. [A Discipline of Seeing](https://karpf.substack.com/p/the-emperor-has-no-clothes)

## Automation Tactics

**October's CVE flood, fact-checked.** In a16z's survey of 100 CISOs cited by Laurent Hausermann, 18% run AI SOC tools in production and only 36% are comfortable letting AI agents act alone on low-risk tasks, though 60% expect to be within a year. "Attackers already automate discovery and exploitation. Defenders know they need automation, but most are not ready to let machines act." [Cyber Builders](https://cyberbuilders.substack.com/p/october-was-cybersecurity-awareness) *Also covered above under Zero Trust Tactics.*

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 64 | 12 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 52 | 25 | 2026-07-14 |
| The Hacker News | Contributed | 76 | 1 | 2026-07-14 |
| The Record | Contributed | 60 | 17 | 2026-07-14 |
| The Canon Project | No Contribution | 18 | 58 | 2026-07-14 |
| FFX Now | No Contribution | 15 | 62 | 2026-07-14 |
| Wired | No Contribution | 48 | 26 | 2026-07-20 |
| CyberScoop | No Contribution | 34 | 14 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 45 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 23 | 25 | 2026-09-01 |
| SecurityWeek | Contributed | 43 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 2 | 24 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 9 | 9 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 17 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 11 | 7 | 2026-10-17 |
| (ISC)² Insights | Contributed | 6 | 12 | 2026-10-17 |
| IAPP News | Contributed | 12 | 6 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 1 | 17 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 10 | 2026-10-17 |
| Risky.Biz | Contributed | 3 | 0 | 2026-11-10 |
| tl;dr sec | No Contribution | 0 | 3 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 0 | 3 | 2026-11-10 |
| Resilient Cyber | No Contribution | 1 | 2 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | Contributed | 2 | 1 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 1 | 2026-11-12 |
| Epoch AI | Contributed | 1 | 0 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 1 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 0 | 1 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 1 | 2026-11-12 |

**No-contribution detail:**

- **N2K Cyberwire Daily Briefing**: no issue since V15 #214 (Nov. 9), covered 11-10; #215 and #216 return "not found."
- **The Canon Project**: no review since *The Ghidra Book* (Nov. 9), covered 11-10.
- **FFX Now**: nothing dated Nov. 11 or 12 at run time (before today's Morning Notes); the Nov. 10 items were checked 11-11.
- **Wired**: no new items in the security RSS feed. WIRED's AI-safety expert panel came through WIRED's AI Lab email and is credited to Gmail Newsletters.
- **CyberScoop**: nothing after the 11-10 LoSapio story, covered 11-11.
- **CSO Online CISO Appointments**: still no October or November section on the page.
- **CISA Cybersecurity Advisories**: no feed items after Nov. 10.
- **LEAP**: the highest wave is still Wave 12 ("Safety Policies").
- **CISO Tribune — The Wire**: the newest entry is still isolved's Satyam Patel (Nov. 10), covered 11-11.
- **NIST Cybersecurity Insights Blog**: no new post since Oct. 27.
- **EFF Deeplinks**: one item, the EFFector 38.20 newsletter, which recaps EFF's records suit over Medicare's WISeR AI prior-authorization program; no CIR fit.
- **CSIS Strategic Technologies Program**: newest cybersecurity item is still Nov. 5; this week's listings are event announcements.
- **AI Alignment Forum**: no new posts since the 11-11 run, only comment threads on posts already covered.
- **tl;dr sec**: no issue inside the pull window (newest is Nov. 5).
- **Detection Engineering Weekly**: newest issue is still DEW #172 (Oct. 29).
- **Resilient Cyber**: newest item is Nov. 10, before the pull window.
- **AI as Normal Technology** *(first run)*: newest post is Nov. 10, before the pull window.
- **Reflective Altruism** *(first run)*: newest post is Nov. 6.
- **Understanding AI (TRIAL)** *(first run)*: newest post is Nov. 5.
- **Marcus on AI (TRIAL)** *(first run)*: one in-window post, on reports about Nvidia's CEO, which fails this source's filter (a dated, testable claim about AI capability limits or timelines).

**Crediting notes:** Risky.Biz is credited for Srsly Risky Biz's Iran-attribution analysis; its China section restates Vapor Panda and Silent Train, already covered. Cybersecurity Dive is credited for the CISA priorities memo, which no other source carried; its N-able hotfix item duplicates SecurityWeek, which is credited. Epoch AI is credited because the Epoch Brief reports three new Epoch measurements, per that source's crediting rule. The Record's three featured stories were all dated Nov. 11 and each was opened individually; its Turla "Cereal" story (Nov. 10) was covered 11-10.

**Also checked, not itemized:** Gmail's local-news digests (ARLnow, ALXnow, WSHnow, InsideNoVa), the VA's Veterans Day emails, the NCSC Wee Dram invitation, Lawrence Lessig on Judge Posner, Garbage Day, AI how-to and pricing newsletters, a Google Alerts digest, an NVIDIA stock-selloff explainer, and a Human in the Loop issue on the Jensen Huang reports had no CIR fit. THN's Daily Updates email and SecurityWeek's 11-11 briefing repeat stories covered 11-11 (Xen Orchestra, Outlook zero-day, Lazarus neurons). SecurityWeek's Notion/Fireworks story repeats 11-11 coverage; its Citrix/Ivanti and Asus/Zoom patch roundups and Finite State's $27M round weren't written up. THN's "We Built An Agent That Broke All of Our Security Rules" is vendor-authored content from Token and wasn't written up. WIRED AI Lab's AI-peer-review study (the best of seven models caught 71 of 100 planted errors) and its robotics items had no CIR fit. Rick's Substack feed has no new essay since Nov. 9.

*Pending artifact approvals: none. No open PRs on raceBannon99/nexus-artifacts.*

*No forecast range moved today. The AI Timeline Forecasting chart in Alexandria's Library (`images/ai-timeline-forecasting.png`) is still out of date from 11-11, when the AGI, Superintelligence, and P(Doom) ranges moved. It can be refreshed with the `nexus-ai-timeline-chart-refresh` skill, which opens a PR for Rick's approval.*
