# Black Hat USA 2026 — Taylor & Francis / CRC Press Bookstore & Author Meet & Greet

**Question:** CRC Press has its own bookstore at Black Hat, located at Booth 8603 in the Business Hall, with its own book signing schedule. Build the same tables for this bookstore.

**Companion report:** this is a second, separate bookstore from the one covered in [2026-07-27's Black Hat Bookstore & Book Signing Schedule report](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-book-signing-schedule.md) (the Professional Programs Bookstore at Breakers Registration Desk, Level 2). The two are run by different organizers, in different locations, with structurally different schedules — see Euclid's note below.

## Alexandria — What do we already know?

Nothing in the artifact library covers CRC Press or a Taylor & Francis presence at Black Hat. The one relevant precedent is the sibling report above, published earlier today — it establishes the format (hours table + day/time/author/book/Canon-status schedule table) this report mirrors, but covers a different bookstore entirely with no author overlap between the two.

## Sherlock — What are the facts?

Rick's booth number checks out: CRC Press is part of the **Taylor & Francis Group** (which also owns the Routledge imprint), and Taylor & Francis runs **"the Taylor & Francis Bookstore"** at Black Hat USA 2026 — **Booth #8603**, in the Business Hall — confirmed directly on Taylor & Francis's own dedicated event page (`routledge.com/go/black-hat-conference`, titled "Black Hat Conference 2026"). CRC Press is the specific imprint responsible for most of the cybersecurity titles sold there, but the booth itself is badged as the Taylor & Francis Bookstore, not "CRC Press" standalone — a naming nuance worth knowing if you're looking for signage on-site.

**Booth hours:** Taylor & Francis's page doesn't post its own separate hours, so the best available figure is the Business Hall's general operating hours (confirmed on blackhat.com), which the booth is presumably staffed throughout:

| Day | Date | Business Hall Hours |
|---|---|---|
| Tuesday | Aug 4 | 4:00 PM – 7:00 PM (Welcome Reception) |
| Wednesday | Aug 5 | 9:00 AM – 6:00 PM (includes 4:00–5:00 PM Booth Crawl) |
| Thursday | Aug 6 | 9:00 AM – 4:00 PM |

**The book signing schedule itself is structurally different from the other bookstore's.** Where the Professional Programs Bookstore runs 14 separate, individually time-slotted author signings across Tuesday–Thursday, Taylor & Francis publishes a single **Author Meet & Greet** block:

| Day | Time | Location |
|---|---|---|
| Wednesday, Aug 5 | 2:00 PM – 3:00 PM | Booth #8603 |

Three authors and five featured titles are listed for that one hour — the page doesn't break out which author is signing at which specific minute within the block, so all three should be assumed present for the full hour unless you learn otherwise on-site:

| Author | Book(s) | Canon status |
|---|---|---|
| Walt Powell | *The CISO 3.0: A Guide to Next-Generation Cybersecurity Leadership*; *Quantum Ready: The Enterprise Guide to Post-Quantum Cryptographic Readiness* | Not confirmed either way — CyberCanon site search was unreliable for this query today (see Popper) |
| Andres Andreu | *The CISO Playbook*; *The CISO Playbook: The Adversarial Mindset* | 🏆 **The CISO Playbook is a HoF Nominee** — confirmed on cybercanon.org. The sequel, *The Adversarial Mindset*, could not be confirmed either way (see Popper) |
| Peter Jay Sorenson | *AI for the Ordinary: A Non-technical Playbook for Citizens, Students, and Managers* | Not confirmed either way — CyberCanon site search was unreliable for this query today (see Popper) |

**One more fact worth carrying over to Rick directly:** Taylor & Francis is offering **30% off Black Hat-featured titles** with code `BlackHatUS26BS` at checkout — usable online at routledge.com or in person at the booth. The code is restricted to Taylor & Francis Black Hat bookstore titles and can't stack with other offers.

No overlap in authors or titles between this bookstore and the Professional Programs Bookstore's schedule — the two are fully independent from a "who to go see" standpoint.

## Euclid — What must be fundamentally true?

The two bookstores are **not the same kind of event wearing a different location**, and treating them as parallel would understate a real structural difference. The Professional Programs Bookstore's schedule is a **sequence** — 14 distinct appointments spread across three days, each author getting their own dedicated slot, which rewards planning around specific times. The Taylor & Francis Meet & Greet is a **single gathering** — three authors sharing one hour, which rewards just showing up sometime in that window rather than timing an arrival precisely. Both are legitimate formats for a publisher-run event, but a reader skimming only the headline "book signing schedule" from each without reading the actual table would come away with the wrong mental model of what to expect on the ground.

The other fundamental: this booth's discount code is a **first-party fact from the publisher**, not something either bookstore's schedule data implies — it's worth surfacing on its own merits since it changes the economics of buying a book at the booth, independent of the signing schedule itself.

## Popper — How could we be wrong?

1. **The single-block format could still resolve into per-author sub-times on-site.** Nothing on Taylor & Francis's page rules out the booth staff running a more granular schedule within the 2:00–3:00 PM hour (e.g., 20 minutes per author) that just isn't published online. Treat "all three for the full hour" as the best available read of the public page, not a guarantee of the on-the-ground mechanics.
2. **CyberCanon verification is incomplete for this bookstore too, and for the same reason as the sibling report.** Direct site-search confirmation succeeded for Andres Andreu's *The CISO Playbook* (HoF Nominee) but repeatedly failed for Walt Powell, the *Adversarial Mindset* sequel, and Peter Jay Sorenson — the same intermittent browser-automation timing issue documented in the sibling report's Popper section, not a data-quality problem. These three are marked "not confirmed either way" rather than guessed at.
3. **The "Business Hall hours = booth hours" assumption is an inference, not a stated fact.** Taylor & Francis's page gives no separate operating hours for Booth #8603 — Sherlock used the general Business Hall hours as the best available proxy, but the booth could plausibly open later or close earlier than the hall itself, particularly on setup/teardown days.
4. **This is a snapshot, same caveat as the sibling report.** No "last updated" timestamp on Taylor & Francis's page — a re-check close to August 5 is reasonable insurance, especially since the single-block format leaves less room to absorb a last-minute change than a multi-slot schedule would.

## Seldon — What is likely to happen next?

Addressing Popper's four points: point 1 (possible on-site sub-scheduling) isn't resolvable from published material — it's a scope boundary, flagged rather than guessed at. Point 2 (incomplete Canon verification) is the same open item as the sibling report and doesn't get better with more reasoning — a working site-search session or direct on-site check would close it. Point 3 (Business Hall hours as a proxy for booth hours) is a reasonable inference given publishers' booths standardly follow hall hours at trade-show-style events, but it's presented as inference rather than fact in the table above, which is the right level of confidence. Point 4 (schedule stability) gets the same forecast as the sibling report and for the same reason — a single well-established annual conference doesn't have a track record suggesting frequent last-minute program changes, but the number of *specific* facts on this page (one time block, three authors, one discount code) likely to shift before August 5 runs from about **0 to 2, with a median around 0** — slightly more stable than the 14-slot schedule simply because there's less surface area to shift. This is reasoned judgment, not a measured record.

## Tufte — How do we make this clear?

Three tables carry this report: Business Hall hours (proxy for booth hours), the single Meet & Greet time block, and the author/book/Canon-status table. Keeping the Meet & Greet as its own one-row table, rather than folding it into the author table, makes the structural difference from the sibling report's 14-row schedule immediately visible at a glance — a reader who's already seen the other report will register in half a second that this one works differently, without needing to re-read Euclid's explanation.

## Turing — Should any of this become a skill?

No. Same conclusion as the sibling report and for the same reason — a single lookup against a publisher's own event page, not a repeatable technique distinct enough to warrant a skill. The `routledge.com/go/black-hat-conference` URL pattern (Taylor & Francis maintains one of these per major conference they exhibit at) might be worth remembering informally if a future question asks about a different conference's Taylor & Francis presence, but that's a fact to recall, not a procedure to encode.

## Sources

**Primary/official**
- [Black Hat Conference 2026, Routledge/Taylor & Francis](https://www.routledge.com/go/black-hat-conference) — booth number (#8603), Author Meet & Greet date/time, all five featured titles and three authors, and the discount code; the single source for nearly everything in this report.
- [Black Hat USA 2026 | Business Hall](https://blackhat.com/us-26/business-hall.html) — Business Hall dates and hours, used as the proxy for Booth #8603's operating hours (see Popper's caveat on this being an inference, not a stated fact).
- [CyberCanon Books](https://cybercanon.org/books/) — direct site search; confirmed *The CISO Playbook* (Andres Andreu) as a HoF Nominee. Searches for Walt Powell's titles, Andreu's *Adversarial Mindset* sequel, and Peter Jay Sorenson's title were attempted but the site's search widget was intermittently unresponsive to automated input this session (documented at length in the sibling report) — not re-attempted exhaustively a second time today.

## New Skills

None. See Turing's note above.

## Library Recommendations

Nothing from this report is recommended for the artifact library, for the same reason as the sibling report: a specific conference bookstore's hours and one-time signing event is time-bound operational information, stale within two weeks. Status: not recommended, no action needed from Rick.
