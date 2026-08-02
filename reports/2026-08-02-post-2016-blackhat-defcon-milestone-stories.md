# Are There Post-2016 Black Hat/DEF CON Stories of the Same Caliber as the Pre-2016 Milestones?

**Question:** The origin-history report's combined timeline clusters its most "iconic" single-incident stories — Ciscogate (2005), Blue Pill (2006), ATM jackpotting (2010), the Jeep hack (2015), Mayhem (2016), plus DEF CON's Sklyarov arrest (2001), NBC filming incident (2007), and the Back Orifice releases (1998/99) — almost entirely before 2017. Is that really a gap, or did genuinely comparable stories happen after 2016 that just didn't make the original timeline?

## Alexandria — What do we already know?

Nothing in the artifact library addresses this directly. In `raceBannon99/The-Nexus`, the origin-history report (`2026-07-27-blackhat-defcon-origin-history.md`) and all six dedicated ELI5 reports built from it cluster in exactly the same 1998–2016 window Rick is asking about — which confirms the pattern is real *in what's been published so far*, but doesn't establish whether that's because nothing comparable happened later, or because nobody asked about anything later. Worth answering directly rather than assuming either way.

## Sherlock — What are the facts?

**The pattern isn't just an artifact of what Nexus has researched — it shows up in Black Hat's own self-told history, too.** Dark Reading's 25th-anniversary retrospective (Aug 2022) — written by and for the Black Hat community, with named interviews from Adam Shostack, Jeremy Rauch, Richard Thieme, and Ira Winkler — runs through its list of "iconic hacks" in strict chronological order: James Bamford's NSA talk (2001), Ciscogate (2005), Blue Pill (2006), Barnaby Jack's ATM jackpotting (2010), and the Jeep hack (2015). It then pivots directly into a section literally titled "Growing Up" — about the Code of Conduct, professionalization, and diversity programming — without naming a single specific technical incident from 2016 onward. That's the community's own curated list agreeing with the same cutoff Rick noticed, not just a gap in this project's prior research.

**That said, a few genuine post-2016 candidates exist — they just aren't the same *kind* of story, which is worth being explicit about rather than papering over:**

- **2023 (DEF CON 31): the AI Village's Generative Red Team Challenge — the strongest candidate by far.** The largest-ever public red-teaming exercise against generative AI models, explicitly backed by the White House Office of Science and Technology Policy, the National Science Foundation, and the Congressional AI Caucus. Eight major AI labs (OpenAI, Google, Anthropic, Meta, Nvidia, Cohere, Hugging Face, Stability AI) submitted models for testing; 2,244 participants exchanged 164,208 adversarial messages across 17,469 conversations over two and a half days, probing for bias, harm, and security flaws. In pure scale and policy footprint, this plausibly outranks everything on the pre-2016 list except the 2012 NSA keynote — but it's a structured, government-convened research exercise, not one researcher forcing a confrontation on stage, which is a different narrative shape than Ciscogate or the Jeep hack.
- **2019: the Crown Sterling "Time AI" scandal.** A sponsored Black Hat talk pitching a dubious new encryption technology ("Time AI") was publicly mocked and challenged live by attendees (including Trail of Bits CEO Dan Guido); Black Hat pulled the talk from its website afterward, and Crown Sterling sued the conference over the backlash. Genuinely notable — but it's a credibility/fraud scandal about a sponsor, not a hacking demonstration.
- **2019: Rep. Will Hurd's keynote rescinded.** Black Hat announced Hurd as a keynote speaker, then reversed the invitation within 24 hours after backlash over his voting record on women's rights, stating in its own release that it had "misjudged the separation of technology and politics." A real governance/culture-war moment, but not a technical milestone.
- **2022: Chris Hadnagy banned from DEF CON.** After multiple Code of Conduct violation reports, DEF CON banned Hadnagy (a DEF CON Social Engineering Village leader) and disbanded an affiliated DEF CON Group. Significant to the community, but an internal conduct story, not a public-facing technical or policy story.

