# The Origin Stories of Black Hat, DEF CON, and BSides Las Vegas, and How They Evolved

**Question:** What is the origin story of Black Hat and its sister conference DEF CON, how has each evolved over the years, what are the major milestones for each, what books discuss their history (including confirming Joe Menn's *Cult of the Dead Cow* as a Cybersecurity Canon Hall of Fame book), and a timeline of major events.

**Update (2026-07-27):** Added BSides Las Vegas — held the same week as Black Hat and DEF CON — per Rick's request. This is an Update Pass: Sherlock (new facts), Euclid (revised framing — a third event changes the shape of the answer, not just its length), Popper (re-review — BSides bears directly on the "corporate vs. authentic" objection already raised), Seldon (addressing the re-review), and Tufte (the timeline table now carries three conferences) all re-ran. Turing's conclusion is unchanged.

## Alexandria — What do we already know?

Nothing in the artifact library or prior Nexus reports covers the history of any of the three conferences — today's two other Black Hat reports (bookstore hours and signing schedules) are pure logistics with no historical content. This is a clean-slate research question. One note worth carrying forward: unlike those two logistics reports, this one produces durable reference material — see the Library Recommendation at the end.

## Sherlock — What are the facts?

**DEF CON came first, by accident, in 1993.** Jeff Moss — known by the handle "The Dark Tangent" — was an 18-year-old member of Platinum Net, a BBS network for Canadian hackers. A friend on the network was leaving town and asked Moss to throw him a farewell party in Las Vegas. The friend left early; Moss was left holding a party with no guest of honor, so he opened it up to everyone on his network instead. About 100 people showed up at the Sands Hotel. It went well enough that attendees asked him to do it again — DEF CON has run every year since. The name comes from two sources at once: the 1983 film *WarGames* (in which Las Vegas is depicted as a nuclear target — "DEFCON" being the U.S. military's readiness scale), and phreaker culture, since "DEF" is also the 3-3-3 keypad reference tied to the word. "The Dark Tangent" itself is a misremembered reference to a comic book called *D'Arc Tangent*.

**Black Hat is a deliberate spinoff of DEF CON, created by the same person for a specific, practical reason.** By 1997 Moss recognized a problem: DEF CON's chaotic, party-first culture made it nearly impossible for security professionals at established companies to get their employer to cover the trip as a legitimate business expense. So he created a second, more corporate-flavored conference — Black Hat Briefings — scheduled deliberately in the same city, the same week, immediately *before* DEF CON, so attendees could expense the "professional" event and stay in town for the "party" one. The first Black Hat ran July 7–10, 1997. Its official pitch: "the Black Hat Briefings will put your engineers and software programmers face-to-face with today's cutting edge computer security experts and 'hackers.'" The inaugural speaker lineup included Mudge (secure coding), Bruce Schneier (cryptography), Adam Shostack (code review), and Dominique Brezinski (Windows NT attacks); the keynote was futurist Richard Thieme. Microsoft attended that first year, and later became a sponsor.

**Both conferences' authority comes from the same underlying mechanism**, not two different ones: neither was designed top-down by an institution — both trace to one individual's personal network and grew by word of mouth and reputation, which is precisely what gave the "hacker perspective" its credibility with corporate and government audiences once they started paying attention.

### Key inflection points, DEF CON

- **1994 (DEF CON 2):** Attendance nearly doubled to ~200, moved to the Sahara Hotel — first sign the 1993 gathering wasn't a one-off.
- **1996 (DEF CON 4):** First Capture the Flag competition — a format that would become one of DEF CON's defining cultural exports.
- **1999 (DEF CON 7):** Cult of the Dead Cow released Back Orifice 2000, then DEF CON's largest-ever presentation.
- **2001:** Russian programmer Dmitry Sklyarov was arrested the day *after* the conference for writing e-book decryption software — a DMCA case that became a flashpoint in the security research/free-speech debate.
- **2007:** An NBC reporter's attempt at covert filming was discovered in advance; Moss publicly outed her to the assembled crowd.
- **2010 (DEF CON 18):** Attendance passed 8,000, at the Riviera Hotel.
- **2012 (DEF CON 20):** NSA Director Gen. Keith Alexander gave the keynote and publicly denied domestic surveillance programs — a claim the 2013 Snowden/PRISM revelations directly contradicted less than a year later.
- **2013 (DEF CON 21):** In direct response, Moss asked federal agencies not to attend that year — "I think it would be best for everyone involved if the feds call a 'time-out.'"
- **2016 (DEF CON 24):** DARPA's Cyber Grand Challenge AI system "Mayhem" won its all-machine competition and then entered the humans-only CTF (finishing last); it received the first Black Badge ever awarded to a non-human entity, later displayed at the Smithsonian.
- **2017 (DEF CON 25):** The first Voting Machine Village found researchers breaching dozens of voting machines, sparking national election-security debate; separately, Marcus Hutchins ("MalwareTech" — credited with stopping WannaCry) was arrested by the FBI at the airport after the conference.
- **2020 (DEF CON 28):** COVID cancelled the in-person event; replaced by the fully virtual "DEF CON Safe Mode."
- **2024 (DEF CON 32):** Caesars Entertainment abruptly cancelled its venue contract (speculated to be linked to a 2023 ransomware attack and a bomb-scare incident), forcing a relocation to the Las Vegas Convention Center.

### Key inflection points, Black Hat

- **2001:** James Bamford (author of *The Puzzle Palace*) gave a talk on NSA surveillance history — 12 years before Snowden, and itself a preview of the same tension that would surface again at DEF CON in 2012–2013.
- **2005 — "Ciscogate":** Researcher Michael Lynn prepared a talk on a critical Cisco IOS router vulnerability. Cisco and Lynn's employer (ISS) pressured him and Black Hat's organizers to suppress it — even sending lawyers to physically cut the relevant pages out of the printed proceedings. Lynn quit his job, gave the talk anyway wearing a hat that said "Good," and was subsequently sued. The incident made the front page of *The Wall Street Journal* and became a formative case study in vulnerability-disclosure norms. **The same year, Moss sold Black Hat to CMP Media** (now part of Informa).
- **2006 (approx.):** Joanna Rutkowska's "Blue Pill" talk — a rootkit built on x86 virtualization, claimed to be undetectable — became one of Black Hat's most-cited technical talks.
- **Late 2000s:** International expansion begins — Amsterdam and Tokyo editions, Washington D.C./Federal events, eventually formal Europe and Asia tracks.
- **2008:** Three attendees expelled for packet-sniffing the press network.
- **2010:** The late Barnaby Jack made two ATMs dispense cash live on stage ("ATM jackpotting"); the Arsenal open-source tool showcase was added the same year.
- **2015:** Charlie Miller and Chris Valasek remotely hacked a Jeep Cherokee while *Wired* journalist Andy Greenberg drove it at 70 mph — killing the engine and disabling the brakes — one of the most widely covered hacking demonstrations in mainstream media history.
- **2018:** Informa Tech acquired Black Hat from UBM.
- **2022:** 25th-anniversary edition; by this point Black Hat runs a formal Code of Conduct, scholarship programs, and diversity-focused programming — a marked shift from, as one long-time attendee recalled, splitting the cheapest bottle of wine on the menu four ways in a hotel room in the early years.
- **Today:** Black Hat runs annual editions in Las Vegas, London, Singapore, and Riyadh.

### The third event: BSides Las Vegas (founded 2009)

**BSides Las Vegas is not a spinoff of DEF CON or Black Hat in the way Black Hat is a spinoff of DEF CON — it's a reaction against both, and its origin story rhymes with DEF CON's own founding.** In the summer of 2009, Black Hat USA announced that year's speaker lineup; a number of submitted talks didn't make the cut simply because there wasn't room. What started as scattered disappointment on Twitter, Facebook, and email among the rejected submitters turned into a plan, driven mainly by Mike Dahn, Jack Daniel, and Chris Nickerson (with Mike Murray and Jennifer Leggio helping shape the logistics), to host those rejected talks anyway — in a rented vacation house, for a small crowd, deliberately without the scale or corporate structure Black Hat had by then acquired. Dahn's original working name was "Security Fringe"; friends talked him into "Security BSides" instead, borrowing the vinyl-record term for the non-hit side of a single — a direct, self-aware metaphor for "the talks that didn't make the main stage." The first BSides ran July 29–30, 2009, with roughly 200 people, and by most accounts was as much a party as a conference — a description almost identical to how DEF CON's own 1993 debut is remembered.

**Growth mirrored DEF CON and Black Hat's own trajectories, just compressed into a shorter timeline.** BSides Las Vegas soon relocated from the original rented house to the Tuscany Suites and Casino. The format proved exportable: by 2010 the BSides model had spread to roughly ten other cities (Berlin, Ottawa, Dallas, Denver, Boston, Austin, San Francisco among them); 2011 brought the first UK event (London) and over 40 BSides events globally that year; by its 10th anniversary in 2019, BSides events had run in 194 countries; by 2020 the global network had produced more than 600 individual events. BSides Las Vegas itself became one of the three legs of what the security community now informally calls **"Hacker Summer Camp"** — the single week in Las Vegas when BSidesLV, Black Hat, and DEF CON all run back-to-back, drawing overlapping but distinct crowds to the same city.

### Books on the conferences' history

Rick's fact-check is correct: ***Cult of the Dead Cow: How the Original Hacking Supergroup Might Just Save the World*** by Joseph Menn (2019) **is a Cybersecurity Canon Hall of Fame book** — confirmed via the Cybersecurity Canon Project's own review, originally published on Palo Alto Networks' blog ("Cybersecurity Canon Book Review: Cult of the Dead Cow"). It's not a history of DEF CON or Black Hat as institutions, though — it's a group biography of the Cult of the Dead Cow (cDc), the hacktivist collective founded in 1984 (predating DEF CON by nine years) whose members were deeply embedded in the culture that produced both conferences, including the revelation that 2020 presidential candidate Beto O'Rourke was a former cDc member. Treat it as essential *cultural* context for the world DEF CON emerged from, not a chronicle of the conferences' own founding or business history — see Popper below.

Other titles worth knowing about, cross-referenced against DEF CON's own official recommended-reading list (`defcon.org/html/links/book-list.html`, "Underground Culture" section) — a primary source in its own right for what the conference considers its literary canon, though it appears not to have been updated recently (Menn's 2019 book doesn't appear on it):

- ***Hackers: Heroes of the Computer Revolution*** by Steven Levy — the foundational account of the hacker ethic that predates and frames both conferences' culture.
- ***The Cuckoo's Egg*** by Cliff Stoll — an early, formative account of computer-espionage tracking that shaped how the security community understood itself.
- ***Kingpin: How One Hacker Took Over the Billion-Dollar Cybercrime Underground*** by Kevin Poulsen — on DEF CON's own list; covers the cybercrime side of the same era.
- ***Cyberpunk: Outlaws and Hackers on the Computer Frontier*** by Katie Hafner and John Markoff, and ***The Hacker Crackdown*** by Bruce Sterling — both cover the early-1990s hacker-underground and law-enforcement climate (including the 1990 Operation Sundevil raids) that DEF CON was founded directly into.

None of these four were independently re-verified against CyberCanon's own Hall of Fame list this pass (see Popper) — they're carried here on DEF CON's own recommendation and general reputation, not confirmed Canon status.

## Euclid — What must be fundamentally true?

Adding BSides doesn't just extend the timeline — it completes a pattern that was only half-visible with two conferences. Three structural facts now do more to explain "how these events evolved" than any single incident on the timeline:

- **Black Hat's existence is causally downstream of DEF CON's, not parallel to it.** It wasn't founded independently and later associated with DEF CON — it was built to solve one specific problem DEF CON's culture created (expense reports), by the same founder, scheduled deliberately adjacent in time and space. Every later divergence between the two — Black Hat's corporate sponsorship, its acquisition history, its Code of Conduct — traces back to that founding split between "the professional front door" and "the community back room" of the same underlying world.
- **BSides Las Vegas is causally downstream of Black Hat's formalization, in the same shape as Black Hat was once downstream of DEF CON's informality — just running the same logic in reverse.** DEF CON in 1993 was an accident born of exclusion (no guest of honor, so everyone was invited instead). Black Hat in 1997 was a deliberate correction to DEF CON's informality (too chaotic to expense). BSides in 2009 was a deliberate correction to Black Hat's own formalization twelve years later (too selective a CFP, too corporate a room) — and it corrected by reaching back for exactly DEF CON's original texture: a rented house, an unplanned guest list, a party that happened to have talks. **This is a three-beat cycle, not two isolated founding stories**: informal → formalized in reaction → re-informalized in reaction to the formalization. Recognizing the cycle changes what the "milestones" mean — they're not just things that happened to each conference independently, they're the visible symptoms of the same institutional pendulum swinging across three iterations.
- **All three events' legitimacy was earned the same way: by giving independent researchers a real platform regardless of who employed them, before the institutions that needed to hear from them understood why that mattered.** That's what got Microsoft into the room in 1997, what made Ciscogate a legible scandal rather than an obscure dispute in 2005, what makes a sitting NSA Director's denial at DEF CON in 2012 look so different in hindsight after 2013, and what BSides explicitly re-asserted in 2009 when it judged that Black Hat's own selection process had started leaving good talks on the floor. The "milestones" on all three timelines are mostly instances of this same mechanism playing out against a bigger stage each time, or in BSides' case, a deliberately smaller one.

## Popper — How could we be wrong?

**Re-reviewed for the update pass**, since BSides bears directly on point 1 below. Five points worth taking seriously:

1. **The "corporate Black Hat vs. authentic DEF CON" framing this kind of history invites is an oversimplification — and BSides is evidence for the objection, not a refutation of it.** DEF CON itself is now a heavily sponsored, tens-of-thousands-attendee event with its own Code of Conduct-equivalent norms; "Spot the Fed" reads as much like nostalgic tradition today as genuine adversarial tension, especially outside the one-year 2013 exception. Meanwhile Black Hat still produces content as edgy as anything at DEF CON — the 2015 Jeep hack and 2010 ATM jackpotting weren't sanitized corporate briefings. But BSides' entire founding premise in 2009 was that Black Hat *had* become too corporate and selective to hold all the community's good talks — that's not Nexus's framing, that's the founders' own stated reason for existing. The honest position isn't "the binary is false," it's narrower: the binary was real enough in 2009 to motivate a whole new event, but it doesn't hold as a *permanent, static* description of either conference today — both DEF CON and Black Hat have moved since, and BSides itself has scaled to 600+ global events by 2020, undermining any claim that it alone stayed "pure" either.
2. **Cult of the Dead Cow is not a history of the conferences, and presenting it as "the book that discusses their history" risks setting the wrong expectation.** It's a biography of one hacking collective (founded 1984, nine years before DEF CON existed) whose members happened to move in the same world. A reader hoping for an institutional account of how DEF CON or Black Hat were run, financed, or governed over time won't find that here — they'll find rich cultural context for the world both conferences emerged from, which is valuable but a different thing.
3. **Retrospective "milestone" timelines like this one have a built-in selection bias.** Sources like DarkReading's 25th-anniversary piece and Wikipedia's event lists are compiled from what made a good story afterward — legal fights, celebrity hacks, arrests — not necessarily what mattered most to the conferences' actual trajectory (steady multi-decade attendance growth, the proliferation of "Villages," the slow professionalization of the vulnerability-disclosure norms both conferences helped establish). Read the timeline below as "the most tellable version of events," not an exhaustive institutional record. BSides' own history is thinner-sourced than the other two (mainly Wikipedia and BSidesLV's own about page, no equivalent of DarkReading's oral-history retrospective) — treat its entry in the timeline as reliable on the founding facts but less richly cross-corroborated than DEF CON's or Black Hat's entries.
4. **The four supplementary books listed (Levy, Stoll, Poulsen, Hafner/Markoff/Sterling) were not independently checked against CyberCanon's Hall of Fame list this pass** — carried on DEF CON's own recommendation, which is a real endorsement but not the same claim as "Nexus confirmed Canon status," and shouldn't be read as equivalent to the *Cult of the Dead Cow* confirmation.
5. **BSides Las Vegas is one instance of a now-global franchise, and this report only covers the flagship.** By 2020 there were 600+ BSides events across many countries; this report's "founded 2009, in Las Vegas" story is the origin of the whole movement, but every other city's BSides has its own local founding story this report doesn't cover. That's the right scope for a question specifically about the Las Vegas conference week, but worth being explicit about so it isn't mistaken for a claim about BSides globally.

## Seldon — What is likely to happen next?

Addressing Popper's five points: point 1 is resolved by narrowing the claim rather than dropping it — Euclid's three-beat cycle (informal → formalized → re-informalized) already captures that the corporate/authentic binary was real enough in 2009 to found a conference over, while also noting BSides' own subsequent 600-event global scale-up means it can't be held up as the permanently "pure" counterpoint either. No further revision needed beyond what's already written. Point 2 is resolved the same way as before — the book's description already states plainly that it's cultural context, not institutional history. Point 3 doesn't get resolved by more research; it's a property of how this kind of history gets written and reported, correctly flagged rather than fixed, and now extended to note BSides' thinner sourcing specifically. Point 4 remains an open item — those four titles' Canon status would need a working cybercanon.org search session to confirm. Point 5 (BSides-the-franchise vs. BSidesLV-the-flagship) is a scope clarification, not something to forecast — it's resolved simply by stating the scope plainly, which Popper's point already does.

One forward-looking read, given Rick is attending next week: the three-beat cycle Euclid identified raises a real question — does a fourth beat happen? If BSides itself formalizes enough (and 600+ global events with an established brand is a long way from a rented vacation house), does *something* eventually splinter off from BSides Las Vegas the way BSides once splintered off from Black Hat? The range for how many years out a comparable "reaction event" might emerge specifically within the Las Vegas Hacker Summer Camp week — a fourth event founded in explicit reaction to BSidesLV's own institutionalization — runs from about **5 to 20+ years, with a median around 12**, and there's a real chance it simply doesn't happen in a clean, nameable way at all (the "Villages" inside DEF CON may already be quietly performing this function via internal fragmentation rather than an external spinoff). The short end assumes the same institutional-pendulum dynamics that produced Black Hat (1997) and BSides (2009) keep operating on a similar ~12-year cadence; the long end assumes BSides' already-decentralized, low-barrier-to-entry format (any city can run one) relieves exactly the pressure that motivated the two prior splits, making a Las Vegas-specific fourth event less likely than the historical pattern alone would suggest. This is speculative pattern-matching from two prior data points, not a measured forecast — two instances of a cycle is a weak base rate to project a third from, and should be read as an interesting question raised by the history, not a prediction to bank on.

## Tufte — How do we make this clear?

The combined chronological timeline now carries a third column instead of two — and that structural change is itself the point Euclid's analysis makes visually. A reader scanning left to right in 2009 sees Black Hat's "Late 2000s" corporate-expansion row sitting directly across from BSides' founding row: the same rough period produced both further institutionalization at Black Hat *and* a reaction against it, side by side, which is a much sharper way to see Euclid's three-beat cycle than the prose alone.

| Year | DEF CON | Black Hat | BSides Las Vegas |
|---|---|---|---|
| 1993 | **Founded** — accidental farewell party turns into DEF CON 1, Sands Hotel, ~100 attendees | — | — |
| 1994 | DEF CON 2 — attendance ~200, Sahara Hotel | — | — |
| 1996 | DEF CON 4 — first Capture the Flag competition | — | — |
| 1997 | — | **Founded** — spun off from DEF CON to solve the "can't expense the party" problem; July 7–10, right before DEF CON 5 | — |
| 1999 | DEF CON 7 — Cult of the Dead Cow releases Back Orifice 2000, then the largest talk in DEF CON history | — | — |
| 2001 | Dmitry Sklyarov arrested the day after the conference (DMCA case) | James Bamford's NSA-history talk previews the whistleblower-vs-traitor debate, 12 years before Snowden | — |
| 2005 | — | **"Ciscogate"** — Mike Lynn's suppressed Cisco IOS talk; front page of the WSJ. Same year, Moss sells Black Hat to CMP Media | — |
| ~2006 | — | Joanna Rutkowska's "Blue Pill" rootkit talk | — |
| 2007 | NBC reporter's covert filming attempt discovered and outed on stage | — | — |
| Late 2000s | — | International expansion begins: Amsterdam, Tokyo, D.C./Federal editions | — |
| 2009 | — | — | **Founded** — a reaction to that same year's Black Hat CFP rejections; rented vacation house, ~200 people, July 29–30 |
| 2010 | DEF CON 18 — attendance passes 8,000, Riviera Hotel | Barnaby Jack's live ATM jackpotting demo; Arsenal tool showcase added | Format spreads to ~10 other cities |
| 2011 | — | — | First UK event (London); 40+ BSides events globally |
| 2012 | DEF CON 20 — NSA Director Gen. Keith Alexander keynotes, denies domestic surveillance | — | — |
| 2013 | DEF CON 21 — Moss asks federal agencies to skip the conference, months before Snowden/PRISM vindicates the 2012 denial's critics | — | — |
| 2015 | — | Miller & Valasek remotely hack a Jeep at 70 mph with a *Wired* reporter driving | — |
| 2016 | DEF CON 24 — DARPA's "Mayhem" AI wins the Cyber Grand Challenge and earns the first non-human Black Badge | — | — |
| 2017 | DEF CON 25 — first Voting Machine Village; Marcus Hutchins arrested by the FBI after the conference | — | — |
| 2018 | — | Informa Tech acquires Black Hat from UBM | — |
| 2019 | — | — | 10th anniversary; BSides events have run in 194 countries |
| 2020 | DEF CON 28 — COVID cancels the in-person event; "DEF CON Safe Mode" goes fully virtual | — | Global network passes 600 total events |
| 2022 | — | 25th anniversary; formal Code of Conduct, scholarship programs | — |
| 2024 | DEF CON 32 — Caesars cancels its venue contract; relocation to Las Vegas Convention Center | — | — |
| 2026 | — | 29th year; Rick attends | Held the same week, as part of "Hacker Summer Camp" |

## Turing — Should any of this become a skill?

No. This was a one-off historical research question — real depth was needed, but not a repeatable technique or tool integration distinct enough to encode as a skill.

## Sources

**Primary/official**
- [Cybersecurity Canon Book Review: Cult of the Dead Cow, Palo Alto Networks](https://www.paloaltonetworks.com/blog/2020/01/cyber-canon-cult-of-the-dead-cow/) — confirms Hall of Fame status for Joseph Menn's book; published under the Cybersecurity Canon Project's own review program.
- [DEF CON® Hacking Conference: Required Reading list](https://defcon.org/html/links/book-list.html) — DEF CON's own official recommended-reading list; source for the four supplementary "Underground Culture" titles.
- [Black Hat Conference 2026, Routledge/Taylor & Francis](https://www.routledge.com/go/black-hat-conference) — corroborates Black Hat's current scale and 2026 programming context (cross-referenced from today's companion report).

**Encyclopedic/reference**
- [DEF CON, Wikipedia](https://en.wikipedia.org/wiki/DEF_CON) — primary source for the DEF CON chronology, badge/CTF culture, and government-involvement history.
- [Black Hat (conference), Wikipedia](https://en.wikipedia.org/wiki/Black_Hat_(conference)) — primary source for the Black Hat chronology, ownership history, and international expansion.
- [Security BSides, Wikipedia](https://en.wikipedia.org/wiki/Security_BSides) — source for BSides' founding story, name origin, and global-expansion figures (update pass).
- [About BSidesLV, bsideslv.org](https://bsideslv.org/about) — BSides Las Vegas's own account of its founding and philosophy, including the move from a rented house to Tuscany Suites and Casino (update pass).

**Journalism/retrospective**
- [Looking Back at 25 Years of Black Hat, Dark Reading (Andrada Fiscutean, Aug 10, 2022)](https://www.darkreading.com/cyber-risk/looking-back-at-25-years-of-black-hat) — first-person recollections from Adam Shostack, Jeremy Rauch, Richard Thieme, and Ira Winkler on Black Hat's founding, Ciscogate, and the "growing up" of the conference culture; source for most of the direct quotes above.
- Web search aggregation (multiple outlets, not individually re-verified line-by-line) — corroborating detail on DEF CON's 1993 founding story and Jeff Moss/"Dark Tangent" name origin.

**Book (subject of the question)**
- *Cult of the Dead Cow: How the Original Hacking Supergroup Might Just Save the World* by Joseph Menn (PublicAffairs, 2019) — [publisher page](https://www.hachettebookgroup.com/titles/joseph-menn/cult-of-the-dead-cow/9781541762374/).

## New Skills

None. See Turing's note above.

## Library Recommendations

**Recommended: a fact-sheet on Black Hat, DEF CON, and BSides Las Vegas's origin history and combined timeline**, adapted from this report's Sherlock/Euclid/Tufte content. Unlike today's two Black Hat bookstore/schedule reports (explicitly not recommended, since conference logistics go stale within weeks), this content is durable — the three-beat founding cycle (informal → formalized → re-informalized), the causal relationships between all three events, and the historical timeline through 2024 won't need revision for years, and would be directly reusable if a future question touches any of the three conferences' history, culture, or a related book. The BSides addition, if anything, strengthens the case for archiving — Euclid's three-beat pattern is a more original and durable analytical finding than the original two-conference version had. Category: `fact-sheet`. Status: recommended, awaiting Rick's decision — not yet submitted to `nexus-artifacts`.
