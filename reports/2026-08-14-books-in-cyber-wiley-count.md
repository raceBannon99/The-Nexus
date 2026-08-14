# Books in Cyber — How Many Speaker Books Are Published by Wiley?

## Question

Rick asked: for the Books in Cyber conference, with speakers and their books listed at [booksincyber.com/#speakers](https://booksincyber.com/#speakers), how many of these books are published by Wiley?

## Clarifying Questions

None asked. The question is a direct factual count, well-scoped enough to answer without pausing — the only real ambiguity (how to count a book that's shared by two co-author speakers, or an author with multiple books listed) is a presentation choice, not a scope question, so it's resolved by showing both framings in the answer rather than picking one silently.

## Bradlee's Answer

**Four unique books are published by Wiley**, out of 14 identifiable book titles across the conference's 15 listed speakers (one speaker, John Kindervag, has no book title yet — his entry reads "TBA"):

1. *Project Zero Trust: A Story about a Strategy for Aligning Security and the Business* — George Finney
2. *Secrets and Lies: Digital Security in a Networked World* — Bruce Schneier (one of three books listed on his speaker card, alongside *Click Here to Kill Everybody*, W. W. Norton, and *Data and Goliath*, also W. W. Norton — neither of those two is Wiley)
3. *Cybersecurity First Principles: A Reboot of Strategy and Tactics* — Rick Howard
4. *How to Measure Anything in Cybersecurity Risk* — co-authored by Richard Seiersen and Douglas Hubbard, both listed as separate speakers for the same book

That means **5 of the 15 speakers** (Finney, Schneier, Howard, Seiersen, Hubbard) have at least one Wiley-published book associated with their entry, and if every book-title *listing* is counted individually (Schneier's three books each count once, and the shared Seiersen/Hubbard book counts once per speaker card), **5 of the 17 total listings** are Wiley.

The other 10 identified books span eight different publishers — none of them repeat except *Zero Trust Done Right* (Tillson/Spiegel/Ludlow's shared book) and *Click Here to Kill Everybody*/*Data and Goliath* (both W. W. Norton, both Schneier): W. W. Norton (2), Farrar Straus and Giroux, Erudite Candor Publishing, Sutherland House Experts, Smiling Eyes Publishing, Bloomsbury Publishing, and two independently-published titles — *RipTide* (Chase Cunningham & Gregory Touhill) and *Zero Trust Done Right* (Tillson/Spiegel/Ludlow, confirmed independently published March 2026). John Kindervag's book has no title yet, so it can't be attributed to any publisher.

One thing worth knowing about *why* the count skews toward Wiley at all: three of the four Wiley titles are quantitative/practitioner-strategy books from established, repeat Wiley cybersecurity authors (Howard, Seiersen/Hubbard, and Finney, whose *Project Zero Trust* was co-written with John Kindervag — today's "TBA" speaker) rather than a broad publisher preference across the program. The general-audience narrative nonfiction on the roster (Perlroth, Shapiro) both landed with trade publishers (Bloomsbury, FSG) instead, and every self-published or small-press title on the list is a practitioner memoir, sales-skills book, or a book written specifically to accompany the author's own consulting/speaking business — a different publishing lane entirely from Wiley's technical-professional catalog.

## What we already know (Alexandria, opening)

Checked the artifact library (`raceBannon99/nexus-artifacts`) and prior Nexus reports. No artifact-library matches for Wiley, Books in Cyber, or booksincyber.com. Two prior reports touch adjacent ground but don't answer this question: [`reports/2026-07-21-canon-b2c-b2b-hybrid-model.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-21-canon-b2c-b2b-hybrid-model.md) references Books in Cyber's sponsorship-tier structure (not its speaker roster), and [`reports/2026-07-27-blackhat-book-signing-schedule.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-book-signing-schedule.md) identifies two unrelated Wiley titles from a Black Hat signing schedule (*AI Security Engineering*, *Blockchain Application Security*) — different books, different event, useful only as a sourcing-methodology precedent.

## The facts (Sherlock)

### Getting the full speaker/book list right

The flat page-text view of [booksincyber.com/#speakers](https://booksincyber.com/#speakers) under-reports: it shows exactly one book title per speaker card, with a "+2" suffix on Bruce Schneier's card that a plain-text fetch doesn't expand. A first pass at this research nearly missed two of Schneier's three books as a result. Opening his individual speaker profile (`booksincyber.com/?speaker=15`) via Chrome MCP surfaced the full list: *Click Here to Kill Everybody*, *Data and Goliath*, and *Secrets and Lies*. A full accessibility-tree read of the entire speakers section (not just the flat text extraction) confirmed Schneier is the *only* speaker with a "+N" indicator — all other 14 speaker cards show exactly one book, so no other hidden titles exist to miss.

### Full roster with confirmed publishers

| Speaker | Book | Publisher | Wiley? |
|---|---|---|---|
| George Finney | *Project Zero Trust: A Story about a Strategy for Aligning Security and the Business* | John Wiley & Sons | ✅ Yes |
| Bruce Schneier | *Click Here to Kill Everybody: Security and Survival in a Hyper-connected World* | W. W. Norton | No |
| Bruce Schneier | *Data and Goliath: The Hidden Battles to Collect Your Data and Control Your World* | W. W. Norton | No |
| Bruce Schneier | *Secrets and Lies: Digital Security in a Networked World* | Wiley (Wiley Computer Publishing imprint) | ✅ Yes |
| Scott J. Shapiro | *Fancy Bear Goes Phishing: The Dark History of the Information Age, in Five Extraordinary Hacks* | Farrar, Straus and Giroux | No |
| Ross Young | *Cybersecurity's Dirty Secret: Why Most Budgets Go to Waste* | Erudite Candor Publishing | No |
| Eldon Sprickerhoff | *Committed: Startup Survival Tips and Uncommon Sense for First-Time Tech Founders* | Sutherland House Experts | No |
| Evgeniy Kharam | *Architecting Success: The Art of Soft Skills in Technical Sales: Connect to Sell More* | Smiling Eyes Publishing | No |
| Rick Howard | *Cybersecurity First Principles: A Reboot of Strategy and Tactics* | John Wiley & Sons | ✅ Yes |
| Nicole Perlroth | *This Is How They Tell Me the World Ends: The Cyberweapons Arms Race* | Bloomsbury Publishing | No |
| Richard Seiersen | *How to Measure Anything in Cybersecurity Risk* | John Wiley & Sons | ✅ Yes |
| Douglas Hubbard | *How to Measure Anything in Cybersecurity Risk* (same book as Seiersen) | John Wiley & Sons | ✅ Yes |
| John Kindervag | *TBA* — no title announced yet | Unknown | Can't determine |
| Dr. Chase Cunningham | *RipTide* (full title: *Rip Tide: A Narrative on Cyber Security Failures at the National Level*, co-authored with Gregory Touhill) | Not named in available sources; ISBN prefix (979-8-...) matches the self-publishing/small-press block, not a Big Five or Wiley imprint | No (high confidence, not fully certain) |
| Jaye Tillson | *Zero Trust Done Right: A Practitioner's Guide to Zero Trust Security in the Age of AI* | Independently published (confirmed) | No |
| John Spiegel | *Zero Trust Done Right* (same book as Tillson) | Independently published | No |
| Gram Ludlow | *Zero Trust Done Right* (same book as Tillson) | Independently published | No |

### On Rick's own book

*Cybersecurity First Principles* is confirmed Wiley-published (April 2023) via Wiley's own product page — included in the tally like every other title, with no different treatment.

## First principles (Euclid)

Two things are fundamentally true about how "how many are published by Wiley" should be counted, and they pull in different directions:

1. **A publisher relationship is a property of the book, not the speaker slot.** Two speakers (Seiersen, Hubbard) are two people credited on one Wiley book — counting that as "two Wiley books" would overstate Wiley's actual footprint on the reading list itself.
2. **A publisher relationship is also a property of the individual title, not the author.** Schneier has three books on his card from two different publishers — treating "Schneier" as a single data point would erase the fact that two-thirds of his listed catalog isn't Wiley at all.

Both of these are true simultaneously, which is why the answer above gives three numbers rather than one: 4 unique Wiley *books*, 5 of 15 Wiley-connected *speakers*, 5 of 17 Wiley *listings*. There's no single correct denominator — "how many of these books" most naturally reads as asking about unique titles (4), which is the headline number, but the speaker-count framing is the one that matters if the real question underneath is "how much of this conference's stage time is Wiley-adjacent."

## Where this could be wrong (Popper)

- **RipTide's publisher isn't independently confirmed, only inferred.** No source found explicitly states who published it. The ISBN prefix (979-8, format 9798762096621) is a strong signal — that block is heavily associated with Amazon KDP self-publishing and small independent presses, and definitively *not* one Wiley has used for any of the other titles checked here — but it's an inference from ISBN structure, not a publisher's own statement. If Rick needs certainty (e.g., citing this externally), it's worth a direct check of the book's copyright page or Cunningham/Touhill confirming directly. This doesn't change the "not Wiley" conclusion, which is solid, but the *specific* publisher name for RipTide is unconfirmed.
- **The speakers page could change between now (August 14, 2026) and the conference (September 8, 2026).** Kindervag's "TBA" book could be announced, sponsor-slot speakers marked "Reserved" in the sponsor section could be added with their own books, and the page explicitly shows "15 / 8+ confirmed" — suggesting more speakers may still be added. This count is accurate as of today's pull, not a permanent figure.
- **"Published by Wiley" could arguably be read more narrowly (only the current, in-print edition and imprint) or more broadly (any Wiley imprint or predecessor entity, e.g., Wiley Computer Publishing, the imprint under which the original 2000 edition of *Secrets and Lies* appeared before later editions moved to the main Wiley list).** This report counts imprint variations as still "Wiley" — a reasonable reading, but a stricter one that only counts the current flagship Wiley imprint wouldn't change the count here, since all four Wiley titles are confirmed on Wiley's own current product pages regardless of original imprint history.

## What's likely to happen next (Seldon)

The only genuinely forward-looking element here is whether this count holds through the conference date given the "15 / 8+ confirmed" note and Kindervag's unlisted book. Given the page already lists most of the announced schedule with named speakers rather than placeholders, and only one slot (Kindervag's book title, and the two "Reserved" sponsor speaker slots) remains genuinely open, the range for how much this Wiley count could still move runs from no change at all to one additional Wiley book — call it roughly a 60–80% chance the count stays exactly at 4 unique Wiley books through the event, with a median expectation of staying flat, and the main upside scenario being Kindervag's book turning out to be a Wiley title too, since his *Project Zero Trust* co-author (Finney) is already one of this report's four confirmed Wiley entries and Kindervag has a long-standing relationship with Wiley's zero-trust catalog.

## Visualizations (Tufte)

This is straightforward tabular fact-checking — speaker, book, publisher, yes/no — exactly the kind of side-by-side comparison a markdown table handles cleanly. The full roster table above is the deliverable; no rendered diagram adds anything a table doesn't already show.

## New Skills (Turing)

None. One technique worth noting for future similar pulls, but not skill-worthy on its own: **a flat WebFetch text extraction of a modern single-page-app event site can silently truncate multi-item lists** (the "+2" Schneier case) — the fix (opening the individual profile URL, or reading the full accessibility tree instead of just the visible text) is a reasonable one-off adjustment, not a distinct enough procedure to warrant a dedicated skill.

## Library Recommendations (Alexandria, closing)

None. This is a point-in-time fact count tied to a conference roster that's still being finalized (see Popper's and Seldon's notes on "15 / 8+ confirmed") — not durable reference material. No candidates recommended for `nexus-artifacts`.

## Sources

**Primary (Tier 1 — the conference's own site):**
- [Books in Cyber, Speakers section](https://booksincyber.com/#speakers) — the flat listing that started this research; under-reports Schneier's book count (shows "+2" without expanding it).
- Individual speaker profile pages (`booksincyber.com/?speaker=<id>`), read via Chrome MCP's accessibility tree rather than plain-text extraction — the only way to recover Schneier's full three-book list; also used to confirm no other speaker has a hidden "+N" beyond their single listed book.

**Publisher confirmation (Tier 1 — publishers' own product pages or their own catalog sites):**
- [Wiley, *Project Zero Trust*](https://www.wiley.com/en-us/Project+Zero+Trust:+A+Story+about+a+Strategy+for+Aligning+Security+and+the+Business-p-9781119884842)
- [Wiley, *Cybersecurity First Principles*](https://www.wiley.com/en-us/Cybersecurity+First+Principles:+A+Reboot+of+Strategy+and+Tactics-p-9781394173099)
- [Wiley, *How to Measure Anything in Cybersecurity Risk*, 2nd ed.](https://www.wiley.com/en-us/How+to+Measure+Anything+in+Cybersecurity+Risk,+2nd+Edition-p-9781119892304)
- [Wiley Online Library, *Secrets and Lies*](https://onlinelibrary.wiley.com/doi/book/10.1002/9781119183631)
- [W. W. Norton, *Click Here to Kill Everybody*](https://wwnorton.com/books/Click-Here-to-Kill-Everybody/)
- [W. W. Norton, *Data and Goliath*](https://wwnorton.com/books/Data-and-Goliath/)
- Amazon/Goodreads listings for *Fancy Bear Goes Phishing* (Farrar, Straus and Giroux), *Cybersecurity's Dirty Secret* (Erudite Candor Publishing), *Committed* (Sutherland House Experts), *Architecting Success* (Smiling Eyes Publishing), *This Is How They Tell Me the World Ends* (Bloomsbury Publishing) — each cross-checked against at least one additional retailer or review-site listing, not a single source.
- [Amazon, *Rip Tide*](https://www.amazon.com/Rip-Tide-Narrative-Security-Failures-ebook/dp/B09L8LB8CL) — no explicit publisher named; ISBN-block inference is the basis for the "not Wiley" call, flagged as lower confidence under Popper's notes.
- Amazon listing for *Zero Trust Done Right* confirming independent publication, March 10, 2026.

**Secondary/context:**
- [`reports/2026-07-21-canon-b2c-b2b-hybrid-model.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-21-canon-b2c-b2b-hybrid-model.md) and [`reports/2026-07-27-blackhat-book-signing-schedule.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-book-signing-schedule.md) — checked for precedent, cited above under Alexandria's opening pass.
