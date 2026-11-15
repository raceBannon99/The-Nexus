# First Principles Daily Intelligence Report

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

*Sunday, Nov. 15. Covers everything published after the 11-14 run; a quiet weekend pull, with 4 of 29 sources contributing. The headlines: Cursor traced the trojanized Claude Code extension it served on Oct. 29 back to an access key stolen in the Fireworks AI breach, and Uber says the same breach exposed drivers' license data; Italy's privacy regulator fined Meta €805 million over Facebook's Android gallery suggestions; CSIS argues the $6 billion Binance heist was avoidable and that crypto exchanges are funding North Korea's missile program; Iran's threat to cut Gulf undersea cables is back in the news; and Yandex says Yandex Cloud customers without backups permanently lost 2.84% of the data hit by Ukraine's October drone strikes. None of the five forecast ranges moved.*

## Today's CIR Matches

- **Adversary Playbook Activity** — Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically.
- **Data Breaches** — Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4.
- **Privacy** — Corporate and government privacy practices, policy, law, and technology — personal-data handling before anything goes wrong, distinct from Government Surveillance (state collection) and Data Breaches (after-the-fact exposure). Covers privacy legislation (CCPA/CPRA, GDPR's privacy provisions), data-broker/ad-tech tracking, biometric/facial-recognition controversies, privacy-enhancing tech, and AI training-data privacy.
- **Critical Infrastructure Attacks** — Cyberattacks against water, power, internet, and government systems.
- **Cybersecurity Executive Leadership Changes** — New CISO, CSO, CIO, and CTO appointments across organizations generally.
- **Nation State Cyber Policy and Law** — Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam.
- **Cybersecurity Resilience Tactics** — Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures.
- **Compliance Trends** — GDPR, ISO, PCI, and other regulatory fines and requirements.

## AI Timeline Forecasting

1. **Forecasted AGI Milestone Dates:** P5 2029 · P50 2045 · P95 2075: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) Nothing matched AGI Arrival Timeline today; none of the AI-timeline feeds published anything new in the window.

2. **Forecasted Singularity Milestone Timeline:** P5 2032 · P50 2046 · P95 2075: a 43-year uncertainty window and a 50% chance we could reach this milestone in 14 years.(unchanged since 2026-11-06) Nothing matched today. Cursor's Fireworks-key disclosure is a human-run supply-chain compromise with no autonomous AI behavior, so it bears on adversary tracking, not on control timing.

3. **Forecasted Superintelligence Milestone Timeline:** P5 2030 · P50 2046 · P95 2076: a 46-year uncertainty window and a 50% chance we could reach this milestone in 16 years.(unchanged since 2026-11-11) This file remains the most derivative of the five standing forecasts: the AGI range plus a stated one-year gap, not an independent seed. Nothing matched today.

4. **Forecasted Harm Timeline (P(Doom)):** P5 2034 · P50 2063 · P95 2091: a 57-year uncertainty window and a 50% chance we could reach this milestone in 29 years.(unchanged since 2026-11-11) This isn't a prediction that disaster will happen, only a guess at when, if it ever does. It assumes an uncontrollable AI eventually gets built *and* ends up hurting people, then asks: if that's true, around what year would it happen? Entry 5 below answers the separate question of how likely that is in the first place. Nothing matched Harm Timeline today.

5. **Forecasted Harm Probability:** Central ~30% (90% credible interval: 15%–55%): a 40-percentage-point range, with the central estimate sitting 15 points above the low end.(unchanged since 2026-11-03) This answers a different, bounded question from entry 4. Entry 4 asks *when* a system that has escaped meaningful human control would cause harm. This one asks *how likely* that system is to cause a catastrophe killing over 10% of the human population within 10 years of losing control. Nothing matched Harm Probability today.

*Seldon's floor checks: neither the AGI nor the Superintelligence range moved, so no floor or gap-model follow applied. No range moved, so the AI Timeline Forecasting chart in Alexandria's Library needs no refresh.*

