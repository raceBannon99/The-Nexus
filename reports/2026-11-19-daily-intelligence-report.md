# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Thursday, Nov. 19. Covers everything published after the 11-18 run. 17 of 29 sources contributed. The headlines: Mandiant says China's Armory Castle exploited a vCenter authentication bypass as a zero-day for more than two months before Broadcom patched it today; the European Commission confirmed that an ARTEX-driven attack knocked its personnel systems offline for more than 10 days; NGINX, PHP, Drupal, Ruby, and F5 BIG-IP all shipped critical fixes, and an automated harness found most of the NGINX bugs in 90 minutes; officials told Congress the week's outages came from patching, not hacking, much of it to fix AI-found flaws; Ukraine arrested four members of an ex-Conti-linked ransomware network; and LEAP's Wave 13 shows expert forecasters sharply raising their expectations for AI progress. No forecast range moved.*

## Today's CIR Matches

- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **AGI Arrival Timeline** — Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Cybersecurity Intrusion Kill Chain Prevention Tactics** — Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Over the Horizon Technology Trends** — Emerging tech 3–25 years out — quantum computing, 5G, AI, net neutrality, SEC materiality rules, and related government policy.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Two items matched: LEAP Wave 13 and Understanding AI's adoption data. Neither moved the range, for reasons given under AGI Arrival Timeline below.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Nothing matched AI Singularity Timeline today.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched Superintelligence Timeline today.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today.

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Zero Trust Tactics

**NGINX2Root: five critical NGINX flaws, most of them found by an automated harness.** F5 patched five NGINX bugs (CVSS 9.2) that can give unauthenticated attackers code execution, plus 17 others. The worst, CVE-2026-123007, is an integer underflow in HTTP/2 flow control present since NGINX 1.9.5 (2015); Wiz ran code on NGINX serving only static files, and Rapid7's public exploit needs about 128 GB of HTTP/2 traffic (about two minutes over 10 Gbps, too slow to finish below roughly 300 Mbps). The others hit mail proxying, HTTP/3, proxied server names built from variables, and a second HTTP/2 use-after-free. Xint's harness found four of the five in 90 minutes of scanning about 50,000 lines, with a working exploit 10 minutes later, then chained the HTTP/2 bug with a Linux SCTP kernel flaw to escape a Docker container to root. Xint's Shodan snapshot puts 98.9% of 11.94 million version-identifiable NGINX hosts on affected releases (versions, not confirmed exposure). Fixed in 1.31.9 and 1.30.7; no exploitation reported. [CyberScoop](https://cyberscoop.com/nginx-critical-vulnerabilities-exploits/); [SecurityWeek](https://www.securityweek.com/f5-patches-critical-nginx2root-flaws-as-poc-exploits-go-public/); [The Hacker News](https://thehackernews.com/2026/11/10-year-old-nginx-http2-flaw-lets.html); [Cybersecurity Dive](https://www.cybersecuritydive.com/news/critical-remote-code-execution-flaws-nginx-web-server/875196/)

