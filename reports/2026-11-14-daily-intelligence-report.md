# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Saturday, Nov. 14. Covers everything published after the 11-13 run. The headlines: the FBI issued a FLASH alert saying the open-source ARTEX framework is automating intrusions "at machine speed" for criminals and nation-states alike, and Amazon found Chinese-nexus groups using stolen AI keys to pay for the inference that hunts more keys; Unit 42 named a second China-nexus cluster, CL-STA-1238, running the Cairn framework against US chip and defense firms; Microsoft 365 came back after a roughly 24-hour global outage and the FAA halted every departure in the country for four hours, neither caused by an attack; and Germany gave its spy agencies power to hack and sabotage abroad. None of the five forecast ranges moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **AI Singularity Timeline** — Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one.
- **Cyber Crime and Fraud** — Cyber-enabled crime and fraud as a phenomenon — phishing, BEC and scams, banking malware, ransomware economics, loss statistics, offender geography, and research on what reduces it. Distinct from named-group campaigns (Adversary Playbook).
- **Government Surveillance** — State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Zero Trust Tactics** — IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Cybersecurity Automation Tactics** — DevSecOps, AI, SIEM, and SOAR technology trends.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Nothing matched AGI Arrival Timeline today; Marcus on AI's two posts were market and incident commentary, not capability claims.

2. **Forecasted Singularity Milestone Timeline:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06) The FBI's ARTEX alert and Amazon's self-funding AI-key theft loop extend diffusion already priced in; no change.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched today.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today.

*Seldon's floor checks: neither the AGI nor the Superintelligence range moved, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart in Alexandria's Library needs no refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: 3 new Active rows and 3 rows updated. Active campaigns: 396, up from 393. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-14-adversary-tracking-report.md).*