**One plausible-sounding candidate was checked and explicitly excluded.** Peiter "Mudge" Zatko — a member of Black Hat's very first 1997 speaker lineup — became Twitter's head of security and filed a whistleblower complaint against the company, testifying before the Senate Judiciary Committee on September 13, 2022, about "widespread security failures." It's a genuinely major story with a poetic tie back to Black Hat's founding roster, but it didn't happen at, or in direct connection with, a Black Hat or DEF CON talk — it's a corporate/congressional event. Excluded from the timeline comparison on that basis, flagged here rather than silently dropped; see Popper below on whether that scope call is the right one.

**Also checked and not confirmed:** a rumored Chris Krebs DEF CON keynote appearance after his 2020 firing from CISA. Search turned up extensive coverage of the firing itself and later 2021 appearances at other venues (e.g., Georgetown), but nothing confirming a specific DEF CON talk — not included.

## Euclid — What must be fundamentally true?

If the pre-2016 cluster is real rather than an artifact of what's been researched, there has to be a structural reason for it — and there is one, visible in the very mechanism the origin-history report's Euclid section already identified:

- **The pre-2016 milestones were shocking because the format itself was new: an independent researcher forcing a live, public confrontation with an unprepared or resistant vendor.** Ciscogate worked as a story because coordinated vulnerability disclosure wasn't yet a norm — Cisco's lawyers cutting pages out of the proceedings *was* the story. By the mid-2010s, most major vendors ran formal bug-bounty and coordinated-disclosure programs, which moved exactly that kind of confrontation out of the "surprise reveal on a Black Hat stage" format and into private-then-published channels. The milestones didn't stop happening; the format that made them mythic stopped being the default path.
- **Novelty decays even when the underlying finding doesn't.** "A hacker can make a real ATM dispense cash" and "a hacker can kill a real car's brakes at 70mph" landed hard specifically because no one had watched it happen live before. A comparably serious demonstration today competes against a decade of prior demonstrations of embedded-systems compromise — the finding can be just as real and still generate less shock.
- **Both conferences' own "growing up" — Code of Conduct, corporate ownership since 2018, diversified track programming — is the same institutionalization arc the origin-history report already traces from DEF CON→Black Hat and Black Hat→BSides.** An event optimized for professionalism and predictability structurally produces fewer unscripted confrontations than one that wasn't yet.
- **DEF CON's fragmentation into 30+ specialized Villages (a trend the origin-history report's Seldon section already flagged as a live hypothesis) diffuses "the one story everyone remembers" even when individual findings inside a Village are just as significant** — there's no single main stage moment left to concentrate attention the way the Jeep hack once did on a Wired cover story.
- **The frontier moved, rather than closing.** The AI Village's 2023 Generative Red Team Challenge is the same underlying mechanism the origin-history report's Euclid section already named as the through-line of all three conferences — giving independent researchers a real platform before institutions understand why it matters — recurring in a new domain (AI) at a scale exceeding most of the pre-2016 list. The "no comparable story since 2016" read is defensible only if "comparable" is implicitly defined as "same narrative shape as Ciscogate," not "same underlying significance."

## Popper — How could we be wrong?

1. **The Dark Reading evidence may just be a canonization-lag artifact, not a real gap.** The Jeep hack (2015) had seven years to become "iconic" by the time of that 2022 retrospective; anything from 2019–2022 had almost no time to be absorbed into the community's own mythology yet. A similar piece written in 2032 might well include a 2023 or 2026 entry that simply hasn't crystallized into "iconic" status as of this research.
2. **"Caliber" is underspecified, and Sherlock's framing implicitly favored one axis over others.** If caliber means technical audacity on a physical system, the pre-2016 list wins outright and nothing since compares. If it means national policy footprint, the 2023 AI Village event plausibly outranks everything except the 2012 NSA keynote. If it means enduring mainstream-media reach, the Jeep hack may never be topped, full stop. Presenting one ranked list would smuggle in a metric choice Rick didn't specify.
3. **Excluding Mudge/Zatko's 2022 testimony is a real judgment call, not an obvious one.** Rick's question didn't specify "must happen physically at the conference," and Mudge is personally continuous with Black Hat's origin story in a way that gives the story real narrative weight even off-stage. A looser scope test changes the answer.
4. **Small-sample problem: the pre-2016 list itself is only ~5 truly iconic entries across 18 years — roughly one every 3–4 years.** A single multi-year gap between 2016 and 2023 isn't necessarily a structural break; it could be ordinary variance in a pattern that was never that dense to begin with.

