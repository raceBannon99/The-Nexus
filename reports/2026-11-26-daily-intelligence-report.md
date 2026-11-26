# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

## Summary

Date: Thursday, November 26th, 2026\
Source Contribution: 13 of 30 sources contributed\
The Headlines:

- None of the five AI timeline forecasts changed.
- Microsoft says China's Salt Typhoon and Crystal Typhoon have built the ARTEX AI hacking agent into their toolkits.
- 1Password disclosed a breach through an employee's GitHub account that exposed customer account data and source code, but not vaults.
- Attackers exploited Mitel MiCollab flaws before a patch existed, possibly with AI help, and CISA added ten exploited flaws to its catalog.
- A suspected ransomware attack forced Guadeloupe's main hospital to suspend surgeries and cancer treatment.
- OpenAI's chief scientist published the company's internal perplexity figures and proposed industry limits on development until AI monitoring catches up.
- Bridgewater says it is managing money on a one-in-three chance of an economically destabilizing cyberattack within the next year.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) One item matched today: Jakub Pachocki's post on OpenAI's internal perplexity figures. Range held; see the AGI Arrival Timeline section below for the Source and Effect lines.

2. **Forecasted Singularity Milestone Timeline:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17) Two items matched today: Apollo Research's report on labs handing AI R&D to their own agents, and Pachocki's warning that alignment auditing will degrade. Both lean Sooner but give no date; range held. See the AI Singularity Timeline section below.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. One item matched today (Pachocki on AI-driven pretraining research). Range held; see the Superintelligence Timeline section below.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today. Considered: Apollo's Handoff report and Pachocki's post (*Source:* see the AI Singularity Timeline section; Credentialed expert judgment. *Effect:* none, since both bear on whether and how soon control is lost, not on how soon harm follows once it is).

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. One item matched today, from the Pending Evidence Queue: WIRED's ten-expert panel, already weighed here on 11-12. Range held; see the Harm Probability section below.

*Seldon's floor checks: the AGI and Superintelligence ranges didn't move, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart doesn't need a refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 6 new rows and 6 rows updated. Active campaigns: 489, up from 483. China passed 50 rows and now renders as two table images. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-26-adversary-tracking-report.md).*

**Microsoft: China's Salt Typhoon and Crystal Typhoon now use ARTEX.** Microsoft says both state-backed groups have built the AI intrusion framework into their toolkits for "network reconnaissance, credential attacks, and web application exploitation," and that North Korean groups have adopted it too. ARTEX, released in July, lets operators set goals for AI agents and "can advance from reconnaissance to persistent, privileged access to a target organization in a matter of minutes." Microsoft says it uses no new techniques and doesn't hide by default, and that the durable signal is behavioral: "a wide variety of requests in a brief time" with retries "at machine speed," since operators change IPs and user agents to beat signatures. The Chinese researcher behind it pulled the source from GitHub last month, but forks circulate and at least one Chinese company sells access. New China row 51 (🤖, Tier 1). [The Record](https://therecord.media/microsoft-china-salt-typhoon-using-artex-ai-tool)

*Newsletter Tracker: Thread 4, ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead) (May 2026), status Holding. Bearing: **Supports.** Microsoft's own advice is the thread's premise: indicators are cheap for the attacker to change, but the procedure (machine-speed bursts and retries) is stable and detectable. Status unchanged.*

