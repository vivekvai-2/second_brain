---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/global
  - institution/international
  - theme/critical-infrastructure
---

# International_26 — NERC CIP, ENISA/NIS2, and IEC 62443: Confirmed Absence of AI-Specific Critical-Infrastructure Cybersecurity Extensions

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026.md`
**Institution:** [[07_Institutions/International]]
**Issuing body:** North American Electric Reliability Corporation (NERC); European Union Agency for Cybersecurity (ENISA); International Electrotechnical Commission / International Society of Automation (IEC/ISA 62443 series)
**Document date:** NERC CIP Roadmap, 11 January 2026; ENISA energy-sector pages current 21 July 2026 (foundational 2017 report; OT/ICS guidelines November 2018); IEC 62443 core series approved 2021
**Pages:** Not applicable — this node consolidates three separate standards bodies' positions rather than a single document
**Domain:** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

---

## Instrument Identity

**Full title:** Consolidated comparator node — NERC Critical Infrastructure Protection (CIP) standards; ENISA cybersecurity-of-critical-sectors (energy) guidance under NIS2; IEC 62443 industrial automation/control-systems security series
**Type:** Three independent, non-binding-to-India comparator regimes (binding within their own jurisdictions)
**Target entities:** NERC CIP — US/Canada bulk electric system operators; ENISA/NIS2 — EU energy-sector entities (electricity, district heating, oil, gas, hydrogen); IEC 62443 — global industrial automation and control systems operators (voluntary international standard)
**Legal basis:** NERC CIP — US Federal Power Act reliability-standard authority; ENISA guidance — EU NIS2 Directive; IEC 62443 — voluntary international standard, no statutory force of its own
**Companion documents:** Consolidates a NERC CIP Roadmap, industry/academic commentary on the CIP-AI gap, ENISA's energy-sector landing pages and 2018 OT/ICS guidelines, and secondary commentary on IEC 62443's treatment of AI as a defensive tool

**Primary source links:**
- NERC CIP Roadmap (11 January 2026): https://www.nerc.com/globalassets/our-work/reports/special-reports/nerc_cip_roadmap_01122026.pdf
- ENISA energy-sector cybersecurity: https://www.enisa.europa.eu/topics/cybersecurity-of-critical-sectors/energy | 2017 foundational report: https://www.enisa.europa.eu/publications/information-sharing-in-the-energy-sector
- ENISA OT/ICS Guidelines (Nov 2018, secondary index): https://www.cs2ai.org/standards-regulations/enisa-guidelines-on-cybersecurity-for-ot-and-ics

---

## Analytical Classification

**Wiki section:** New — Critical Infrastructure / Power Sector, International Comparators
**Jurisdiction:** US (NERC), EU (ENISA), Global voluntary standard (IEC 62443)
**Confidence:** High for NERC CIP Roadmap and ENISA landing pages (direct primary links); Medium for IEC 62443 AI-treatment claims (secondary vendor commentary — Rockwell Automation, Keyfactor)
**AI explicit:** No — across all three; each explicitly confirmed as having a recognised-but-unaddressed AI gap
**Tier classification:** Tier A comparator value — despite none being AI-specific, the *confirmed absence itself* is Tier A evidence for the domain's central claim
**AI Governance Wiki relevance:** HIGH — this is the evidentiary backbone for the domain's cross-jurisdictional-vacuum finding

---

## Substantive Content

### NERC CIP (US) — confirmed gap, explicitly acknowledged by industry and academia
The NERC CIP Roadmap (January 2026) evaluates current CIP coverage and ongoing standards projects but does not itself introduce AI-specific provisions. A June 2026 industry commentary states directly: **"NERC CIP Was Not Built for AI... that framework has not yet been updated to address AI systems in a comprehensive way,"** recommending interim compensating controls — extending CIP-010 (change management), CIP-013 (supply-chain risk), and CIP-009 (recovery plans) to cover AI systems — pending formal NERC guidance. A companion academic paper (*Journal of Information Systems Engineering & Management*, "Understanding the Risk of Implementing AI for Managing Critical Infrastructure Cybersecurity") explicitly recommends NERC update CIP standards to address AI-specific risks such as model explainability — confirming this as a recognised, unaddressed gap rather than settled guidance.

### ENISA/NIS2 (EU) — same pattern
ENISA's energy-sector guidance remains scoped to NIS2-driven general cybersecurity (risk management, OT/IT segmentation, sector-specific ISACs) across electricity, district heating, oil, gas, and hydrogen. No ENISA publication specifically addressing AI in energy-sector critical infrastructure was located — a confirmed absence mirroring the US and Indian findings.

### IEC 62443 — AI recommended only as a tool, not as a governed object
The IEC 62443 series (approved 2021) is structured around a zones/conduits security model. Secondary vendor commentary (Rockwell Automation, Keyfactor) notes organisations are encouraged to "leverage advanced technologies such as AI and machine learning for enhanced threat detection and response" — but this is guidance on **using AI as a defensive tool** within the existing model, not a supplementary standard governing AI systems themselves as objects of risk. No dedicated AI-specific extension to IEC 62443 was located.

### The pattern, stated plainly
**All three major frameworks examined — one binding national standard (NERC CIP), one EU directive-driven guidance regime (ENISA/NIS2), and one voluntary international industrial standard (IEC 62443) — are in an identical posture: mature OT/ICS cybersecurity governance exists, the AI-specific gap is explicitly recognised by industry and/or academic commentary, and no formal regulatory or standards-body response has yet closed it.** This is not three independent gaps; it is one gap, replicated across every jurisdiction and standards body examined, including India's own CEA/NCIIPC architecture (see [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]]).

---

## Analytical Significance for PRIS Research

### For the new Power Grid/Critical Infrastructure domain — the central finding
This is not a case where India lags global peers (the pattern seen everywhere else in this corpus — DPDP behind implementation, IRDAI behind RBI/SEBI, TRAI "anticipatory"). It is the **only sector in the entire PRIS corpus where India is in lockstep with, rather than behind, its international comparators** — because nobody has solved this problem yet. This is worth stating explicitly and prominently in the domain synthesis: it changes the research framing from "why is India behind" to "this is a live global regulatory frontier with no first-mover yet," which is a more interesting and more defensible framing for original contribution.

### A methodological caution for fsQCA, if this sector is ever added as a case
If AI-in-critical-infrastructure governance were added as an fsQCA case or condition, **every jurisdiction examined would calibrate at or near 0.00 on any AI-specific-regulation condition** — a case with no variance cannot support a configurational (QCA) causal argument. This sector is better suited to a qualitative "regulatory frontier" framing (why has no jurisdiction moved yet — capacity, technology-uncertainty, or genuine absence of documented incidents?) than to inclusion in the existing 10-case fsQCA model as currently designed. Flag this explicitly before any attempt to fold Power Grid/Critical Infrastructure into [[fsQCA_Thesis_Chapter]].

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]], [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]], [[07_Institutions/Corpus/NCIIPC/NCIIPC_1_Guidelines_Protection_NCII_V2_2015]]
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (global capacity constraint, not India-specific), [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (contrast — global silence, not parallelism)
**Related frameworks:** None yet — this sector has no Framework-tier node in any jurisdiction examined, consistent with the finding
**Related projects:** New domain, not yet assigned to a numbered project; explicit caution flagged for [[08_Methods/fsQCA]] above
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Not applicable
- **Wiki intake status:** Pending — High priority, this is the domain's central comparative finding

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] Power Grid prompt. Consolidates three comparator regimes under one node per PRIS evidence-reuse threshold, since all three confirm the identical negative finding rather than offering three distinct positive data points.
