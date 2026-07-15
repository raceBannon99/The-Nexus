---
title: "Harmony Horizon Bridge Hack — Cyber Kill Chain Analysis"
date: 2026-07-15
question: "Analyze the Harmony Horizon Bridge hack (June 2022, ~$100M, DPRK/Lazarus attributed) through the Lockheed Martin Cyber Kill Chain — what did the hackers do at each phase?"
format: intelligence-brief
agents: [Sherlock, Alexandria, Euclid, Popper, Seldon, Turing]
---

# Harmony Horizon Bridge Hack — Cyber Kill Chain Analysis

## Bottom Line

On June 23, 2022, at 11:06 UTC, attackers drained roughly $100M (~$99.6M) in ETH, BNB, USDC, USDT, BUSD, WBTC, and DAI from Harmony's Horizon Bridge, using compromised multisig keys to authorize a handful of fraudulent withdrawals. That theft — the *Actions on Objectives* phase — is the best-evidenced fact in this entire report: it is an immutable, independently verifiable on-chain event that anyone with a block explorer can confirm today. Everything the kill chain says happened *before* that moment rests on a single source: Harmony's own self-published post-mortem, written by a victim with strong institutional incentive to frame a widely-criticized security design (an undersized multisig, publicly flagged as risky before the hack) as an unstoppable nation-state operation rather than a preventable failure.

This produces an evidentiary inversion that is the central finding of this brief: the kill chain phase that is *easiest to verify* (the theft itself) is also the *last* one, while the phases that require the most trust — reconnaissance, weaponization, delivery, exploitation, installation, and command-and-control — are attested by exactly one interested party and, in several places (weaponization and C2 above all), by no Harmony-specific evidence at all. Where Harmony's account is thin, the natural instinct is to fill gaps with the well-documented Ronin/Axie Infinity heist (fake LinkedIn recruiter, malicious PDF "offer letter," same actor) — but that is pattern-matching from a *different* incident, not evidence about Harmony, and this brief marks every such inference accordingly.

The attack's underlying logic holds regardless of the disputed details (Harmony says 2-of-4 multisig and 11 transactions; Halborn, Elliptic, and CFR say 2-of-5 and 14 transactions — a discrepancy that is itself a signal of how thin third-party visibility into this incident is): a minority of total signers was sufficient to authorize withdrawal, meaning the real attack surface was the people holding keys, not the smart contract. Attribution to Lazarus Group/APT38/DPRK is MO-consistent and independently claimed by both Elliptic (within about a week) and the FBI (January 2023) — but neither has disclosed methodology, and Lazarus is the default explanation attached to nearly every DPRK-adjacent crypto theft in this era, which carries real anchoring-bias risk alongside genuinely strong multi-dimensional MO overlap with Ronin.

**Confidence in this bottom line: high** for the theft mechanics and laundering path (on-chain, multi-sourced); **low-to-moderate** for the pre-theft kill chain narrative (single-sourced, self-interested); **moderate** for attribution (independent convergence, undisclosed methodology, real anchoring risk).

## The Kill Chain, Phase by Phase

Each phase below is labeled with its evidence tier. **Tier 1** facts are multi-sourced and independently verifiable on-chain. **Tier 2** claims are sourced only to Harmony's own post-mortem (Jack Chan, Medium, mirrored on Harmony's forum) — read every "Harmony states" or "Harmony has claimed" below as exactly that and no more. **Tier 3** content is not attested for Harmony at all; it is imported by analogy from the Ronin/Axie Infinity hack or the general CISA/FBI/Treasury TraderTraitor advisory (AA22-108A, April 2022), and is flagged explicitly wherever it appears.

### 1. Reconnaissance — Tier 2
Harmony states that server logs showed attacker(s) "reviewing the Horizon Bridge implementations as early as June 2, 2022" — three weeks before the theft. No other party has independently confirmed this log evidence, its retention chain, or its interpretation. Treat this as Harmony's claim about its own logs, not a verified finding.

