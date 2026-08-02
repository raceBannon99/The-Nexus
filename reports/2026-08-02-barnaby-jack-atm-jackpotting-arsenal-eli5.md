# ELI5: Barnaby Jack's ATM Jackpotting Demo and the Arsenal Showcase (2010)

**Question:** Explain, simply, the origin-history report's timeline entry: "2010: The late Barnaby Jack made two ATMs dispense cash live on stage ('ATM jackpotting'); the Arsenal open-source tool showcase was added the same year."

## Alexandria — What do we already know?

Nothing in the artifact library covers this. Yesterday's Black Hat/DEF CON origin-history report carries a single compressed sentence — this report builds it out, and corrects a small mixup in how the question was framed.

**One correction worth flagging up front: both events happened at Black Hat, not DEF CON.** The question as asked names "Black Hat DEFCON" together; the origin-history report's own timeline places both the ATM demo and Arsenal's launch specifically under Black Hat's 2010 column, not DEF CON's. Worth being precise about, since the two conferences ran (and still run) the same week but aren't the same event.

## Sherlock — What are the facts?

**ELI5 first, then the sourced detail.**

**ELI5, the ATM demo:** A security researcher named Barnaby Jack wanted to prove something simple: the ATM machines you see in gas stations and bars — not bank-lobby ones, the standalone kind — could be made to just start spraying out cash on command, like a slot machine, without anyone swiping a card or entering a PIN. He bought two of these machines himself, found the security holes in each one, and did it live on stage in front of an audience: the machine lit up, played a little tune, flashed the word "JACKPOT" on its screen, and started dispensing bills. He showed it two different ways — one where he plugged in a USB drive and installed his own software directly into the machine, and one where he did the whole thing remotely, over the network, without even touching it. The point wasn't to rob anyone — it was to force ATM manufacturers, an industry that hadn't really been under this kind of scrutiny before, to take their security as seriously as, say, Microsoft had been forced to after a decade of attacks.

**ELI5, Arsenal:** The same year, Black Hat added a new, more casual section of the conference called Arsenal — basically a room where researchers set up tables and demo their own free security tools in person, let people ask questions and try them out, rather than giving a formal stage talk. It's less "watch me present" and more "come poke at the thing I built."

**The sourced facts, with names and dates confirmed:**

- **The presentation, "Jackpotting Automated Teller Machines Redux," was actually delivered at Black Hat USA 2010** — but Jack had originally planned to give it a year earlier, at **Black Hat 2009**, and it was pulled from the schedule before then.
- **Why the 2009 talk was pulled has a small, unresolved ambiguity in this pass's sourcing.** One account (Computerworld) describes it plainly as the ATM vendors themselves asking for more time to patch the vulnerabilities Jack had found. A separate contemporaneous piece (Risky Business, from a 2009 blog post) frames it more pointedly, titled "Juniper Networks Gags 'ATM Jackpot' Researcher" — Jack's employer at the time was Juniper Networks, and that headline suggests internal/employer pressure, not just vendor-requested delay. This report can't fully resolve which framing is more accurate from the sources checked — see Popper.
- **Jack changed employers between the two talks — from Juniper Networks to IOActive, where he became Director of Embedded Device Security** — and the 2010 talk went ahead under IOActive's backing.
- **The two ATM brands he demonstrated against, by name: Triton and Tranax** — both makers of the free-standing, non-bank-lobby ATMs common in convenience stores and bars, the kind more likely to be poorly secured or unmonitored than a bank's own lobby machines.
- **His own direct quotes on why it mattered:** *"The goal of the talk is to spark discussion on the best ways to remediate."* And, more pointedly about the ATM industry specifically: *"It's time to give these devices an overhaul. Companies who manufacture the devices aren't Microsoft. They haven't had 10 years of continual attacks against them."*
- **Arsenal launched as its own dedicated section of Black Hat starting in 2010**, specifically designed to give researchers and the open-source security community a live, hands-on, conversational venue for showcasing tools — distinct from a formal briefing-style talk. It has run every year since and remains a standard part of Black Hat's program today.
- **Barnaby Jack's later work extended the same "prove it live" approach to a much higher-stakes target: implanted medical devices** — insulin pumps and pacemakers — research that reportedly influenced FDA regulatory changes around device security in 2012. He died on **July 25, 2013**, one week before he was scheduled to present new medical-device hacking research at that year's Black Hat.

## Euclid — What must be fundamentally true?

Two structural facts connect these two 2010 entries, even though they look unrelated at first glance:

- **The ATM demo and Arsenal's launch are both instances of the same underlying shift: Black Hat moving from "tell me about it" to "show me, live, in a form I can touch."** A stage talk describing a vulnerability is one register of proof; a machine on stage physically spitting out cash is a different, higher register — and Arsenal institutionalized that same instinct (demonstration over description) as its own permanent category, rather than leaving it to individual speakers to decide how dramatic to make their proof. Both are 2010 expressions of Black Hat leaning further into "working exploit code and live demos" as its core credibility mechanism — the same mechanism yesterday's origin-history report identified as the through-line connecting Ciscogate, Back Orifice, and DEF CON's whole founding logic.
- **The 2009-to-2010 delay on Jack's talk is the same corporate-pressure pattern Ciscogate established five years earlier, just resolved more quietly.** Where Ciscogate involved lawyers physically cutting pages out of a printed program and a subsequent lawsuit, the ATM story (on the account that vendors requested more patch time, rather than Juniper actively suppressing it) resolves through a comparatively ordinary, cooperative delay — a year to fix things, then the talk goes ahead. Whether that's because ATM vendors handled it better than Cisco/ISS did in 2005, or because this report simply doesn't have the full picture of what pressure Jack was actually under at Juniper, is exactly the kind of distinction Popper should weigh in on.