## Seldon — What is likely to happen next?

Addressing each point: Point 1 (canonization lag) can't be resolved by more research now — it's an honest open uncertainty, not a flaw to fix; the right response is to hold the finding as *directional*, not *conclusive*. Point 2 (caliber axis) is resolved below in Tufte's table by presenting the post-2016 candidates against multiple axes explicitly rather than forcing one ranking — Rick can weight the axis he actually cares about. Point 3 (Mudge scope) is resolved by stating the judgment call plainly, as Sherlock already did, rather than picking a side quietly. Point 4 (small sample) is folded into the forecast below rather than dismissed.

**Forecast:** given the historical ~3–4 year cadence between iconic-caliber stories (Bamford 2001 → Ciscogate 2005 → Blue Pill 2006 → ATM jackpotting 2010 → Jeep hack 2015), and treating the 2023 AI Village event as the pattern's most recent entry if AI-security spectacles count as the same phenomenon in a new domain, the range for the next comparably iconic story from 2026 runs from about **1 to 6 years out, with a median around 3 years**. The short end is driven by how fast AI security is currently escalating — a live compromise of an agentic AI system, or a repeat of the Generative Red Team format at larger scale, are both plausible near-term candidates. The long end assumes the Village-fragmentation and institutionalization dynamics Euclid identified keep suppressing single unifying "main stage" moments even as individually significant findings continue to occur — meaning the next comparable story might happen but simply not get canonized as iconic within a few years the way the older ones eventually were.

## Tufte — How do we make this clear?

The pre-2016 list and the post-2016 candidates aren't really comparable on one axis — laying them out against the specific kind of caliber each represents makes that visible instead of forcing a single ranked list:

| Year | Story | Primary caliber axis | Comparable to pre-2016 list? |
|---|---|---|---|
| 2001 | Bamford's NSA talk | National-security policy | — (pre-2016 baseline) |
| 2005 | Ciscogate | Vendor-suppression drama / disclosure norms | — (pre-2016 baseline) |
| 2006 | Blue Pill | Technical audacity | — (pre-2016 baseline) |
| 2010 | ATM jackpotting | Technical audacity / mainstream shock | — (pre-2016 baseline) |
| 2015 | Jeep hack | Mainstream media reach | — (pre-2016 baseline) |
| 2016 | Mayhem / Cyber Grand Challenge | Technical milestone (AI) | — (pre-2016 baseline, already on timeline) |
| 2019 | Crown Sterling "Time AI" | Fraud/credibility scandal | Different kind — no |
| 2019 | Will Hurd keynote rescinded | Governance / culture-war controversy | Different kind — no |
| 2022 | Chris Hadnagy DEF CON ban | Internal conduct scandal | Different kind — no |
| 2022 | Mudge/Zatko Twitter testimony | National-security policy (off-site) | Comparable caliber, but not a conference event — excluded |
| **2023** | **AI Village Generative Red Team Challenge** | **Policy footprint + technical scale** | **Yes — strongest candidate, same underlying mechanism as the pre-2016 list, new domain** |

## Turing — Should any of this become a skill?

No. This is a one-off comparative research question — genuinely required fresh searching and judgment calls about scope, but not a repeatable technique distinct enough to encode as a skill.

## Sources

