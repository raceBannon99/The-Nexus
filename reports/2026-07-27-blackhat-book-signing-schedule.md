# Black Hat USA 2026 Bookstore & Book Signing Schedule

**Question:** The annual Black Hat security conference is next week. The conference organizers have a bookstore and have authors come in for book signings. What is the current book signing schedule?

**Note for Rick:** you're on it — Wednesday, August 5 at 2:00 PM.

## Alexandria — What do we already know?

Nothing in the artifact library or prior Nexus reports covers Black Hat's bookstore or a past signing schedule — this is a clean-slate lookup, not a topic The Nexus has touched before. Worth noting for context (not a substitute for today's answer): the artifact library does hold a fact-sheet on a B2C/B2B business-model test derived from the Canon Project's book analysis work, but it has no connection to the Black Hat bookstore itself.

## Sherlock — What are the facts?

Black Hat USA 2026 runs **August 1–6** at the Mandalay Bay Convention Center in Las Vegas — Trainings August 1–4, Summits August 4, Briefings August 5–6. "Next week" from today (July 27) is correct.

The Bookstore is physically located at the **Breakers Registration Desk, Level 2**, run by Professional Programs Bookstore, and open:

| Day | Date | Hours |
|---|---|---|
| Sunday | Aug 2 | 8:00 AM – 6:00 PM |
| Monday | Aug 3 | 8:00 AM – 6:00 PM |
| Tuesday | Aug 4 | 8:00 AM – 6:00 PM |
| Wednesday | Aug 5 | 7:30 AM – 6:00 PM |
| Thursday | Aug 6 | 8:00 AM – 4:00 PM |

The full signing schedule, pulled directly from Black Hat's own event-schedule system (filtered to the Bookstore track), lists 14 individual signing slots — all at the same Breakers Registration Desk location, all open to any pass type (Briefings, Business Hall, Summits, or Trainings):

| Day | Time | Author(s) |
|---|---|---|
| Tuesday, Aug 4 | 9:45 AM | Sherri Davidoff & Matt Durrin |
| Tuesday, Aug 4 | 10:30 AM | Ashish Rajan |
| Tuesday, Aug 4 | 12:30 PM | Marco Morano |
| Tuesday, Aug 4 | 12:45 PM | Helen Patton |
| Tuesday, Aug 4 | 1:15 PM | Andy Ellis |
| Tuesday, Aug 4 | 3:30 PM | Sara Armstrong-Smith |
| Wednesday, Aug 5 | 11:15 AM | Teri Green |
| Wednesday, Aug 5 | 12:45 PM | Adam Shostack |
| Wednesday, Aug 5 | 1:15 PM | Byron Acohido |
| **Wednesday, Aug 5** | **2:00 PM** | **Rick Howard** |
| Wednesday, Aug 5 | 3:30 PM | Savannah Lazzara, Omar Santos & Wesley Thurner |
| Wednesday, Aug 5 | 4:00 PM | Pete Green |
| Thursday, Aug 6 | 10:00 AM | Tony Martin |
| Thursday, Aug 6 | 2:00 PM | Bob Gourley |

No signings are listed for Sunday or Monday (bookstore-open-only, no author events yet), and Thursday has only two slots — the schedule is heavily weighted toward Tuesday and Wednesday, the two Summits/early-Briefings days.

Note on data quality: every name on this list is a recognizable, established cybersecurity author or practitioner (Shostack wrote *Threat Modeling*, Ellis and Patton are well-known CISOs/authors, Santos has written extensively for Cisco Press, Acohido co-founded LastWatchdog) — except "Marco Morano," a name that doesn't match any cybersecurity author Sherlock could independently corroborate. This is flagged here rather than silently corrected; it's reported exactly as Black Hat's own schedule system displays it, but it's the one entry worth double-checking against the printed program on-site.

## Euclid — What must be fundamentally true?

