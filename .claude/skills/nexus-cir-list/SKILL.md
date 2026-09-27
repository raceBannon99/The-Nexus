---
name: nexus-cir-list
description: Print a quick-reference list of every top-level CIR (Command Information Requirement) category from CIR-Definition.md, each with a plain-language summary under 250 characters. Use when Rick asks for the CIR list, the CIR categories, the CIR taxonomy, or "what CIRs do we track."
---

# Nexus CIR List

Produces a compact, at-a-glance summary of the CIR taxonomy every Nexus story gets matched against — the full category definitions live in `Intelligence Reports/CIR-Definition.md`, this skill's job is a shorter, glanceable version of that same list.

## How to run this

1. **Read `Intelligence Reports/CIR-Definition.md` first — it's the source of truth, not this skill file.** The cached table below (last verified 2026-09-27) is a starting point, not a substitute for checking: CIR-Definition.md has grown before (three AI-timeline categories added 2026-09-11/09-18) and can grow again.
2. **Diff the live file against the cached table's category list.** If every `##`-level category in CIR-Definition.md still matches a row below, the cache is current — present it as-is.
3. **If a category was added, removed, or its definition/examples changed meaningfully**, regenerate that row (and only that row, unless the whole file has drifted more broadly): write a plain-language summary of the category strictly under 250 characters, no statistical notation or jargon beyond what a reader unfamiliar with the file would need, matching the voice and structure of the other rows (what it covers, named examples where the source file gives them). Update the cached table below with the new row so the next run doesn't have to redo the work.
4. Present the list to Rick as a table (category name, summary) in the order CIR-Definition.md itself uses — that order is deliberate (the three AI-timeline categories are grouped with Adversary Playbook at the top; "Political" and "Adulting" close it out).

## Cached CIR summary table (last verified 2026-09-27, 25 categories)

| CIR | Summary |
|---|---|
| Adversary Playbook Activity | Cybercrime, hacktivist, and nation-state threat-actor activity by country (China, Russia, Iran, North Korea, Pakistan, Israel, more), plus the Russia-Ukraine, Israel-Gaza, and US-Israel-Iran cyber wars specifically. |
| AI Singularity Timeline | Evidence on when the world might experience an irreversible, civilizational-scale loss of control over a frontier AI system — a control question, not a capability one. |
| AGI Arrival Timeline | Evidence on when a machine first matches or exceeds broad human performance across nearly every intellectual domain — a capability milestone, earlier and softer than the Singularity. |
| Superintelligence Timeline | Evidence on when a machine might exceed, not just match, human intelligence — a higher, later capability bar than AGI, inferred structurally with no external forecaster basket. |
| Law Enforcement Disruption | Government takedown/disruption operations against criminal or adversary infrastructure — e.g. Operation Cronos, the Hive takedown, Radar/Dispossessor. |
| Government Surveillance | State surveillance programs and operations — e.g. PRISM, Tempora, Russia's SORM, China's Golden Shield/Great Firewall. |
| Data Breaches | Reported breaches of personal or organizational data — e.g. OPM, Ashley Madison, Cam4. |
| Critical Infrastructure Attacks | Cyberattacks against water, power, internet, and government systems. |
| Cybersecurity Canon Project Book Reviews | Reviews from the CyberCanon cybersecurity reading-list project. |
| Cybersecurity Executive Leadership Changes | New CISO, CSO, CIO, and CTO appointments across organizations generally. |
| Cybersecurity Vendor Executive Leadership Changes | Executive changes specifically at security vendors — e.g. Palo Alto Networks, Cisco, Fortinet, Tidal Cyber, Resilience, Hedy. |
| Cybersecurity Research Reports and Papers | Foundational or notable research — e.g. the Lockheed Martin Kill Chain paper, DoD's Diamond Model, MITRE ATT&CK's design paper, Forrester's Zero Trust paper. |
| Cybersecurity First Principle Strategies | The field's core strategic approaches — Zero Trust, Kill Chain Prevention, Resilience, Risk Forecasting, Materiality, Automation, Workforce Development. |
| Nation State Cyber Policy and Law | Government cyber policy and legislation from countries like China, North Korea, Russia, the US, Iran, Pakistan, and Vietnam. |
| Cybersecurity Zero Trust Tactics | IAM, SBOM, vulnerability management, SSO, two-factor auth, software-defined perimeter, and SASE/SSE trends. |
| Cybersecurity Intrusion Kill Chain Prevention Tactics | Intel sharing, attribution, SOC, CTI, red/blue/purple teaming, the Kill Chain and Diamond Model, and ATT&CK framework trends. |
| Cybersecurity Risk Forecasting Tactics | Quantified cost/impact/risk reporting — superforecasting, Bayesian methods, FAIR methodology, and risk-forecasting case studies. |
| Cybersecurity Resilience Tactics | Crisis handling, chaos engineering, backups, encryption, incident response, and notable resilience failures. |
| Cybersecurity Automation Tactics | DevSecOps, AI, SIEM, and SOAR technology trends. |
| Cybersecurity Workforce Development Tactics | Unconventional hiring/development approaches — e.g. "Moneyball for Cybersecurity." |
| Compliance Trends | GDPR, ISO, PCI, and other regulatory fines and requirements. |
| Cybersecurity Framework Trends | NICE, NIST, and UK Cyber Governance Code of Practice framework developments. |
| Over the Horizon Technology Trends | Emerging tech 3–25 years out — quantum computing, 5G, AI, net neutrality, SEC materiality rules, and related government policy. |
| Political | Election oversight and presidential decision directives. |
| Adulting | Non-cyber personal content — good news, things learned, recipes, events. |

## Origin

Created 2026-09-27, per Rick's request for a standing skill to print the CIR summary drafted that day, rather than redrafting it by hand each time it's needed.