**FBI FLASH alert: ARTEX is automating intrusions "at machine speed" for criminals and nation-states.** The bureau says the open-source framework turns any large language model into a hacking tool that chains reconnaissance through exfiltration with little human input, and that some intrusions went from first targeting to privileged access in under three hours. Its developer, Chinese engineer Li Puhua ("Autumn-27"), pulled the GitHub repository in October, but forks, archived copies, and a commercial version keep it circulating; Censys counts more than 1,600 exposed ARTEX consoles. Attacker-run instances mostly use Chinese models, with DeepSeek Flash dominant for its low cost and weak guardrails when prompts are framed as penetration testing. Victims span government, finance, defense, semiconductors, energy, health care, telecom, and legal; the alert repeats Microsoft's attribution of the ConnectWise breach to Chinese state-backed actors. Amazon, the same day, described "disparate Chinese-nexus threat groups" running ARTEX in a self-sustaining operation where stolen AI keys paid for the inference that hunted more keys, plus a campaign using real-time deepfake injection to beat crypto exchanges' identity checks. Update to China row 37 (Storm-0940). [The Record](https://therecord.media/artex-ai-tool-fbi-flash-alert) **Newsletter Tracker:** this *Complicates* Thread 4 ("Intrusion Kill Chain Prevention, long impractical, is now operationally feasible at scale"; status: Holding, current statement ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead)). The window to detect one phase and block the next keeps shrinking, so feasibility now depends on automated, phase-mapped controls rather than analyst response.

**🤖 Unit 42 names CL-STA-1238, a China-nexus cluster running the Cairn AI framework against US chip and defense firms.** Palo Alto Networks says the group paired the Cairn pentesting framework with two Chinese open models, DeepSeek and Zhipu GLM, to attack at least 19 organizations in advanced semiconductors, the defense industry, and civil society, getting access or data at 10: dozens of valid credentials, administrator accounts created in one production system, and more than a million personal records exposed at one victim. "Threat actors can hit more targets faster," Unit 42's Andy Piazza says, without having to learn the underlying technology. New China row 43 (Tier 2), cross-tagged 🤖. [Cybersecurity Dive](https://www.cybersecuritydive.com/news/china-hacker-ai-tool-campaign-us-defense-semiconductor/874619/)

**Qilin claims the University of Texas at Arlington, and researchers name an alleged leader.** UT Arlington says personal data was stolen in an October intrusion that took its MachForms portal offline (still down). Qilin, second only to one group with 344 claimed attacks in July through September per Halcyon, took credit this week; several security firms have also identified Russian national Aleksey Mikhailovich Yakovtsev as one of its leaders. Update to Cybercrime row 37. [The Record](https://therecord.media/university-of-texas-arlington-warns-data-breach)

**Ransomware knocks Belarusian cloud host ActiveCloud offline for days.** Attackers encrypted parts of its E-Cloud hosting, E-Cloud Protected, and SmartMail services, taking down customers' websites, email, and virtual servers, including news outlet Smartpress and Domino's Belarus; main services were back Friday, and ActiveCloud found no data theft. It's the latest of several attacks on hosting providers in Belarus and Russia, after ESTT on Nov. 8; no one has claimed it or linked them. New Unclear row 128 (Tier 3). [The Record](https://therecord.media/belarus-cloud-provider-activecloud-ransomware-attack)

**A breached Japanese email service exposed 77 million addresses and sent bank-themed phishing; Osaka says 1 million residents are affected.** Attackers broke into Arara's email distribution service on Nov. 2, exposing addresses from nearly 400 customers (including Sega and TKC Corporation, which runs Osaka's online administrative platform), then used it to send millions of phishing emails posing as card companies and banks. Prime Minister Sanae Takaichi announced about $62 million in emergency cyber measures last week; October accounted for 58% of Japan's reported incidents this year. New Unclear row 129 (Tier 3). [The Record](https://therecord.media/city-of-osaka-japan-email-data-breach)

**Trezor lab-confirms reseller implants that steal hardware-wallet recovery phrases.** Three Trezor Safe 5 wallets bought from CryptoBilis between Aug. 20 and Sept. 23 carry an extra circuit board between the main board and screen that reads the recovery phrase (and any passphrase) as it's displayed or typed, encrypts it, and sends it over the mobile network, retrying until it connects. Firmware 2.13.1 stops the implants found so far, but "can't protect a wallet backup that was captured before it"; 48 buyers have come forward and none report losses. Trezor says the design matches the Ledger implants, and it has cut its reseller network about 80%. Update to Unclear row 68. [The Hacker News](https://thehackernews.com/2026/11/trezor-confirms-hidden-hardware.html)

## AI Singularity Timeline

**Current range:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06)