## Adversary Playbook

*The Adversary Tracking Report was updated this run: no new rows, 2 rows updated. Active campaigns: 396, unchanged. [Dated snapshot](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-15-adversary-tracking-report.md).*

**Cursor: a key stolen in the Fireworks AI breach led to the trojanized Claude Code extension.** In a Friday update, Cursor says an attacker took an access key it had issued to Fireworks AI, exposed when Fireworks was breached, and used it to copy a read-only storage bucket the two companies shared. The bucket held coding-agent traces, mostly from 2025, from sessions not in Privacy Mode, and some of those traces still contained credentials (fewer than 0.01% of customers' API keys). With those, the attacker reached select Cursor SaaS tools: archived non-production repositories, support emails, usage data, agent-conversation summaries, and credentials users had sent to support. On Oct. 29, a stolen internal credential let the attacker plant trojanized Claude Code builds (2.1.312 and 2.1.313) directly in the cache serving Cursor's extension marketplace. At most 5,000 users may have received them during an 11-hour window. Cursor has moved all inference off Fireworks and reports no malicious activity since Nov. 1. Separately, Uber told California regulators that a service provider's stolen internal credentials were used to take drivers' license data (count undisclosed); TechCrunch reports the provider was Fireworks, which makes Uber the third named downstream victim after Notion and Cursor. Updates to Unclear row 90 (the extension) and Cybercrime row 128 (🤖 "Black October"). [The Hacker News](https://thehackernews.com/2026/11/stolen-fireworks-ai-key-led-to-cursor.html)

## Data Breaches

**Cursor's Fireworks-key root cause exposed support data, archived repos, and some customer credentials; Uber lost drivers' license data in the same chain of breaches.** [The Hacker News](https://thehackernews.com/2026/11/stolen-fireworks-ai-key-led-to-cursor.html) *Also covered above under Adversary Playbook.*

## Privacy

**Italy fines Meta €805 million (about $887 million) over Facebook's Android gallery suggestions.** The Garante found that the feature, on by default since 2023, let the Facebook app read Italian users' photos, videos, and metadata without explicit consent. Gallery access came through a single app-wide permission, and the notice users saw first didn't say it also enabled gallery suggestions. The regulator ruled it a breach of Article 122 of Italy's Privacy Code (its version of the EU ePrivacy Directive), which treats a phone's contents as part of a person's private life, so any access needs free, informed consent whether or not data leaves the device. Meta has 60 days to turn the feature off by default, including for people who already granted access, and to ask for consent separately. The fine, about 0.47% of global revenue, reflects roughly 20 million affected Android users, a breach that is still ongoing, a 2019 decision against the company, and limited cooperation. The regulator rejected Meta's argument that Ireland should handle the case, because ePrivacy has no one-stop-shop mechanism. It did not examine AI training, which Meta denies, but may look separately at a newer cloud-processing feature. Meta calls the fine "disproportionate" and plans to appeal. [SecurityWeek](https://www.securityweek.com/meta-fined-887-million-in-italy-over-android-gallery-photos-and-videos-on-facebook/); [The Hacker News](https://thehackernews.com/2026/11/italy-fines-meta-805-million-over.html)

## Critical Infrastructure Attacks

**Iran's threat to cut undersea internet cables resurfaces.** Matt Devost's Global Frequency leads this week with a Financial Times report that Iran threatens to destroy undersea cables. The FT is paywalled and couldn't be read, so this summary draws on the October reporting it builds on. On Oct. 19, IRGC spokesman Hossein Mohebbi warned that Iran could target the internet cables under the Strait of Hormuz if the US resumes hostilities; another IRGC official named seven major cables. Reuters reported on Oct. 23 that Tehran has detailed plans to hit Gulf communications cables if the US and Israel attack again. This is a threat, not an attack; no cable has been cut. It earns a place here because the cables are bundled through a few chokepoints and, as the 2024 Red Sea cuts showed, take months to repair. [Financial Times](https://www.ft.com/content/492b2c62-8e15-47b3-bf24-842ae62e7217) (paywalled; via [Global Frequency](https://globalfrequency1001.substack.com/p/global-frequency-15-november-2026), Gmail); [GV Wire/Reuters (Oct. 23)](https://gvwire.com/2026/10/23/iran-has-detailed-plans-to-hit-gulf-undersea-cables-if-war-resumes-officials-say/)

## Executive Leadership Changes

**Sean Sweeney becomes CIO of the City of Charleston, South Carolina.** SecurityWeek's Saturday Debrief lists the appointment under People on the Move, with no date or detail. A search found the city's earlier CIO job posting but no announcement, so treat this as SecurityWeek's one-line report and not yet independently confirmed. [SecurityWeek](https://www.securityweek.com/) (People on the Move, Nov. 14 Saturday Debrief; no per-item permalink)

## Nation-State Cyber Policy & Law

**CSIS: the Binance heist was avoidable, and Washington's light touch on crypto keeps funding North Korea.** Taylar Rajic and Nikita Shah recap the Oct. 29 TraderTraitor operation (a LinkedIn fake-interview lure, a separate malicious ad, then most of $6 billion moved out in about 20 minutes) and note that Binance's own security team says it detected and stopped 57 suspected North Korea-linked cases earlier in 2026. North Korea has stolen about $12.8 billion in crypto since 2017, $7.8 billion of it this year, and a 2024 UN panel estimated that stolen crypto funds up to 40% of its defense budget. The authors fault the administration's pro-innovation reluctance to regulate exchanges (including the pardon of Binance cofounder Changpeng Zhao), and note that its memo authorizing private-sector offensive operations against cybercrime bars companies from targeting state-affiliated actors like Lazarus. They call for global standards for protecting crypto transactions, stronger cross-border enforcement, and action against enabling states, especially China, whose banks launder the proceeds. [CSIS](https://www.csis.org/analysis/largest-crypto-heist-history-could-have-been-avoided) **Newsletter Tracker:** this *Complicates* Thread 4 ("Intrusion Kill Chain Prevention, long impractical, is now operationally feasible at scale"; status: Holding, current statement ["The Kill Chain Rises From the Dead"](https://diffuser.substack.com/p/the-kill-chain-rises-from-the-dead)). Fifty-seven stopped attempts against one adversary is what kill-chain prevention at scale looks like, yet one miss cost more than all those successes saved. Feasibility gets judged on the miss rate against the most valuable target, and prevention needs fast containment of the final, minutes-long phase.

## Resilience Tactics

**Yandex says 2.84% of the cloud data hit by Ukraine's October drone strikes is gone for good; customers with backups lost nothing.** Yandex restored access to 97.16% of the affected Yandex Cloud customer data after Ukrainian drone strikes on its Sasovo, Kaluga, and Vladimir data centers on Oct. 7–11. The rest is unrecoverable because of hardware damage and because those customers kept no backups on the platform. Customers who used Yandex's backup tools kept 100% of their data. Backups had to be switched on manually before; Yandex has now made them the default for new virtual machines. The 2.84% covers only data touched by the strikes, not all of Yandex Cloud. The strikes themselves were covered 10-13 and are tracked under the Russia-Ukraine data-center-strike campaign, a row not updated today since there was no new strike. Reported Nov. 10 and surfaced this run by Global Frequency. [Reuters](https://www.reuters.com/technology/russias-yandex-says-nearly-3-cloud-customer-data-lost-after-attacks-2026-11-10/) (via [Global Frequency](https://globalfrequency1001.substack.com/p/global-frequency-15-november-2026), Gmail); [Meduza](https://meduza.io/en/news/2026/11/10/yandex-admits-it-cannot-restore-nearly-3-of-customer-data-in-yandex-cloud-after-ukrainian-attacks) **Newsletter Tracker:** this *Supports* Thread 3 ("Resilience, not prevention, is the affordable strategy for most organizations"; status: Holding, current statement ["Peacemaker for Resilience"](https://diffuser.substack.com/p/peacemaker-for-resilience)). No customer could have prevented a missile strike on its provider's building; the only control that mattered was an off-site backup, and every customer who had one came through whole.

## Compliance Trends

**Italy's Garante fines Meta €805 million under the ePrivacy rules and orders the gallery feature off by default within 60 days.** [SecurityWeek](https://www.securityweek.com/meta-fined-887-million-in-italy-over-android-gallery-photos-and-videos-on-facebook/); [The Hacker News](https://thehackernews.com/2026/11/italy-fines-meta-805-million-over.html) *Also covered above under Privacy.*

---

## Source Contribution Scorecard

| Source | Today | All-Time Contributed | All-Time No Contribution | Active Since |
|---|---|---|---|---|
| Gmail Newsletters | Contributed | 67 | 12 | 2026-07-14 |
| N2K Cyberwire Daily Briefing | No Contribution | 53 | 27 | 2026-07-14 |
| The Hacker News | Contributed | 79 | 1 | 2026-07-14 |
| The Record | No Contribution | 62 | 18 | 2026-07-14 |
| The Canon Project | No Contribution | 18 | 61 | 2026-07-14 |
| FFX Now | No Contribution | 15 | 65 | 2026-07-14 |
| Wired | No Contribution | 50 | 27 | 2026-07-20 |
| CyberScoop | No Contribution | 36 | 15 | 2026-09-01 |
| CSO Online CISO Appointments | No Contribution | 3 | 48 | 2026-09-01 |
| CISA Cybersecurity Advisories | No Contribution | 24 | 27 | 2026-09-01 |
| SecurityWeek | Contributed | 46 | 5 | 2026-09-01 |
| Forecasting Research Institute — LEAP | No Contribution | 2 | 27 | 2026-10-02 |
| CISO Tribune — The Wire | No Contribution | 10 | 11 | 2026-10-17 |
| NIST Cybersecurity Insights Blog | No Contribution | 1 | 20 | 2026-10-17 |
| EFF Deeplinks | No Contribution | 12 | 9 | 2026-10-17 |
| (ISC)² Insights | No Contribution | 6 | 15 | 2026-10-17 |
| IAPP News | No Contribution | 14 | 7 | 2026-10-17 |
| CSIS Strategic Technologies Program | Contributed | 3 | 18 | 2026-10-17 |
| AI Alignment Forum | No Contribution | 8 | 13 | 2026-10-17 |
| Risky.Biz | No Contribution | 4 | 2 | 2026-11-10 |
| tl;dr sec | No Contribution | 1 | 5 | 2026-11-10 |
| Detection Engineering Weekly | No Contribution | 1 | 5 | 2026-11-10 |
| Resilient Cyber | No Contribution | 3 | 3 | 2026-11-10 |
| Cybersecurity Dive (TRIAL) | No Contribution | 4 | 2 | 2026-11-10 |
| AI as Normal Technology | No Contribution | 0 | 4 | 2026-11-12 |
| Epoch AI | No Contribution | 2 | 2 | 2026-11-12 |
| Reflective Altruism | No Contribution | 0 | 4 | 2026-11-12 |
| Understanding AI (TRIAL) | No Contribution | 0 | 4 | 2026-11-12 |
| Marcus on AI (TRIAL) | No Contribution | 0 | 4 | 2026-11-12 |

**No-contribution detail:**

- **N2K Cyberwire**: the newest issue is still #217 (Nov. 13), covered 11-14; no weekend issues.
- **The Record**: nothing newer than Nov. 13; all three featured stories (NATO taxi app, FBI ARTEX alert, NYC surveillance pricing) and every Nov. 13 item were covered 11-13 or 11-14.
- **The Canon Project**: no review since *The Ghidra Book* (Nov. 9), covered 11-10.
- **FFX Now**: nothing published after Nov. 13 (all checked 11-14).
- **Wired**: its newest item, the AI-fueled ransomware feature, was covered 11-14.
- **CyberScoop**: its Pall Mall Process guidelines story repeats the event covered 11-12; the Copeland refrigeration piece was covered 11-14.
- **CSO Online CISO Appointments**: still no October or November section on the page.
- **CISA**: no advisory after the Nov. 13 KEV update, covered 11-14.
- **LEAP**: the highest wave is still Wave 12 ("Safety Policies").
- **CISO Tribune**: newest moves (Cohere, JetBlue) covered 11-14.
- **NIST Cybersecurity Insights Blog**: no new post since Oct. 27.
- **EFF Deeplinks**, **IAPP News**: newest items covered 11-14.
- **(ISC)² Insights**: only the "ISC2 Merch Mart" launch; no CIR fit.
- **AI Alignment Forum**: no posts since Nov. 11 (checked via the site's API).
- **Risky.Biz**: no bulletin after the Nov. 13 issue, covered 11-13.
- **tl;dr sec** (#354) and **Detection Engineering Weekly** (#173): both covered 11-13; nothing newer.
- **Resilient Cyber**: its kill-switch essay was covered 11-14.
- **Cybersecurity Dive (TRIAL)**: its three newest items (White House task force, CL-STA-1238, the North Korea crypto crackdown) were covered 11-13 or 11-14.
- **AI as Normal Technology**, **Epoch AI**, **Reflective Altruism**, **Understanding AI (TRIAL)**: no posts in the pull window.
- **Marcus on AI (TRIAL)**: no new posts; the two in the window were judged 11-14.

**Crediting notes:** Gmail is credited for Matt Devost's Global Frequency (the Iran cable item and the Yandex Cloud data-loss item). The Hacker News is credited for Cursor's root cause and the Meta fine. SecurityWeek reported the Meta fine first (Nov. 14) and is also credited for the Charleston CIO from its Saturday Debrief. CSIS is credited for the Binance commentary. The Hacker News article pages loaded over plain curl today with no Cloudflare challenge, the first clean fetch since 11-03.

**Also checked, not written up:** SecurityWeek's Saturday Debrief (Top Headlines, Nov. 9–13) arrived after the 11-14 run. Its items were either covered 11-10 to 11-14 or dated before the pull window: Plex2Shell exploitation against QNAP NAS users, a Chrome/Firefox batch of 180+ fixes, and the Intel/AMD Patch Tuesday, which earlier runs passed on. Its funding items (Bay, Daylight, Dreeze, Finite State, and others) have no CIR fit. Joshua Goldfarb's SecurityWeek column, "Is AI Making Us Worse at Cybersecurity?", is opinion with no new data. The FBI's North Korea deepfake-video-call item (The Hacker News) repeats the FaceStealer takedown covered 11-13. The rest of Global Frequency's links (Vanderbilt, France's Iran attribution, the FAA ground stop, Patch Tuesday volume) were covered 11-11 to 11-14; its content-piracy, delivery-robot, space-asset, and in-space-assembly links had no CIR fit. Bruce Schneier's monthly Crypto-Gram reprints his blog's past month. CISO Tradecraft's deepfake-identity essay, Google Alerts, InsideNoVa, and lifestyle newsletters had no CIR fit. The Pending Evidence Queue had no pending rows. Rick's Substack feed has no new essay since Nov. 9.

*Pending artifact approvals: none. No open PRs on raceBannon99/nexus-artifacts.*

*No forecast range moved today, so the AI Timeline Forecasting chart in Alexandria's Library (`images/ai-timeline-forecasting.png`) needs no refresh.*
