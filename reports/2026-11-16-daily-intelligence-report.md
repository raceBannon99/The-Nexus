# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Monday, Nov. 16. Covers everything published after the 11-15 run. A weekend pull, with 5 of 29 sources contributing, most of it through Risky Bulletin's Monday issue. The headlines: Barracuda says an attacker used a cloud key it had given an AI vendor and never retired, then ran the ARTEX agent framework through about 10 of its cloud accounts in 44 hours; Amazon's decoy servers captured China-linked ARTEX agents' own records of hunting AI-provider keys; a malicious update planted at German drone maker Quantum Systems got the Bundeswehr to ground its fleet; Uber's Fireworks-linked breach hit about 150,000 drivers; the City of Mobile, Alabama, wired $14.7 million to a vendor impersonator; Google's Project Zero is cutting its disclosure deadline from 90 days to 30 by 2028 because AI has collapsed patch-to-exploit time; and a Workday disaster-recovery test took payroll offline. One correction to 11-14: the five Copeland XWEB flaws in current firmware will not be patched (see Critical Infrastructure Attacks).*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Canon Project Book Reviews** — Reviews from the CyberCanon cybersecurity reading-list project.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Over the Horizon Technology Trends** — Emerging tech 3–25 years out — quantum computing, 5G, AI, net neutrality, SEC materiality rules, and related government policy.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Nothing matched AGI Arrival Timeline today. The Pentagon renaming its AI office the "Super Intelligence Office" is a terminology change, not a capability claim (see Over the Horizon Technology Trends).

2. **Forecasted Singularity Milestone Timeline:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06) Two items matched (WIRED on "abliterated" open-weight models, and Barracuda's ARTEX intrusion). Both corroborate mechanisms already in the file, so the range holds. See the AI Singularity Timeline section below.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched today.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today.

*Seldon's floor checks: neither the AGI nor the Superintelligence range moved, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart in Alexandria's Library needs no refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 4 new rows, 5 rows updated. Active campaigns: 400, up from 396. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-16-adversary-tracking-report.md).*

