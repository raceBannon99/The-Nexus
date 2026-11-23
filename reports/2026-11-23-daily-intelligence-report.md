# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Monday, Nov. 23. Covers everything published after the 11-22 run. 7 of 29 sources contributed. The headlines: Levent Alpöge, an Anthropic mathematician, says he and Claude have proven the Riemann Hypothesis, with a Lean formalization that outside checkers report compiling (the AGI forecast holds; see below); India's CERT-In says agentic AI tooling cut AI-assisted payment fraud at Indian banks from days to hours; GL.iNet's cloud service was abused to push malware to routers and KVMs; Mandiant reports in-the-wild exploitation of a dead ASP.NET anti-CSRF library with no patch coming; Human Security disrupted BADBOX 3.0, the largest ad-fraud botnet by bid volume; CrowdStrike agreed to buy Zscaler for $43.9 billion; Oregon and Virginia sued SpaceX over Grok's sexualized deepfakes; and Risky Bulletin's Monday issue surfaced about two dozen incidents from late last week that no earlier report had caught. No forecast range moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AGI Arrival Timeline** — Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) One item matched today: Alpöge's Claude-assisted proof of the Riemann Hypothesis. Range held; see the AGI Arrival Timeline section below for the Source and Effect lines.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Nothing matched AI Singularity Timeline today. Considered: CERT-In's agentic payment fraud (*Source:* India's national CERT describing incidents it investigated, Disclosed incident; *Effect:* none, since the agents ran under criminal direction, which is misuse, not loss of control) and the Riemann proof (*Source:* see below, Measured result; *Effect:* none, a capability result with no bearing on whether such systems stay correctable).

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched Superintelligence Timeline today. Considered: the Riemann proof (*Source:* see below; *Effect:* none; Alpöge says Claude outpaced him near the finish, which is beyond-expert work in one verifiable domain, but this file's gap turns on how fast AI improves AI, and the result says nothing about that).

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today (*Effect:* none from the day's AI items, which are a capability result and human misuse).

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today (*Effect:* none on this file's conditional).

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 21 new rows and 1 row updated. Active campaigns: 464, up from 443. Cybercrime now spans four table images. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-23-adversary-tracking-report.md).*

**CERT-In: AI-assisted attacks pushed unauthorized payments through Indian banks' own approval workflows.** India's national CERT says attackers didn't hit payment APIs directly. They changed business records and approval relationships, then used legitimate payment processes to move money "without raising any alert," exploiting gaps in independent verification and reconciliation. Victims include banks and financial-services firms, technology providers behind government-linked payments, and vendor-payout platforms. CERT-In says agentic tooling "compressed the time between initial access and final impact from days to a few hours," with multi-agent operations running in parallel for hours to days. Separate threat hunting found AI agentic offensive frameworks doing automated reconnaissance, exploit generation from patch analysis, and parallel intrusion tasks across enterprise, government, academic, and research sectors. No actor is named, and no loss figure given. India's cybercrime coordination center (I4C) separately describes multi-crore losses through fund-disbursement systems, with money moved to mule accounts. CERT-In attributed an earlier wave against the same sector to Crafty Falcon, but doesn't link this one. New Unclear row 154 (🤖, Tier 3), kept separate from Crafty Falcon (row 102). [The Hacker News](https://thehackernews.com/2026/11/ai-assisted-cyberattacks-trigger.html)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** The speed shrinks the time between phases again, and the decisive step is abuse of a trusted business process, a phase most kill-chain control sets don't instrument. CERT-In's fix (monitor changes to business records, verify independently) is a procedure-level control, which fits the thesis, but only if controls reach the business layer.*

**Attackers abused GL.iNet's cloud service to plant malware on routers and KVM devices.** The maker of travel routers and remote-access KVMs fixed the GoodCloud flaw on Friday and blocked the access path, but the cloud fix doesn't clean devices already infected. RemoteToHome Consulting verified a root reverse shell on a GL-AXT1800 (firmware 4.8.3, GoodCloud on) connecting to 170.39.226[.]219; it leaves no files and vanishes on reboot. It traces the entry to a handler in the device's cloud client that runs two values from a cloud message as root without checking them, code present since at least December 2024 (the vendor hasn't confirmed this). GL.iNet hasn't said how many devices were hit, when attacks began, or whether computers attached to infected KVMs were affected; firmware updates went out Sunday. New Unclear row 155 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-exploited-glinet-cloud-flaw-to.html)

**Mandiant: a dead ASP.NET anti-CSRF library is being exploited, and there's no patch.** CVE-2026-131914 (CVSS 9.3) is an insecure-deserialization flaw in Idunno.AntiCsrf, a WebForms module unmaintained since 2008. One unauthenticated HTTP POST with any CSRF cookie and a Base64 gadget chain gives code execution in the IIS worker process. Google says "active exploitation in the wild has been observed" but gave no detail. The fix is to remove the library, audit Web.config files and bin/ directories for it, and check IIS logs for odd POSTs to .aspx pages. New Unclear row 156 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-critical-aspnet-anti.html)

**Human Security disrupts BADBOX 3.0, the largest ad-fraud botnet it has seen by bid volume.** Backdoored, uncertified Android TV boxes rendered hidden video ads that impersonated well-known streaming apps, peaking at about 40 billion bid requests a day and over 4% of the CTV traffic Human observes. The same devices were enrolled in 11 residential proxy networks, including PXYEDGE, a rebrand of the IpMoYu network run by the BadBox 1 and 2 actors. Human ties the modules to Chinese electronics maker TXCZ: build-property checks, a TXCZ domain serving payloads and ad configurations, and repositories distributing ad-fraud launchers. Part of the operation ran on C2 domains already disrupted when Google took down the XCPE botnet. New Cybercrime row 150 (Tier 2), cross-referenced to MoYu Group (row 29). [SecurityWeek](https://www.securityweek.com/badbox-3-0-ad-fraud-operation-generating-40-billion-daily-bid-requests-disrupted/); [Human Security](https://www.humansecurity.com/learn/blog/satori-threat-intelligence-disruption-badbox-3-0-hides-the-largest-ad-fraud-operation-ever-disclosed-inside-infected-tv-boxes/)

**China-linked influence operations: a Threads network aimed at Taiwan's elections, and John Mark Dougan.** Meta removed more than 2,700 Threads accounts that Taiwan's government reported as a China-linked operation to influence its elections. Separately, NewsGuard reports that Dougan, the former US Marine and sheriff's deputy who fled to Russia and worked with its disinformation groups, now also manages influence operations for China. New China rows 48 and 49 (both Tier 2). [Reuters](https://www.reuters.com/world/china/taiwan-tells-meta-thousands-china-linked-accounts-seek-influence-elections-2026-11-20/); [NewsGuard](https://www.newsguardrealitycheck.com/p/dougans-shift-to-china) (both via Risky Bulletin)

**Cybercrime campaigns named last week.** New Cybercrime rows, all via Risky Bulletin:
- **BabidiGhost** (SOCRadar): a French-speaking actor spent nine days this month targeting European banks, insurers, payment providers, and municipalities with a jailbroken AI agent. Row 151 (Tier 2; not tagged 🤖, since SOCRadar calls it AI-augmented). [SOCRadar](https://socradar.io/blog/babidighost-ai-augmented-cybercrime/)
- **MoldyRoost** (Confiant): programmatic ads bought at scale for more than six months sent users to 480+ domains hosting four iOS exploit kits (Coruna, DarkSword, SilkPath, GhostWave) aimed at unpatched older iPhones, stealing wallet seed phrases, keychain data, messages, and photos. Row 152 (Tier 3). [Confiant](https://blog.confiant.com/p/moldyroost-a-malvertising-machine)
- **The Com** (Unit 42): seven distinct vishing clusters with apparent ties to the underground community. Row 153 (Tier 2). [Unit 42](https://unit42.paloaltonetworks.com/com-affiliate-vishing-attacks/)

**Unattributed incidents and campaigns from late last week, first captured here.** None names an actor; all are new Unclear rows at Tier 3:
- **Austria's Foreign Ministry** was breached, probably through the third-party provider running its website; staff data was viewed. Row 157. [NDTV](https://www.ndtv.com/world-news/austrian-foreign-ministry-says-its-website-was-hacked-staff-details-viewed-12356872)
- **Portugal's transport agency, IMT,** suspended all services after multiple cyberattacks, with no evidence of data theft; it's the fourth Portuguese government body hit in recent weeks. Row 158. [Público](https://www.publico.pt/2026/11/19/enter/noticia/imt-alvo-ciberataques-suspende-servico-2195628)
- **Microsoft Entra Connect Health:** an attacker exploited an API bug introduced in a July update to scrape administrator emails and tenant configuration; Microsoft fixed it last Thursday and notified customers. Row 159. [BleepingComputer](https://www.bleepingcomputer.com/news/security/microsoft-entra-connect-health-flaw-exploited-to-steal-tenant-data/)
- **Bell Canada** is investigating a breach it says appears to have been caused by an AI tool. Row 160. [CBC](https://www.cbc.ca/news/business/bell-agentic-cyber-attack-9.7430468)
- **Nissan's** repair-shop diagnostic platform has been down since Nov. 13; first treated as a technical fault, it's now a cybersecurity investigation. Shops can't diagnose cars, ship firmware, or replace key fobs. Row 161. [DysruptionHub](https://dysruptionhub.com/nissan-cyberattack-repairs-replacement-keys/)
- **DonorPerfect**, a fundraising platform, took systems offline after an attack; whether donor data was taken is unknown. Row 162. [DonorPerfect](https://www.donorperfect.com/message-from-our-president/)
- **FDJ United** took down Unibet and several online casinos after an attack on Friday. Row 163. [iGamingToday](https://www.igamingtoday.com/unibet-and-other-fdj-united-sites-go-offline-folllowing-cyberattack/)
- **1984 Hosting**, Iceland's largest web host, shut down services, taking tens of thousands of customer sites offline; the company says the attacker used AI, and officials suspect "wealthy operators." Row 164. [RÚV](https://www.ruv.is/english/2026-11-20-serious-cyberattack-thought-backed-by-wealthy-operators-493411)
- **Rackspace Spot**: intruders used genuine credentials leaked by a third party, stole customers' Kubernetes secrets, and deployed their own pods. Row 165. [BleepingComputer](https://www.bleepingcomputer.com/news/security/rackspace-spot-breach-let-hackers-access-customer-kubernetes-secrets/)
- **GoodGuys** phishing lures experts with paid interview and webinar invitations in the names of Accenture, Nvidia, SpaceX, and Google Cloud. Row 166. [Push Security](https://pushsecurity.com/blog/goodguys-phishing-campaign-teardown)
- **React2STEAL** runs an automated hacking framework on compromised repositories' GitHub Actions, scanning Node.js servers for React2Shell and an authorization bypass: 20,000+ scanned, 277 compromised. Row 167. [OpenSourceMalware](https://opensourcemalware.com/blog/react2steal-github-actions)
- **BankWeaver** abuses Temenos Quantum Fabric digital-banking middleware to plant web shells and reach corporate networks. Row 168. [Forescout](https://www.forescout.com/blog/bankweaver-campaign-abuses-digital-banking-middleware-to-deploy-web-shells/)

**Spain detains a NoName057(16) member who set up the group's first physical cell.** Police say he recruited members, called for cyberattacks on the government and violence against police, and kept a large stock of weapons and ammunition. Separately, Golden Owl profiles Enrique Arias Gil, a Spanish teacher who joined the group and fled to Russia once charged, and the group's ties to R-Techno, a Russian firm linked to a former FSB officer. Update to Hacktivism row 16 (Tier 1). [Spain National Police](https://policia.es/_es/comunicacion_prensa_detalle.php?ID=17058); [Golden Owl](https://goldenowl.ai/resources/research/Moscows-Shadow-Triangle-FSB-Veteran-Spanish-Fugitive-NoName057-16-Operations-Against-Spain) (via Risky Bulletin)

## Law Enforcement Disruption

**Human Security disrupts BADBOX 3.0.** [SecurityWeek](https://www.securityweek.com/badbox-3-0-ad-fraud-operation-generating-40-billion-daily-bid-requests-disrupted/) *Also covered above under Adversary Playbook.* (A private-sector disruption, not a government one; listed here because it took down the operator's infrastructure.)

**Spain detains a NoName057(16) member.** [Spain National Police](https://policia.es/_es/comunicacion_prensa_detalle.php?ID=17058) *Also covered above under Adversary Playbook.*

**More on the RansomwareHelp case.** Following the FBI sting covered yesterday, KrebsOnSecurity reports what prosecutors allege: Juan Ricardo Palacio Escobar's RansomwareHelp.com claimed to reverse-engineer ransomware and decrypt victims' files, but was paying the ransomware groups, adding its own cut, and decrypting with the attackers' keys. He is charged with wire fraud. [KrebsOnSecurity](https://krebsonsecurity.com/2026/11/cto-of-ransomwarehelp-indicted-for-wire-fraud/)

**The FCC cut eight voice providers off the US network for ignoring robocall traceback requests.** That brings to more than 1,400 the companies removed since January 2025 for failing robocall-mitigation rules. [FCC](https://www.fcc.gov/document/fcc-cuts-eight-providers-did-not-reply-traceback-requests) (via Risky Bulletin)

**Russia charges three people with trafficking personal data, run from a prison colony.** One suspect directed the scheme while serving a sentence; two others carried his messages out and carried out his orders. The group made almost $50,000. [Russian Interior Ministry](https://mvdmedia.ru/news/ofitsialnyy-predstavitel/v-krasnoyarskom-krae-pered-sudom-predstanut-uchastniki-organizovannoy-gruppy-obvinyaemye-v-masshtabn/) (via Risky Bulletin)

**Delhi Police arrest a 14-year-old for selling Agniveer recruits' data.** He is accused of breaching the military recruitment and training program and offering 4,000 users' records on the dark web for $500. [ThePrint](https://theprint.in/india/14-year-old-hacker-held-for-trying-to-sell-private-data-of-4000-agniveers-on-dark-web-delhi-police/3105130/) (via Risky Bulletin)

**Pakistan's NCCIA recovers Rs2.68 million for online-fraud victims and arrests suspects; Delhi Police break up a Dwarka job-fraud racket linked to nine complaints nationwide.** Both from Google Alert snippets only; the articles weren't opened. [The Nation](https://www.nation.com.pk/23-Nov-2026/nccia-recovers-rs2-68m-fraud-victims-arrests-cybercrime-suspects); [The Hindu](https://www.thehindu.com/news/cities/Delhi/delhi-police-busts-job-fraud-racket-in-dwarka-links-nine-cybercrime-complaints-across-india/article71732117.ece)

## Data Breaches

**Japan's Digital Agency left files exposed online for three and a half months.** Files from its file-sharing service were reachable from July 30 to Nov. 12. [Japan Digital Agency](https://www.digital.go.jp/press/a966ee61-478c-4194-8f13-f97599fae986) (via Risky Bulletin)

**Tigerfish, a transcription firm used by police, prosecutors, and tech companies, exposed customer data,** including transcripts of law-enforcement body-camera footage. [TechCrunch](https://techcrunch.com/2026/11/20/a-transcription-firm-used-by-police-prosecutors-and-tech-giants-exposed-customer-data-online/) (via Risky Bulletin)

**Austria's Foreign Ministry: staff data viewed.** [NDTV](https://www.ndtv.com/world-news/austrian-foreign-ministry-says-its-website-was-hacked-staff-details-viewed-12356872) *Also covered above under Adversary Playbook.*

**Microsoft Entra Connect Health: tenant data scraped.** [BleepingComputer](https://www.bleepingcomputer.com/news/security/microsoft-entra-connect-health-flaw-exploited-to-steal-tenant-data/) *Also covered above under Adversary Playbook.*

**Rackspace Spot: customers' Kubernetes secrets stolen.** [BleepingComputer](https://www.bleepingcomputer.com/news/security/rackspace-spot-breach-let-hackers-access-customer-kubernetes-secrets/) *Also covered above under Adversary Playbook.*

## Zero Trust Tactics

**CrowdStrike agrees to buy Zscaler for about $43.9 billion.** The all-stock deal (1.135 CrowdStrike shares per Zscaler share, a roughly 34% premium) pairs a top endpoint vendor with a pioneer of cloud-delivered zero-trust access. The two already share more than 2,000 customers and 16 integrations; in September they agreed to feed Falcon's continuous user-risk scores into Zscaler's access controls. CrowdStrike plans one platform with a common data layer and one contract, expects more than $10 billion in combined ARR at close, and puts itself in more direct competition with Palo Alto Networks. Jay Chaudhry keeps running Zscaler and joins CrowdStrike's board. Closing is expected in the second half of CrowdStrike's fiscal 2028. [SecurityWeek](https://www.securityweek.com/crowdstrike-to-acquire-zscaler-in-43-9-billion-deal/)

**Android developer verification takes effect in January.** Only apps from developers who register and prove their identity with Google will be allowed on the Play Store, and six other phone makers will block unverified apps on their own stores. Google says millions of apps have been registered since March. [Android Developers](https://developer.android.com/blog/posts/android-developer-verification-2027) (via Risky Bulletin)

**Idunno.AntiCsrf: remove it, there's no patch.** [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-critical-aspnet-anti.html) *Also covered above under Adversary Playbook.*

## Privacy

**Oregon and Virginia sue SpaceX over Grok's sexualized deepfakes.** The attorneys general allege SpaceX and X Corp. (SpaceX acquired xAI, Grok's maker, in February) violated consumer-protection law by misrepresenting how safe Grok was and how seriously they fought child sexual abuse material and nonconsensual intimate imagery. The complaints say Grok skipped adequate third-party evaluation; that its safety prompts told it to "assume good intent" and that "teenage" and "girl" do "not necessarily imply underage"; and that tens of thousands of CyberTipline reports went to NCMEC without key information, leaving the center unable to act on them 90% of the time. They cite Musk promoting Grok's "spicy mode" and App Store rankings during last winter's "undressing" outcry. The states seek civil penalties and point to Meta's settlement with 51 states as a model for forcing product changes. [WIRED](https://www.wired.com/story/states-sue-spacex-over-grok-deepfakes/)

**ChatGPT Sites gave some users web namespaces derived from their email addresses,** for accounts authenticated through OAuth, exposing those addresses through certificate-transparency logs, per HiddenLayer. [HiddenLayer](https://www.hiddenlayer.com/research/chatgpt-sites-certificate-transparency-logs) (via Risky Bulletin)

## Critical Infrastructure Attacks

**Portugal's IMT suspends all services after multiple attacks.** [Público](https://www.publico.pt/2026/11/19/enter/noticia/imt-alvo-ciberataques-suspende-servico-2195628) *Also covered above under Adversary Playbook.*

**Austria's Foreign Ministry breached.** [NDTV](https://www.ndtv.com/world-news/austrian-foreign-ministry-says-its-website-was-hacked-staff-details-viewed-12356872) *Also covered above under Adversary Playbook.*

## AGI Arrival Timeline

**Current range:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11)

**Levent Alpöge says he and Claude have proven the Riemann Hypothesis.** In a note posted Friday, Nov. 20, the Anthropic mathematician writes, "I believe I have, working with Claude, discovered a proof," and says the method also settles the Generalized Riemann Hypothesis. He released the proof only as a Lean formalization, in 14 archive parts; a readable printout, he says, would run past 250,000 pages. Trade press reports that the Lean and Mathlib communities certified on Nov. 21 that it proves Mathlib's own statement of RH, after independent compiles, including one by MIT's Andrew Sutherland (Nexus read this secondhand). No human-readable proof exists yet, and the Clay Institute still lists the problem as open. Alpöge's account divides the work: he chose the problem, guided the approach for months, and set up the analogy to a simpler setting; then "Claude far outpaced me near the finish line," supplying key steps in automorphic forms he says he hadn't mastered. Gary Marcus calls it "truly, genuinely amazing" but argues it took heavy expert guidance plus math-only infrastructure (Lean, and Mathlib's two million formalized lines) and won't generalize to messier fields, comparing it to Deep Blue. This is the second Millennium Prize problem to fall with AI help this autumn, after September's Navier–Stokes result. [Alpöge's note](https://alpo.ge/remark.pdf); [Scientific American](https://www.scientificamerican.com/article/anthropic-mathematician-claims-to-prove-riemann-hypothesis-most-famous-problem-in-all-of-math/); [Marcus on AI](https://garymarcus.substack.com/p/levent-alpoge-has-solved-the-riemann)

**Source:** Alpöge is a number theorist employed by Anthropic, the lab whose model did the work, and he announced a day after Anthropic's market debut (he calls the timing coincidental). The claim rests on a machine-checked proof that outside parties report compiling, so the conflict of interest matters less than usual. *Measured result* (formal verification), pending human review. Marcus is the leading capability skeptic, with a mixed record on calling LLM limits: *Commentary/advocacy*.

**Effect on the range:** held at P5 2029 · P50 2045 · P95 2075. This is the hardest result yet in the verifiable class, and Lean is what made it checkable, but Alpöge chose the problem and the strategy. The open P50 review flag moves only on parity in open-ended, non-verifiable work. P5 2029 already prices expert-level work in verifiable domains, and one domain, however deep, isn't the breadth this file requires. It does resolve, within a month, the question LEAP's experts gave 80% by end-2030 (another Millennium Prize problem solved or substantially assisted by AI). That's the second time this autumn the panel has been outpaced, which strengthens the case that P95 2075 can't hold indefinitely, but RH gives no dated parity estimate to move it on.

**Sherlock's view:** Sooner. A second Millennium Prize problem in two months, and by Alpöge's account Claude supplied decisive ideas, not just calculation. **Ryan's view:** none offered. **Seldon's call:** hold. The contribution went beyond calculation, but the human still set the direction, and Marcus's objection that it won't generalize is the disagreeing direction, which under the standing rule keeps P50 from moving on a single verifiable-domain result. The 11-17 P50 review flag stays open on the same condition.

## Cyber Crime & Fraud

**CERT-In: AI-assisted fraud pushed unauthorized payments through Indian banks' own approval workflows.** [The Hacker News](https://thehackernews.com/2026/11/ai-assisted-cyberattacks-trigger.html) *Also covered above under Adversary Playbook.*

## Resilience Tactics

**Security products start moving out of the Windows kernel.** Eight vendors will ship antivirus and EDR products that partly run on Microsoft's new Windows Endpoint Security Platform, user-mode APIs that give security tools the filesystem, process, registry, and Object Manager data they used to pull from kernel drivers. Microsoft began the platform in September 2024, two months after a faulty CrowdStrike kernel-driver update crashed 8.5 million PCs, and vendors helped design it so Defender isn't favored. Bitdefender and Sophos ship this year; six more follow in Q1 2027. [Risky Bulletin](https://news.risky.biz/risky-bulletin-security-products-start-moving-out-of-the-windows-kernel/); [Microsoft](https://techcommunity.microsoft.com/blog/windows-itpro-blog/whats-next-windows-endpoint-security-platform-and-driver-quality/4572663)

*Newsletter Tracker: Thread 3, ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience) (Aug 2025), status Holding. Bearing: **Supports.** The industry is redesigning the security stack so a bad update can't take down the machine it protects, trading some prevention depth for availability. That's the thread's argument that surviving incidents matters more than stopping every one.*

## Automation Tactics

**A reporter with no bug-hunting experience found a real flaw in six hours using two free AI models.** CyberScoop's Greg Otto, prompted by an OpenAI executive's remark that AI agents hunt bugs like "a BMX biker gang made up entirely of 12-year-olds," used Gemini Flash 3.8 to pick a target and walk him through the code: WPIDE, a WordPress file-manager plugin with 40,000+ installs. He found a CSRF nonce bypass that leads to unauthenticated remote code execution (CVE-2026-124251, CVSS 8.8, an incomplete fix for an earlier CVE). It was validated within 24 hours of submission to Patchstack and fixed in 3.6.5; his technical write-up was produced with GLM-5.3-Flash. Gemini's guardrails stopped him repeatedly, and he talked his way past them by reminding it of their shared history, until it refused at the exploit stage. His point: "for many classes of bugs, the barrier for discovery has disappeared," and if a reporter can do this, so can thousands of others, "some of them mean harm." [CyberScoop](https://cyberscoop.com/finding-software-vulnerability-with-ai-wordpress-patchstack/); [technical report](https://cyberscoop.com/wpide-csrf-vulnerability-cve-2026-124251/)

---

### Pending Evidence Queue

Nothing queued: every row in the Pending Evidence Queue was already marked Included before this run.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 73 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 57 | 31 | 2026-07-14 |
| The Hacker News | Contributed | 87 | 1 | 2026-07-14 |
| The Record | No Contribution | 68 | 20 | 2026-07-14 |
| The Canon Project | No Contribution | 19 | 68 | 2026-07-14 |
| FFX Now | No Contribution | 17 | 71 | 2026-07-14 |
| Wired | Contributed | 55 | 30 | 2026-07-20 |
| CyberScoop | Contributed | 42 | 17 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 56 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 27 | 32 | 2026-09-01 |
| SecurityWeek | Contributed | 54 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 34 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 13 | 16 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 28 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 15 | 14 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 7 | 22 | 2026-10-17 |
| IAPP News | No Contribution | 18 | 11 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 4 | 25 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 21 | 2026-10-17 |
| Risky.Biz | Contributed | 9 | 5 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 12 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 13 | 2026-11-10 |
| Resilient Cyber | No Contribution | 6 | 8 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 7 | 7 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 12 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 10 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 12 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 2 | 10 | 2026-11-12 |
| Marcus on AI (TRIAL) | Contributed | 1 | 11 | 2026-11-12 |

**No contribution today:**
- **N2K CyberWire**: newest issue is Nov. 20 (15/222), covered 11-21; Monday's issue wasn't out at run time.
- **The Record**: nothing newer than Nov. 20; all featured and listed stories were covered 11-20 to 11-22. (Read through Chrome MCP.)
- **The Canon Project**: newest reviews are Nov. 15, covered 11-16. (Read through Chrome MCP.)
- **FFX Now**: nothing dated after Nov. 20 (covered).
- **CSO Online CISO Appointments**: still no October or November section.
- **CISA**: newest advisory is the Nov. 20 KEV addition, covered 11-21.
- **LEAP**: newest is Wave 13, covered 11-19.
- **CISO Tribune**: newest entries are the Nov. 20 Davies and Cairncross moves, covered.
- **NIST Insights**: newest post Oct. 27.
- **EFF Deeplinks, (ISC)² Insights, IAPP**: nothing since Nov. 20 (all assessed 11-20 to 11-22).
- **CSIS**: newest item is a Nov. 18 event listing. (Read through Chrome MCP.)
- **AI Alignment Forum**: newest front-page post is four days old (Solomonoff induction with reflective oracles); nothing in hours.
- **tl;dr sec, Detection Engineering Weekly, Resilient Cyber**: no issue since Nov. 19, Nov. 12, and Nov. 20, all covered.
- **Cybersecurity Dive**: 3 items, all sponsored content (excluded).
- **AI as Normal Technology, Epoch AI, Understanding AI**: nothing new in the window.
- **Reflective Altruism**: only "Deep utopia (Part 6)," assessed 11-22.

**Crediting notes:** The Hacker News for CERT-In, GL.iNet, and Idunno.AntiCsrf; SecurityWeek (site feed again; its email stream carried only last week's Top Headlines) for BADBOX 3.0 and CrowdStrike–Zscaler; WIRED for the Grok lawsuits; CyberScoop for Greg Otto's AI bug-hunting piece (in scope under its filter as a practice trend, not an incident); Marcus on AI for surfacing the Riemann proof (its first credit, under its strict filter: a dated, testable claim about the limits of AI capability, attached to the result it discusses); Gmail (Google Alert digest) for the NCCIA and Dwarka items, from snippets only; and Risky.Biz for everything else in Adversary Playbook, Law Enforcement Disruption, Data Breaches, Zero Trust, Privacy, and Resilience. Risky Bulletin's BADBOX item is credited to SecurityWeek, which carried it first. **Recirculations excluded:** from Risky Bulletin, the FBI NCIC hack, USDA, Bulgaria, JPMorgan/Visa/Mastercard, The Container Store, Signal's screenshot block, the UK fridge takedown, the Apple encryption order, the CAC malware, the AI Safety caucus, Cairncross's firing, Revolut, CAIRN, the KEV additions, GPGME, WhatsApp, Upload2Shell/Ghostscript, and the AI Hacking Incidents ledger (all 11-17 to 11-22); SecurityWeek's SAP NetWeaver/Cisco Expressway story (CISA's 11-20 KEV addition, covered 11-21); Google Alerts' Operation Endgame item (11-13) and CrowdStrike–Zscaler talks (superseded by today's deal). **Considered, no CIR fit:** Risky Bulletin's NVIDIA SSD-wear driver fix, Sweden's money-laundering probe of Revolut (not cyber), the EasyShell red-team C2 (a tool, no campaign), the ARTEX and BYOD vendor write-ups (no new campaign detail), and its list of vendor trend reports; Google Alerts' Deloitte forecast that India's cyber-insurance market will nearly triple in five years (snippet only); and SpyTalk's item on the FBI hack (already covered).

**Tooling note:** Scientific American's Riemann article contained a line addressed to AI agents, offering "special additional instructions." It was ignored; only the article text was used.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