A few things about how this schedule actually functions, stripped to fundamentals: it's a **single fixed location** (Breakers Registration Desk, Level 2) for every slot, so there's no cross-venue routing to plan around — only timing. It's **built for walk-up attendance**, not registration — nothing in Black Hat's system suggests these require an RSVP the way some Summits or party events do. And it's **calendar-published by the organizer, not crowdsourced or aggregated** — this came directly from blackhat.com's own schedule system, which is the authoritative source for this kind of operational detail; there's no better source to triangulate against.

## Popper — How could we be wrong?

Two real risks, both about *time*, not about whether this data was read correctly:

1. **This is a snapshot, not a guarantee.** Conference schedules — especially the "additional programs" tier below Briefings/Trainings — are known to shift in the final week before an event: a flight gets rebooked, an author drops out, a slot moves by 30 minutes. Nothing on Black Hat's page carries a "last updated" timestamp, so there's no way to know how fresh this pull is relative to the live system. Treat this table as accurate as of today, July 27, and worth a quick re-check against the printed on-site program or the Black Hat mobile app once you're at Mandalay Bay.
2. **The "Marco Morano" entry, flagged above.** It's possible this is simply an author outside Sherlock's frame of reference rather than an error — Black Hat's speaker roster is large and not everyone signing books is a broadly recognized industry-author name. This isn't a reason to doubt the rest of the schedule, just a reason to confirm that one specific slot if it matters to you.

## Seldon — What is likely to happen next?

Addressing Popper's points directly: the on-site verification recommendation stands as the practical mitigation for risk #1 — there's no way to resolve "how stable is this schedule" without either a re-pull closer to the date or on-site confirmation, so this is a scope boundary rather than something to forecast away. For the Marco Morano entry, no correction is warranted without better evidence than Sherlock had — it stays in the table as published, flagged.

On stability: for a 14-slot schedule published about a week out from a well-established annual conference (this is Black Hat's 29th year), the number of these specific slots likely to shift time or lineup before August 4 runs from about **0 to 3, with a median around 1** — small logistics-tier programming like author signings is more volatile than headline content (Keynotes, Briefings) but Black Hat's own bookstore program is a routine, recurring fixture, not a new or fragile addition this year. This is reasoned judgment based on how conference-adjacent programming typically behaves in the final week, not a measured track record of Black Hat's bookstore specifically — there's no dataset tracking year-over-year signing-schedule change rates to anchor it more tightly.

## Tufte — How do we make this clear?

The two tables above (bookstore hours, and the day/time/author signing schedule) are the visualization — a chronological table is the correct form for a schedule, and no further chart or diagram would add clarity. Rick Howard's own slot is bolded in the schedule table so it isn't lost among the other 13 rows.

## Turing — Should any of this become a skill?

No dedicated skill is warranted from this — it was a single lookup against a known conference's public schedule system. One reusable detail worth remembering informally rather than encoding as a skill: Black Hat's schedule pages support a `?track[]=<name>` query filter (e.g. `features/schedule/index.html?track[]=bookstore`) that returns just one program track instead of the full multi-day agenda — useful if a future question asks about a different Black Hat feature (Arsenal, Summits Leaders Lounge, etc.) rather than re-scanning the whole schedule by hand.

## Sources

**Primary/official**
- [Black Hat USA 2026 | Features](https://blackhat.com/us-26/features.html) — bookstore location, hours, and general description ("Several Black Hat Speakers and Trainers will be signing copies of their authored books").
- [Black Hat USA 2026 | Features Schedule (Bookstore track)](https://blackhat.com/us-26/features/schedule/index.html?track[]=bookstore) — the complete day/time/author signing schedule; source for every row in the schedule table above.
- [Black Hat USA 2026](https://blackhat.com/us-26/) — conference dates (August 1–6, 2026) and venue (Mandalay Bay Convention Center, Las Vegas), confirming "next week" is accurate relative to today's date.

## New Skills

None. See Turing's note above for a minor reusable technique (the `track[]` query-filter pattern) that doesn't rise to a standalone skill.

## Library Recommendations

Nothing from this report is recommended for the artifact library. A specific conference's book-signing schedule is time-bound operational information that will be stale within two weeks (the event ends August 6) — it has no standing reference value the way a fact-sheet or durable framework would. Status: not recommended, no action needed from Rick.