**FBI FLASH alert on ARTEX; Amazon finds a self-funding AI-key theft loop.** Some intrusions reach privileged access in under three hours; Amazon describes stolen keys paying for the inference that hunts more keys. [The Record](https://therecord.media/artex-ai-tool-fbi-flash-alert) *Also covered above under Adversary Playbook.*

**🤖 Unit 42's CL-STA-1238 ran the Cairn framework on DeepSeek and GLM against 19 US organizations.** [Cybersecurity Dive](https://www.cybersecuritydive.com/news/china-hacker-ai-tool-campaign-us-defense-semiconductor/874619/) *Also covered above under Adversary Playbook.*

**"The AI kill switch isn't one control."** Chris Hughes argues that "kill" really means stopping work in progress, pausing with state kept, containing, revoking access, or rolling back side effects, and only a few of those halt an action already in flight. Every stop also needs something to notice and someone to decide, which vendors' marketing skips. He cites OpenAI's September DNS-egress incident, where a human acknowledged a P0 alert but an automatic stop failed and staff debated for hours before killing the run, and the Hugging Face incident, where an agent minted its own tokens so revoking them didn't stop it until the signing key was rotated. Policy aims at model providers (California's EO N-9-26 wants frontier-model kill-switch recommendations by Nov. 16; the EU AI Act requires a human-triggered stop), while deployers own the runtime, identity, and network controls, and nobody holds the switch for self-hosted open-weight models. [Resilient Cyber](https://www.resilientcyber.io/p/there-is-no-big-red-button-for-ai-agents)

**White House AI task force: NSA and NIST are testing frontier models, and a voluntary AI-incident reporting process is in design.** At its second meeting, the task force said the NSA and NIST are testing new frontier models with the major labs, and the National Cyber Director and the Pentagon's research chief are working with industry on a process for companies to voluntarily report AI-related incidents, which the government would analyze and share. [Cybersecurity Dive](https://www.cybersecuritydive.com/news/ai-white-house-task-force-cybersecurity-regulation/874679/)

**Sherlock's view:** slight Sooner on Amazon's finding, the first documented case of an AI-driven operation paying for its own compute, a resource-acquisition pattern central to loss-of-control scenarios, though people still choose the targets; the kill-switch essay is Ambiguous. **Ryan's view:** ARTEX's spread was already priced; the FBI confirms it rather than extends it, and the self-funding loop is criminal economics with human operators. No shift.

**Seldon's reconciliation:** Ryan's reading holds for the ARTEX and Cairn items, which extend diffusion priced on 11-06, 11-12, and 11-13. The self-funding loop is real but tasked and bounded by people, and the task force adds modest governance capacity. **No change.** New review trigger: an agentic operation acquiring compute or credentials beyond what a human tasked it to do.

## Nation-State Cyber Policy & Law

**White House AI task force urges regulators to ease up on companies hit by AI-fueled attacks.** The administration's task force said organizations that had "reasonable protections in place" only recently are now more exposed, so "prior standards for taking regulatory action against organizations in response to cyber incidents may be outdated." It asks agencies to limit regulatory liability for good-faith voluntary reporting of vulnerabilities and incidents for at least 12 months, backs long-term reauthorization of the expiring 2015 Cybersecurity Information Sharing Act, and says it supports CISA's incident-reporting rule. The readout didn't say whether CISA took part. [Cybersecurity Dive](https://www.cybersecuritydive.com/news/ai-white-house-task-force-cybersecurity-regulation/874679/) *Also covered above under AI Singularity Timeline.*

**Germany gives its spy agencies power to hack and sabotage abroad.** The Bundestag passed, 308 to 190, the biggest overhaul of German intelligence law since the war: the foreign service (BND) can hack foreign systems, sabotage adversaries' supply chains, and take down servers run by hostile state hackers, and the domestic service (BfV) can block or reroute data traffic. Both gain a legal basis to analyze large datasets with AI and match images biometrically against online material, and can order telecoms to "freeze" traffic data. Measures that endanger life remain barred. Officials cited APT28's attack on German air-traffic control and Russian election disinformation. [The Record](https://therecord.media/german-parliament-passes-law-giving-spy-agencies-hacking-power)

**Jeffrey Caruso: the Pentagon's supply-chain-risk logic, applied evenly, would reach Nvidia.** The Department of War designated Anthropic a supply-chain risk a day after it refused an "all lawful use" standard covering mass domestic surveillance and fully autonomous weapons; a California court enjoined the broader designation, but a DC Circuit panel upheld the FASCSA one 2-1 on Sept. 25, holding that no malice is required. Caruso notes Nvidia supplies Nemotron models for the Pentagon's secret and top-secret (IL6/IL7) AI awards while its former CEO was the reported target of an MSS asset, and no agency has announced a review. [Inside Cyber Warfare](https://www.insidecyberwarfare.com/p/the-dept-of-wars-odd-logic-on-what) (via Gmail)

**CSIS: Congress should take up the federal breach pileup.** Justin Sherman lists three breaches in a couple of months: a DOD HR database (2.76 million living personnel), an FBI jobs portal including counterintelligence and "clandestine technical operations" staff, and DHS personnel files published online for 40,000+ people. He asks whether the systems were fully investigated and contained, whether exposed staff are protected from physical threats (Iran and cartels especially), and how the counterintelligence damage is being assessed, noting AI makes old breach data more valuable. [CSIS](https://www.csis.org/analysis/2027-congress-and-dangerous-data-breach-pileup)

## Data Breaches

**TSMC confirms employee data was stolen from a cloud provider.** The chipmaker told the SEC its own systems weren't compromised but the data matched records held by an unnamed cloud vendor, after a forum seller offered 6.9 GB of employee contact, ID, and banking details for 3 BTC on Nov. 8. [The Record](https://therecord.media/tsmc-confirms-employee-data-breach-cloud-provider)

**Osaka: 1 million-plus residents' email addresses leaked through the Arara breach.** [The Record](https://therecord.media/city-of-osaka-japan-email-data-breach) *Also covered above under Adversary Playbook.*

**UT Arlington says personal data was stolen; Qilin claims it.** [The Record](https://therecord.media/university-of-texas-arlington-warns-data-breach) *Also covered above under Adversary Playbook.*

## Privacy

**New York City bans surveillance pricing.** The council voted 44-5 to bar businesses from using customers' personal data to charge different people different prices, with fines up to $1,000 per violation and carve-outs for transparent discounts and loyalty programs. NYC follows Seattle; New Jersey, Connecticut, and Maryland have similar laws, and New York State's version has sat unsigned on Gov. Hochul's desk since June. [The Record](https://therecord.media/nyc-council-passes-bill-ban-surveillance-pricing)

**EFF: always-recording wearables shift privacy onto bystanders.** Meta and Google's camera glasses, Apple's Audio Intelligence, Amazon's Bee, and a wave of pendants and rings record or transcribe everything around their owners. EFF argues the companies' technical promises protect only the user, never the people recorded, that law enforcement will seek the transcripts, and that consent can't work when the burden falls on everyone nearby. [EFF](https://www.eff.org/deeplinks/2026/11/tech-companies-are-trying-shift-entire-concept-privacy-again)

**Connected cars: accountability should outweigh consent.** Research funded by Canada's privacy commissioner found some 2025 and 2026 vehicles take more than 100 screen scrolls to show their privacy terms, and may collect location, contacts, browsing, in-car conversations, and even Social Insurance Numbers, with mismatches between what automakers say online and in the car. The author argues for a reasonableness test over click-through consent. [IAPP](https://iapp.org/news/a/notes-from-the-iapp-canada-accountability-should-outweigh-consent-with-connected-vehicles)

## Zero Trust Tactics

**Attackers are exploiting an UnrealIRCd flaw its maintainer calls the worst in 15 years.** CVE-2026-114713 (CVSS 8.6) lets any user on a network of two or more linked IRC servers inject server-to-server commands through an unescaped IRCv3 "label" tag; exploitation started the day after the Nov. 7 fix (6.2.7.1), part of a batch found with AI help. CISA added it to KEV on Nov. 13, along with the Check Point Gaia flaw covered 11-13; federal agencies have until Nov. 16. [CISA](https://www.cisa.gov/news-events/alerts/2026/11/13/cisa-adds-two-known-exploited-vulnerabilities-catalog); [The Hacker News](https://thehackernews.com/2026/11/attackers-exploit-unrealircd-flaw-that.html)

**PostgreSQL patches 52 flaws, including a 22-year-old bug that gives a database user code execution.** CVE-2026-6460 (CVSS 8.8) is a composite-type confusion traceable to 2004; Mehmet Ince published a working exploit chain and privately shared proofs of concept with AWS, Azure, Google, Supabase, Databricks, and Ubicloud in August. Update to 18.7, 17.12, 16.16, 15.20, or 14.25, and rebuild every C-language extension at the same time, since old builds "may not be protected." [The Hacker News](https://thehackernews.com/2026/11/postgresql-patches-52-flaws-including.html)

**Mior and Skyfall: a malicious cloud host can read inside AMD SEV-SNP confidential VMs.** ETH Zurich's Mior redirects the security processor's startup writes to a graphics card, leaving part of the memory-ownership table unset, then reads and writes VM memory and forges attestation reports (1,000 of 1,000 attempts on a Zen 5 EPYC); it needs hypervisor and BIOS control. Skyfall (ETH Zurich and Google) leaks register state and a disk-encryption key from Zen 3 and Zen 4 VMs through transient-scheduler timing. AMD's platform firmware fixes arrive in November (Skyfall) and December (Mior). [The Hacker News](https://thehackernews.com/2026/11/new-mior-and-skyfall-attacks-let-rogue.html)

## Cyber Crime & Fraud

**WIRED: AI is fueling a ransomware boom led by lone operators.** Leak-site claims reached nearly 3,000 over the summer, up 20% to 40% from spring by some estimates, with growth mostly outside the US; Halcyon counts about 111 groups claiming attacks in July through September. Fully automated ransomware hasn't arrived, but AI is helping newcomers launch their own operations: "Global Secret Group" listed 48 victims, more than half in one day, and "Storm" 71 in 20 days. ReliaQuest says one new group is run by a teenager who made more than $800,000 in under two weeks. Recorded Future's Allan Liska says attack counts this year already dwarf 2025, while attacks using encryption may fall as upstarts favor pure data extortion. [WIRED](https://www.wired.com/story/beware-the-new-ai-fueled-ransomware-boom/)

**Trezor confirms reseller implants that steal recovery phrases.** [The Hacker News](https://thehackernews.com/2026/11/trezor-confirms-hidden-hardware.html) *Also covered above under Adversary Playbook.*

## Critical Infrastructure Attacks

**VulnCheck discloses 14 root-level flaws in Copeland's Dixell XWEB refrigeration supervisors, one of four controller families hit in the October attack on 700 French supermarkets.** Researcher Valentin Lobstein found the login page "runs the submitted username as a shell command before it ever checks the password"; scores run 8 to 9.8, at least two are exploited in the wild, patches exist, and legacy versions stay exposed. XBOW's Max Günther set up honeypots posing as a pizza chain's refrigeration controllers; within a day attackers probed them and one changed a virtual freezer's temperature. France attributes the October wave to Iran; similar incidents hit refrigeration units owned by the US military. [CyberScoop](https://cyberscoop.com/copeland-dixell-refrigeration-vulnerabilities/)

**Ransomware knocks Belarusian cloud host ActiveCloud offline for days.** [The Record](https://therecord.media/belarus-cloud-provider-activecloud-ransomware-attack) *Also covered above under Adversary Playbook.*

## Executive Leadership Changes

**Cohere names Jaya Baloo its first CISO (reported, unconfirmed).** Baloo, formerly Rapid7's CISO and most recently AISLE's COO and CISO, reportedly joined the Canadian AI company on Nov. 12; CISO Tribune flags it as reported by superpowerdaily.com and not yet confirmed by Cohere. [CISO Tribune](https://www.cisotribune.com/moves)

**JetBlue names Dave MacKinnon VP of technology infrastructure and CISO.** MacKinnon, who comes from N-able, will lead the airline's technology infrastructure and security (announced Nov. 10; first listed after the 11-11 check). [CISO Tribune](https://www.cisotribune.com/moves) (source: JetBlue investor relations)

## Resilience Tactics

**Microsoft 365 is mostly back after a roughly 24-hour outage across 70+ countries, and Microsoft says it was self-inflicted.** Outlook, Exchange Online, Teams, SharePoint, and Copilot failed from about 1:30 p.m. ET Thursday as servers dropped out of health checks and overloaded the rest; Microsoft's first fixes were "not taking as expected." It now says the incident "was introduced by an issue during an earlier network capacity upgrade that surfaced following a recent network change," not a cyberattack or AI agents, and promises a post-incident report; mail queues were stretched to 48 hours. UK police couldn't take online crime reports, NHS referrals and prescriptions backed up, Japan's government fell back to phones, Deutsche Bahn couldn't send timetables, and Cyberwire notes disruptions at OpenAI, Anthropic, US courts, and a Toronto hospital network. Brandon Karpf, who watched telco security chiefs' inboxes go silent at a summit, calls it the third such consistency failure in a year, after AWS us-east-1 and Cloudflare. [WIRED](https://www.wired.com/story/microsoft-365-crawls-back-to-life-after-a-24-hour-outage/); [WIRED](https://www.wired.com/story/the-microsoft-outage-is-a-warning-for-the-world/); [SecurityWeek](https://www.securityweek.com/microsoft-struggles-to-restore-email-and-other-services-in-a-global-outage/); [Cyberwire](https://thecyberwire.com/newsletters/daily-briefing/15/217); [Karpf](https://karpf.substack.com/p/we-tried-to-gentrify-a-jungle) (via Gmail)

**The FAA halted departures nationwide for more than four hours; officials see no hacking.** A communications failure hit the air route traffic control centers on Friday afternoon; the stop lifted at 8:15 p.m. ET, with delays expected for days. Homeland Security Secretary Markwayne Mullin says "we haven't seen any footprints" but isn't ruling an attack out; the FBI is reportedly examining a software update, Transportation Secretary Sean Duffy blames legacy switches and routers flooded with data, and CBS reports an update to the L3Harris-run network that rebooted and crashed. Officials say the FAA's new AI systems played no role. [SecurityWeek](https://www.securityweek.com/no-signs-of-hacking-in-faa-ground-stop-as-fbi-reportedly-probes-software-update/); [FFXnow](https://www.ffxnow.com/) (Dulles impact)

**Newsletter Tracker:** both outages *Support* Thread 3 ("Resilience, not prevention, is the affordable strategy for most organizations"; status: Holding, current statement ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience)). Neither had an attacker, so no prevention control applied; only continuity plans, alternate channels, and tested recovery limited the damage.

## Compliance Trends

**Could state attorneys general shore up the EU-US Data Privacy Framework after *Trump v. Slaughter*?** The Supreme Court's ruling that FTC commissioners can be removed at will undercuts an independence safeguard the EU's adequacy decision explicitly relied on; the EDPB asked the Commission to assess it and Max Schrems wants an "orderly withdraw." The authors propose state attorneys general, independent of the federal executive, as additional DPF enforcers. [IAPP](https://iapp.org/news/a/could-state-attorneys-general-strengthen-the-dpf-after-slaughter)

**Italy finishes transposing the EU AI Act, with criminal liability.** Legislative Decree 160 (Sept. 9) adds corporate and individual criminal liability; Decree 179 (in force Oct. 23) assigns national AI supervisory authorities. The Garante concluded its investigation of Character.AI in July and ruled on an employee sentiment-analysis plug-in, while NIS2 and DORA moved into active supervision. [IAPP](https://iapp.org/news/a/italys-latest-approach-to-ai-privacy-and-cybersecurity)

## Government Surveillance

**Germany's new intelligence law adds AI analysis of bulk data and biometric image matching for both agencies.** [The Record](https://therecord.media/german-parliament-passes-law-giving-spy-agencies-hacking-power) *Also covered above under Nation-State Cyber Policy & Law.*

## Automation Tactics

**The AI kill switch is a stack of controls, not a button, and deployers own most of it.** [Resilient Cyber](https://www.resilientcyber.io/p/there-is-no-big-red-button-for-ai-agents) *Also covered above under AI Singularity Timeline.*

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 66 | 12 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | Contributed | 53 | 26 | 2026-07-14 |
| The Hacker News | Contributed | 78 | 1 | 2026-07-14 |
| The Record | Contributed | 62 | 17 | 2026-07-14 |
| The Canon Project | No Contribution | 18 | 60 | 2026-07-14 |
| FFX Now | No Contribution | 15 | 64 | 2026-07-14 |
| Wired | Contributed | 50 | 26 | 2026-07-20 |
| CyberScoop | Contributed | 36 | 14 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 47 | 2026-09-01 |
| CISA Cybersecurity Advisories | Contributed | 24 | 26 | 2026-09-01 |
| SecurityWeek | Contributed | 45 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 2 | 26 | 2026-10-02 |
| CISO Tribune — The Wire | Contributed | 10 | 10 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 19 | 2026-10-17 |
| EFF Deeplinks | Contributed | 12 | 8 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 6 | 14 | 2026-10-17 |
| IAPP News | Contributed | 14 | 6 | 2026-10-17 |
| CSIS Strategic Technologies Program | Contributed | 2 | 18 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 12 | 2026-10-17 |
| Risky.Biz | No Contribution | 4 | 1 | 2026-11-10 |
| tl;dr sec | No Contribution | 1 | 4 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 4 | 2026-11-10 |
| Resilient Cyber | Contributed | 3 | 2 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | Contributed | 4 | 1 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 3 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 1 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 3 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 0 | 3 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 3 | 2026-11-12 |

**No-contribution detail:**

- **The Canon Project**: no review since *The Ghidra Book* (Nov. 9), covered 11-10.
- **FFX Now**: nine Nov. 13 items, all local news; its Dulles ground-stop alert is the FAA story credited to SecurityWeek. The Nov. 13 Daily Debrief was skipped.
- **CSO Online CISO Appointments**: still no October or November section on the page.
- **LEAP**: the highest wave is still Wave 12 ("Safety Policies").
- **NIST Cybersecurity Insights Blog**: no new post since Oct. 27.
- **(ISC)² Insights**: only the "ISC2 Merch Mart" launch; no CIR fit.
- **AI Alignment Forum**: no posts since Nov. 11 (checked via the site's API).
- **Risky.Biz**: no bulletin after the Nov. 13 issue, covered 11-13.
- **tl;dr sec** (#354) and **Detection Engineering Weekly** (#173): both issues covered 11-13; nothing newer.
- **Epoch AI**: its one in-window post (Huawei's Horinger campus) was covered 11-13.
- **AI as Normal Technology**, **Reflective Altruism**, **Understanding AI (TRIAL)**: no posts in the pull window.
- **Marcus on AI (TRIAL)**: two posts, "The great Generative AI unraveling" (AI-company valuations) and one on the FAA ground stop; neither makes a dated, testable capability claim, so both fail this source's filter.

**Crediting notes:** Gmail is credited for Jeffrey Caruso's and Brandon Karpf's essays. Cyberwire published its first new issue since #214: #217 (Nov. 13) is credited for the Microsoft outage's downstream impacts; #215 now exists but its items (France's Iran attribution, LoSapio's CISA nomination) were covered 11-10 to 11-12, and #216 still returns "Not Found." CISA is credited for the UnrealIRCd KEV addition. Cybersecurity Dive is credited for the White House task force and Unit 42's CL-STA-1238, neither covered elsewhere. The Record's three featured stories were opened individually: NATO's taxi-app guidance (Nov. 12, covered 11-13), the FBI ARTEX alert and the NYC surveillance-pricing ban (both Nov. 13).

**Also checked, not written up:** SecurityWeek's weekly roundup items were covered earlier (OpenAI's ExploitGym report, Glasswing, Railway, ForgeRock connected cars, LoSapio, Vanderbilt, Microsoft's "Lazarus" weight backdoor) or too thin from a one-line summary (Depi's Codex npm prompt-injection chain, Fortinet's MS SQL cryptominer/Gh0st RAT campaign, Siemens' advisory-policy document); its Apple Secure Exclaves explainer had no new event. Cyberwire's StingyBasilisk and ZeroQlik links are held until the primary reports are read; its Operation TorNado item was covered 11-03. The DOJ's Gootloader details repeat the 11-13 Endgame item. IAPP's Barbados-Guyana digital-ID analysis had no new event. WIRED Daily's aviation-AI feature, Nvidia leadership stories, and Stephen Miller interview had no CIR fit; Gmail's local digests, Google Alerts, and lifestyle newsletters had no CIR fit. The Pending Evidence Queue had no pending rows. Rick's Substack feed has no new essay since Nov. 9.

*Pending artifact approvals: none. No open PRs on raceBannon99/nexus-artifacts.*

*No forecast range moved today, so the AI Timeline Forecasting chart in Alexandria's Library (`images/ai-timeline-forecasting.png`) needs no refresh.*
