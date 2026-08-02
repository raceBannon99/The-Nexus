# ELI5: "Ciscogate" and Moss Selling Black Hat (2005)

**Question:** Explain, simply, the origin-history report's timeline entry: "2005 — 'Ciscogate': Mike Lynn's suppressed Cisco IOS talk; front page of the WSJ. Same year, Moss sells Black Hat to CMP Media."

## Alexandria — What do we already know?

Nothing in the artifact library covers this. Yesterday's Black Hat/DEF CON origin-history report carries a compressed paragraph on Ciscogate with the core shape of the story right, but this report goes deeper into the actual mechanics (exactly what was suppressed, how, and how the lawsuit resolved) and separately researches the Moss/CMP Media sale, which the origin report only noted in one clause without detail.

## Sherlock — What are the facts?

**ELI5 first, then the sourced detail.**

**ELI5 — Ciscogate:** A security researcher named Michael Lynn found a serious bug in the software that runs Cisco's routers — the boxes that move a huge chunk of the internet's traffic. He was scheduled to explain it at Black Hat. Cisco and his own employer got scared and tried to make the talk disappear: they literally had lawyers **rip 30 pages out of the printed conference handbook** the morning of the talk, and yanked the CD with his slides. Lynn's employer told him not to give the talk at all. He stood up anyway, wearing a hat that said "Good," quit his job on the spot, and gave the real talk — explaining exactly how an attacker could take over a Cisco router completely. Cisco and his old employer then sued him and Black Hat. It ended in a settlement: Lynn had to hand over his research to get wiped and agree never to talk about it again. But the story was already out, front-page WSJ material, and it became a landmark moment in the fight over whether researchers are allowed to tell the truth about security holes even when the company that made the broken thing doesn't want to hear it.

**ELI5 — Moss selling Black Hat:** That same year, Jeff Moss (the guy who started both DEF CON and Black Hat) sold Black Hat — just Black Hat, not DEF CON — to a media company called CMP Media, for a reported **$13.9 million**. He kept running Black Hat day-to-day as an employee of the new owner, and he **kept DEF CON entirely for himself**, personally owned, completely separate. It's the moment the "professional" side of what Moss built formally became a corporate media asset, while the "underground" side stayed independent.