**1Password breached through an employee's GitHub account.** Starting Nov. 19, an attacker used a compromised corporate GitHub account to push malicious code to backend services, copy source code from private repositories, and reach the CI/CD system. Stolen customer records include names, emails, account IDs, public keys, authentication parameters (including Secure Remote Password verifiers), and tokens from invitation and recovery emails; a "small number" of users mid-recovery were notified individually. 1Password says vault contents, recovery keys, and the keys protecting vaults weren't touched, the verifiers can't be brute-forced without Secret Keys it doesn't store, and customers needn't act beyond watching for phishing. It rotated credentials, hardened GitHub and CI/CD, and lengthened email codes from six digits to ten characters. How the account was taken isn't known. New Unclear row 182 (Tier 3). [SecurityWeek](https://www.securityweek.com/1password-breach-exposes-customer-data-internal-source-code/); [The Hacker News](https://thehackernews.com/2026/11/1password-hacked-customer-data-and.html)

**Mitel MiCollab flaws were exploited before the patch, possibly with AI help.** Accenture's Apex Labs found a web shell on a victim's MiCollab server on Nov. 15, a day before Mitel's advisory for five unauthenticated flaws (two allow command execution). The attackers ran commands 12 minutes after their first request, had root within half an hour, and reached backup and database servers about 20 hours later, stealing business data. Their infrastructure talked to two commercial AI API services, and traffic resumed "at precisely the same second" as an authentication-bypass request, which Accenture reads as possible AI-assisted triage or extortion prep. A second victim's server had talked to the same infrastructure since Nov. 9. No group named; Accenture suspects extortion. CISA added all five flaws to KEV. New Unclear row 183 (Tier 3). [SecurityWeek](https://www.securityweek.com/mitel-micollab-zero-days-exploited-in-suspected-ai-assisted-attacks/)

**Suspected ransomware halts surgeries and cancer treatment at Guadeloupe's main hospital.** Outages began Saturday evening at the University Hospital of Guadeloupe, the largest on the French Caribbean island of about 380,000; databases were encrypted, staff are back to paper and couriers, radiation therapy is suspended, and chemotherapy and surgeries were canceled through at least Friday. France's ANSSI is investigating whether attackers came in through an IT supplier compromised months ago. No ransom demand has arrived and the hospital won't pay. Bordeaux University Hospital and France's National Cancer Institute disclosed separate attacks the same week. New Unclear row 184 (Tier 3). [The Record](https://therecord.media/guadeloupe-ransomware-hospital-cyber)

**FIFA confirms a breach claimed by the Handsome Boy Hacking Club.** FIFA says attackers reached "a limited set of personal and business information." The group, which surfaced last week, claimed 12-plus GB from FIFA's Microsoft environment, failed to extort it, and posted the data on a cybercrime forum (it says identity and immigration documents, financial, legal, and governance records). It follows attacks on LaLiga, Ajax, and the French Football Federation. New Cybercrime row 156 (Tier 3; the link rests on the group's own claim). [The Record](https://therecord.media/fifa-data-breach-limited)

**ShinyHunters claims a comeback; Inception denies any tie.** An Exploit-forum account linked to ShinyHunters since 2020 announced the group's return with a new leak site and PGP key; the original key reportedly leaked, so impostors can't be ruled out. Inception, whose leak site now lists AMD, PepsiCo, Lucid Motors, Henry Schein, and Cigna Healthcare (unverified), says Okta's evidence is only shared commodity services: "We are not ShinyHunters." Okta has found 21 confirmed and 41 likely phishing domains, including ones aimed at Anthropic, OpenAI, Amazon, Adobe, Netflix, Nintendo, and Tesla, with no sign those companies were breached. Updates to Cybercrime rows 20 (ShinyHunters, Tier 1) and 154 (INCEPTION, Tier 2). [SecurityWeek](https://www.securityweek.com/shinyhunters-claims-comeback-new-inception-group-rejects-alleged-ties/)

**Thirteen malicious NuGet packages hide in a fake .NET job assessment.** Socket found packages posing as WinUI 3 and WPF button controls, referenced by a "take-home assessment" repository; building the project downloads a DLL sideloaded next to a copied osk.exe, or fetches and runs an executable. The first package went up July 23 and the last two Nov. 4; all are now removed. The job-lure pattern resembles North Korean tradecraft, but Socket names no actor. New Unclear row 185 (Tier 3). [The Hacker News](https://thehackernews.com/2026/11/13-malicious-nuget-packages-turn-fake.html)

**CISA adds Danfoss refrigeration-controller flaws tied to the Iranian attacks.** Among ten KEV additions on Nov. 25 are three flaws in Danfoss AK-SM 800A controllers (path traversal, input validation, improper authentication), which The Hacker News ties to the October attacks on retail refrigeration attributed to the IRGC's Shahid Kaveh (CyberAv3ngers). Danfoss itself doesn't mention exploitation, and CISA separately warned of a new, unpatched critical Danfoss flaw (CVE-2026-129713). Update to Iran row 20 (Tier 2). [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-10-vulnerabilities.html); [CISA](https://www.cisa.gov/news-events/alerts/2026/11/25/cisa-adds-10-known-exploited-vulnerabilities-catalog)

**Microsoft confirms its fix for the Azure flaw used against Norwegian energy firms.** It fully deployed a fix for Azure API Management Classic tiers on Nov. 19 (v2 tiers unaffected) but issued no public advisory or CVE and still recommends rotating secrets. Norway's security authority says it doesn't know how far exploitation went against Equinor and Skagerak Energi, and has raised the national cyber risk level to high. Update to Unclear row 143 (Tier 3). [Cybersecurity Dive](https://www.cybersecuritydive.com/news/microsoft-remediates-azure-flaw-following-attacks-against-norwegian-energy/875755/)

**Updates to two of yesterday's rows.** The National Geospatial-Intelligence Agency is named alongside the CIA and ODNI in the breach of the unclassified OSINT system (Unclear row 171, 🤖). Check Point says the flaw GreyNoise's GT13 used against its management servers (CVE-2026-16232) was disclosed, patched, and flagged as exploited in July, through an adaptation of a public Metasploit module (Unclear row 174, 🤖). [N2K CyberWire, issue 225](https://thecyberwire.com/newsletters/daily-briefing/15/225)

## Resilience Tactics

**Krebs and Easterly: "a couple years to burn down all the bugs."** Former CISA director Chris Krebs told Face the Nation on Nov. 22 that "everybody needs to buckle up," two days after Rob Joyce warned CYBERWARCON that AI has defenders heading into a forest fire. His successor Jen Easterly expects "much more secure and resilient infrastructure" on the other side but a "significant ramp up in incidents" first, which she traces to decades without software liability. Chris Hughes's takeaway: "we can't patch our way out of this," so prioritize by known exploitation and asset criticality. [CBS News transcript](https://www.cbsnews.com/news/full-transcript-of-face-the-nation-with-margaret-brennan-nov-22-2026/) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

*Newsletter Tracker: Thread 3, ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience) (Aug 2025), status Holding. Bearing: **Supports.** Former CISA leaders conceding a multi-year run of incidents that prevention can't stop is the thread's case for investing in recovery. Status unchanged.*

**Critical-infrastructure CEOs get four questions to answer in 30 days.** The Alliance for Critical Infrastructure, now covering 12 of 16 sectors after adding chemical, manufacturing, defense, food, healthcare, and commercial-facility CEOs, asks each to know which systems they can't lose, how fast they can respond, whether recovery has been verified, and who owns the risk of systems that can't be patched. "No enterprise can fully eliminate cyber risk, but every enterprise can get faster." [Cybersecurity Dive](https://www.cybersecuritydive.com/news/alliance-critical-infrastructure-guidance-cybersecurity-ai/875741/)

**Microsoft declares a "Code Red" on outages.** After the Nov. 12-13 Microsoft 365 outage, which a memo calls the most customer-affecting incident in Exchange Online's history, M365 Core president Jason Henderson made preventing and responding to outages "the highest priority work for our team," per Reuters. [N2K CyberWire, issue 225](https://thecyberwire.com/newsletters/daily-briefing/15/225) (no Reuters permalink was found)

**"When nobody checks the work."** An IAPP analysis uses the Microsoft 365 and FAA outages (neither linked to AI; both a routine change that safeguards missed) to argue that as AI writes and applies changes faster, review capacity has to keep pace or failures will multiply. [IAPP](https://iapp.org/news/a/when-nobody-checks-the-work-what-recent-system-outages-mean-for-ai-governance)

**Camille Stewart Gloster: the cost of an off switch rises with dependence.** Organizations may keep the technical ability to disconnect an AI agent long after losing the operational freedom to do it, once staff, skills, and commitments have reorganized around it. She proposes "dependency assurance": work back from each promise to customers to what must stay true, and test visibility, verifiability, resilience, and the ability to intervene throughout an agent's life. Reuters reports several US banks are reviewing kill switches and testing backup processes for agent-run functions. [Camille Stewart Gloster](https://camilleesq.substack.com/p/ai-dependence-and-control) (via Gmail)

**Guadeloupe hospital back on paper.** [The Record](https://therecord.media/guadeloupe-ransomware-hospital-cyber) *Also covered above under Adversary Playbook.*

## Zero Trust Tactics

**Drupal's installer patch left a gap that attackers are already using.** A new flaw, CVE-2026-136716, lets attackers take over sites left in unusual or incomplete install states even after last week's fix for CVE-2026-132165 (the bug Anthropic's OSS Scanner found); Drupal says the vulnerable state isn't visible in the interface and already-compromised sites may no longer show it. Fixed in 11.4.14, 11.3.23, and 10.6.23, plus an update hook production sites must run; admins should check logs and the user 1 account. StepSecurity counts about 55,800 internet-facing Drupal sites, 31,500 on vulnerable branches and 15,000 on end-of-life 8 and 9. [SecurityWeek](https://www.securityweek.com/drupal-installer-patch-left-a-gap-attackers-are-already-exploiting/); [The Hacker News](https://thehackernews.com/2026/11/drupal-warns-of-new-highly-critical.html)

**Attackers probe two GeoServer flaws that chain to unauthenticated code execution.** watchTowr sees exploit probes for CVE-2026-120705 (XML injection) and CVE-2026-129243 (admin access bypass), two of a five-bug chain Rapid7's Jonah Burgess reported in August; Eye Security separately showed unauthenticated RCE on Linux and Windows. No successful exploitation reported yet. GeoServer, used widely by government agencies and utilities, is fixed in 3.0.2, 2.28.6, and 2.27.7. [SecurityWeek](https://www.securityweek.com/two-newly-disclosed-geoserver-vulnerabilities-under-attack/); [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-two-geoserver-flaws-as.html)

**CISA's Nov. 25 KEV update: ten exploited flaws.** Alongside the five Mitel and three Danfoss flaws, a Vates Xen Orchestra authentication bypass (CVSS 9.8, an empty-JSON token grants admin; Vates published an attacker IP and TOR domain) and a Juniper Session Smart command injection (CVSS 9.8, root via a crafted salt minion ID; Juniper confirms one exploitation). Agencies have until Nov. 28 for most. [CISA](https://www.cisa.gov/news-events/alerts/2026/11/25/cisa-adds-10-known-exploited-vulnerabilities-catalog); [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-10-vulnerabilities.html)

**Securing the "invisible workforce" of non-human identities.** An ISC2 Security Congress session put the ratio as high as 144 machine identities per human, and argued service accounts, build runners, and AI agents need their own lifecycle and ownership, since they don't leave when their creator does. A demo compared two leaked credentials: a read-only pipeline token led nowhere further, while an AI agent's broad credential gave elevated access and persistence. [(ISC)²](https://www.isc2.org/Insights/2026/11/isc2-security-congress-2026-securing-your-invisible-workforce-of-non-human-identities)

**1Password's GitHub-account breach.** [SecurityWeek](https://www.securityweek.com/1password-breach-exposes-customer-data-internal-source-code/) *Also covered above under Adversary Playbook.*

## Critical Infrastructure Attacks

**Guadeloupe University Hospital.** [The Record](https://therecord.media/guadeloupe-ransomware-hospital-cyber) *Also covered above under Adversary Playbook.*

**Danfoss refrigeration-controller flaws added to KEV.** [The Hacker News](https://thehackernews.com/2026/11/hackers-exploit-10-vulnerabilities.html) *Also covered above under Adversary Playbook.*

**Microsoft's Azure APIM fix after the Norwegian energy attacks.** [Cybersecurity Dive](https://www.cybersecuritydive.com/news/microsoft-remediates-azure-flaw-following-attacks-against-norwegian-energy/875755/) *Also covered above under Adversary Playbook.*

**The Alliance for Critical Infrastructure's CEO guidance.** [Cybersecurity Dive](https://www.cybersecuritydive.com/news/alliance-critical-infrastructure-guidance-cybersecurity-ai/875741/) *Also covered above under Resilience Tactics.*

## Data Breaches

**1Password: customer account data and source code stolen.** [SecurityWeek](https://www.securityweek.com/1password-breach-exposes-customer-data-internal-source-code/) *Also covered above under Adversary Playbook.*

**FIFA: "a limited set of personal and business information."** [The Record](https://therecord.media/fifa-data-breach-limited) *Also covered above under Adversary Playbook.*

**The NGA is named in the OSINT system breach.** [N2K CyberWire, issue 225](https://thecyberwire.com/newsletters/daily-briefing/15/225) *Also covered above under Adversary Playbook.*

## Nation-State Cyber Policy & Law

**Britain delays its National Cyber Action Plan again, to December.** First due by the end of 2025 as a national strategy, then rebranded and nearly published in July, the plan slipped again for reasons the government won't give, a week after a House of Lords committee found the government "appears complacent" about catastrophic risks including attacks from Russia, China, and Iran. The Cyber Security and Resilience Bill isn't expected to be enforced until 2028, and ransomware rules (mandatory reporting, a payment licensing regime, a ban for critical infrastructure) still await a National Security Bill next year. Last month's budget did fund the AI Security Institute (£120 million), a National Agentic Security Unit (£40 million), an AI vulnerability-hunting center at NCSC (£70 million), and the first phase of "Cyber Shield" (£60 million), and promised a consultation on "where liability for cyber breaches should sit." [The Record](https://therecord.media/britain-delays-national-cyber-action-plan-again)

**Australia passes the Digital Duty of Care Act.** Platforms must detect and reduce harmful content, protect under-18s, run annual written risk assessments, flag risky design changes such as endless scrolling, let users opt out of algorithmic feeds, and verify age for pornography, with possible fines in the billions. US officials call it a threat to free speech and American business models. [The Record](https://therecord.media/australia-passes-online-safety-legislation-preempt-harms)

**Srsly Risky Biz: Starshield slowdowns and homegrown open weights.** Tom Uren notes SpaceX's military Starshield service was speed-limited in Ukraine twice since mid-October, which Zelensky says hurt air defenses against jet-powered Shaheds; who ordered it is disputed, and incoming House Intelligence chair Jim Himes threatens to withhold Starshield funding without answers. Uren's advice to allies: find alternatives. He also backs the House committees' call (covered 11-22) for a national American open-weight AI initiative, since "holding back China's AI labs" alone hasn't worked. [Risky.Biz](https://news.risky.biz/srsly-risky-biz-america-needs-homegrown-open-weight-models/)

## Intrusion Kill Chain Prevention Tactics

**"Vulnpocalypse": SOCs need a vulnerability-response loop.** Zack Allen counts six "drop-everything" disclosures in a month (PHP2Shell, Node2Shell, a GitLab RCE, eMudhra's weak CA key, SSHole, Java4Shell and NGINX2Shell) and argues the rapid-response model isn't sustainable. His proposal: SOC teams replicate exploits with agents, hunt for prior exploitation, write detections as a compensating control until patches land, and use per-service threat models (citing Anthropic's THREAT_MODEL.md) to decide which deployments actually need urgent patching. [Detection Engineering Weekly](https://www.detectionengineering.net/p/vulnpocalypse-and-vulnerability-response)

**An open repository of detections for agentic attack frameworks.** ThreatDefence's MIT-licensed collection holds rules, hunting queries, and 572 sourced indicators for 11 frameworks including ARTEX, Cairn, and PentAGI, and counts 3,968 exposed framework consoles active in the week to Nov. 23. [GitHub](https://github.com/ThreatDefence/agentic-attack-detections) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

**Microsoft: ARTEX's most durable signal is behavioral.** [The Record](https://therecord.media/microsoft-china-salt-typhoon-using-artex-ai-tool) *Also covered above under Adversary Playbook.*

## Risk Forecasting Tactics

**Bridgewater is investing on a one-in-three chance of an economically destabilizing cyberattack within a year.** The fund's researchers say AI-enabled cyber warfare is "spreading exponentially with limited controls," that zero-day exploits roughly doubled after the first cyber-capable open-source models shipped, and that time from disclosure to exploitation fell from a month to 11 days. Lab programs (Glasswing, Daybreak, Fairwind) find bugs faster than volunteer maintainers can fix them, and Japan's and South Korea's responses don't address that. Bridgewater built its own incident time series and hasn't published it, so the figures can't be checked against KEV or Project Zero. [Bridgewater](https://www.bridgewater.com/research-and-insights/current-efforts-arent-enough-to-slow-the-ai-cyber-virus) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

**CSET: judge the cyber apocalypse by the data.** Andrew Lohn finds technical indicators favor attackers (monthly CVEs tripled from January to September, patching is slower), yet significant incidents are down, health-care breach counts are stable, breach costs are flat, and ransomware payouts are down. His reading: attackers' motives and fear of retribution may be the binding limit, so attribution and enforcement matter more, resilience can cut impact, and the calm may not survive a crisis. [CSET](https://cset.georgetown.edu/article/judge-the-cyber-apocalypse-by-the-data-not-the-headlines/)

*Newsletter Tracker: Thread 2, ["A Board Presentation on Cyber First Principles"](https://diffuser.substack.com/p/a-board-presentation-on-cyber-first) (Apr 2026), status Holding. Bearing: **Supports.** A major investor states an explicit annual probability and acts on it, and CSET argues the estimate should be tested against impact data: both treat cyber risk as a number to forecast, not a color. Status unchanged.*

**100,000 CVEs in 322 days.** Jerry Gamblin notes the first 100,000 CVEs took 18 and a half years to publish; 2026 reached 100,000 in 322 days. [Jerry Gamblin](https://infosec.exchange/@jgamblin/117645602395628518) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

## AI Singularity Timeline

**Current range:** P5 2031 · P50 2046 · P95 2075: a 44-year uncertainty window and a 50% chance we could reach this milestone in 15 years.(unchanged since 2026-11-17)

**Apollo Research: labs are handing AI R&D to their own agents, and oversight is falling behind.** The report defines "Handoff" as the delegation of all AI R&D, including safety assessments and deployment decisions, to internally deployed agents. Agents write over 90% of code merged at Anthropic, and humans see 0.001–0.01% of OpenAI's internal coding trajectories. Apollo warns of "a significant chance" that a lab "will eventually and unknowingly hand control of its AI R&D process to misaligned AI agents," with no human positioned to catch it, a risk it says doesn't depend on recursive self-improvement. It recommends a federal transparency standard for Handoff, with labs reporting to an authority such as Commerce. [Apollo Research](https://www.apolloresearch.ai/governance/handoff-at-frontier-ai-companies) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

**Source:** an independent AI-evaluation lab (one of four outside evaluators OpenAI is embedding, 11-20), compiling the labs' own voluntary disclosures. *Credentialed expert judgment*, built on disclosed figures, with no date or probability.

**Effect on the range:** held. It's the clearest statement yet of the oversight-erosion path this file watches, so it leans Sooner, but the figures come from the companies and partly overlap what the file already holds (Anthropic's code-share growth, 11-24), and "a significant chance" with no date can't be sized against P5 or P50.

**OpenAI's chief scientist expects alignment auditing to degrade and proposes development limits.** Jakub Pachocki writes that as models pass further perplexity thresholds, "we should also expect further degradation in currently dominant forms of alignment auditing and further increases in evaluation and training awareness," and that alignment progress is "unlikely to be fast enough" to keep up with a possible 2027 "avalanche" of AI-driven pretraining advances. He calls full recursive self-improvement without human oversight something "we should obviously avoid," and proposes common limits, measured by perplexity, that labs commit not to cross until monitoring reaches a concrete milestone such as a successor to chain-of-thought monitors. [OpenAI](https://openai.com/index/perplexity-and-intelligence/) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

**Source:** OpenAI's chief scientist, writing about his own lab's models. *Credentialed expert judgment* from inside a lab, with a commercial stake.

**Effect on the range:** held. P5 already moved a year on 11-17 for Christiano's insider warning that capability can outrun control; Pachocki is a second insider in the same direction but gives no date, and his limits proposal, if adopted, would cut the other way.

*Context only:* Camille Stewart Gloster's argument that the cost of an off switch rises with dependence (above, under Resilience Tactics). **Source:** a cybersecurity policy writer, in her own newsletter; *Commentary*. **Effect on the range:** none; it describes gradual loss of practical control by organizations, the argument the file already logged from Ezra Klein (10-20).

**Sherlock's view:** two independent Sooner-leaning sources in one day, neither dated; not enough to move a percentile. **Ryan's view:** Microsoft's report of Salt Typhoon and Crystal Typhoon adopting ARTEX is human-directed misuse, no bearing. **Seldon's call:** hold at P5 2031 · P50 2046 · P95 2075. A dated estimate from either source would justify revisiting P50.

*Newsletter Tracker: Thread 5, ["A Pinky Swear at the White House"](https://diffuser.substack.com/p/a-pinky-swear-at-the-white-house) (Oct 2026), status Under Pressure. Bearing: **Supports** (Apollo) and **Ambiguous** (Pachocki). Apollo's case for a mandatory federal reporting standard, because "almost everything we know about Handoff comes from the companies themselves, disclosed voluntarily," is the thread's argument. Pachocki's limits are a stronger idea than the accord's basic controls but are still a voluntary pledge among competitors, the kind the thread distrusts. Status unchanged.*

## Automation Tactics

**Four sandboxes for AI coding agents, none finished.** Kudelski Security's Nils Amiet scored Docker Sandboxes and NVIDIA's OpenShell 4.5 of 5 and nono and Microsandbox 4. Docker and Microsandbox isolate agents in microVMs; nono starts fastest but shares the host kernel; only nono and OpenShell scope injected credentials to both a domain and an endpoint. None can deny a single file inside an allowed directory (so a .env stays readable), and none has reached version 1.0. Amiet cites Johann Rehberger's 60–80% prompt-injection success against Claude Code's Auto Mode. [Kudelski Security](https://kudelskisecurity.com/research/sandboxing-coding-agents) (via [Resilient Cyber](https://www.resilientcyber.io/p/resilient-brief-124-burning-down-the-bugs))

**Salt Typhoon and Crystal Typhoon adopt ARTEX.** [The Record](https://therecord.media/microsoft-china-salt-typhoon-using-artex-ai-tool) *Also covered above under Adversary Playbook.*

## Compliance Trends

**Wells Fargo now holds customers responsible for their AI agents.** Its Online Access Agreement, effective Nov. 24, treats instructions from third-party agents a customer authorizes as the customer's own, including unintended actions and actions beyond the authority granted. Camille Stewart Gloster notes the contrast with banks tightening controls on their own agents. [Camille Stewart Gloster](https://camilleesq.substack.com/p/ai-dependence-and-control) (via Gmail)

**EU law assigns AI accountability faster than anyone can reconstruct a decision.** An IAPP analysis: EU law is getting clearer about which organization bears the legal duty for an AI-assisted decision (a hiring filter, a credit score), but the evidence needed to explain it (model version, prompt, retrieved documents, thresholds) is often held by suppliers, and enterprise logs rarely capture it. [IAPP](https://iapp.org/news/a/who-is-responsible-when-the-ai-is-wrong-why-legal-duty-does-not-equal-technical-visibility)

## AGI Arrival Timeline

**Current range:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11)

**OpenAI publishes its internal perplexity figures.** Pachocki reports log-perplexity on OpenAI's held-out codebase set: GPT-3.5 about 0.99, GPT-4 about 0.91. Below 0.8, "we have seen the emergence of transformative capabilities in fields like cybersecurity and mathematics," and a model at about 0.76 "started producing groundbreaking results" on open math problems. He expects more, unknown transformative capabilities in the 0.68–0.70 window, and says 2026's steep acceleration came mostly from compute and research investment, "only in a smaller part" from automation. He concedes the metric misses reasoning gains and has an unknown floor. [OpenAI](https://openai.com/index/perplexity-and-intelligence/) *Also covered above under AI Singularity Timeline.*

**Source:** OpenAI's chief scientist. *Measured result* (internal and unaudited) for the loss figures; *Credentialed expert judgment* for the extrapolation; a direct commercial stake.

**Effect on the range:** held. The math and cyber jumps are already priced (the Riemann proof, 11-23; METR, 11-06). Perplexity gives no date or threshold for broad human parity, so it argues neither for an earlier P5 nor for moving P50 off its open review flag (parity in open-ended, non-verifiable work).

**Sherlock's view:** slight Sooner lean, already priced. **Ryan's view:** none offered. **Seldon's call:** hold at P5 2029 · P50 2045 · P95 2075.

## Superintelligence Timeline

**Current range:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap.

**Pachocki: the step change may come from AI doing pretraining research.** Rather than full recursive self-improvement, he points to AI taking part in algorithmic research on pretraining: having watched a model produce one math breakthrough after another, "as soon as 2027 we could conceivably see a similar avalanche of fundamental pretraining advancements." [OpenAI](https://openai.com/index/perplexity-and-intelligence/) *Also covered above under AI Singularity Timeline.*

**Source:** OpenAI's chief scientist. *Credentialed expert judgment*, no probability given.

**Effect on the range:** held. "Conceivably" by 2027 is a possibility, not a forecast, and it's the mechanism the one-year gap already assumes; his own footnote that automation drove only a small part of 2026's speed-up supports keeping the gap rather than shrinking it.

**Sherlock's view:** no shift. **Ryan's view:** none offered. **Seldon's call:** hold. Floor check: the AGI file didn't move, so no gap-model follow.

## Harm Probability

**Current range:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03)

**WIRED's ten-expert panel, queued by Rick (already weighed 11-12).** Lauren Goode asked ten experts whether the world is going to end. Most treat AI-enabled cyber, bio, and nuclear catastrophe as real and extinction as implausible or unquantifiable: Sayash Kapoor calls "runaway intelligence" the most overblown risk, Niels Provos "doesn't really see a path" to humanity being cooked, Rob Reich finds extinction "pretty implausible" but catastrophe "imaginable," and Heidy Khlaaf refuses extinction percentages because "there are no numbers to back it." Yoshua Bengio alone says of rogue AI, "we shouldn't take a chance," and backs a pause. [WIRED](https://www.wired.com/story/the-ai-safety-debate-has-lost-the-plot-we-asked-10-experts-what-the-real-nightmares-are/) (read from Rick's vault clipping; this file logged the same article on 11-12, so this is a recirculation with fresh Source and Effect lines)

**Source:** a credentialed, mostly skeptical panel spanning safety engineering, AI policy, security research, biosecurity, and ethics, assembled by a journalist. *Credentialed expert judgment*, no numbers.

**Effect on the range:** held at Low 15%, Central ~30%, High 55%. No panelist addresses this file's conditional (a >10%-of-humanity catastrophe within 10 years of losing control); their doubt is mostly about whether control is lost at all. Under the disagreeing-source rule it argues against raising Low, as the XPT median and Delangue did, and Khlaaf's objection argues for humility about the whole interval rather than a different center.

**Sherlock's view:** slight Lower lean, as on 11-12. **Ryan's view:** none offered. **Seldon's call:** hold.

## Law Enforcement Disruption

**A Florida ransomware-recovery CEO is indicted for secretly paying ransoms.** A federal grand jury charged Juan Ricardo Palacio Escobar, co-founder of RansomwareHelp.com, with three counts of wire fraud. Prosecutors say he claimed proprietary decryption tools but paid the attackers instead: in a June FBI sting he paid about $6,000 in bitcoin to an undercover "ransomware actor" and billed the undercover victim about $13,260. Arrested Oct. 22, he was released on bond Nov. 20. The sting itself was covered 11-22. [The Record](https://therecord.media/ransomware-doj-indictment-recovery)

## Executive Leadership Changes

**ArcelorMittal names Varun Singla group CISO (reported, unconfirmed).** The former Airtel security lead is to strengthen the steelmaker's cybersecurity strategy; CISO Tribune flags the report, from cxodigitalpulse.com, as not yet confirmed by ArcelorMittal or an established publication. [CISO Tribune](https://www.cisotribune.com/moves)

---

### Pending Evidence Queue

One row processed: WIRED's ten-expert AI-safety panel (queued 11-25, Harm Probability), written up above. Its category fits, but this file already weighed the same article on 11-12, so it ran as a recirculation and the range held. The row is now marked Included.

### Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **AGI Arrival Timeline** — Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity.
- **Superintelligence Timeline** — Evidence on when a machine might exceed, not just match, human intelligence — a higher, later capability bar than AGI, inferred structurally with no external forecaster basket.
- **Harm Probability** — Evidence on how likely — not how soon — a system that's escaped human control is to cause a catastrophe killing over 10% of humanity within 10 years; a bounded probability question, tracked separately from Harm Timeline's open-ended date question.
- **Law Enforcement Disruption** — Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Intrusion Kill Chain Prevention Tactics** — Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends.
- **Cybersecurity Risk Forecasting Tactics** — Quantified cost/impact/risk reporting — superforecasting, Bayesian methods, FAIR methodology, and risk-forecasting case studies.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.

### Source Contribution Scorecard

| Source | Today | Contributed (all-time) | No Contribution (all-time) | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 76 | 14 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 60 | 31 | 2026-07-14 |
| The Hacker News | Contributed | 90 | 1 | 2026-07-14 |
| The Record | Contributed | 71 | 20 | 2026-07-14 |
| The Canon Project | No Contribution | 20 | 70 | 2026-07-14 |
| FFX Now | No Contribution | 18 | 73 | 2026-07-14 |
| Wired | No Contribution | 57 | 31 | 2026-07-20 |
| CyberScoop | No Contribution | 44 | 18 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 59 | 2026-09-01 |
| CISA Cybersecurity Advisories | Contributed | 30 | 32 | 2026-09-01 |
| SecurityWeek | Contributed | 57 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 3 | 37 | 2026-10-02 |
| CISO Tribune — The Wire | Contributed | 14 | 18 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 31 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 16 | 16 | 2026-10-17 |
| (ISC)² Insights | Contributed | 9 | 23 | 2026-10-17 |
| IAPP News | Contributed | 21 | 11 | 2026-10-17 |
| CSIS Strategic Technologies Program | No Contribution | 5 | 27 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 9 | 23 | 2026-10-17 |
| Risky.Biz | Contributed | 11 | 6 | 2026-11-10 |
| tl;dr sec | No Contribution | 2 | 15 | 2026-11-10 |
| Detection Engineering Weekly | Contributed | 2 | 15 | 2026-11-10 |
| Resilient Cyber | Contributed | 8 | 9 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | Contributed | 10 | 7 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 1 | 14 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 13 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 15 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 4 | 11 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 1 | 14 | 2026-11-12 |
| Zero Trust Forum | No Contribution | 0 | 3 | 2026-11-24 |

**No contribution today:**
- **The Canon Project**: newest review is still Nov. 23, covered 11-24 (read through Chrome; the listing is behind Cloudflare).
- **FFX Now**: 7 items dated Nov. 25 (Thanksgiving storm advisories, a Beltway crash, ALU zoning, a state Senate candidate, Small Business Saturday, a Thanksgiving 5K, Morning Notes); no CIR fit. Today's Morning Notes wasn't up at run time.
- **Wired**: the only item in the window is the "True Crime Community" TikTok piece, already judged no fit 11-25.
- **CyberScoop**: one item, FinCEN taking systems offline, covered 11-25.
- **CSO Online CISO Appointments**: still no October or November section.
- **LEAP**: newest is Wave 13, covered 11-19.
- **NIST Insights**: newest post Oct. 27.
- **EFF**: the only item is the EFFector 38.21 newsletter, which repeats Deeplinks posts already covered.
- **CSIS**: nothing after Justin Sherman's Nov. 24 commentary, covered (read through Chrome).
- **AI Alignment Forum**: no post since Eli Lifland's (Nov. 24), covered.
- **tl;dr sec**: no issue since Nov. 19.
- **AI as Normal Technology, Epoch AI, Reflective Altruism, Understanding AI, Marcus on AI**: nothing new in the window.
- **Zero Trust Forum**: newest item is still the Nov. 20 podcast.

**Crediting notes:** The Record for Salt Typhoon and ARTEX, Guadeloupe, FIFA, the UK action plan, Australia's law, and the Palacio indictment; SecurityWeek (site feed) for 1Password, Mitel, the Drupal gap, ShinyHunters and Inception, and GeoServer; The Hacker News for the NuGet packages and the KEV and Danfoss details; CISA for the Nov. 25 KEV update; N2K CyberWire (issue 225, its last before a Thanksgiving break) for the NGA, Check Point's GT13 statement, and Microsoft's Code Red; Cybersecurity Dive for the ACI guidance and Microsoft's APIM fix; Risky.Biz for Srsly Risky Biz (Starshield, open weights); Detection Engineering Weekly for Zack Allen's essay; Resilient Cyber (Brief #124) for Bridgewater, CSET, Gamblin, Krebs and Easterly, Apollo, Pachocki, Kudelski, and ThreatDefence; (ISC)² for the non-human-identity session; IAPP for the two AI-governance analyses; CISO Tribune for Singla; Gmail for Camille Stewart Gloster's essay (Wells Fargo terms, dependency assurance). **Recirculations excluded:** FinCEN (CyberScoop, SecurityWeek, The Hacker News; covered 11-25), the CrowdStrike–Zscaler deal, Shirudo, Signal's screenshot block, the House report on Chinese open-weight models, Amazon's Cairn finding, OpenRouter's provider removals, and Jensen Huang's reinstatement (Resilient Cyber, Srsly Risky Biz; all covered 11-21 to 11-25), the Fail2Install exploit write-up (The Hacker News; the Drupal flaw was covered 11-25), the newspaper skimmer, Windows Endpoint Security Platform, and Windows Baseline Protection items in Srsly's Bulletin digest (covered 11-20 to 11-25), and Danfoss's earlier ICS advisory (covered 11-17). **Considered, no CIR fit:** SecurityWeek's interview with Western Carolina University CISO Matt Martin (no appointment), Lindsey Cerkovnik joining Anthropic as head of vulnerability disclosure (not a C-suite role), The Hacker News's sponsored pieces on credential remediation and phishing kits, Palo Alto's reported talks to buy Terra Security (covered 11-21), Axios's "AI 2027: the reckoning" (paywalled, not read), Google Alerts snippets on cyber insurance and Gartner placements, and ExecutiveGov's piece on GAO's 16 AI-in-cyber policy options (page returned empty; still unread). **Tooling notes:** Gmail `search_threads` again returned no snippets, so messages were read with `get_thread` in plain text; nearly every page came through headless Chrome, while the Canon Project, CSIS, and openai.com were read through Chrome MCP.

*Pending artifact approvals (raceBannon99/nexus-artifacts): none open.*