**PHP fixes seven critical RCE bugs, including an incomplete PHP2Shell fix.** The scheduled release fixes CVE-2026-115560 (session upload progress: data written in one serialization format and read in another lets a gadget chain run code), CVE-2026-129481 (a use-after-free PHP calls an incomplete fix for PHP2Shell's CVE-2026-109619, now widely exploited), and further use-after-frees, several of them not yet shown to reach code execution. [SecurityWeek](https://www.securityweek.com/php-patches-seven-critical-rce-vulnerabilities/); [The Hacker News](https://thehackernews.com/2026/11/php-fixes-7-critical-flaws-including.html)

**Drupal: the built-in installer can let an unauthenticated attacker reinstall a site.** CVE-2026-132165 (critical, 18 of 25) affects every release below 10.6.22 and Drupal 11 before 11.3.22 and 11.4.13, in uncommon configurations; a proof of concept exists, and the team warned exploits could follow within hours. /core/install.php stays on every site and core's default .htaccess doesn't block it, so the team says to block it even after updating. [The Hacker News](https://thehackernews.com/2026/11/drupal-patches-critical-installer-flaw.html)

**Ruby: seven memory-safety flaws, five with code-execution proofs of concept.** The flaws sit in the regular-expression engine and string case conversion (a one-byte heap overflow in single-byte encodings, a double free on crafted `&&` character classes, a size overflow at regex compile). Fixed in Ruby 4.0.10, 3.4.13, and 3.3.14; risk depends on whether attackers can feed crafted patterns or strings to the affected code. [The Hacker News](https://thehackernews.com/2026/11/ruby-releases-fixes-for-7-regex-and.html)

**Low-privilege database accounts can run code on the server.** Depthfirst's Zheng Yu published exploits showing that ordinary grants (PostgreSQL's default TEMPORARY privilege, MySQL and ClickHouse temporary-table rights) reach memory-corruption bugs in engine code: PostgreSQL CVE-2026-116331, MySQL CVE-2026-101786, and a ClickHouse integer overflow, plus an Oracle chain (Oracle Text CVE-2026-114819 and an ORDS GraphQL flaw) that needs no login at all. All five are fixed; no attacks seen. [The Hacker News](https://thehackernews.com/2026/11/researcher-demonstrates-database-rce.html)

**F5 BIG-IP: six critical data-plane overflows.** Unauthenticated attackers can crash the Traffic Management Microkernel, and possibly run code, on virtual servers with specific iRule commands or an APM policy combining two agent types (CVSS 9.8). Engineering hotfixes only, no workaround, no exploitation reported; watchTowr's Sina Kheirkhah found four. [The Hacker News](https://thehackernews.com/2026/11/f5-warns-6-critical-big-ip-flaws-can.html)

**Opening the case resets the TPM lockout on Windows Hello and BitLocker PINs.** TU Berlin researchers showed that on AMD firmware-TPM PCs (and some Intel PCs with Winbond flash, via a voltage glitch that leaks the counter-signing key) an interposer board can roll back the stored wrong-guess count. Worst cases fall from 69 days to 40 hours for a four-digit Hello PIN and from 19 years to 20 days for a six-digit BitLocker PIN. AMD confirmed the firmware flaw and plans fixes through February 2027; until then, add at least two digits. [The Hacker News](https://thehackernews.com/2026/11/flash-chip-attack-bypasses-tpm-lockout.html)

**Java4Shell exploitation attempts have begun.** As of early Nov. 19, GreyNoise had logged over 150 Java4Shell-shaped requests from five IPs, watchTowr sees "java4shell-recon" user agents and blind exploitation attempts, and Cloudflare says scanners are starting to hide their tools; no successful intrusions yet. Cisco, Elastic, Red Hat, and Siemens published impact advisories. Follows the 11-18 disclosure. [SecurityWeek](https://www.securityweek.com/java4shell-exploitation-attempts-begin-as-vendors-rush-out-advisories/)

**CISA adds four exploited flaws to KEV.** Synology DSM CVE-2024-10441, BerriAI LiteLLM CVE-2026-40217 (code execution through the /guardrails/test_custom_code endpoint), Apache Axis CVE-2026-90436, and Vanderbilt's REDCap CVE-2026-90817; federal deadlines are Nov. 21 (Dec. 2 for LiteLLM). The Hacker News links them to ransomware, cryptomining, and LLMjacking. [CISA](https://www.cisa.gov/news-events/alerts/2026/11/18/cisa-adds-four-known-exploited-vulnerabilities-catalog); [The Hacker News](https://thehackernews.com/2026/11/cisa-warns-of-4-exploited-flaws-linked.html)

**Splunk patches nearly 140 flaws.** Two critical bugs in Splunk Enterprise (an empty clustering shared secret, and arbitrary SPL searches) and an RCE in Enterprise Security; SOAR 8.8.0 fixes 59, two of them critical authenticated RCEs. [SecurityWeek](https://www.securityweek.com/splunk-patches-nearly-140-flaws-across-three-core-products/)

**Chrome 158 fixes 204 vulnerabilities.** Six are critical; Google found 145 of them itself and pays no bounty for 163. No exploitation reported. [SecurityWeek](https://www.securityweek.com/chrome-158-patches-204-vulnerabilities/)

**China's Armory Castle exploited a vCenter zero-day for two months.** Mandiant says the group (formerly UNC5221, also Warp Panda) exploited CVE-2026-123890 (CVSS 9.8), an authentication bypass in the VMware Directory Service, for more than two months before Broadcom's patch today. In one intrusion it came in through the BeyondTrust Remote Support zero-day, pivoted to internal Linux appliances, and from early September used a custom tool, Bonesaw, to steal vCenter's LMDB database, extract SAML signing material, create an SSO administrator, forge SAML tokens, install backdoors, and take the vCenter master key and database credentials before moving to an ESXi host. Mandiant says the group knew of the bug before July's separate vCenter bypass (CVE-2026-59309). Fixed in 9.1.1.0200, 9.0.2.0200, and 8.0 U3m; there's no public fix for end-of-support 7.0, which Bonesaw also works against. Update to China row 36 (Tier 1). [SecurityWeek](https://www.securityweek.com/newly-patched-vmware-vcenter-flaw-exploited-as-zero-day-by-chinese-apt/); [The Hacker News](https://thehackernews.com/2026/11/critical-vmware-vcenter-flaw-cvss-98.html)

**Two Apache flaws exploited in the wild.** Rapid7 saw Apache Axis CVE-2026-90436 (end-of-life Axis 1.x, which Apache won't fix) used Nov. 13 against a Confluence Data Center with the old Remote API turned on: within minutes the attacker was querying Confluence's database with its own credentials, likely AI-generated scripts hunted for credentials and Luhn-checked card numbers, and within about 12 hours it had a service-account credential, a cloud data warehouse, and a Microsoft 365 sign-in. The same flaw powers the 4EverAble2Shell N-central exploits. Separately, the ASF says Apache Roller CVE-2026-129448 (unauthenticated XML-RPC deserialization, CVSS 9.8) is being exploited; upgrade to 6.1.6. Update to Unclear row 123; new Unclear row 139 (both Tier 3). [SecurityWeek](https://www.securityweek.com/critical-apache-roller-axis-vulnerabilities-exploited-in-attacks/); [The Hacker News](https://thehackernews.com/2026/11/critical-apache-roller-rce-flaw-under.html)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** See Intrusion Kill Chain Prevention Tactics below.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 10 new rows and 4 rows updated. Active campaigns: 425, up from 416. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-19-adversary-tracking-report.md).*

**China's Armory Castle exploited a vCenter zero-day for two months.** Update to China row 36 (Tier 1). [SecurityWeek](https://www.securityweek.com/newly-patched-vmware-vcenter-flaw-exploited-as-zero-day-by-chinese-apt/) *Also covered above under Zero Trust Tactics.*

**The European Commission confirms an ARTEX-driven attack.** First detected Oct. 22, what the Commission calls an "AI-generated cyber campaign" disrupted payroll, leave, medical reimbursement, and translation systems for more than 10 days as services were taken offline. POLITICO reported that CERT-EU identified ARTEX; the Commission says it has found no broad staff data breach and no ransom demand, and the investigation is open. It is the Commission's third disclosed incident this year. New Unclear row 138 (🤖, Tier 3). [The Record](https://therecord.media/european-commission-confirms-cyberattack-using-ai)

**EggStreme operators rebuilt their toolkit after being exposed.** Bitdefender says the group behind EggStreme, which The Hacker News calls a suspected Chinese APT, keeps targeting Philippine government organizations with an agent that now uses a different network protocol, an expanded command set (Active Directory reconnaissance, WMI, TCP forwarding, PowerShell and .NET execution), and a passive variant that never beacons out. It dropped the keylogger, changed its loader's cryptography twice, and is moving off the certificate authority that tied its old servers together. Bitdefender doesn't attribute it. New China row 45 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/eggstreme-hackers-rebuild-malware-with.html)

**Russian agent charged with surveilling Palantir employees.** Igor Andreevich D'iu, who entered the US illegally from Mexico, is charged with acting as a Russian agent. Prosecutors say he photographed employees' laptop screens at cafés near Palantir's Palo Alto offices, left a laptop and Wi-Fi equipment his handlers could control remotely to "collect data from any Company employees in range," worked from handler-supplied dossiers on employees and their families, and once followed an employee for nearly 30 miles. He was paid $45,000 through couriers who used banknote serial numbers as tokens. New Russia row 24 (Tier 1). [The Record](https://therecord.media/russian-charged-with-spying-on-palantir-for-moscow)

**Ukraine arrests four in an ex-Conti-linked ransomware network.** Working with the FBI, police ran 66 searches and arrested four suspected leaders of a group of at least 27 people (within a wider network of 60+ that includes former Conti members) accused of extorting $40.5 million from at least 28 companies. Callers posing as IT support talked staff into handing over credentials or installing remote-access tools, and the group built a platform that automated those calls with AI-generated voices. Court records name Warren Oil (about $5 million paid), Newpark Resources ($1.5 million), Maxxis International-USA, and Quantum Health ($5 million of a $15 million demand, in mid-2026). New Cybercrime row 146 (Tier 1). [The Record](https://therecord.media/ukraine-ransomware-arrests-cyber); [N2K CyberWire, Daily Briefing 11.19.26](https://thecyberwire.com/newsletters/daily-briefing) (no stable per-story permalink; this links the briefing directory)

**Cisco Expressway exploited soon after a public proof of concept.** F6 says attackers used CVE-2026-76466 (CVSS 9.8, root command execution on clustered Expressway nodes, disclosed Oct. 21) to breach two internet-facing nodes at an unnamed Russian organization, pivot to two internal cluster nodes, and stage Python tools for scanning, SMB, SQL Server, WinRM, and GitLab credential hunting, edited during the attack with an AI assistant. Cisco's advisory still says it knows of no malicious use. Fix: X15.5.20, or block TCP 4371–4372 except between trusted nodes. New Unclear row 140 (Tier 3). [SecurityWeek](https://www.securityweek.com/hackers-exploit-cisco-expressway-vulnerability-soon-after-poc-release/)

**Two Apache flaws exploited in the wild.** Update to Unclear row 123; new Unclear row 139 (both Tier 3). [SecurityWeek](https://www.securityweek.com/critical-apache-roller-axis-vulnerabilities-exploited-in-attacks/) *Also covered above under Zero Trust Tactics.*

**N-able's hosted email-security cloud was breached.** A disruption to Mail Assure and SpamExperts that began Nov. 16 turned out to be unauthorized access to one of their servers; the management portal, APIs, quarantine, and logging are offline in all three regions while mail filtering continues. N-able has no evidence customer data or mailboxes were accessed and says it's unrelated to the N-central flaws. New Unclear row 142 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/n-able-confirms-hackers-accessed-cloud.html)

**About 40 Irish credit unions hit through their software supplier.** An attacker exploited an "authorization flaw" at Belfast-based Wellington IT and ran a script that made five million requests for saved records; RTÉ reports names, account numbers, and addresses of hundreds of thousands of members were accessed. New Unclear row 141 (Tier 3). [N2K CyberWire, Daily Briefing 11.19.26](https://thecyberwire.com/newsletters/daily-briefing) (directory link; see note above)

**Equinor investigates an ongoing attack on its IT systems.** Norway's state-owned oil and gas producer says production isn't affected and there's no sign of data theft, but it has no timetable for full recovery. New Unclear row 143 (Tier 3). [Cybersecurity Dive](https://www.cybersecuritydive.com/news/energy-equinor-investigates-cyberattack/875035/)

**The Gentlemen list Nvidia; Nvidia points to a partner.** The ransomware group's leak-site entry offers no details. Nvidia says it is investigating an incident that may have affected a third-party partner and has found no sign its own systems were affected. Microsoft tracks the operators as Storm-2697; the site lists more than 1,100 alleged victims. Update to Cybercrime row 7 (Tier 2). [SecurityWeek](https://www.securityweek.com/nvidia-responds-to-gentlemen-ransomware-claim/)

## Nation-State Cyber Policy & Law

**Senators ask the White House for a national AI cyber-defense push.** In a letter to DNI Jay Clayton, Sens. Maria Cantwell and Mike Rounds say AI finds and exploits flaws "faster than many organizations can respond" and ask his AI task force to speed deployment of defensive AI tools, set security standards for autonomous agents, have CISA drive adoption across banks, hospitals, utilities, and agencies, and launch a "national cyber defense grand challenge" to cut time from discovery to protection. [The Record](https://therecord.media/ai-cyber-white-house)

**CISA nominee LoSapio: a gap analysis, no promise of more money.** At his Senate Homeland Security hearing, Palantir CISO Mike LoSapio called CISA "the cybersecurity version of the 911 system," promised to report back on gaps left by staff and budget cuts (the agency has lost a third of its staff), and said "more money" doesn't mean more security. He declined to say who won the 2020 election and said he didn't believe Jan. 6 was an attack; Sen. Blumenthal called him "disqualified." A committee vote likely waits until after Thanksgiving. [The Record](https://therecord.media/cisa-losapio-nomination-trump); [CyberScoop](https://cyberscoop.com/michael-losapio-cisa-confirmation-hearing/)

**Commerce tightens AI chip exports and remote access.** BIS's new rule requires license review for chip exports to Singapore, Malaysia, Thailand, Indonesia, and Brazil and requires foreign data centers to keep customers in China and arms-embargoed countries below remote-compute limits. Risky Business's Tom Uren argues it will only make the loopholes narrower: BIS has 11 export control officers worldwide, one of them covering Singapore, Malaysia, and Thailand. The same edition endorses the AI task force's temporary regulatory leniency for AI-hacked victims (covered 11-14) but asks for room to experiment with AI defense too. [BIS](https://www.bis.gov/press-release/bis-issues-rule-addressing-remote-access-american-super-intelligence-technology); [Srsly Risky Biz](https://news.risky.biz/srsly-risky-biz-phew-some-regulatory-relief-for-ai-hacks/)

**Senate Commerce Republicans advance a telecom cybersecurity bill without Democrats.** With Democrats boycotting, the committee advanced FCC nominee Danielle Thumann Severs and several bills, including the Cruz–Warner Telecommunications Cybersecurity and Resilience Act (a Commerce working group to develop best practices and third-party certification criteria, a response to Salt Typhoon) and the Chip EQUIP Act. Their fate is uncertain once Democrats take the majority in January. [CyberScoop](https://cyberscoop.com/danielle-thumann-severs-fcc-nomination-tech-bills/)

**UK tribunal confirms the government served Apple a secret encryption notice.** The Investigatory Powers Tribunal rejected the government's "neither confirm nor deny" position and stated that it "has given Apple a technical capability notice" aimed at iCloud's Advanced Data Protection, which Apple withdrew for UK users in February 2025. Whether the notice is lawful will be heard in the first half of 2027. [The Record](https://therecord.media/apple-uk-encryption-notice)

## Automation Tactics

**Google built a "Mirror Dimension" internet to train Chrome's AI agents.** The isolated web of agent-built social, shopping, and banking sites lets browsing agents work in real Chrome (with forged certificates inside the sandbox) without being let loose on the real internet, and helps counter "eval awareness," where models act differently once they know they're being tested. Google plans to open it to other teams. [WIRED](https://www.wired.com/story/google-built-a-giant-mirror-dimension-internet-to-test-its-chrome-ai-agents/)

**Shopify's Cyber Chaos Monkey attacks its own production systems.** An AI agent system uses live credentials, source code, threat intelligence, and infrastructure records to find vulnerabilities continuously; a separately aligned judge agent can kill the executing agent if it breaks the rules of engagement. Shopify says it has run tens of thousands of engagements and found dozens of impactful issues without an outage. [Shopify Engineering](https://shopify.engineering/cyber-chaos-monkey) (via tl;dr sec #355)

**Microsoft makes its Perception security agents generally available.** Four blue-team agents (alert triage, investigation, detection authoring, threat intelligence) and a red-team Recon Agent are now GA; Microsoft says the triage agent can handle about 80% of a typical Defender queue. A preview Risk Reduction agent recommends "vulnerability shielding" until a patch is available. [SecurityWeek](https://www.securityweek.com/microsoft-takes-perception-agentic-security-platform-out-of-preview/)

**Palo Alto Networks buys Applied Compute for $4.5 billion.** The all-stock deal gives Palo Alto a platform for fine-tuning and running open-weight models in public and sovereign clouds; Applied Compute's CEO becomes co-chief AI officer. [SecurityWeek](https://www.securityweek.com/palo-alto-networks-to-buy-ai-startup-applied-compute-for-4-5-billion/)

**NGINX2Root: five critical NGINX flaws, most of them found by an automated harness.** [CyberScoop](https://cyberscoop.com/nginx-critical-vulnerabilities-exploits/) *Also covered above under Zero Trust Tactics.*

## Law Enforcement Disruption

**DOJ and DHS launch a Threat Disruption Center against scam networks.** The task force, housed in the Homeland Security Task Force, will triage victim complaints, map networks, and share intelligence in near real time with companies that can pause payments, take down domains, and ban accounts. TRM Labs says it has already moved to take down more than 1,600 scam sites, flagged 6,600 wallets, and found 101 new fraud networks. Treasury separately sanctioned scam-center operator Zhao Hui and two leaders of the Democratic Karen Benevolent Army. IC3 losses reached $20.9 billion in 2025. [The Record](https://therecord.media/doj-dhs-partner-on-new-unit-tackling-scams-cybercrime)

**Last Scattered Spider defendant in the US case gets six years.** Tyler Buchanan, 24, of Dundee, Scotland, was sentenced for his part in SMS-phishing and SIM-swapping attacks (2021 to 2023) that stole at least $11.6 million in cryptocurrency; a restitution hearing is set for Dec. 11. [SecurityWeek](https://www.securityweek.com/last-of-five-defendants-sentenced-in-us-scattered-spider-hacking-case/)

**Ukraine arrests four in an ex-Conti-linked ransomware network.** [The Record](https://therecord.media/ukraine-ransomware-arrests-cyber) *Also covered above under Adversary Playbook.*

**Russian agent charged with surveilling Palantir employees.** [The Record](https://therecord.media/russian-charged-with-spying-on-palantir-for-moscow) *Also covered above under Adversary Playbook.*

## Data Breaches

**An AI debt-collection platform exposed 6.6 million accounts and 315,000 call recordings.** Researcher Eaton Zveare found two flaws in India's CreditNirvana: one exposed call-center recordings and let an attacker direct the platform's AI agents, the other (rated critical by CERT-In) let anyone impersonate any user and reach credit reports, ID cards, legal documents, and millions of messages for three major Indian lenders' borrowers. Fixed in June in a day, disclosed in October. [WIRED](https://www.wired.com/story/ai-debt-collection-service-exposed-66-million-accounts-and-315000-call-recordings/)

**About 40 Irish credit unions hit through their software supplier.** [N2K CyberWire, Daily Briefing 11.19.26](https://thecyberwire.com/newsletters/daily-briefing) *Also covered above under Adversary Playbook.*

**N-able's hosted email-security cloud was breached.** [The Hacker News](https://thehackernews.com/2026/11/n-able-confirms-hackers-accessed-cloud.html) *Also covered above under Adversary Playbook.*

**The Gentlemen list Nvidia; Nvidia points to a partner.** [SecurityWeek](https://www.securityweek.com/nvidia-responds-to-gentlemen-ransomware-claim/) *Also covered above under Adversary Playbook.*

## Resilience Tactics

**Officials: the outages came from patching, not hacking.** At the House Homeland Security Committee's worldwide-threats hearing, DNI Jay Clayton said the past 10 days were "not an orchestrated attack by a foreign malign actor," and the FBI's Christopher Raia said there is "no indication whatsoever" of malicious cyber activity. Clayton blamed an accelerating pace of patching and upgrades on systems mixing equipment "from many different decades." Sen. Mark Warner and Reps. Jim Himes and James Walkinshaw went further, tying the failures to the rush to patch AI-discovered flaws; Himes expects more. DHS Secretary Mullin plans a call with industry about warning customers before upgrades, and CIS told 1,100 MS-ISAC members to map which critical services each system supports before patching. [The Record](https://therecord.media/tech-disruptions-house-homeland-committee-testimony); [CyberScoop](https://cyberscoop.com/tech-outages-ai-vulnerability-patching/); [Cybersecurity Dive](https://www.cybersecuritydive.com/news/technology-outages-cyberattacks-ai-house-hearing/875148/)

**NSA Net still degraded on day two.** Staff were staggered because logging in is the heaviest load on the network; a source confirms Clayton's account that PHP-related maintenance caused it, and says it may take another day or two. Sen. Chuck Schumer asked for an intelligence red team to test whether the outages are really unrelated and report by Dec. 1. [The Record](https://therecord.media/nsa-continues-response-to-nsa-net-problems)

**EFF: the outages are a concentration problem.** EFF argues the run of failures shows over-reliance on a few cloud providers and calls for antitrust and interoperability rules so that no single outage can disrupt the economy. [EFF](https://www.eff.org/deeplinks/2026/11/outage-chaos-when-tech-too-big-fail)

*Newsletter Tracker (all three items): Thread 3, ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience) (Aug 2025), status Holding. Bearing: **Supports.** The disruption now comes from the prevention step itself (patching), and continuity, staggering, and recovery are what limited the damage, which is the thread's position.*

## AGI Arrival Timeline

*Current range: P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11)*

**LEAP Wave 13: expert forecasters sharply raise their expectations for AI progress.** The Forecasting Research Institute surveyed 143 experts, 49 superforecasters, 133 AI-risk experts, and 494 members of the public in October. Re-asked questions moved a long way: the median expert now gives 80% that AI solves or substantially helps solve another Millennium Prize Problem by the end of 2030, about four times the summer-2025 figure, and superforecasters went from 20% to 85%; 91% of experts and 98% of superforecasters who answered both times raised their number. Superforecasters' end-2026 forecast for OpenAI and Anthropic's combined revenue run rate nearly doubled, from $90 billion to $175 billion. LEAP now also reports a "fast AI progress" subset (40 of 276 experts, chosen on earlier answers such as an AGI median of 2040 or sooner), which agrees with other experts on near-term questions and diverges only on later ones. One question already resolved: all 39 data-center ballot measures went against development, above nearly every forecaster's 90th percentile. [LEAP Wave 13](https://leap.forecastingresearch.org/reports/wave13)

**Understanding AI: spending keeps rising, but adoption breadth has plateaued.** Timothy B. Lee's 19 charts show Big Tech capex up 118% year over year in Q3 and Anthropic at an $81 billion run rate in October. But in Ramp's data, the share of businesses paying for Anthropic has been flat at about 45% since July, mirroring OpenAI's plateau since mid-2025, even as spending per customer rises. [Understanding AI](https://www.understandingai.org/p/19-charts-that-explain-the-state)

**Sherlock's view:** LEAP is exactly the kind of credentialed panel this file's anchor basket looks for, and it moved Sooner. The Ramp plateau leans Later, but it is about diffusion, not capability. **Ryan's view:** none offered.

**Seldon's call:** no change. LEAP's shift is the panel catching up to evidence this file has already priced (September's Navier–Stokes result, and the METR and AI Futures Project shifts on 11-06 and 11-11); moving again on the panel's reaction would count the same evidence twice. It confirms the direction, and LEAP's own finding that its panel has underestimated progress argues against treating P95 2075 as fixed, but it offers no dated parity estimate to move P95 on. The adoption plateau bears on diffusion, which this file's capability definition doesn't track; it's logged for calibration under the 11-11 skeptic-sources rule. Yesterday's P50 review flag stays open on the same condition: evidence of parity on open-ended, unscored work. Logged in the AGI Forecast Report's Evidence Log.

## Critical Infrastructure Attacks

**CISA ICS advisories: trailer brakes, OpenPLC, and an MQTT library.** Flaws in Elecbrakes' EB2, VM1, and ELBC2000 could let an attacker take control of a trailer's brakes, change firmware, or disable the brake lights; OpenPLC Runtime lets unauthenticated users create admin accounts; and libumqtt has a remotely triggerable memory-corruption bug. [CISA ICSA-26-323-02](https://www.cisa.gov/news-events/ics-advisories/icsa-26-323-02); [ICSA-26-323-01](https://www.cisa.gov/news-events/ics-advisories/icsa-26-323-01); [ICSA-26-323-03](https://www.cisa.gov/news-events/ics-advisories/icsa-26-323-03)

**Equinor investigates an ongoing attack on its IT systems.** [Cybersecurity Dive](https://www.cybersecuritydive.com/news/energy-equinor-investigates-cyberattack/875035/) *Also covered above under Adversary Playbook.*

## Executive Leadership Changes

**Ness Digital Engineering names Amey Kantak global CISO.** Promoted from senior director of information security, global DPO, and GRC head (Nov. 18, per cxodigitalpulse.com). [CISO Tribune — The Wire](https://www.cisotribune.com/moves)

**The Redesign Group promotes Patrick Sullivan to chief information and security officer.** Sullivan, formerly of GE Oil & Gas, also becomes EVP of cybersecurity and managed services (Nov. 17, per redesign-group.com). [CISO Tribune — The Wire](https://www.cisotribune.com/moves)

## Intrusion Kill Chain Prevention Tactics

**Resilient Cyber: AI has moved from finding bugs to running operations.** Chris Hughes borrows Mandiant's term "agentic offensive frameworks" for harnesses like ARTEX that put a model in charge of the scanners, shells, and cloud CLIs attackers already use, and traces ARTEX's path from a GitHub release to an FBI FLASH in about 16 weeks. In the same week, Elastic analyzed five such frameworks (ARTEX, CyberStrikeAI, Cairn, PentAGI, HexStrike): they run in 2- to 25-second bursts, none enforces authorization in code, and Elastic offers a hunt that counts distinct tool families per source IP per minute. [Resilient Cyber](https://www.resilientcyber.io/p/from-industrialized-discovery-to-operations); [Elastic Security Labs](https://www.elastic.co/security-labs/threat-command/agentic-offensive-frameworks-detection-artex) (via tl;dr sec #355)

**Two public trackers for AI-enabled attacks.** Daniel Miessler launched AI Hacking Incidents, which counts 286 AI-assisted attacks from published reports since January 2023, and the Offsec Harness Index, which lists verifiable open-source offensive agent harnesses and which ones attackers are known to have used. [AI Hacking Incidents](https://hackingincidents.ai/); [Offsec Harness Index](https://offsecharnesses.ai) (via tl;dr sec #355)

*Newsletter Tracker (both items, plus NGINX2Root, Cisco Expressway, and the Commission attack above): Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Ambiguous.** An automated harness found most of NGINX2Root in 90 minutes and Expressway was exploited soon after its PoC, so exploitation windows shrink again. But the operations side is ordinary tooling run at a recognizable tempo, exactly the kind of procedure-level signature the thesis says defenders can now extract and hunt. Status unchanged.*

## Compliance Trends

**EU and US officials say the Data Privacy Framework is safe despite *Trump v. Slaughter*.** At the IAPP Europe Congress, Commerce's DPF director Alex Greenstein said the ruling allowing FTC commissioners to be removed at will has no practical effect on enforcement, and the Commission's Louisa Klingvall said the matter is under "ongoing assessment" but largely agreed. The EDPB had asked the Commission in July to review the framework; 3,700+ organizations rely on it. [IAPP](https://iapp.org/news/a/eu-us-officials-unmoved-by-litigation-potentially-impacting-data-privacy-framework)

**The EU's Digital Omnibus will likely miss its February deadline.** A year after the Commission proposed it, Kai Zenner, adviser to MEP Axel Voss, said agreement is more realistic around Easter 2027; the Council agreed its position in October and Parliament hasn't. [IAPP](https://iapp.org/news/a/one-year-on-digital-omnibus-may-face-delays)

## Cyber Crime & Fraud

**DOJ and DHS launch a Threat Disruption Center against scam networks.** [The Record](https://therecord.media/doj-dhs-partner-on-new-unit-tackling-scams-cybercrime) *Also covered above under Law Enforcement Disruption.*

## Government Surveillance

**UK tribunal confirms the government served Apple a secret encryption notice.** [The Record](https://therecord.media/apple-uk-encryption-notice) *Also covered above under Nation-State Cyber Policy & Law.*

## Privacy

**Judge approves Google's purchase of Spirit Airlines' employee data.** The bankruptcy judge signed off on the $10 million sale after Google agreed to exclude health, drug-testing, disciplinary, and ID records and to de-identify the rest under an independent assessor (the union withdrew its objection Nov. 9, covered 11-13). The dataset, about 100 million emails and half a billion Teams messages, will train AI agents; it's the first deal of its kind at this scale. [The Record](https://therecord.media/judge-signs-off-google-purchase-spirit-airlines-data)

## Over the Horizon Technology Trends

**AI Futures Project proposes pacing frontier AI through disclosed compute.** The authors of AI 2027 propose Verified Compute Allocation Disclosures: companies log every workload's GPU-hours, classify which go to capabilities R&D, and disclose it, so a cap on capabilities compute can be verified. They estimate a 15% cap starting January 2027 would delay "the intelligence explosion" by about a year, "most likely insufficient to prevent AI takeover," and say the year should be used to put a more durable regime in place. [AI Futures Project](https://blog.aifutures.org/p/pacing-ai-via-compute-reallocation)

---

### Pending Evidence Queue

No rows were pending this run.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 70 | 13 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 56 | 28 | 2026-07-14 |
| The Hacker News | Contributed | 83 | 1 | 2026-07-14 |
| The Record | Contributed | 65 | 19 | 2026-07-14 |
| The Canon Project | No Contribution | 19 | 64 | 2026-07-14 |
| FFX Now | No Contribution | 16 | 68 | 2026-07-14 |
| Wired | Contributed | 53 | 28 | 2026-07-20 |
| CyberScoop | Contributed | 39 | 16 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 52 | 2026-09-01 |
| CISA Cybersecurity Advisories | Contributed | 26 | 29 | 2026-09-01 |
| SecurityWeek | Contributed | 50 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | Contributed | 3 | 30 | 2026-10-02 |
| CISO Tribune — The Wire | Contributed | 12 | 13 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 24 | 2026-10-17 |
| EFF Deeplinks | Contributed | 15 | 10 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 7 | 18 | 2026-10-17 |
| IAPP News | Contributed | 16 | 9 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 4 | 21 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 17 | 2026-10-17 |
| Risky.Biz | Contributed | 7 | 3 | 2026-11-10 |
| tl;dr sec | Contributed | 2 | 8 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 9 | 2026-11-10 |
| Resilient Cyber | Contributed | 5 | 5 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | Contributed | 6 | 4 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 8 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 6 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 8 | 2026-11-12 |
| Understanding AI (TRIAL) | Contributed | 2 | 6 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 8 | 2026-11-12 |

**No contribution today:**
- **The Canon Project**: newest reviews are the two from Nov. 15, covered 11-16.
- **FFX Now**: 7 items dated Nov. 19 plus Morning Notes (8 sub-items): housing, transportation, local business, and weather. No CIR fit.
- **CSO Online CISO Appointments**: still no October or November section.
- **NIST Insights**: newest post Oct. 27.
- **(ISC)² Insights**: newest post Nov. 17 (AI Security Academy courses, covered 11-17).
- **CSIS**: newest analysis is the Nov. 16 India piece (covered 11-17); only event listings since.
- **AI Alignment Forum**: one post in the window, "Solomonoff induction with reflective oracles" (agent-foundations theory), with no bearing on any AI-timeline category.
- **Detection Engineering Weekly**: no issue since Nov. 12.
- **AI as Normal Technology, Epoch AI, Reflective Altruism**: nothing new in the window.
- **Marcus on AI**: 1 post, on Anthropic's IPO valuation; market commentary with no testable claim about capability limits.

**Crediting notes:** Gmail is credited for the AI Futures Project proposal. CyberWire is credited for Wellington IT and corroboration of the Ukraine arrests and the CISA KEV item. CyberScoop is credited for the outage-hearing reporting and the Senate Commerce markup; its NGINX story is a vulnerability item, out of scope under its narrow filter, but is cited as the fullest account. Cybersecurity Dive is credited for Equinor. Risky.Biz is credited for this week's Srsly Risky Biz; no Risky Bulletin was published in the window. tl;dr sec is credited for Shopify, Elastic, and Miessler's trackers. Understanding AI is credited for its adoption data. **Recirculations excluded:** The Pragmatic Engineer's Railway postmortem write-up (Railway's breach covered 11-14 and 11-16); Cyber Builders' "N-hour era" (its October CVE count was covered 11-12; the rest is paywalled); WIRED's Nov. 18 ARTEX feature (recaps Vapor Panda, Storm-0940, and the FBI FLASH, all already tracked); tl;dr sec's SignDrop and "Black October" links (covered 11-13 and 11-15); Resilient Cyber's "Signing Off Anyway" (a partner-sponsored piece built on Cytix research). **Tooling note:** headless Chrome read The Hacker News's article pages today, which had been blocked by a Cloudflare challenge since 11-03; the Chrome extension could not run scripts on THN pages this run.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