**The sourced facts, with exact dates (confirmed against Wikipedia's dedicated Ciscogate page and contemporaneous coverage):**

- **The talk was scheduled for July 27, 2005**, at Black Hat Briefings in Las Vegas. The suppression effort began the day before, **July 26**.
- **On the morning of July 26, attendees found 30 pages physically torn out** of the printed conference proceedings, at Cisco's request — and the accompanying CD-ROM of presentation slides was withheld entirely. Black Hat itself printed an apologetic insert acknowledging it: *"Due to some last minute changes beyond Black Hat's control...the included materials aren't up to the standards Black Hat tries to meet."*
- **Lynn's employer, ISS (Internet Security Systems, later part of IBM), had actually approved the talk originally, then reversed course two days before it was scheduled**, per his lawyer's account. ISS's own spokesperson, Roger Fortier, gave a softer public explanation: *"The decision was made on Monday to pull the presentation because we wanted to make sure the research was fully baked."*
- **On stage, Lynn started with a decoy topic (VoIP security), then pivoted back to the real subject** — the Cisco router vulnerability — and disclosed the technical details anyway, saying he'd rather resign than keep it quiet. (The origin-history report's detail about a hat reading "Good" is consistent with contemporaneous retrospective coverage of the talk, though this pass's direct source-checking focused on the suppression/lawsuit mechanics rather than re-confirming the hat detail specifically.)
- **Cisco and ISS then jointly sued both Lynn and Black Hat.** Their legal claims were specific: that ISS held copyright over the presentation itself, that Cisco owned copyright over the decompiled machine code Lynn had reverse-engineered to find the bug, and that the material contained trade secrets.
- **The case settled rather than going to trial.** Terms: Lynn had to hand over forensic images of all his research data to a neutral third party, then erase his own copies — and he was **permanently barred from discussing the vulnerability again**, ever. The FBI reportedly showed up asking questions during the conference itself, though no arrest warrant was issued.
- **The Black Hat sale: November 2005, to CMP Media** (a subsidiary of the UK's United Business Media, now part of Informa — the same lineage confirmed in yesterday's origin-history report). The reported price was **$13.9 million**, per multiple sources — one source found in this pass cited a lower figure (~$10 million), a discrepancy this report couldn't fully resolve (see Popper). **Moss stayed on as Director of Black Hat under the new ownership, and — separately confirmed — kept DEF CON entirely under his own personal ownership**, outside the sale.

## Euclid — What must be fundamentally true?

Two things have to both be true for this pair of 2005 events to belong on the same timeline entry, and they're more connected than the compressed original bullet suggests:

- **Ciscogate is the clearest possible demonstration of exactly the tension Black Hat was founded to manage, and it happened at the worst possible moment for that tension to become visible.** Yesterday's origin-history report established that Black Hat exists specifically because DEF CON's informal culture made it hard for corporate security professionals to get their trip expensed — Black Hat was built to be the *safe, professional* venue. Ciscogate is a corporation using lawyers, employment pressure, and a lawsuit to try to control what happens on that "safe" stage — the exact opposite of what made the underlying research credible in the first place. It's a direct stress-test of Black Hat's founding premise, playing out in public, in the same year Moss sold ownership of the event.
- **Selling Black Hat months after Ciscogate is not necessarily "cause and effect," but the timing makes the sale read differently than a routine business transaction would.** A conference that just proved it could survive a major corporation and a lawsuit trying to control its content — and came out with front-page WSJ credibility rather than a reputation for caving — was a more valuable, more legitimate asset in November 2005 than it would have been in January. Whether or not Ciscogate directly motivated CMP's interest or Moss's decision to sell (this report found no direct source connecting the two events causally), the sale price and terms (Moss staying on, DEF CON deliberately excluded) suggest a business being sold at a moment of real, demonstrated institutional credibility, not being cashed out under duress.

## Popper — How could we be wrong?

1. **The Black Hat sale price has a real discrepancy across sources that this report couldn't resolve.** Multiple sources converge on $13.9 million, but one source found in this pass's research cited roughly $10 million. This report presents $13.9 million as the better-supported figure (multiple independent citations vs. one), but doesn't have a definitive primary-source (e.g., an SEC filing or CMP's own press release with an exact number) to settle it conclusively.
2. **This report did not independently re-verify the "Good" hat detail** carried over from the origin-history report — it's consistent with how the story is generally told in retrospective coverage, but this pass's direct source-checking (Wikipedia's Ciscogate page, contemporaneous coverage) focused on the suppression and lawsuit mechanics rather than re-confirming that specific visual detail from a primary photo or first-person account.
3. **No direct source found connects Ciscogate causally to Moss's decision to sell Black Hat** — Euclid's reasoning above is explicitly framed as "the timing makes the sale read differently," not as a documented cause. It's plausible the sale process was already underway well before July 2005 and simply happened to close in November of the same year, making the connection coincidental rather than causal. This report doesn't have evidence to distinguish between those two possibilities.
4. **The settlement terms found here (forensic wipe, permanent gag on the topic) come from Wikipedia's own account** — a generally reliable but secondary source for this kind of legal detail. This pass didn't independently pull the actual settlement/injunction filing to confirm the exact wording of the terms.

## Seldon — What is likely to happen next?

Addressing Popper's four points: point 1 (sale price discrepancy) would need a primary financial document (SEC filing, CMP press release) to resolve definitively — worth a targeted follow-up search if the exact figure matters for a specific purpose, but $13.9 million is the better-supported number as things stand from this pass. Point 2 (the hat detail) is a minor, low-stakes gap that doesn't affect the substance of the story — not worth further research unless Rick specifically wants it nailed down. Point 3 (causal link between Ciscogate and the sale) doesn't resolve through more reasoning — it needs either a direct Moss interview addressing the timing, or business-press coverage from that specific window describing when sale talks began, neither of which this report has. Point 4 (settlement terms sourcing) is a reasonable secondary-source citation for legal detail that isn't disputed anywhere else this report checked — treated as reliable, not certain.

No forward-looking forecast is warranted — this is a closed historical episode from 2005 with a settled legal outcome and a completed business transaction, not a question involving future uncertainty.

## Tufte — How do we make this clear?

A short timeline table separates the two intertwined but distinct 2005 storylines (the suppression fight, and the ownership sale) so a reader can see they're parallel events in the same year rather than one causing the other:

| Date | Ciscogate | Black Hat ownership |
|---|---|---|
| ~2 days before the talk | ISS reverses its earlier approval, tells Lynn not to present | — |
| July 26, 2005 | Cisco has 30 pages physically removed from the printed proceedings; slide CD withheld | — |
| July 27, 2005 | Lynn gives the talk anyway, discloses the vulnerability, resigns from ISS on the spot | — |
| Following weeks | Cisco and ISS sue Lynn and Black Hat jointly | — |
| (settlement, date not independently pinned down this pass) | Case settles: Lynn's research wiped by a third party; permanently barred from discussing the vulnerability | — |
| November 2005 | — | Moss sells Black Hat to CMP Media (~$13.9M reported); stays on as Director; keeps DEF CON personally, outside the sale |

## Turing — Should any of this become a skill?

No. This was a one-off historical-explainer question, well-served by direct research rather than a repeatable procedure.

## Sources

**Primary/encyclopedic**
- [Ciscogate, Wikipedia](https://en.wikipedia.org/wiki/Ciscogate) — source for the exact dates, the 30-page removal detail and Black Hat's own printed disclaimer quote, ISS's shifting position and spokesperson quote, the on-stage pivot from VoIP back to the real topic, the lawsuit's specific legal claims, and the settlement terms (forensic wipe, permanent gag).

**Journalism/contemporaneous**
- [CMP Media dons Black Hat, The Register (Nov 17, 2005)](https://www.theregister.com/2005/11/17/cmp_buys_black_hat/) — source for the sale date, a lower reported price point (~$10M, flagged as a discrepancy — see Popper), Moss's continued role as Director of Black Hat, and CMP's stated commitment to keep Black Hat editorially separate.
- Web search aggregation (multiple outlets, not individually re-verified line-by-line) — source for the more commonly cited $13.9 million sale figure and confirmation that DEF CON was excluded from the sale and remained under Moss's personal ownership.

**Prior Nexus report (context)**
- [The Origin Stories of Black Hat, DEF CON, and BSides Las Vegas, and How They Evolved](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-defcon-origin-history.md) — source of the original compressed timeline entry this report expands on, and of Black Hat's founding premise (the "professional front door" framing Euclid's reasoning above builds on).

## New Skills

None. See Turing's note above.

## Library Recommendations

**Recommended: a short fact-sheet on Ciscogate and the 2005 Black Hat/CMP Media sale**, adapted from this report's Sherlock/Tufte content. This is durable reference material — a landmark vulnerability-disclosure case with a closed legal outcome, directly reusable if a future question touches disclosure-norms history, Black Hat's ownership lineage, or corporate pressure on security researchers (the same theme already connecting the Sklyarov case and the NSA-surveillance talks documented elsewhere in this report series). Category: `fact-sheet`. Status: recommended, awaiting Rick's decision — not yet submitted to `nexus-artifacts`.
