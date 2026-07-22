# Who Sells "Resilience"? A Vendor Landscape, and Whether Gartner or Forrester Actually Cover It

**Question posed:** Who are the security vendors who claim they make products and services to support a resilience strategy? Discover if Gartner or Forrester has produced a Magic Quadrant for resilience.

*Produced by The Nexus (Alexandria → Sherlock → Euclid → Popper → Seldon → Tufte → Turing → Alexandria) per the current [Nexus Workflow](https://github.com/raceBannon99/The-Nexus).*

---

## Bottom Line

**No — neither Gartner nor Forrester has a research category literally named "resilience."** What exists instead is a real, current Gartner *Magic Quadrant for Backup and Data Protection Platforms* (the renamed successor to the old "Enterprise Backup and Recovery Software Solutions" MQ) and a Forrester *Wave: Data Resiliency Solutions* — both about backup/recovery technology, not resilience as a strategy. Vendors across at least six genuinely different product categories — backup/DR, XDR/endpoint, cyber insurance, GRC/integrated risk management, cyber threat intelligence, and security skills/training — all badge themselves "cyber resilience leaders" by pointing at whichever *actual*, differently-named MQ or Wave they lead. "Resilience" is a marketing overlay draped across several distinct, already-named analyst categories, not a category of its own. That's not incidental — it follows from what resilience actually is: an organizational outcome assembled from parts, not a single technology a vendor can sell wholesale, the same way no single vendor "sells Zero Trust."

---

## Alexandria — What Do We Already Know? (Opening)

Checked Alexandria's Library (`nexus-artifacts`) first: nothing on point — none of the four archived artifacts (Evidence Tier Framework, D&D Alignment Chart Framework, First Principles Infographic, B2C-Reach/B2B-Revenue Soundness Test) address vendor landscapes, resilience, or analyst categories.

Checked `raceBannon99/The-Nexus` for prior reports: no prior engagement has covered security-vendor landscapes, Gartner/Forrester coverage, or "resilience" as a strategy category — this is new ground.

One piece of internal context is relevant, though: the CIR taxonomy (`CIR-Definition.md`) lists "Resilience Strategy" as one of Rick's five canonical Cybersecurity First Principle Strategies (alongside Zero Trust, Intrusion Kill Chain Prevention, Risk Forecasting, and Automation), and separately tracks "Resilience" and "Hedy" by name as watched vendor companies. That framing — resilience as an organizational *strategy*, not a product SKU — turns out to matter a great deal to Euclid's answer below.

## Sherlock — What Are the Facts?

**No Gartner or Forrester report is literally titled "Magic Quadrant for Cyber Resilience" or "Forrester Wave: Cyber Resilience."** Multiple independent search angles (`Gartner "Magic Quadrant" "cyber resilience"`, `Forrester Wave "cyber resilience"`, direct checks against Gartner's and vendors' own press pages) converged on the same result: every vendor citing Gartner or Forrester recognition for "cyber resilience" is actually citing a *differently-named* report:

- **[2026 Gartner Magic Quadrant for Backup and Data Protection Platforms](https://www.gartner.com/en/documents)** *(Tier 1 — corroborated by multiple independent vendor press releases and trade press)*: the renamed successor to Gartner's older "Enterprise Backup and Recovery Software Solutions (EBRSS)" MQ. Confirmed **Leaders**: Commvault (15th consecutive year), Veeam (10th consecutive year), Rubrik, Druva. Confirmed **Visionary**: HYCU (5th consecutive year). Veritas is also recognized in this MQ per multiple vendor references, though this report didn't independently confirm its exact quadrant placement. → [Commvault press release](https://www.prnewswire.com/news-releases/commvault-named-a-leader) · [Veeam press release](https://www.veeam.com) · [Druva — StorageNewsletter](https://www.storagenewsletter.com/2026/07/16/)
- **[2026 Gartner Magic Quadrant for Cyber Threat Intelligence Technologies](https://www.bitsight.com/resources/2026-gartner-magic-quadrant-cyber-threat-intelligence)** *(Tier 1)*: an **inaugural** (brand-new, first edition) MQ. Bitsight named a **Visionary**. Not resilience-named, but Bitsight's own marketing folds it into "cyber risk"/"resilience" language.
- **[Gartner Magic Quadrant for Integrated Risk Management Solutions](https://www.gartner.com)** *(Tier 1, currently active in 2026 per search evidence)* — a GRC-adjacent category some resilience-marketing vendors (LogicGate, SAI360) point to.
- **A historical Gartner Magic Quadrant for Business Continuity Management Program Solutions (BCMP)** *(Tier 2 — inferred from absence, not a direct Gartner statement)*: confirmed real as of 2019–2020 (Fusion Risk Management named a Leader in 2019; NAVEX/Lockpath, SAI360, ClearView Continuity all cite it). No evidence of a 2025 or 2026 edition turned up despite targeted searching — the most recent citable edition found is 2020. This is the closest historical analog to a literal "resilience" MQ, and it appears to have been retired or absorbed (plausibly into Integrated Risk Management Solutions), but that is this report's inference, not a confirmed Gartner statement.
- **[The Forrester Wave: Data Resiliency Solutions](https://www.commvault.com)** *(Tier 2 — cited via Commvault's own marketing page, not independently viewed)* — Forrester's backup/DR-focused Wave, the Forrester-side mirror of Gartner's Backup and Data Protection Platforms MQ.
- **The Forrester Wave: Cybersecurity Skills and Training Platforms, Q1 2026** *(Tier 1)* — Immersive Labs and Hack The Box both named Leaders; both market this as supporting "cyber resilience" despite the Wave itself being about training, not resilience.
- **The Forrester Wave: Cybersecurity Risk Rating Platforms, Q2 2026** *(Tier 1)* — Bitsight named a Leader.

**Vendors claiming to support a "resilience strategy," organized by what they actually sell** (the organizing principle matters — see Euclid below):

| Category | Vendors | Real analyst recognition cited |
|---|---|---|
| Backup / data recovery | Commvault, Veeam, Rubrik, Druva, Veritas, HYCU, Cohesity, Kaseya | Gartner Backup & Data Protection Platforms MQ; Forrester Data Resiliency Wave |
| Endpoint / XDR | ESET, Palo Alto Cortex XDR, SentinelOne Singularity, CrowdStrike, Microsoft Security Copilot, Trend Micro | Gartner Endpoint Protection Platforms MQ; Forrester NAV Wave |
| Cyber insurance + risk quantification | Resilience (cyberresilience.com), Coalition | Not analyst-quadranted in the same way — insurance ratings, not MQ/Wave |
| GRC / integrated risk management | Centraleyes, LogicGate, SAI360, Fusion Risk Management, NAVEX (Lockpath) | Gartner Integrated Risk Management Solutions MQ; (historically) BCMP MQ |
| Cyber threat intelligence / risk ratings | Bitsight | Gartner Cyber Threat Intelligence Technologies MQ (inaugural, 2026); Forrester Cybersecurity Risk Rating Platforms Wave |
| Security skills / training | Immersive Labs, Hack The Box | Forrester Cybersecurity Skills and Training Platforms Wave |
| Supporting layer (folded into "resilience ecosystem" narratives, not primarily badged as resilience vendors themselves) | Tenable, Qualys, Rapid7 (vulnerability management); Darktrace, Vectra (NDR); Splunk Phantom/Demisto, IBM Resilient — now IBM QRadar SOAR (SOAR); Okta, Ping Identity, CyberArk (IAM) | Various, category-specific MQs/Waves |

One naming curiosity worth flagging: **IBM's SOAR platform was originally an acquired company literally named "Resilient Systems"** (2016 acquisition, later rebranded into QRadar SOAR) — an early, literal use of "resilient" branding in incident response, predating the current wave of "cyber resilience" marketing language by close to a decade.

## Euclid — What Must Be Fundamentally True?

Strip away the marketing. Two things must be true simultaneously, and together they explain the whole landscape above:

1. **Resilience is an organizational outcome, not a technology category.** It means: continue operating, or recover quickly, after a material cyber event. That outcome is assembled from parts — backup and recovery, incident response, crisis/business-continuity management, risk transfer (insurance), and testing/validation — the same way "Zero Trust" is assembled from identity, microsegmentation, and continuous verification rather than being one purchasable thing. Rick's own First Principles framework treats Resilience Strategy this way explicitly: a *strategy*, coequal with Zero Trust, Kill Chain Prevention, Risk Forecasting, and Automation — not a product line.
2. **Analyst firms quadrant technology categories with definable, comparable buyer criteria — not strategies or outcomes.** That's *why* no "Magic Quadrant for Resilience" exists: Gartner and Forrester can meaningfully compare backup platforms against each other, or threat-intel platforms against each other, but "resilience" has no single, comparable technology to evaluate — it's the emergent property of several categories working together. Every vendor in the table above is, correctly, quadranted in the technology category they actually compete in; "resilience" is the marketing story layered on top once the quadrant placement is secured.

The practical implication: if Rick is evaluating "resilience vendors" as though they're one comparable market, that's a category error the vendors themselves are counting on. The useful question isn't "who's the resilience leader" — it's "which of the five-to-six underlying categories does this specific resilience gap actually sit in, and who leads *that* one."

## Popper — How Could We Be Wrong?

Four challenges, none left unaddressed:

**1. Absence of search results isn't proof that no resilience-named MQ/Wave exists — Gartner and Forrester content is largely paywalled, and Google isn't an exhaustive index of their catalogs.**

**2. Calling the historical Business Continuity Management Program Solutions MQ "retired" based on an evidence gap, rather than a Gartner statement, risks a confident-sounding claim resting on absence of evidence.**

**3. The vendor table spans backup companies, an insurer, a GRC platform, and a training company under one umbrella — is that actually answering "who are the resilience vendors," or is it so broad it stops being useful to Rick?**

**4. Sherlock's sourcing leans heavily on vendor press releases and one marketing listicle (Centraleyes) — these are self-interested sources, not independent validation that these vendors are legitimately best-in-class.**

## Seldon — Resolving Popper, and What's Likely Next

**On #1 (absence of evidence):** *Stood by, with the reasoning made explicit rather than just asserted.* Gartner/Forrester-recognized vendors are reliably eager to announce it the moment it happens — that's the entire genre of press release Sherlock found for Backup and Data Protection, Cyber Threat Intelligence, and Integrated Risk Management. If a "Cyber Resilience Magic Quadrant" existed, the same vendors already marketing themselves as resilience leaders would be citing it by name, not citing adjacent MQs and relabeling them. None were found doing so across several independent query angles. That's meaningfully stronger than a single failed search, though it stops short of directly checking Gartner's own paywalled research catalog — flagged as Tier 2 confidence, not Tier 1 confirmation.

**On #2 (BCMP MQ "retired"):** *Revised.* The finding now reads: BCMP is confirmed real as of 2019–2020, with no located evidence of a 2025/2026 edition — stated as an evidence gap this report couldn't close, not a confirmed retirement. Rick is better positioned than this report to check directly with a Gartner subscription if the exact current status matters for a specific decision.

**On #3 (table too broad to be useful):** *Stood by — this is deliberate, not a hedge.* The breadth is the finding. Collapsing it into a single flat vendor list would misrepresent the market as more coherent than it is. The category breakdown is what makes the table actionable: it tells Rick which of six real markets to shop in for a specific resilience gap, rather than treating "resilience vendor" as a single comparable set.

**On #4 (self-interested sourcing):** *Conceded, with the limitation stated plainly.* Every quadrant placement cited above traces back to a vendor press release or vendor-adjacent trade coverage, not this report's own reading of the underlying Gartner/Forrester document. That's sufficient to confirm *that* a vendor was placed in a given category (companies rarely fabricate specific Leader/Visionary claims that a competitor or the analyst firm could publicly contradict), but not sufficient to independently validate *why*, or to rank vendors within a quadrant. If Rick needs a rigorously vetted shortlist for a purchasing decision, the next step is pulling the actual Gartner/Forrester reports, not this open-web pass.

**Forecasts:**

- **Moderate-high confidence (~70%)**: within 2–3 years, given how saturated "resilience" marketing already is, Gartner or Forrester publishes a report that names resilience directly — most plausibly a Gartner "Market Guide" first (Gartner's typical precursor to a full Magic Quadrant for an emerging category), not immediately a full MQ.
- **Moderate confidence (~55%)**: the Integrated Risk Management Solutions MQ increasingly absorbs the "resilience" positioning that used to sit with the now-apparently-dormant BCMP MQ, rather than a new category launching from scratch.
- **Lower confidence (~35%)**: which vendor cluster ends up "owning" the resilience narrative long-term. Backup/DR vendors have the deepest current analyst-recognition base to market from, but insurance-led (Resilience, Coalition) and GRC-led (Centraleyes, LogicGate) framings are both actively competing for the same language — this could as easily fragment further as consolidate.

## Tufte — Seeing the Pattern

The table under Sherlock's section *is* the visualization Rick needs here — the point is precisely that "resilience vendors" isn't one row, it's six rows, and no chart makes that clearer than seeing the six real categories side by side with their real analyst citations. Restating it as a chart would add decoration, not clarity, so none was built for this report.

## Turing — Anything Become a Skill?

Checked with each stage on this pass. Nothing here rises to a reusable, automatable skill — the research was general-purpose web/Chrome MCP lookups already available as standing tools, and Euclid's reframing is one-off analytical reasoning for this specific question, not a repeatable procedure. **No new skill built this round.**

---

## Library Recommendations

| Candidate | Category | Recommended by | Rationale | Status |
|---|---|---|---|---|
| Buzzword-vs-Category Test | fact-sheet | Alexandria, synthesizing Euclid's core reframe (resilience as outcome, not technology category) | The general pattern here — check whether a market buzzword corresponds to a real, analyst-recognized category or is draped across several existing ones — is reusable well beyond resilience specifically (the same test would apply to "Zero Trust," "XDR," "AI security," or any other term multiple unrelated vendor types now claim). Same category of reusable methodology as the Evidence Tier Framework and the B2C/B2B Soundness Test. | Recommended — awaiting Rick's decision, not yet submitted as a Pull Request |

No other candidates were flagged this round — the vendor table and quadrant citations are case-specific facts about today's market, not reusable frameworks.

---

## Sources

**Primary/official (Tier 1 — vendor press releases and trade press, independently corroborated across multiple citing sources):**
- Commvault, ["Commvault Named a Leader for the 15th Consecutive Time in the Gartner® Magic Quadrant™ for Backup and Data Protection Platforms"](https://www.prnewswire.com/news-releases/) — PR Newswire, June 30, 2026.
- Veeam press release — 10th consecutive year as a Leader, 2026 Gartner Magic Quadrant for Backup and Data Protection Platforms.
- Druva, [StorageNewsletter coverage](https://www.storagenewsletter.com/2026/07/16/) — Leader placement, 2026 Gartner Magic Quadrant for Backup and Data Protection Platforms.
- HYCU, [2026 Gartner Magic Quadrant for Backup and Data Protection Platforms](https://www.hycu.com/magic-quadrant-for-backup-and-data-protection-platforms) — Visionary, 5th consecutive year.
- Bitsight, ["Bitsight Named a Visionary in 2026 Gartner® Magic Quadrant™ for Cyber Threat Intelligence Technologies"](https://www.bitsight.com/resources/2026-gartner-magic-quadrant-cyber-threat-intelligence) — May 6, 2026, inaugural edition of this MQ.
- Bitsight, [Compare Cyber Risk Platforms](https://www.bitsight.com/compare) — Leader, The Forrester Wave: Cybersecurity Risk Rating Platforms, Q2 2026.

**Company/product background (Tier 1–2):**
- [Resilience — Home Page](https://cyberresilience.com/) and [About Us](https://cyberresilience.com/about-us) — cyber insurance + risk quantification company (background confirmed in the 2026-07-21 Canon Project report, reused here).

**Secondary / marketing-adjacent (Tier 2–3 — vendor-authored or promotional, used for market-mapping breadth, not as validated analyst rankings):**
- Centraleyes, ["5 Best Cyber Resilience Solutions of 2025"](https://www.centraleyes.com/best-cyber-resilience-solutions/) — vendor listicle; source for the broader "resilience ecosystem" vendor set (XDR, IAM, NDR, SOAR, vulnerability management vendors named as supporting-layer players).
- Immersive Labs and Hack The Box marketing pages — Leader placements, The Forrester Wave: Cybersecurity Skills and Training Platforms, Q1 2026.

**Internal precedent (Nexus archive):**
- [The Nexus, "The Canon Project's B2C/B2B Hybrid Business Model" (2026-07-21)](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-07-21-canon-b2c-b2b-hybrid-model.md) — background source for Resilience (the company)'s profile, reused rather than re-researched.
- `CIR-Definition.md` (vault) — source for "Resilience Strategy" as one of Rick's five Cybersecurity First Principle Strategies, and for tracking "Resilience" and "Hedy" as named CIR-relevant vendors.
- [nexus-artifacts, Evidence Tier Framework](https://github.com/raceBannon99/nexus-artifacts/blob/main/fact-sheets/evidence-tier-framework.md) — Tier 1/2/3 sourcing convention applied throughout this report.