### 2. Weaponization — Tier 3 (total evidentiary gap for Harmony)
There is **zero** Harmony-specific evidence here. Harmony's account says only that the attacker used "malicious software" / "trojan-horse software" — no malware family, file hash, or toolset has ever been publicly disclosed, by Harmony or anyone else. Any statement about *what* was actually built or used is necessarily an inference from the general DPRK/TraderTraitor toolkit described in the CISA advisory or from Ronin, where Mandiant and Sky Mavis did publish concrete malware detail. That specificity does not exist for Harmony. If you read a confident description of "the malware" used against Harmony anywhere, it is not sourced to this incident.

### 3. Delivery — Tier 2, with a Tier 3 shadow
Harmony states the initial vector was "a phishing scheme to trick at least one software developer to install malicious software on their laptop," occurring around June 17, 2022. Harmony never specified the channel — email, LinkedIn, Telegram, and a fake job offer are all plausible but unconfirmed for this incident. The well-documented Ronin precedent (a Sky Mavis engineer lured via a fake LinkedIn recruiter and a malicious PDF "offer letter") is frequently cited as *the* Harmony delivery mechanism in secondary coverage — that is a Tier 3 inference by analogy, not a Harmony-specific fact. It is also unclear from Harmony's account whether one developer or multiple were targeted.

### 4. Exploitation — Tier 2
Harmony states the malware gave the attacker the ability to "read chat threads to understand how to operate the bridge, and/or gain access to non-public bridge infrastructure code." Separately, Harmony describes a June 18 vulnerability in a software package used by its internal "subgraph" service that exposed the addresses of all servers in its private cloud — and states this was chained into the same intrusion. No CVE identifier or package name has been disclosed for this vulnerability. This phase, like the two before it, depends entirely on Harmony's own account of its own compromise.

### 5. Installation — Tier 2
Harmony states the attackers obtained "backdoor access to one or more servers," and that decrypting the bridge's signing keys required operations "performed on servers with privileged access." This is a materially significant claim: it implies the attacker was operating *inside* the trusted signing environment itself, not merely exfiltrating a static key file from disk. No backdoor or implant name has ever been published, and this claim — like Reconnaissance through Exploitation — has never been corroborated by an independent forensic firm.

### 6. Command and Control — Tier 3 (total evidentiary gap for Harmony)
There is no Harmony-specific public reporting on C2 infrastructure — no IP addresses, no domains, no protocol detail. This is a complete gap, not a thin claim; nothing in Harmony's post-mortem addresses it, and no third party has filled it in. Any assumption about C2 tradecraft here is imported wholesale from general DPRK/Lazarus TTPs, not observed in this case.

### 7. Actions on Objectives — Tier 1
At 11:06:46 UTC on June 23, 2022, the attacker used the compromised signing keys to authorize fraudulent withdrawals — roughly $100M across 11 transactions per Harmony and CNBC, or 14 per Halborn and CFR — draining assets affecting an estimated ~64,000 wallets holding bridged tokens. This phase is independently, immutably verifiable by anyone with a block explorer, and it is the only phase in this kill chain that does not depend on Harmony's word. The laundering that followed is equally well-evidenced: stolen tokens were immediately swapped into ~85,837 ETH via Uniswap, then batched into Tornado Cash starting June 27, 2022 (Elliptic notes idle periods in the laundering cadence consistent with APAC nighttime hours). Roughly $60M more moved through the RAILGUN privacy protocol starting January 13, 2023, partially converted to BTC. Total recovery to date: 124 BTC (~$2.84M, roughly 2.8% of the theft), frozen years ago — nothing further has been recovered since.

## Attribution: How Solid Is "Lazarus Group / DPRK"?

Attribution should be read as **MO-consistent and independently claimed by Elliptic and the FBI, with anchoring-bias risk explicitly named** — not as flatly established fact, and it should not be conflated with the on-chain facts above, which are independently verifiable by anyone.