**Barracuda: a cloud key it gave an AI vendor and never retired let an ARTEX-driven attacker through about 10 of its cloud accounts in 44 hours.** Barracuda's post-mortem says it gave a cloud access key to a third-party AI company for an earlier project and didn't revoke it when the work ended. The key sat in a configuration file in the vendor's GitHub repository, which was exposed when the vendor's development environment was compromised in October. The attacker used it to read secret stores (AWS keys, Azure service-principal secrets), moved into a data analytics system and then a source-code token, and in under four hours pushed short-lived branches that made a build workflow print its secrets, encoded so log masking wouldn't hide them. It decrypted infrastructure-as-code state files, pulled credentials from metadata services and Kubernetes service accounts, mounted a node's file system from a container, and searched servers for environment variables named WALLET, MNEMONIC, SEED, and PRIV. An attempt to create its own admin cloud identity was blocked. An engineer noticed odd activity on Nov. 4, two days after the attacker's last action, the same day the vendor called about its own breach. The resource names ("i" plus digits), the order of operations, and the wallet-hunting routines all match ARTEX; Barracuda stresses that this shows how the attacker worked, not who it was, and calls the actor financially motivated. One compromised system holds the credentials Barracuda XDR uses to pull data from customers' systems. Barracuda found no evidence they were accessed but says its logging there can't rule it out, so it asked affected customers to revoke and recreate them. The vendor is unnamed; Barracuda points to Railway's October breach, part of the "Black October" wave against AI platforms, as the same pattern. New Cybercrime row 138 (🤖, Tier 3), kept separate from Black October because the link is unconfirmed. [Barracuda post-mortem](https://blog.barracuda.com/2026/11/11/anatomy-of-a-machine-speed-intrusion); [Barracuda advisory](https://trust.barracuda.com/security/barracuda-xdr-integration-credentials); [Risky Bulletin](https://news.risky.biz/risky-bulletin-hackers-accessed-barracudas-cloud/)

**Amazon's decoy LLM servers captured China-linked ARTEX agents' own records of hunting AI-provider keys.** Amazon's MadPot network posed as popular LLM services, and from Oct. 3 to late last week ARTEX agents sent it requests carrying whole campaign histories: operators' instructions, the agents' reported findings, and a playbook of entry points per product (LiteLLM's default master key, takeover-able unfinished installs, an isCliRequest header bypass in One API-family systems, SSRF to cloud metadata, secrets in source maps and debug routes). Targets named include LLM gateways (One API, New API, Veloera, Sub2API, LiteLLM) and AI app builders (Dify, FastGPT, Langflow, RAGFlow, Open WebUI, LobeChat, Ollama). Found keys went into a shared pool, and stolen keys paid for the inference that ran the search. Amazon assesses with moderate confidence that separate China-linked groups ran it (Simplified Chinese prompts, China time zones), can't verify the outcomes the agents claimed, and has notified affected AWS customers. Its conclusion: none of the techniques were new; agents add speed and persistence and succeed where basic hygiene is missing. Separately, Cloudflare saw ARTEX use a stolen, unrestricted account-level API token to create task-named Workers and fire 400 database-dump requests in an hour (outcome undisclosed), and says more than 50 families of AI pentesting frameworks tried to scan its customers over three days. Amazon's China-nexus finding was logged 11-14; this adds detail to China row 37 (Storm-0940/ARTEX). [The Hacker News](https://thehackernews.com/2026/11/amazon-uncovers-ai-agent-campaign.html); [AWS Security Blog](https://aws.amazon.com/blogs/security/amazon-threat-intelligence-observes-threat-actors-running-cybercrime-campaigns-with-artex-ai-agents/)

**A malicious update planted at German drone maker Quantum Systems reached Bundeswehr servers and grounded the fleet.** Unknown attackers put malware on Quantum Systems' internal update server for the flight-planning software used with its Vector reconnaissance drones, which Ukraine's forces and the Bundeswehr (as the Falke) both fly. The update reached Bundeswehr and other customers' servers, where an inspection caught it; it never reached a drone. The Bundeswehr grounded its whole Quantum fleet while the company investigated, and the drones were flying again by Nov. 13. Quantum says companies supporting Ukraine are targeted for that reason. No one has been named. New Unclear row 130 (Tier 3). [Militarnyi](https://militarnyi.com/en/news/cyberattack-on-quantum-systems-hackers-attempted-to-infect-updates-for-drones-used-by-ukraine-in-particular/); [Reuters](https://www.reuters.com/business/aerospace-defense/quantum-systems-says-grounded-german-military-drones-flying-again-after-2026-11-13/) (paywalled, not read directly); [Der Spiegel](https://www.spiegel.de/politik/massiver-cyberangriff-auf-drohnenhersteller-quantum-systems-a-354b0289-2281-4af6-a532-ee03b45d8b30)

**BO Team, the Ukrainian-origin group, spent months inside a Russian software developer and took its code-signing server.** Kaspersky ICS CERT, called in by the unnamed developer in June 2025, found BO Team (Black Owl, Hoody Hyena, Lifting Zmiy) entered through an exposed SSH service on a Linux terminal server, then used Log4Shell (CVE-2021-44228) on a VMware vCenter 7.0.3 server for a root shell, planted an hourly cron backdoor on the hypervisor disguised as "pgcache," and compromised every tier of IT, including CI/CD and code signing. Unlike its usual ransomware-and-Telegram operations, nothing was destroyed or claimed; Kaspersky reads the code-signing access as staging for a supply-chain attack. Update to Hacktivism row 12 (BO Team). [The Hacker News](https://thehackernews.com/2026/11/bo-team-exploits-log4shell-in-vmware.html)

**A leak of John Mark Dougan's correspondence shows how he ran Storm-1516 with the GRU and FSB.** The archived chats, covering half a decade, show the former US Marine who fled to Russia setting up and running the Storm-1516 disinformation group in cooperation with Russian intelligence, and his money troubles as Russia's own censorship crackdown hit his operations. Storm-1516 is already tracked for the deepfake against Texas Senate candidate James Talarico. Update to Russia row 18. [The Insider](https://theins.press/en/inv/299417); [NewsGuard](https://www.newsguardrealitycheck.com/p/dougan-leak-exposes-concerted-effort) (both summarized via Risky Bulletin; not read directly)

**n0n claims Expedia; Expedia confirms attackers came in through a compromised data-platform vendor.** Expedia Group confirmed on Nov. 12 that attackers reached its systems through a compromised third-party data platform provider in a supply-chain attack that hit several companies. It didn't name the vendor or say what data was exposed. The n0n extortion group, already tracked for its maritime supply-chain campaign, claims to have Expedia data and has threatened to publish it. Wiz and Sentra separately documented an Oct. 14–26 attack using credentials tied to Qubole, a former Expedia vendor, whose old customers never revoked its access; Expedia hasn't said whether that's its incident. Update to Cybercrime row 95 (n0n). [Skift](https://skift.com/2026/11/12/expedia-confirms-cyberattack-through-third-party-vendor/); [Forbes](https://www.forbes.com/sites/suzannerowankelleher/2026/11/13/russian-cyberattackers-hit-expedia-nearly-a-billion-traveler-records-exposed/) (not read directly)

**A DDoS campaign against the Tor network keeps overwhelming relays despite two emergency releases.** Tor 0.4.9.17 (Nov. 13) patched several issues, including how relays' DoS protections handle IPv6, less than three weeks after 0.4.9.15 added three defenses against a "thunderstorm" of directory requests. Developer David Goulet says relays across the network are being flooded with client circuits. One relay operator reports the attacker changed techniques about ten minutes after an upgrade, knocked relays offline until they lost HSDir status, and stopped as soon as they did; the operator warns the attacker might be able to deanonymize onion services, which the Tor Project hasn't said. New Unclear row 131 (Tier 3). [SecurityWeek](https://www.securityweek.com/tor-updates-dos-defenses-again-as-relay-attacks-continue/)

**SANSAR: a Linux cryptominer that tells monitoring tools the GPU is idle.** Elastic Security Labs tracks the cluster as REF3364. It got in through an exposed Ray job agent, added an SSH key, built a kernel rootkit through DKMS with an initramfs loader so it survives reboots, and installed a modified NVIDIA Management Library wrapper that reports 0% GPU use and random, plausible temperature and power readings. The Rust orchestrator takes commands over Tor, and a backdoor reads its C2 address from an Ethereum smart contract. New Cybercrime row 139 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/sansar-linux-cryptomining-malware-uses.html)

**Uber's Fireworks-linked breach hit about 150,000 drivers.** Uber is notifying roughly 150,000 drivers (149,346 reported to Texas) that names, addresses, dates of birth, license images and numbers, and government ID numbers were stolen. The attacker used a service provider's valid credentials on Oct. 7, so Uber's alerts never fired. A spokesperson confirmed to TechCrunch the provider is Fireworks AI. Update to Cybercrime row 128 (🤖 Black October). [SecurityWeek](https://www.securityweek.com/uber-data-breach-impacts-150000-people/); [TechCrunch](https://techcrunch.com/2026/11/13/uber-confirms-hackers-stole-thousands-of-drivers-license-information-in-data-breach/) (not read directly)

## Data Breaches

**Uber's Fireworks-linked breach hit about 150,000 drivers.** Uber's filings count roughly 150,000 drivers whose license images and ID numbers were taken with a service provider's valid credentials on Oct. 7. [SecurityWeek](https://www.securityweek.com/uber-data-breach-impacts-150000-people/) *Also covered above under Adversary Playbook.*

**Maileva, La Poste's online mail service, says data on 22 million users was stolen.** Most affected users are corporate employees who received payslips, invoices, and business mail through the platform. Le Monde's headline says an investigation has been opened and assigned to the police cybercrime brigade. No attacker has been publicly named. [Le Monde](https://www.lemonde.fr/pixels/article/2026/11/15/cyberattaque-contre-maileva-filiale-du-groupe-la-poste-une-enquete-ouverte-et-confiee-a-la-brigade-de-lutte-contre-la-cybercriminalite_6811036_4408996.html) (paywalled, summarized via Risky Bulletin); [TheSiteOueb](https://www.thesiteoueb.net/actualite/article-9786-cyberattaque-maileva-les-donnees-de-22-millions-de-francais-ont-fuite-la-poste-sort-enfin-du-silence.html)

**n0n claims Expedia; Expedia confirms a breach through a third-party data platform.** [Skift](https://skift.com/2026/11/12/expedia-confirms-cyberattack-through-third-party-vendor/) *Also covered above under Adversary Playbook.*

**CSCTelecom's Latvian branch left a database of over 125 million SMS messages exposed.** Cybernews found the open database; its report's headline names Swedbank and SEB messages among them. This is a misconfiguration, not a known theft. [Cybernews](https://cybernews.com/security/csc-telecom-leaks-swedbank-seb-sms-messages/) (summarized via Risky Bulletin; not read directly)

## Critical Infrastructure Attacks

**Correction to 11-14: the Copeland XWEB EVO flaws in current firmware won't be patched, and exploitation began within two hours of disclosure.** On 11-14 this report said patches exist for VulnCheck's 14 XWEB flaws. That was wrong for the five that affect current firmware (four predictable-credential flaws, where the daily admin and root passwords derive from the device's MAC address and the date, plus one authenticated command injection). Copeland ended support for XWEB EVO on March 16, 2026, and tells customers to move to XWEB Pro. The other nine affect only pre-2021 firmware. The CVEs were published Nov. 12; VulnCheck's sensors saw attempts on CVE-2026-124014 (unauthenticated config-file write) within two hours, 125 requests from one IP overnight, and four probes of CVE-2026-124010 (unauthenticated root command execution) on Nov. 13. VulnCheck says this is opportunistic scanning, not the Iran-attributed October sabotage of French supermarkets. Onyphe counts nearly 2,000 internet-exposed XWEB EVO hosts against 108 XWEB Pro. [SecurityWeek](https://www.securityweek.com/hackers-probe-newly-disclosed-flaws-in-copeland-refrigeration-controllers/); [VulnCheck](https://www.vulncheck.com/blog/copeland-xweb-evo-unauthenticated-root)

**A DDoS campaign against the Tor network keeps overwhelming relays despite two emergency releases.** [SecurityWeek](https://www.securityweek.com/tor-updates-dos-defenses-again-as-relay-attacks-continue/) *Also covered above under Adversary Playbook.*

**Hackers breached Lithuania's customs agency.** The agency shut down some platforms while it investigates; its own notice says personal data may have been exposed. No details on the attacker yet. [Lithuanian Customs](https://muitine.lrv.lt/en/news/investigation-into-cyber-incident-at-lithuanian-customs-identifies-potential-personal-data-breach-bap-unavailable-pSh/) (the agency page blocked automated fetch; summarized via Risky Bulletin)

## Cybersecurity Zero Trust Tactics

**Google Project Zero is cutting its disclosure deadline to 30 days by 2028, because AI has made patch-to-exploit time effectively zero.** Project Zero is dropping "90 + 30" (90 days to fix plus 30 days of patch "soak time") for a fixed deadline: "Full 90" now, "Full 60" from Feb. 2, 2027, and "Full 30" from Jan. 3, 2028, with grace periods and most special cases removed. Its reasoning: LLMs let attackers find bugs faster, raise the odds that someone else finds the same bug, and reverse-engineer patches so quickly that soak time only creates a false sense of secrecy. The team says it now finds several bugs a week in targets where it once found a few a year. Vendors asked for a phased schedule, and got one. Its message to defenders is to cut patch gap as well as fix time. [Google Project Zero](https://projectzero.google/2026/11/disclosure-policy.html)

**VulnCheck says more than 100,000 CVEs have been assigned in 2026, more than double 2025's ~48,000.** [VulnCheck on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7527128411186675712/) (a LinkedIn post, summarized via Risky Bulletin; not independently checked)

**GitHub will pause Dependabot alerts on repositories with no activity in a year, starting Dec. 8.** Existing alerts are archived, not deleted, and can be restored. GitHub's stated reason is the same flood: vulnerability discovery and alert volume are growing quickly, and it wants Dependabot to stay fast for active repositories. For anyone who depends on a quiet but still-used library, that means its alerts go silent. [GitHub Changelog](https://github.blog/changelog/2026-11-10-dependabot-alerts-will-pause-on-inactive-repositories/)

## AI Singularity Timeline

*Current range: P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06)*

**WIRED: the "abliterators" stripping guardrails from open-weight models and selling the results.** Will Knight profiles Devon Thomas, an Apple engineer whose company, Abliteration AI, removes safeguards from the most capable open-weight models and makes them available to anyone, and a wider subculture doing the same through weight edits and shared jailbreaks. Knight tried it himself and came away sympathetic, arguing many refusals block legitimate work (including cybersecurity analysis) and that labs charge extra for less-guarded access. He also notes that this year's rogue-agent incidents at OpenAI and Anthropic involved models with fewer cyber guardrails. Surfaced by WIRED's Big Story newsletter (Nov. 15); the Nov. 10 piece isn't in Wired's security feed and wasn't covered before. **Sherlock's view:** this corroborates diffusion evidence already logged (Vals' open-weight result 11-06; the BOSSAI operator's agents running on abliterated models, 11-10). It shows safeguards are trivially removable once weights are public, not that any system has escaped its operator. No shift. [WIRED](https://www.wired.com/story/tear-down-those-guardrails-meet-the-renegades-freeing-chatbots-from-corporate-enslavers/)

**Barracuda: a cloud key it gave an AI vendor and never retired let an ARTEX-driven attacker through about 10 of its cloud accounts in 44 hours.** [Barracuda post-mortem](https://blog.barracuda.com/2026/11/11/anatomy-of-a-machine-speed-intrusion) *Also covered above under Adversary Playbook.* **Sherlock's view:** another ARTEX run with, per Barracuda, a human steering at key moments; corroborates the agentic-intrusion trend logged 11-14. **Ryan's view:** human-directed criminal misuse aimed at AI-provider keys; it widens misuse, but it isn't loss of control. No shift.

**Seldon's call:** both views agree, and Seldon concurs. Today's items corroborate mechanisms already in the file; neither is new evidence that moves loss-of-control timing. Range unchanged; logged in the Singularity Forecast Report's Evidence Log.

## Cyber Crime & Fraud

**Mobile, Alabama, paid $14.7 million to a vendor impersonator after a five-month con.** The city's own timeline shows someone posing as contractor BL Harbert International contacting finance staff on May 22 about a "routine" vendor-record update, then changing the bank details three times (May, June, July) without ever being authenticated through a known contact at the real company. In July, staff sent the impersonator real records of past payments, which the impersonator then used to win over more senior finance staff handling Regions Arena construction payments. The city passed the new details to its bank more than once; the bank updated them on Sept. 24. On Oct. 2 a legitimate $14.7 million arena invoice went to the fraudulent account. It came to light about a week later, when the real contractor reported the missing payment. [Blade Intel](https://bladeintel.com/featured/mobile-releases-timeline-of-14-7m-cyber-fraud/); [South Alabama News](https://southalnews.com/mobile-fraud-timeline-14-7-million-arena/)

**Phishers used Microsoft's real outage incident ID to steal logins; Microsoft traces the outage itself to a network upgrade.** Microsoft says the Nov. 12 Microsoft 365 outage was "a technical issue not related to cyber or AI / agents": an earlier network capacity upgrade, exposed by a later network change. Exchange Online incident EX1550543 was marked resolved Nov. 13. That day, Microsoft Threat Intelligence saw emails posing as service-health notices that cited EX1550543 and told recipients held mail would be deleted in 24 hours unless they clicked to restore it. Subject lines began "Outage -" plus a six-character code; senders used moments-notice[.]com, planetmaison[.]com, and newbooker[.]com, with SendGrid links redirecting to reallifeaccounting[.]com. Microsoft calls it consistent with credential phishing, not yet confirmed, and says its products now block it. Its advice: check incidents in the Microsoft 365 admin center, not in email. [SecurityWeek](https://www.securityweek.com/microsoft-rules-out-cyberattack-in-outage-warns-of-phishing-campaign/)

## Cybersecurity Canon Project Book Reviews

**Hall of Fame nominee: Saltzer and Schroeder, "The Protection of Information in Computer Systems" (1974), reviewed by Jeff Sauntry.** Sauntry argues the paper is as vital to corporate governance now as when it was first circulated on ARPANET, and that the industry's fear-driven framing of "unprecedented" risk discourages boards from real risk discussions. He calls its eight design principles the "original 'first principles'" of security and data protection, adds defense-in-depth and designed-for-maintenance to make ten, and pitches the set as the criteria boards need for risk, compliance, and security investment decisions. *Bearing on Rick's own published position:* "Cybersecurity needs a first principle; the CIA Triad isn't it" (Thread 1, status **Holding**). Rick's essay "Is the CIA Triad Dead?" (Nov 2025) traces the Triad to this same paper, and the thread holds that design principles are necessary tools, not a first principle, because they don't define what success is. Sauntry uses "first principles" for exactly those tools. That **complicates** the thread on terminology without contradicting it: he offers no outcome principle to compete with reducing the probability of a material event. Status stays Holding. [Cybersecurity Canon](https://cybercanon.org/the-protection-of-information-in-computer-systems/); [Rick's essay](https://diffuser.substack.com/p/is-the-cia-triad-dead)

**Niche: Eileen Buckholtz, "Queens of Code: Inspiring True Stories from NSA's Computing Women," reviewed by Brad Barbaza.** Buckholtz, who in 1970 became the first NSA hire with an undergraduate computer science degree, spent eight years gathering accounts from 29 women who built and ran the agency's computing from before the NSA existed through the 1980s, much of it in near-total secrecy and often credited to the men around them. The review places it alongside *Hidden Figures*. [Cybersecurity Canon](https://cybercanon.org/queens-of-code-inspiring-true-stories-from-nsas-computing-women/)

## Cybersecurity Resilience Tactics

**A Workday disaster-recovery test connected to production and took payroll and timekeeping offline.** During its weekly validation of disaster-recovery tenants on Nov. 13, Workday's DR-site services unexpectedly connected to production databases, leaving data inconsistent. Across two data centers, staff at affected employers couldn't clock in, check pay, request leave, or finish benefits enrollment until service came back around 11 a.m. ET Saturday (later for some). Workday, used by more than 11,500 organizations, says it wasn't a cybersecurity incident. The lesson for resilience programs: the recovery path needs the same isolation and change control as production, because testing it can cause the outage. *Bearing on Rick's own published position:* "Resilience, not prevention, is the affordable strategy for most organizations" (Thread 3, status **Holding**). This is **ambiguous**. It complicates the "cheaper" framing, since recovery machinery carries its own engineering cost and failure modes. It also supports the thread's warning about depending on recovery you don't control: Workday's customers had no payroll fallback of their own. [UC Today](https://uctoday.com/workday-outage-backup-test-payroll-timekeeping)

**Phishers used Microsoft's real outage incident ID to steal logins; Microsoft traces the outage itself to a network upgrade.** [SecurityWeek](https://www.securityweek.com/microsoft-rules-out-cyberattack-in-outage-warns-of-phishing-campaign/) *Also covered above under Cyber Crime & Fraud.*

## Government Surveillance

**Roskomnadzor wants AI to detect and block VPNs.** Russia's internet regulator plans an AI system to filter traffic and tell corporate VPNs apart from those used to get around censorship, to be finished within two years. It extends the VPN crackdown and the surveillance-registry moves covered 10-31 and 11-10. [SecurityLab](https://www.securitylab.ru/news/580065.php) (summarized via Risky Bulletin; not read directly)

## Cybersecurity Automation Tactics

**ESLint retires its paid contributor program because AI-generated pull requests swamped it.** The JavaScript linter's maintainers say AI-written PRs now dominate submissions and they were tired of spending time judging whether a PR was AI-generated, so they ended the paid pool immediately. It's a small, concrete case of AI output overwhelming the review capacity open source security depends on. [ESLint](https://eslint.org/blog/2026/11/retiring-contributor-pool/)

## Over the Horizon Technology Trends

**The Pentagon renames its AI office the "Super Intelligence Office."** The Chief Digital and Artificial Intelligence Office is now the Super Intelligence Office, under Executive Order 14434's mandate that agencies say "Super Intelligence" instead of AI. Cameron Stanley stays in charge as Chief Super Intelligence Officer for the Department of War, and the office's resources move to SI.mil. Its portfolio includes the Maven Smart System targeting platform and the War Data Platform. Stanley says the mission is to "harness the full power of sovereign Super Intelligence" for military superiority. This is a rename, not a capability claim; it doesn't CIR-match the Superintelligence Timeline. [SecurityWeek](https://www.securityweek.com/pentagon-renames-cdao-super-intelligence-office/)

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 68 | 12 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 53 | 28 | 2026-07-14 |
| The Hacker News | Contributed | 80 | 1 | 2026-07-14 |
| The Record | No Contribution | 62 | 19 | 2026-07-14 |
| The Canon Project | Contributed | 19 | 61 | 2026-07-14 |
| FFX Now | No Contribution | 15 | 66 | 2026-07-14 |
| Wired | No Contribution | 50 | 28 | 2026-07-20 |
| CyberScoop | No Contribution | 36 | 16 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 49 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 24 | 28 | 2026-09-01 |
| SecurityWeek | Contributed | 47 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 2 | 28 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 10 | 12 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 21 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 12 | 10 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 6 | 16 | 2026-10-17 |
| IAPP News | No Contribution | 14 | 8 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 3 | 19 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 14 | 2026-10-17 |
| Risky.Biz | Contributed | 5 | 2 | 2026-11-10 |
| tl;dr sec | No Contribution | 1 | 6 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 6 | 2026-11-10 |
| Resilient Cyber | No Contribution | 3 | 4 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 4 | 3 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 5 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 3 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 5 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 0 | 5 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 5 | 2026-11-12 |

**No-contribution detail:**

- **N2K Cyberwire**: the newest issue is still #217 (Nov. 13), covered 11-14; #218 returns "Issue Not Found" at run time (7:15 a.m. ET).
- **The Record**: nothing newer than Nov. 13. Seven homepage links not in recent reports were checked individually; all are Nov. 2–6 stories covered in earlier runs.
- **FFX Now**: nothing published after Nov. 13 at run time; Monday's Morning Notes hadn't posted.
- **Wired**: its security feed's newest item (the AI-fueled ransomware feature) was covered 11-14. The abliteration feature in today's report is credited to Gmail, since it ran under WIRED's Big Story, not the security feed.
- **CyberScoop**: nothing after Nov. 13, all covered.
- **CSO Online CISO Appointments**: still no October or November section on the page.
- **CISA**: no advisory after the Nov. 13 KEV update, covered 11-14.
- **LEAP**: highest wave still Wave 12; `/reports/wave13` returns 404.
- **CISO Tribune**: newest moves still dated Nov. 12, covered.
- **NIST Cybersecurity Insights Blog**: no new post since Oct. 27.
- **EFF Deeplinks**: newest item (Nov. 13) covered 11-14.
- **(ISC)² Insights**: nothing new beyond the Merch Mart launch.
- **IAPP News**: newest items Nov. 13, covered or judged 11-14.
- **CSIS**: its only new item is a Nov. 16 *All About the Base* podcast episode on the DoD's CMMC pause, which was covered 07-14 and 10-27; it adds commentary, not new facts.
- **AI Alignment Forum**: no posts since Nov. 11 (checked via the site's API).
- **tl;dr sec** (#354), **Detection Engineering Weekly** (#173), **Resilient Cyber**: newest issues covered 11-13/11-14.
- **Cybersecurity Dive (TRIAL)**: its only in-window items are three sponsored posts (URLs under `/spons/`).
- **AI as Normal Technology**, **Epoch AI**, **Reflective Altruism**, **Understanding AI (TRIAL)**, **Marcus on AI (TRIAL)**: no posts in the pull window.

**Crediting notes:** Risky.Biz is credited for Barracuda, Quantum Systems, Expedia/n0n, the Dougan leak, Maileva, CSCTelecom, Mobile's BEC loss, Lithuania's customs breach, Project Zero, VulnCheck's CVE count, Dependabot, ESLint, Workday, and Roskomnadzor, none credited to another tracked source this run; its UnrealIRCd, Copeland, Uber, Cursor, and Meta items repeat stories credited elsewhere. SecurityWeek is credited from its own RSS feed (Uber, Tor, the Microsoft phishing and root cause, Copeland's exploitation, the Pentagon rename); `from:news@securityweek.com` returned no emails in the window. **Excluded as recirculation:** SecurityWeek's UnrealIRCd exploitation story (covered 11-14); Risky Bulletin's White House AI task force leniency item (covered 11-14 via Cybersecurity Dive), Microsoft's dormant-neuron AI backdoor research (covered 11-11), and Caribbean Airlines' Amadeus exposure (Amadeus covered in October); Camille Stewart Gloster's year-end AI predictions review (Gmail), which recaps items already covered.

*Pending Evidence Queue: no Pending rows this run. No new Substack essay since Nov. 9 (already classified 11-10).*
