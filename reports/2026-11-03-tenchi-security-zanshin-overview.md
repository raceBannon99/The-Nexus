# Tenchi Security and Zanshin: What the Panel Sponsor Sells

**Date:** 2026-11-03
**Question:** Scan the sponsor's website and summarize what their products do: https://www.tenchisecurity.com/en

Companion to [`reports/2026-11-03-tpcrm-state-of-the-industry.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-03-tpcrm-state-of-the-industry.md) and [`reports/2026-11-03-tpcrm-panel-draft-responses.md`](https://github.com/raceBannon99/The-Nexus/blob/main/reports/2026-11-03-tpcrm-panel-draft-responses.md).

---

## The Answer (Agent Bradlee)

Tenchi Security sells one product, **Zanshin**, a third-party cyber risk management platform. Its pitch is the panel's title. Instead of rating vendors from the outside or trusting their questionnaires, Zanshin connects inside a consenting vendor's own systems and checks how they are actually configured, every day.

It works in three steps. The customer that buys Zanshin invites its vendors. Each vendor connects Zanshin to its own cloud, identity, endpoint, and SaaS platforms with read-only permissions. Tenchi says it cannot change anything, never touches business data, and passes only metadata about security findings back to the customer. Zanshin then runs what Tenchi calls "thousands" of vulnerability and misconfiguration checks each day, combined with outside-in monitoring of the vendor's internet-facing domains. Platforms named on the site include Microsoft 365, Okta, JumpCloud, CrowdStrike, SentinelOne, Sophos, Bitdefender, Trend Micro, IBM Cloud, DigitalOcean, Azure DevOps, and Zoom.

The customer pays. Vendors use it free, and Tenchi frames that as being "helped rather than being forced to be audited." A Tenchi remediation team works directly with vendors to fix what the scans find. Around the monitoring core, Zanshin has grown a full program toolkit: pre-contract due diligence, self-assessment questionnaires with automatic grading and an AI summary of vendor-submitted PDFs, compliance mapping (NIST CSF 2.0, ISO 27001, PCI DSS, CIS Controls), business-impact tagging, and dashboards. Results come out as a 1.0–10.0 score, an A–F grade, severity-ranked alerts, and a risk-matrix chart.

The company appears to be Brazilian. The site defaults to Portuguese, and its named customers are Brazilian financial institutions: Bradesco, B3, BTG Pactual, Cielo, and IRB(Re). It raised a $7 million Series A led by Bradesco, L4 Venture Builder, and Accenture. Its founders, CEO Felipe Bouças and CTO Alexandre Sieira, previously built Niddel, which Verizon acquired. Tenchi says Gartner lists it as a representative vendor in its 2026 buyer's guide for third-party cyber risk tools. Its headline claims, an 81% drop in vendor vulnerabilities in the first week and more than 90% at Bradesco, are its own unaudited marketing figures.

**One fact matters most for tomorrow.** Tenchi contributed data to the 2026 Verizon DBIR: the analysis of how slowly third parties fix cloud MFA and privilege problems. The figure your drafts cite, that only 23% of third parties fully remediated missing MFA, comes from that dataset. Citing it is accurate, and it's a graceful nod to the sponsor.

**Two adjustments to your drafts.** First, "inside-out" means something different to Tenchi than in your essays. For Tenchi it is telemetry from inside the vendor. For you it is adjusting an industry baseline with knowledge of your own organization. They fit together: better inside-out evidence narrows the forecast. Say that rather than letting the word mean two things on stage. Second, Zanshin itself reports letter grades and a risk matrix. Your line about grades being "the heat map in a new costume" could land as a jab at the host. Frame it instead as: grades are the right tool for running the program, and the board needs a probability. That keeps your position intact without taking a shot at the sponsor.

---

## Clarifying Questions (Agent Bradlee, pre-flight)

None asked. The question is scoped: summarize the sponsor's products from its own website. Assumption logged: since this is panel prep, the summary also flags where the sponsor's positioning touches Rick's drafted answers.

---

## What Do We Already Know? (Agent Alexandria, opening)

Nothing in the Library or prior reports on Tenchi Security or Zanshin. Today's two TPCRM reports are the context: the industry status report and Rick's panel drafts, whose Q3 answer cites the DBIR's third-party MFA figure that turns out to be Tenchi's data. Yesterday's São Paulo briefing (`reports/2026-11-02-sao-paulo-brazil-conference-briefing.md`) is consistent with a Brazilian sponsor, though the site never states Tenchi's location.

---

## The Facts (Agent Sherlock)

All from Tenchi's own site unless noted. This is vendor self-description: claims are the company's, not independently verified.

### Company
- **Product:** Zanshin, a "Third-Party Cyber Risk Management" platform. Homepage tagline: "Immediate. Continuous. Scalable." / "Third-Party Cyber Risk Reduction."
- **Leadership:**
  - Felipe Bouças, co-founder and CEO. Previously co-founded Cipher (acquired by Prosegur) and Niddel (acquired by Verizon).
  - Alexandre Sieira, co-founder and CTO, from the same two companies.
  - Also listed: a CFO, CMO, engineering director, and sales director.
- **Funding:** "US$7 million in a Series A round led by Bradesco, L4 Venture Builder, and Accenture." Investor logos also show Maya Capital, Itaú Ventures, OneVC, and GFC. A linked announcement slug says "R$ 35 milhões." That wasn't opened, and the currency discrepancy is unresolved.
- **Location and founding year:** not stated. The site defaults to Portuguese, and its customers and team are Brazilian.
- **Recognition (self-reported):** Gartner Buyer's Guide for TPCRM Tools 2026 ("representative vendor"), Gartner Market Guide for TPRM Technology Solutions, Gartner Market Overview for TPRM Solutions (July 2026), Verizon 2026 DBIR contributor, IT-Harvest Cyber 150 (2024).

### How Zanshin works
- **Model:** "combin[es] inside-out and outside-in visibility — linking external attack surface monitoring with automated, continuous, scalable, and non-intrusive assessments of cloud infrastructure (IaaS, PaaS, SaaS) and security controls." Testing is "daily."
- **Positioning against ratings:** "Instead of relying on external scans, scores, and firms, our solution unites both parties." "External security scoring services provide a limited understanding of third-party security posture."
- **What the vendor grants:** read-only connectors with "the minimal set of permissions to review security-relevant settings." For Microsoft 365, "only the specific read-only scopes Zanshin needs."
- **Tenchi's commitments to vendors:**
  - "We are read-only and cannot modify your infrastructure."
  - "We cannot and will not get access to your business data."
  - "We do not record any private data, code, or traffic."
  - "Zanshin only provides metadata in reports to your customers."
- **Consent model:** "third-parties consent to being helped rather than being forced to be audited." Relationship modes are "Anonymous or Cooperative," and vendors choose which customers see their scan targets.
- **Who pays:** the customer. Vendors pay nothing ("Your access to Zanshin is paid for completely by your customers"). First-party pricing isn't published.
- **Remediation service:** "Team Tenchi, our Risk Remediation Task Force," works directly with vendors to explain and guide fixes.

### Coverage (named in release notes)
Microsoft 365 (including Intune and Defender for Endpoint), Azure DevOps, Okta Workforce Identity, JumpCloud, CrowdStrike Falcon, SentinelOne Singularity, Sophos Endpoint, Bitdefender, Trend Micro Vision One, IBM Cloud, DigitalOcean, Zoom Workplace, and domain targets. **AWS, Google Cloud, Google Workspace, Salesforce, and GitHub aren't named on any public page read.** The product documentation (docs.zanshin.tenchisecurity.com) sits behind a login, so the full connector list couldn't be confirmed. Don't assume either way on stage.

### Modules and outputs (from release notes, Mar 2025 – Sep 2026)
- **Scoring:** organization score on a 1.0–10.0 scale and an A–F letter grade. An "Absolute Security Score" (Nov 2025) changes only with the organization's own actions.
- **Monitoring and dashboards:** severity-ranked alerts, a notifications center, a Following dashboard with a "3rd party risk chart (Risk Matrix)," and a My Organization dashboard.
- **Pre-Contract Due Diligence** (Jun 2025): continuous monitoring or a one-time assessment of a prospective vendor.
- **Questionnaires:** self-assessment questionnaires ("send an unlimited amount"). Automatic grading with Accept/Reject/Request Clarification recommendations (Sep 2026). An **"AI Summary for SAQ"** (Feb 2026) summarizes vendor-submitted PDF evidence. These are the only AI features found.
- **Compliance mapping:** NIST CSF 2.0, ISO 27001:2022, CIS Controls 8.1, PCI DSS 4.0.1.
- **Program features:** business-impact tagging per vendor, role-based access control, organization profiles (industry codes, revenue, headcount), and detection of missing scan targets.

### Customers and claims (self-reported, unaudited)
- **Named customers:** B3 (Brasil Bolsa Balcão), Bradesco, BTG Pactual, Cielo, IRB(Re). Smaller testimonials from Finnet, Workfacilit, NovaQuest, and commarket.
- **Bradesco's CISO:** "reduction of more than 90% in identified vulnerabilities," with a pilot that began in 2021.
- **Homepage:** "Our customers report an 81% reduction in third-party vulnerabilities in the first week." No methodology given.
- **Partners (logos):** Accenture, FS-ISAC, Third Party Risk Association, MITRE, CIS, Howden Brasil, ABBC.

### Tenchi and the 2026 DBIR
- **Tenchi's own blog post** (May 19, 2026): "Tenchi Security contributed this dataset and participated in its analysis" about the DBIR's third-party cloud authentication and privilege remediation data.
- **Tenchi's summary of that data:** "Half of all third-party cloud-based MFA exposures are solved in roughly a month, and only 32% of all issues linger after 240 days."
- **Cross-check:** the DBIR text verified this morning says "only 23% of third-party organizations fully remediated missing or improperly secured MFA... with 50% of all findings being resolved within a month." The "half within a month" figures match. The 23% figure (organizations fully remediated) and Tenchi's 32% (issues still open after 240 days) measure different things. Both come from the same Tenchi-contributed dataset.
- **Other context:** a Tenchi podcast featured the DBIR team's Alex Pinto alongside Sieira.

### First Principles Newsletter Tracker check
**Thread 2 (heat maps vs. probability forecasting): Supports. Logged 2026-11-03.** Even the vendor defining "inside-out" TPCRM presents results as scores, letter grades, and a risk matrix. Better data, same ordinal output, which is the gap this thread names. No other thread bears on it.

**Library candidates:** none. This is a vendor profile tied to one event.

---

## Adversary Playbook (Agent Ryan)

No adversary or campaign involved. One observation: a platform holding read-only access into many companies' Microsoft 365, Okta, and EDR consoles is itself a concentration point, the same "one trusted intermediary, many victims" pattern seen in Salesloft Drift and ConnectWise. Read-only, metadata-only design limits the damage, but stolen read-only tokens across many identity providers would still be valuable reconnaissance. This is a question to ask any such vendor, not an accusation.

---

## First Principles (Agent Euclid)

What Zanshin changes, reasoned from the morning report's framework:
1. **It fixes the clock.** Daily checks replace annual questionnaires. This directly addresses the staleness gap: 27% of organizations get vendor-posture updates only annually, and assessments take months.
2. **It improves the evidence.** Configuration read directly from the source beats self-attestation and beats an outside scan for anything not internet-facing (MFA settings, privileges, EDR coverage).
3. **It partly addresses the trust path.** Zanshin sees the vendor's own posture (is MFA on, are admins over-privileged). It doesn't necessarily map the specific tokens and integrations the vendor holds into the *customer's* environment. That inventory lives on the customer side.
4. **It doesn't address dependency.** Concentration and replaceability (CrowdStrike, Change Healthcare) aren't configuration findings. The business-impact tagging is where that judgment gets recorded, by hand.
5. **It doesn't change the output format.** Scores, grades, and a risk matrix are good for running the program and driving vendors to fix things. They are not the probability-of-material-loss a board needs. They are, though, exactly the Inside-Out evidence that would narrow such a forecast.

---

## How Could We Be Wrong? (Agent Popper)

1. **Everything here is the vendor's own description.** The 81% and 90% claims have no methodology. Gartner "representative vendor" status is a listing, not an endorsement.
2. **Coverage may be broader than the public pages show.** The docs are behind a login. AWS, GCP, Google Workspace, and Salesforce may well be supported. Asserting they're not would be wrong.
3. **Point 3 above could be unfair.** A first party can also onboard its *own* environment ("My Organization"), so the customer-side view may exist. The distinction is about what a vendor-side scan sees, not what the product can never do.
4. **Advising Rick to soften his position for the sponsor could look like spin.** His heat-map thesis is published. Changing it because of who's paying would be a credibility risk of its own.
5. **"Brazilian" is inferred,** not stated.

---

## Resolution (Agent Seldon)

1. **Accepted.** Claims are labeled self-reported throughout, including in the synthesis.
2. **Accepted.** The coverage list is stated as "named on public pages," with an explicit "don't assume either way."
3. **Revised.** Euclid's point 3 is phrased as a limit of vendor-side scanning, not of the product.
4. **Resolved:** the advice doesn't change Rick's position, only its framing. "Grades run the program, probabilities inform the board" is his actual thesis stated without a target. The position stays fully intact.
5. **Accepted.** Stated as "appears to be."

No forecast: the question doesn't call for one.

---

## Visualization (Agent Tufte)

No diagram. The product's three-party flow (customer invites, vendor connects read-only, metadata flows back) fits in one sentence, and a rendered graphic wouldn't add anything for a one-day-use briefing. The table below covers what Rick needs on stage.

| Zanshin does well | Not visible from public pages / outside its scope |
|---|---|
| Daily, inside-out configuration checks at consenting vendors | Full connector list (docs require login) |
| Free to vendors, so adoption friction is lower | First-party pricing |
| Remediation help delivered directly to vendors | The tokens a vendor holds into *your* environment (customer-side inventory) |
| Pre-contract due diligence, questionnaires, AI PDF summaries, compliance mapping | Concentration and dependency risk beyond manual business-impact tagging |
| Contributed the DBIR's third-party MFA and privilege data | Board-level probability of loss (outputs are scores, grades, risk matrix) |

---

## Sources

### Primary (Tenchi Security's own site, vendor self-description)
- [Homepage](https://www.tenchisecurity.com/en): positioning, inside-out plus outside-in, consent framing, customers, 81% claim.
- [Why Zanshin](https://www.tenchisecurity.com/en/why-zanshin): daily testing, "thousands of vulnerability checks," licensing model, unlimited questionnaires.
- [For Third Parties](https://www.tenchisecurity.com/en/for-third-parties): read-only and metadata-only commitments, free to vendors, Team Tenchi.
- [Third-Party Security Posture Management](https://www.tenchisecurity.com/en/third-party-security-posture-management): critique of external scoring.
- [Meet Tenchi](https://www.tenchisecurity.com/en/meet-tenchi): leadership, Series A, Gartner recognition.
- [Release notes](https://www.tenchisecurity.com/en/release-notes): connectors, modules, scoring scales, AI SAQ summary, risk matrix. Partly read verbatim, partly summarized.
- [Partners](https://www.tenchisecurity.com/en/company/partners), [Customer testimonials](https://www.tenchisecurity.com/en/customer-testimonials), and [Accelerating growth](https://www.tenchisecurity.com/en/accelerating-growth): partners, named customers, Bradesco 90% quote.
- [Tenchi blog on the 2026 DBIR](https://www.tenchisecurity.com/en/insights-news/the-verizon-2026-data-breach-investigations-report-third-party-breaches-credential-exposures-and-more-insights): "Tenchi Security contributed this dataset and participated in its analysis."

### Cross-check
- [Verizon 2026 DBIR Executive Summary](https://www.verizon.com/business/resources/executivebriefs/2026-dbir-executive-summary.pdf): 23% and 50%-within-a-month MFA figures (verified this morning).

### Not readable
- docs.zanshin.tenchisecurity.com: behind a login.
- The Zanshin datasheet PDF wasn't fetched.

### Internal precedent
- `reports/2026-11-03-tpcrm-state-of-the-industry.md`, `reports/2026-11-03-tpcrm-panel-draft-responses.md`, and `reports/2026-11-02-sao-paulo-brazil-conference-briefing.md`.

### Rick Howard's First Principles Newsletter
- ["Outside-In and Inside-Out Superforecasting"](https://diffuser.substack.com/p/outside-in-and-inside-out-superforecasting) and ["Heat Maps Are Just Bad Science"](https://diffuser.substack.com/p/heat-maps-are-just-bad-science) (Thread 2).

---

## New Skills (Agent Turing)

None. A vendor-site scan is a standard Sherlock fetch.

---

## Library Recommendations (Agent Alexandria, closing)

Nothing recommended. The profile is tied to one event and is entirely vendor self-description.

---

## Number Check (Agent Popper, second pass)

- **$7M Series A:** stated as on the English page. The R$ 35 million slug discrepancy is flagged, not resolved ✓.
- **81% and 90%:** labeled self-reported in both the synthesis and the Facts ✓.
- **1.0–10.0 score and A–F grade:** consistent in the synthesis, Facts, and Euclid ✓.
- **DBIR MFA:** 23% (organizations fully remediated) vs. Tenchi's 32% (issues open after 240 days) are explained as different measures from the same dataset. The "half within a month" figure matches between DBIR and Tenchi ✓. The synthesis cites 23% only ✓.
- **27% annual-only updates:** matches the morning report (Ponemon) ✓.
- **No mismatches found.**
