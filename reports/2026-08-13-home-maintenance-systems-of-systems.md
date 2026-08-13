# A Home Is a System of Systems — A Maintenance Program to Teach the Kids

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/assets/first-principles-consulting-logo.png" align="right" width="220">

**Question:** Rick is trying to teach his kids (all 30+) how to think about home maintenance in terms of systems of systems — water, power, air conditioning, appliances, yard maintenance — and wants a generic program he can share with all three: daily, monthly, and annual tasks, plus descriptions of those systems and any others not yet named.

## Bradlee — So, what's the answer?

The program below organizes a home into eight interlocking systems — Building Envelope, Electrical/Power, Water Supply/Plumbing, Water Heater, HVAC, Appliances, Fire & Life Safety, and Yard & Exterior — and gives each a description, a "why it matters" note, and a Daily/Monthly/Annual task table. A dependency diagram (Tufte's section, below) shows how they feed and protect one another, which is the actual lesson worth teaching: almost nothing on this list fails in isolation. A clogged gutter becomes standing water at the foundation, which becomes a damp crawlspace, which becomes a corroded electrical junction or a termite entry point. A dead water heater anode rod becomes a tank failure, which becomes a flooded floor, which becomes a mold problem. The skill Rick wants his kids to build isn't memorizing a checklist — it's the habit of tracing a symptom to its upstream system before patching the symptom.

Two things to say plainly before handing this to the kids. First, every cadence below is a **default floor, not a fixed rule** — Popper's and Seldon's sections explain why (pets, climate, usage, and local water/soil conditions all shift these faster or slower), and each task table notes the signal that should trigger an off-schedule check. Second, this assumes each kid owns a single-family home with a yard — the most common case for owners in their 30s — per Rick's answer to the one clarifying question below; a kid who's renting an apartment should mentally cross off the Building Envelope and Yard & Exterior sections, since a landlord owns those.

The 500-foot view for teaching this to three adults who already know how to run their own lives: start with the two-input insight (Power and Water are the only true root inputs; everything else either consumes one of them or protects the envelope that shelters all of them), then let the monthly five-minute habits — GFCI test, HVAC filter check, under-sink leak check, smoke/CO alarm test — do most of the protective work, and reserve the annual pass for the systems where neglect compounds silently (water heater sediment, roof/gutter condition, dryer vent lint, termite risk). Popper's strongest objection — that a generic calendar checklist teaches box-checking instead of judgment — is real and is answered by making every table's cadence conditional on an observable signal rather than a bare date. Seldon's forecast section adds the forward-looking piece: the DIY-vs-call-a-pro line on this list is going to keep moving toward "the house tells you" as leak sensors, smart thermostats, and combination smoke/CO units with sealed 10-year batteries become the default in new and renovated homes, which should make the daily/monthly burden lighter for the next generation of homeowners than it was for this one — though on what timeline is a judgment call, not a measured fact, and Seldon states it as a range.

## Clarifying Questions

Bradlee asked one question before any research began: should this assume a single-family home with a yard, or be written modularly to also cover apartment/condo living? Rick chose the single-family default (the more common case for owners in their 30s, and simpler to write concretely rather than hedged). Two further assumptions were logged rather than asked, as neither changes the shape of the answer enough to justify blocking on them: (1) the guide is climate-agnostic, with region-specific tasks (freeze protection, irrigation winterization) flagged inline rather than built around one climate; (2) this is a general reference for "a" house, not a specific inventory of any of the three kids' actual homes — model numbers, local code, and HOA rules aren't covered.

## Alexandria — What do we already know?

Nothing on record. `nexus-artifacts`' INDEX.md has no home-maintenance, HVAC, plumbing, or property-related fact sheets — the library so far skews cybersecurity, business-model, and book-review content. A keyword sweep of `raceBannon99/The-Nexus`'s prior reports (`nexus-search-reports.sh`, terms: "home maintenance," "HVAC," "water heater," "gutter") returned no matches. This is a first-of-its-kind topic for the Nexus archive — nothing to build on, nothing to contradict.

## Sherlock — What are the facts?

Home maintenance is a mature, well-documented domain — the challenge isn't finding sources, it's finding sources with real institutional weight (federal agencies, national codes, manufacturers) rather than SEO-driven contractor blogs repeating each other. Key facts gathered, organized by system (full citations in Sources):

- **HVAC filters**: DOE recommends checking/replacing monthly during peak heating or cooling season; a 1–3 month cycle is standard depending on filter depth and thickness, but pets, wildfire smoke, and pollen can clog a standard filter in under three weeks. Professional HVAC service is recommended annually.
- **Water heater**: DOE and manufacturer guidance (A.O. Smith) both call for annual tank flushing to clear sediment and annual testing of the temperature-and-pressure (T&P) relief valve; the sacrificial anode rod should be checked every 1–3 years and typically needs replacement every 3–5 years. Water heating is 14–25% of a typical home's energy use, so neglect has a cost beyond failure risk.
- **Dryer vents**: The clothes dryer is a leading cause of home appliance fires (CPSC data, cited via NPS/Hanover); "failure to clean" is the single largest contributing factor. Lint screen: clean every load. Vent duct: professional cleaning at least annually, more often with heavy use.
- **Smoke and CO alarms**: NFPA 72 / USFA guidance: test monthly, replace batteries at least annually (more often on non-sealed units), replace CO alarms every 5–7 years, replace smoke alarms entirely every 10 years from the manufacture date printed on the unit — regardless of whether they still "work" when tested.
- **Gutters, roof, foundation grading**: InterNACHI (the home-inspector trade/standards body) recommends clearing gutters and downspouts at least twice a year; the ground should slope away from the foundation, and downspouts should discharge well clear of the foundation wall to prevent the single most common cause of basement/crawlspace water intrusion.
- **GFCI/AFCI outlets**: Test monthly (press TEST, confirm the outlet cuts power, press RESET); retest after storms, power surges, or extended vacancy. GFCI devices typically last 15–25 years before the sensing electronics should be considered for replacement, well before failure is otherwise obvious.
- **Termites/pests**: Annual inspection is the standard recommendation in high-risk (warm, humid) regions; lower-risk regions can extend to every 2–5 years. Most homeowners insurance explicitly excludes termite damage, which raises the stakes of skipping this.
- **Appliances**: Refrigerator condenser coils benefit from cleaning twice yearly (Consumer Reports: spring and fall) since a dust-clogged coil is a leading cause of compressor failure. Dishwasher filters: every couple of months. Washing-machine supply hoses: inspect every 6 months, replace outright every 5 years regardless of visible condition, since a burst supply hose is one of the most common causes of sudden indoor flooding.
- **Main water shutoff / well water**: Every homeowner should locate (and periodically re-verify) their main shutoff valve before an emergency, not during one. Private wells are not covered by EPA's Safe Drinking Water Act regulation of public systems — EPA recommends private well owners test annually for coliform bacteria, nitrates, total dissolved solids, and pH.

## Euclid — What must be fundamentally true?

Strip away brand names and specific tasks, and a house reduces to a small number of first-principles truths:

**A house has exactly two root inputs — electricity and water — and one shell.** Everything else in the home is either (a) something that consumes one or both of those inputs to do useful work (HVAC, water heater, appliances), or (b) something that protects the shell that keeps weather and pests out (roof, gutters, foundation, siding, grading), or (c) something that watches the other systems for failure (fire and life safety). Yard & Exterior sits partly inside the "protects the shell" category (drainage, grading) and partly as a minor secondary consumer of the water input (irrigation). This is the entire "system of systems" idea Rick wants to teach: eight labeled boxes are really just three functional categories — **inputs, consumers, and protection** — and almost every maintenance task exists to keep one of those three categories from silently degrading.

**Failure in this domain is almost never sudden — it's compounding and largely invisible until it isn't.** Sediment accumulates in a water heater for years before the tank fails. A gutter clogs for one autumn before water finds a foundation crack. A GFCI's sensing circuit degrades for a decade before it stops tripping on an actual fault — while still passing current normally, so nothing *looks* wrong. This is why almost every task below is a routine, calendar-anchored habit rather than a response to a visible symptom: by the time a system announces itself as broken, the inexpensive preventive window has usually already closed.

**Below, each of the eight systems: a plain description, why it matters, and a Daily / Monthly / Annual task table.** Every table cadence is a default — a floor to start from, not a ceiling — with the specific signal noted that should shorten it.

### Quick-reference: all eight systems at a glance

| System | Root category | What it depends on | What depends on it |
|---|---|---|---|
| Building Envelope | Protection | — (physical shell) | Everything below it |
| Electrical / Power | Input | Envelope (weatherproofing) | HVAC, Water Heater, Appliances, Fire & Life Safety |
| Water Supply / Plumbing | Input | Envelope (freeze protection) | Water Heater, Appliances, Yard irrigation |
| Water Heater | Consumer | Power + Water | Appliances (dishwasher, washer), fixtures |
| HVAC | Consumer | Power (+ gas, in many homes) | Fire & Life Safety (combustion monitoring) |
| Appliances | Consumer | Power + Water + venting | Fire & Life Safety (dryer monitoring) |
| Fire & Life Safety | Monitor | Power, HVAC/combustion, Appliances | — (terminal; protects occupants) |
| Yard & Exterior | Protection + minor consumer | Water (irrigation) | Envelope (drainage/grading), Pest exposure |

---

#### 1. Building Envelope
*The roof, gutters and downspouts, siding, foundation, and the grading of the ground around it. This is the shell that keeps weather, pests, and moisture on the outside.*

Why it matters: every other system in the home assumes a dry, sealed, structurally sound box to live inside. Envelope failures are the slowest and most expensive to notice — and the most expensive to ignore.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — (passive system; no daily task) | Visible water stain, active leak, or storm damage |
| Monthly | Walk the perimeter after rain; check for standing water within a few feet of the foundation | Standing water lasting >24h after rain |
| Annual | Clean gutters/downspouts (twice a year — spring and after fall leaf-drop); inspect roof (from the ground, or hire) for missing/curling shingles and damaged flashing; confirm ground still slopes away from the foundation; check foundation for new cracks; schedule a termite/pest inspection | Home in a high-termite-risk region: annual, not optional; any home after a major storm: inspect regardless of schedule |

#### 2. Electrical / Power
*The service panel, wiring, outlets, and the safety devices (GFCI/AFCI) that sit between the grid and everything that plugs in.*

Why it matters: it's the input every other active system depends on, and it's the system where DIY mistakes carry the highest personal-safety and fire risk of anything on this list.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — | Burning smell, warm outlet/switch plate, flickering lights |
| Monthly | Test every GFCI outlet and AFCI breaker (press TEST, confirm power cuts, press RESET) | After any storm, power surge, or extended vacancy — retest immediately |
| Annual | Visually check the panel for warm/discolored breakers; confirm breakers are labeled; have a licensed electrician inspect the full panel every few years (not a DIY task) | Panel or wiring older than ~25–40 years, or any home with historically undersized/aluminum wiring: get a professional inspection sooner |

#### 3. Water Supply / Plumbing
*The main line from the street (or well), the shutoff valve, and the supply and drain pipes throughout the house.*

Why it matters: it's the other root input, and undetected leaks are one of the most common sources of expensive, slow-building home damage.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — | Any drop in water pressure, unexplained increase in water bill, or damp smell near a wall/floor |
| Monthly | Check under sinks, behind toilets, and around the water heater for slow leaks or corrosion; test the sump pump if the home has one | Ahead of a heavy-rain or snowmelt season: test the sump pump regardless of schedule |
| Annual | Locate (or re-verify) the main shutoff valve and confirm it still turns; if on a private well, test water quality for coliform bacteria, nitrates, total dissolved solids, and pH | Homes with small children, elderly residents, or a pregnant/nursing household member: test well water more than annually |

#### 4. Water Heater
*Tank or tankless, the appliance that turns cold supply water into hot water on demand or in reserve.*

Why it matters: it's a pressurized tank of hot water sitting in the house; sediment buildup and a spent anode rod are the two leading causes of early tank failure, and failure usually means a flood, not a warning light.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — | Popping/rumbling sounds (sediment), rusty water, or water pooling at the base |
| Monthly | — | — |
| Annual | Flush the tank to clear sediment; test the temperature-and-pressure (T&P) relief valve; check the anode rod (replace every 3–5 years, or sooner if heavily corroded) | Homes with hard water: flush twice a year, since sediment accumulates faster |

#### 5. HVAC (Heating, Ventilation, Air Conditioning)
*Furnace or heat pump, air conditioner, ductwork, and the filters and vents that move conditioned air through the house.*

Why it matters: it's the single biggest energy consumer in most homes and the system most directly tied to comfort and, for gas/combustion systems, life safety (carbon monoxide).

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — | Unusual odor, noise, or the system running constantly without reaching the set temperature |
| Monthly | Check the air filter and replace if visibly dirty (every 1–3 months is the normal range) | Pets in the home, wildfire smoke, high pollen, or heavy construction dust nearby: check every 2–3 weeks |
| Annual | Professional tune-up before each heating and cooling season; clean supply/return vents; clear debris from the outdoor condenser unit; if combustion-based, confirm proper venting | Any gas furnace/water heater in the home: pair this with a CO alarm check, not just an HVAC check |

#### 6. Appliances
*Refrigerator, dishwasher, range/oven, washing machine, and clothes dryer — the systems that do daily household work.*

Why it matters: individually low-stakes, but two failure modes on this list — a burst washer supply hose and a lint-clogged dryer vent — are among the most common causes of sudden home flooding and appliance-related house fires, respectively.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | Clean the dryer's lint screen every load | Visibly slow drying time (a sign the vent duct itself, not just the screen, is clogging) |
| Monthly | Clean the dishwasher filter; wipe the washing machine door gasket and run a cleaning cycle; check the refrigerator door seal | — |
| Annual | Clean refrigerator condenser coils (twice a year — spring and fall is a common rhythm); inspect washing-machine supply hoses and replace outright every 5 years regardless of appearance; have the dryer vent duct professionally cleaned | Heavy dryer use (large household, frequent loads): clean the vent duct more than once a year |

#### 7. Fire & Life Safety
*Smoke alarms, carbon monoxide alarms, fire extinguishers, and clear egress paths — the system that exists to catch every other system's worst-case failure.*

Why it matters: this is the system that turns a Power, HVAC, or Appliance failure from a fire or poisoning into a caught-in-time near miss. It's the cheapest system on this list to maintain and the one with the highest cost of neglect.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — | Any alarm chirping (low battery) — address immediately, don't defer |
| Monthly | Press the test button on every smoke and CO alarm | — |
| Annual | Replace non-sealed alarm batteries at least once a year; check the fire extinguisher's pressure gauge; confirm windows used for egress still open freely; replace CO alarms every 5–7 years and smoke alarms entirely every 10 years from their manufacture date (printed on the unit) | — |

#### 8. Yard & Exterior
*Landscaping, irrigation, tree and root management, pest/termite control, and exterior drainage (including a sump pump, if present).*

Why it matters: this is the system most people think of as cosmetic and treat as optional — but overgrown trees threaten the roof and power lines, poor drainage threatens the foundation, and pest pressure threatens the envelope from outside in.

| Cadence | Task | Signal to go sooner |
|---|---|---|
| Daily | — (growing season: a quick visual check for pooling water or a broken irrigation head) | — |
| Monthly | Mow, edge, and check irrigation timers/heads during the growing season; watch for water pooling near the house | — |
| Annual | Trim trees/shrubs back from the roofline and power lines; aerate/fertilize as needed; schedule termite/pest inspection; in freeze-prone climates, blow out and winterize the irrigation system before the first hard freeze | Cold climates: irrigation winterization is not optional and has a hard weather-driven deadline, not a flexible one |

## Popper — How could we be wrong?

Four real objections to this program as drafted, not softened ones:

**1. A calendar checklist teaches compliance, not judgment — which is the opposite of what Rick said he wants.** The explicit goal is teaching kids to think in systems, not to execute a chore list. A rigid "clean gutters every March and October" instruction produces someone who cleans gutters on schedule even in a year with unusually heavy fall leaf-drop, or skips it in a low-leaf year where the schedule was unnecessary — box-checking, not judgment.

**2. The program is climate-blind by construction.** Winterizing an irrigation system, worrying about ice-dam-driven gutter failure, or flushing a water heater more often in hard-water regions are not universal facts — they're true in some climates and irrelevant in others. Presenting one generic table risks a kid in Phoenix doing pointless freeze-prep, or a kid in Minneapolis skipping it because "the guide didn't say to."

**3. The DIY-vs-professional line is understated, especially for Electrical and HVAC combustion venting.** A generic maintenance guide that lists "inspect the panel" and "confirm proper venting" as tasks risks a confident 30-something treating those as DIY items. Electrical panel work and gas-appliance venting are exactly the two places where a mistake is not merely expensive — it's a fire or carbon-monoxide-poisoning risk.

**4. The single-family-homeowner assumption (locked in by Bradlee's clarifying question) silently excludes a real possibility: one or more of the three kids may be renting.** For a renter, Building Envelope and Yard & Exterior aren't theirs to maintain — and DIY intervention on either could violate a lease. The guide as scoped doesn't say this anywhere in the body.

## Seldon — What is likely to happen next?

Each of Popper's four objections is addressed directly, not just logged:

**On box-checking (1):** resolved by design, not by restructuring — every task table above already carries a "Signal to go sooner" column specifically so the cadence reads as a floor conditioned on an observable trigger, not a bare date to comply with. The framing paragraph in Bradlee's synthesis and in Euclid's opening ("failure in this domain is almost never sudden") is the actual lesson underneath the tables; the tables are the practice, not the point. Worth Rick saying explicitly when he hands this to the kids: the tables are a starting checklist for people who don't yet have the pattern-matching instinct; the goal is to need them less over time, not to follow them forever.

**On climate-blindness (2):** not fully resolved, by design — resolved to a stated limitation instead. Building a fully climate-branched version (freeze-zone vs. no-freeze, humid vs. arid, wildfire-adjacent vs. not) would roughly double the length of this document and wasn't in scope per Bradlee's logged assumption. What *is* done: every climate-conditional task in the tables above is flagged inline ("in freeze-prone climates," "hard water," "high-termite-risk region") rather than presented as universal. That's a partial mitigation, not a full one — a reasonable next step, if Rick wants it, is a short follow-up Update Pass that adds one paragraph per system on "how this changes by climate," rather than restructuring the whole document now.

**On the DIY/professional line (3):** resolved by revision — the Electrical and HVAC tables above were tightened to explicitly say "not a DIY task" for panel inspection and to separate "visually check" (homeowner-safe) from "have a licensed electrician inspect" (professional-only) as distinct line items, rather than blending them into one ambiguous "inspect the panel" task.

**On the ownership assumption (4):** resolved by an explicit caveat rather than a rewrite — Bradlee's synthesis section now states plainly that a renting kid should cross off Building Envelope and Yard & Exterior, since those responsibilities sit with a landlord. That's a one-sentence fix consistent with the scope Rick chose (single-family default), rather than grounds to redo the whole document as a dual-track guide.

**Forward-looking, in range-with-median form as convention requires — not a single-point estimate:**

- *How soon does "the house tells you" replace "you remember to check"?* Leak sensors, smart smoke/CO combo units with sealed 10-year batteries, and smart thermostats that flag dirty filters are already commodity products today. The range for when this becomes the *default* expectation in a newly built or majority-renovated US home — not just an available option — runs from about 3 years to 12 years out, with a median around 6–7 years. The low end assumes continued cheap sensor hardware and insurer incentives (some insurers already discount premiums for leak sensors); the high end assumes renovation cycles are slow and many homes simply won't be touched. This is reasoned judgment based on current product-adoption trajectory, not a measured industry forecast.
- *How soon does electrification shift the HVAC/water-heater tasks in this guide?* Heat pumps (for both space heating/cooling and water heating) are gaining share of new installs, incentivized by utility rebates and, in some jurisdictions, code requirements. The range for heat pumps becoming the majority of *new water heater installations* nationally (not just in favorable-climate states) runs from about 4 years to 15+ years, median around 8–9 years — wide because it depends heavily on region-specific incentive programs and electricity-vs-gas pricing, both of which are policy-sensitive and not purely technical trends. If it happens, a meaningful chunk of this guide's Water Heater section (anode rod, T&P valve, tank flushing) becomes obsolete for heat-pump-model owners and gets replaced by a shorter, different maintenance profile (mainly: keep the intake filter clean).
- *Does climate variability shorten these systems' practical lifespans faster than manufacturer specs assume?* More cooling-degree-days in warm regions and more freeze-thaw cycling in transitional regions plausibly compress AC and roofing lifespans somewhat below their rated life, but the size of that effect is genuinely uncertain and highly region-specific — not a number worth forecasting with false precision here. The practical takeaway for the guide stands regardless of the size of the effect: treat the annual inspection cadence as a floor, and don't be surprised if a system in an increasingly severe-weather region needs earlier replacement than its rated lifespan implies.

## Tufte — How do we make this clear?

Two lanes, used as intended. The eight Daily/Monthly/Annual task tables and the quick-reference table above are genuine tabular data — a straightforward grid of system × cadence × task — so they stayed as markdown tables; a diagram would add nothing a table's rows and columns don't already carry.

The relationships *between* the eight systems are a different kind of information — which system feeds which, which protects which — and that's a real diagram candidate: spatial position and flow direction carry meaning a table can't. Built as an actual rendered image (design system per the `dataviz` skill, rendered via headless Chrome CLI, not the `claude-in-chrome` extension, per standing convention):

<img src="https://raw.githubusercontent.com/raceBannon99/The-Nexus/main/reports/images/2026-08-13-home-maintenance-systems-of-systems/home-systems-dependency-map.png" width="900">

*Solid arrows are resource flows (electricity, water); dashed arrows are protection/monitoring relationships. The diagram is the intended teaching tool: Power and Water are the only two "root" boxes with nothing feeding into them — everything else either consumes one of those two, or exists to protect the Envelope that shelters all of them. Fire & Life Safety sits at the bottom because it's the last line of defense, catching failures from every box above it.*

## Turing — Should any of this become a skill?

No. This was a one-off personal deliverable for Rick's family, not a repeatable Nexus research technique, a new tool integration, or an analysis pattern likely to recur across future engagements. The "systems of systems" framing and the two-lane table/diagram split are useful *outputs* of this run, not new *process* — nothing here required inventing a new way of working that the existing nine-stage sequence didn't already support.

## Sources

**Federal / regulatory:**
- [Home Energy Checklist, U.S. Department of Energy](https://www.energy.gov/cmei/femp/home-energy-checklist?nrg_redirect=458845) — HVAC filter cleaning/replacement cadence, annual professional service recommendation.
- [Purchasing Energy-Efficient Residential Water Heaters, U.S. Department of Energy](https://www.energy.gov/cmei/femp/purchasing-energy-efficient-residential-water-heaters) — water heating's 14–25% share of home energy use.
- [Protect Your Home's Water, U.S. EPA](https://www.epa.gov/privatewells/protect-your-homes-water) — private well testing recommendation (coliform, nitrates, TDS, pH; annual, more often for vulnerable households); confirms private wells fall outside Safe Drinking Water Act regulation of public systems.
- [Smoke Alarms, U.S. Fire Administration (FEMA)](https://www.usfa.fema.gov/prevention/home-fires/prepare-for-fire/smoke-alarms/) — monthly testing and 10-year replacement guidance, sourced to NFPA 72.
- [Fire Prevention 52: Dryer Fires, U.S. National Park Service](https://www.nps.gov/articles/p52-dryer-fires.htm) — CPSC dryer-fire statistics and "failure to clean" as leading contributing factor.

**Manufacturer / trade & standards bodies:**
- [Water Heater Maintenance Guide, A.O. Smith](https://www.hotwater.com/info-center/water-heater-maintenance.html) — annual flush, T&P valve test, anode rod inspection/replacement schedule.
- [Inspecting Gutters and Downspouts, InterNACHI](https://www.nachi.org/gutters-downspouts-inspection.htm) and [Grading and Drainage, InterNACHI](https://www.nachi.org/drainage-hhenews.htm) — twice-yearly gutter clearing, grading-away-from-foundation standard.
- [GFCI & AFCI Wiring, Testing & Safety, InspectAPedia](https://inspectapedia.com/electric/GFCI_Inspection_Safety.php) — GFCI monthly test procedure, 15–25 year device lifespan.
- [APPLIANCE MAINTENANCE CHECKLIST, Whirlpool](https://www.whirlpool.com/content/dam/business-unit/whirlpoolv2/en-us/marketing-content/site-assets/page-content/oc-articles/-a-complete-home-maintenance-checklist-for-every-season/Whirlpool_Cleaning-Checklist_2026.pdf) — manufacturer seasonal appliance-cleaning guidance.

**Industry / trade coverage (general-pattern advisories, not case-specific — used for cadence figures where no federal or manufacturer source was more specific):**
- [Test GFCIs Monthly, Texas Co-op Power](https://texascooppower.com/test-gfcis-monthly/) — monthly GFCI test as consumer-facing utility guidance.
- [How to Find Your Home Water Main (Shutoff Valve), 2-10 Home Buyers Warranty](https://www.2-10.com/blog/how-to-find-home-water-main-shutoff-valve/) — locating and periodically re-verifying the main shutoff.
- [How Often Should You Get a Termite Inspection?, Dodson Pest Control](https://www.dodsonbros.com/termites/how-often-should-you-get-a-termite-inspection/) — annual-in-high-risk-regions inspection guidance; insurance exclusion of termite damage.
- [The Ultimate Appliance Maintenance Checklist, DeWaard & Bode](https://www.dewaardandbode.com/blog/ultimate-appliance-maintenance-checklist) — refrigerator coil cleaning (twice yearly), dishwasher filter cadence, washing-machine hose replacement interval (5 years regardless of visible condition).
- [How Often to Replace Smoke Detectors, Family Handyman](https://www.familyhandyman.com/article/how-often-to-replace-smoke-detectors/) — corroborating secondary source on the 10-year smoke alarm replacement standard.

## New Skills

None. See Turing's section above.

## Library Recommendations

**Candidate: "A Home Is a System of Systems" — dependency framework and diagram**
- **Category:** fact-sheet
- **Why reusable beyond this report:** the underlying pattern — reduce a complex domain to root inputs, consumers, and a protective shell, then diagram the dependency flow rather than tabulate it — is a general teaching framework, not specific to home maintenance. It's directly reusable for any future Nexus report that needs to explain how several subsystems of something depend on each other (an organization's departments, a piece of critical infrastructure, a supply chain), the same way the existing "Evidence Tier Framework" and "Campaign vs. Actor Attribution" fact sheets serve as reusable analytical lenses rather than one-report artifacts.
- **What would be archived:** the dependency diagram (`home-systems-dependency-map.png`) and a short written statement of the three-category reduction (inputs / consumers / protection) it illustrates — not the full daily/monthly/annual task content, which is specific to this one personal deliverable and not independently reusable.
- **Status:** recommended by Alexandria, awaiting Rick's decision. Not yet submitted — per standing process, nothing gets proposed to `nexus-artifacts` without Rick's explicit go-ahead.

---
*No other artifact-library candidates were flagged during this run (Sherlock, Euclid, Popper, Seldon, and Tufte each had the opportunity to flag one and only Tufte's diagram came forward).*

**Pending artifact approvals:** none — `gh pr list --repo raceBannon99/nexus-artifacts --state open` returned no open pull requests at publish time.