**Primary/official**
- [Generative Red Team Challenge results, AI Village blog](https://aivillage.org/blog/generative-red-team/) — the AI Village's own announcement/results post; source for participant counts, message counts, and partner list.
- [Black Hat USA 2019 Keynote Update, blackhat.com](https://blackhat.com/latestintel/06142019-black-hat-usa-2019-keynote-update.html) — Black Hat's own statement rescinding Rep. Will Hurd's keynote invitation.

**Journalism/retrospective**
- [Looking Back at 25 Years of Black Hat, Dark Reading (Andrada Fiscutean, Aug 10, 2022)](https://www.darkreading.com/cyber-risk/looking-back-at-25-years-of-black-hat) — the community's own 25th-anniversary retrospective; source for the observation that its "iconic hacks" list stops at the 2015 Jeep hack before pivoting to a "Growing Up" section with no further named technical incidents. Retrieved via Chrome MCP after WebFetch returned HTTP 403.
- [Why Biden's White House Just Got Behind The 'Biggest AI Hacking Event Ever,' Forbes (Thomas Brewster, May 4, 2023)](https://www.forbes.com/sites/thomasbrewster/2023/05/04/biden-white-house-backs-biggest-ai-hacking-event-with-google-and-chatgpt/) — corroborates White House OSTP backing of the AI Village event.
- [Virtual News Conference to Discuss the Generative Red Team Challenge, BusinessWire (Aug 4, 2023)](https://www.businesswire.com/news/home/20230804075084/en/) and [results release, BusinessWire (Aug 29, 2023)](https://businesswire.com/news/home/20230829684414/en/) — corroborate scale figures (2,244 participants, 164,208 messages).
- [Black Hat Talk About 'Time AI' Causes Uproar, Is Deleted by Conference, Vice (2019)](https://www.vice.com/en/article/black-hat-talk-about-time-ai-causes-uproar-is-deleted-by-conference/) and [Biz forked out $115k to tout 'Time AI' crypto at Black Hat. Now it sues organizers, The Register (Aug 26, 2019)](https://www.theregister.com/2019/08/26/black_hat_sued/) — corroborate the Crown Sterling scandal and subsequent lawsuit.
- [Black Hat scraps Rep. Will Hurd as keynote speaker amid voting record controversy, TechCrunch (June 14, 2019)](https://techcrunch.com/2019/06/14/black-hat-will-hurd-keynote/) and [Will Hurd's Black Hat keynote nixed amid criticism of voting record, CyberScoop](https://cyberscoop.com/will-hurd-black-hat-keynote-canceled/) — corroborate the Hurd episode.
- [Twitter whistleblower Peiter "Mudge" Zatko testifies to Congress, NPR (Sept 13, 2022)](https://www.npr.org/2022/09/13/1122671582/twitter-whistleblower-mudge-senate-hearing) — source for the Zatko testimony date and content; checked and excluded as not a conference event (see Sherlock).
- The best of Black Hat: The consequential, the controversial, the canceled, CSO Online (2017) — checked for post-2016 content; the piece predates 2017's conference and contains none by construction, not used as evidence either way.

**Internal precedent**
- [The Origin Stories of Black Hat, DEF CON, and BSides Las Vegas, and How They Evolved, Nexus report (2026-07-27, updated through 2026-08-02)](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-27-blackhat-defcon-origin-history.md) — the combined timeline this question is checking for a post-2016 gap.

## New Skills

None. See Turing's note above.

## Library Recommendations

**Not recommended for archiving as a standalone fact-sheet.** This report's real content is a comparative judgment call (what counts as "same caliber," and why the post-2016 record looks thin) rather than a durable, reusable set of facts — it would need re-litigating rather than just re-citing if asked again in a year, especially since Popper's point 1 (canonization lag) means the honest answer could change as later events get mythologized. If Rick wants the 2023 AI Village Generative Red Team Challenge specifically added to the origin-history report's combined timeline — the strongest candidate found this pass — that would follow the same two-step pattern already used for Back Orifice: a dedicated deep-dive report first, then an explicit Update Pass adding it to the timeline with a hotlink, only on Rick's go-ahead. Status: not proposed to `nexus-artifacts`; timeline addition not yet requested.