- Elliptic attributed the hack to Lazarus/APT38 within about a week (by June 30, 2022) via blockchain-forensic wallet clustering; Chainalysis corroborated. The FBI issued a press release "confirming" Lazarus/APT38/DPRK on January 23, 2023 — seven months later — tying it to WMD/missile-program funding and the broader "TraderTraitor" campaign. Neither Elliptic nor the FBI has publicly disclosed the underlying methodology for either call, and it is not established whether the FBI's assessment is independently derived or substantially a ratification of the same private-sector clustering analysis that seeded the public narrative.
- Working against over-confidence: Lazarus is the default attribution for nearly every DPRK-adjacent crypto theft in this era, creating genuine pattern-matching risk — reflexively attaching the name to a new incident is not the same as proving it.
- Working for the attribution, beyond reputation alone: the MO overlap with Ronin and the broader TraderTraitor pattern is strong on several independent dimensions at once — a spear-phished developer lured with a fake job/coding-test pretext, trojanized software as the entry point, a bridge/custody infrastructure target, and laundering funneled through Tornado Cash. That combination of features co-occurring is more diagnostic than any single element would be alone.

## The Evidence Discrepancies, Stated Plainly

Two factual disputes exist in public reporting and neither has been resolved — both are left explicit rather than silently picking a side, because the disagreement is itself informative about how thin outside visibility into this incident really is:

- **Multisig threshold:** Harmony's own post-mortem says 2-of-4. Most third-party sources — Halborn, Elliptic, the Council on Foreign Relations — say 2-of-5.
- **Transaction count:** Harmony and CNBC report 11 fraudulent transactions. Halborn and CFR report 14.

Separately, Harmony's 2-of-4/5 multisig had already been publicly criticized as reckless *before* the hack: a Chainstride Capital founder had predicted a "9-figure hack" on Twitter, and CertiK had flagged the low signer threshold. That prior public criticism is the direct conflict of interest behind Tier 2 in this report — it does not mean the phishing/trojan story is false, but it is the reason a single self-interested account is the sole source for six of this kill chain's seven phases.

## What Doesn't Depend on the Disputed Details

Two structural facts about this attack hold true regardless of whether the multisig was 2-of-4 or 2-of-5, and regardless of whether 11 or 14 transactions were used:

1. A **minority of total signers** was sufficient to authorize withdrawal from the bridge. The exploited attack surface was the people holding keys, not the underlying infrastructure or smart contract logic.
2. The attacker needed to **persist across multiple compromised signers without detection** long enough to accumulate signing authority, regardless of the exact threshold required.