## Popper — How could we be wrong?

1. **The reason for the 2009 pull is the biggest open question in this report, and it matters for how sympathetically the story reads.** "Vendors asked for more time to patch" (Computerworld's framing) is a fairly benign, cooperative-disclosure story. "Juniper Networks Gags... Researcher" (Risky Business's framing, from closer to the actual 2009 event) suggests something closer to employer-driven suppression, echoing Ciscogate's dynamic more directly. This report presents both without resolving which is more accurate — a primary source (Jack's own contemporaneous statement, or Juniper's own account) would be needed to settle it.
2. **This report didn't verify whether Triton and Tranax (the two ATM makers named) issued any public response** to being named in the demo, the way Cisco and Adobe did in the Ciscogate and Sklyarov stories already documented — that's a real gap if the full corporate-response picture matters for comparison across these stories.
3. **The claim that Arsenal "has run every year since" is asserted from general knowledge of Black Hat's current program structure**, not independently re-verified for every single year 2010–2026 in this pass — a plausible, low-risk claim given Arsenal's clear continued presence in recent Black Hat materials, but not a year-by-year confirmed fact.

## Seldon — What is likely to happen next?

Addressing Popper's three points: point 1 (the 2009 pull's real cause) doesn't resolve through more reasoning — it needs either Jack's own contemporaneous account (he's since passed away, making this harder to newly source) or Juniper's own statement from that period, neither located in this pass. Worth flagging as a genuine, likely-permanent gap rather than something a future search is likely to close easily. Point 2 (Triton/Tranax's response) would need a separate, targeted search if Rick wants the vendor side of the story specifically. Point 3 (Arsenal's continuity) is low-stakes and doesn't need further verification unless a specific year's status matters for some other purpose.

No forward-looking forecast is warranted — both events are closed historical facts from 2010, and Arsenal's continued existence is a settled, observable current fact rather than an uncertain future one.

## Tufte — How do we make this clear?

A short timeline separates the two storylines (the delayed talk, and Arsenal's launch) clearly, since they're parallel 2010 developments rather than one causing the other:

| Date | ATM jackpotting | Arsenal |
|---|---|---|
| 2009 | Talk scheduled for Black Hat, then pulled — reason disputed between sources (vendor-requested delay vs. employer pressure) | — |
| Between 2009–2010 | Jack leaves Juniper Networks for IOActive (Director of Embedded Device Security) | — |
| **2010** | "Jackpotting Automated Teller Machines Redux" delivered live at Black Hat — two ATMs (Triton, Tranax) made to dispense cash via USB-installed and remote-network methods | Arsenal launches as a new, dedicated Black Hat section for live, hands-on open-source security tool demos |
| 2012 | (Jack's later medical-device work reportedly influences FDA device-security regulation) | Arsenal continues annually as a standard part of Black Hat's program |
| July 25, 2013 | Jack dies, one week before a scheduled Black Hat talk on medical-device hacking | — |

## Turing — Should any of this become a skill?

No. This was a one-off historical-explainer question, well-served by direct research rather than a repeatable procedure.

## Sources

**Primary/journalism (contemporaneous and retrospective)**
- [ATM Hacking Video - Barnaby Jack Demonstrates ATM Hacking at Black Hat USA 2010, SecurityWeek](https://www.securityweek.com/atm-hacking-video-barnaby-jack-demonstrates-atm-hacking-black-hat-usa-2010/) — confirms the 2010 Black Hat venue and general demo description.
- [Barnaby Jack hits ATM jackpot at Black Hat, Computerworld](http://www.computerworld.com/article/2519671/computer-hardware/barnaby-jack-hits-atm-jackpot-at-black-hat.html) — source for the Triton/Tranax vendor names, the "vendors asked for more time to patch" framing of the 2009 pull, both direct quotes from Jack, and the "Jackpot" program's on-screen/audio behavior.
- [Juniper Networks Gags "ATM Jackpot" Researcher, Risky Business (2009)](https://risky.biz/news_and_opinion/patrick-gray/2009-06-30/juniper-networks-gags-atm-jackpot-researcher/) — the competing, more pointed framing of the 2009 pull, cited here specifically to preserve the ambiguity rather than resolve it in either direction — see Popper point 1.
- [Barnaby Jack, Wikipedia](https://en.wikipedia.org/wiki/Barnaby_Jack) — source for the USB/remote dual attack-method description, his later medical-device work and its regulatory influence, and the July 25, 2013 date of his death.

**Official/institutional**
- [Black Hat | Arsenal](https://blackhat.com/html/arsenal.html) — confirms Arsenal's purpose (open-source tool showcase, live/conversational format) and its 2010 origin.

**Prior Nexus report (context)**
- [The Origin Stories of Black Hat, DEF CON, and BSides Las Vegas, and How They Evolved](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-defcon-origin-history.md) — source of the original compressed timeline entry this report expands on, and confirmation that both events belong to Black Hat's column specifically, not DEF CON's.

## New Skills

None. See Turing's note above.

## Library Recommendations

**Recommended: a short fact-sheet on the ATM jackpotting story and Arsenal's founding**, adapted from this report's Sherlock/Tufte content. This is durable reference material — both are closed historical facts (Arsenal's continued existence aside, which is a stable, low-maintenance claim), directly reusable if a future question touches embedded-device security history, Black Hat's program evolution, or Barnaby Jack's broader career. Category: `fact-sheet`. Status: recommended, awaiting Rick's decision — not yet submitted to `nexus-artifacts`.