(A third candidate invariant — "large, fast extraction over stealth once signing authority is obtained" — was considered and rejected: that behavior is expected and unremarkable once an attacker holds sufficient keys, and isn't diagnostic of this actor or attack specifically.)

## Forward Look: What's Likely Next

| Forecast | Confidence | Basis |
|---|---|---|
| No material further fund recovery | ~90-95% (i.e., ~5-10% chance of any further recovery; ~0% of majority recovery) | Only 124 BTC (~2.8%) recovered to date, all years ago from the BTC leg. Industry-wide crypto theft recovery rates are falling, not rising (~21.2% recovered industry-wide in Q1 2024 vs. ~0.4% in Q1 2025), even as total DPRK-attributed theft roughly doubled year-over-year (~$2.02B in 2025; ~$6.75B cumulative). RAILGUN, where most remaining Harmony funds were shielded from January 2023, is fully decentralized with no operator to sanction or seize — unlike Tornado Cash or the Sinbad.io mixer (seized Nov. 2023 by Treasury/FBI/Dutch FIOD, citing Harmony/Axie-linked laundering), and that seizure did not unwind funds already shielded. |
| No fuller technical disclosure (malware name, C2 infrastructure, delivery vector) | ~85-90% (i.e., ~10-15% chance of disclosure) | The evidentiary window is functionally closed four years on. Contrast with Ronin (Mandiant/Sky Mavis published concrete forensics within about a year) and Bybit (Feb. 2025 — Safe{Wallet}, Sygnia, NCC Group, and TRM Labs published detailed forensics within *weeks*). Harmony has produced neither, then or since; device images, logs, and cloud records have likely degraded past recoverability, and Harmony's institutional incentive and resources to fund retrospective forensics have shrunk as its relevance has declined. |
| Kill-chain pattern has moved up the stack, industry-wide | ~75% | Harmony and Ronin (2022) targeted a bridge operator's own employee directly to obtain validator/signing keys. Bybit (Feb. 2025, $1.5B, the largest crypto heist on record, also Lazarus/TraderTraitor-attributed) instead targeted a *third-party shared infrastructure vendor* — Safe{Wallet}, multisig tooling used industry-wide — via a compromised developer workstation, injecting malicious JavaScript to spoof the transaction-signing UI during a routine transfer. This is a supply-chain pivot: compromising one shared vendor trusted by many operators, rather than each operator individually. This forecast leans on the general DPRK trend and Bybit-specific data, not on new Harmony-specific confirmation, and should be read as pattern-based extrapolation. |
| Blind-signing/transaction-spoofing becomes a more prominent technique | ~60% | Precisely because it defeats the fix the industry drew from Ronin and Harmony ("raise the multisig threshold") — Bybit's multisig was far more robust than Harmony's 2-of-5 and was defeated anyway, because signers were shown false data rather than facing a weak threshold. The one constant from 2022 to 2025: initial access is still human-targeted social engineering against someone holding privileged access, not a smart-contract bug or brute force. |
| A new, dedicated Harmony-specific indictment or civil action | ~10-15% | DPRK operators remain unreachable for individual prosecution; DOJ's established pattern (per the 2018/2021 Park Jin Hyok precedent) bundles incidents into omnibus indictments rather than pursuing case-by-case action. Four years of quiet through two natural trigger points — the January 2023 FBI attribution and the November 2023 Sinbad sanctions — without dedicated Harmony action is itself informative. |
| Harmony cited as a line item in a *future broader* DPRK sanctions/indictment package | ~35-40% | Consistent with the cumulative-bundling pattern already observed: the Sinbad sanctions cited Harmony/Axie-linked laundering, and the January 2025 joint multi-agency statement addressed DPRK crypto theft broadly rather than incident-by-incident. |

## Open Questions

- What malware family or toolset was actually used? (Zero Harmony-specific evidence exists.)
- What was the actual delivery channel — email, LinkedIn, Telegram, a fake job offer — and was it one developer or several? (Unconfirmed; the Ronin fake-recruiter/PDF vector is an analogy, not a Harmony finding.)
- What C2 infrastructure did the attacker use? (Total public gap.)
- What was the exact privilege-escalation mechanic that turned "backdoor on a server" into "ability to decrypt bridge signing keys"? (Harmony's account asserts the outcome but not the mechanism.)
- Was the subgraph-service vulnerability (June 18) genuinely chained into the same intrusion, or a parallel/coincidental finding folded into a single narrative after the fact? (No CVE or package name has ever been published to check this against.)
- Does the FBI's January 2023 attribution reflect independent investigative work, or substantially a ratification of Elliptic's earlier private-sector wallet-clustering call? (Neither party has disclosed methodology.)
- Is the 2-of-4 vs. 2-of-5 / 11-vs-14-transaction discrepancy a matter of definitional differences (e.g., counting a batch differently) or a sign that no party outside Harmony ever had full visibility into the incident?

## What This Means for Rick

Treat this report as two separate documents fused into one. The back half — the theft and laundering — is about as solid as crypto forensics gets: on-chain, immutable, checkable by anyone. The front half — everything that explains *how* the attackers got in — is a single company's account of its own worst day, told by the only party with both the full picture and a strong reason to shape it. Both things can be true at once: the phishing-and-trojan story is plausible and consistent with Lazarus's well-documented MO at Ronin, *and* it is the only account we have, from a source that had already been publicly warned its multisig was too weak before the hack happened. The forward-looking signal worth tracking is the Bybit comparison: the industry's post-Harmony fix (raise the signer threshold) was already circumvented by a smarter attack (spoof what the signers see) within three years — so "harden the multisig" alone should not be treated as a durable defense going forward.
