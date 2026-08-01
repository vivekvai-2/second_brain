---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S5
  - tier/high-medium
  - project/p3
  - project/p1
  - project/fsqca
---

# PwC Netherlands: Navigating Third Party Risk Management in the Digital and Geopolitical Era (2025)

**Node ID:** F045  
**Type:** Wiki Intake Note  
**Wiki Section:** S5 (Data, Privacy & Security) / P3 (BFSI JEIM)  
**Status:** Active  
**Tier:** High-Medium  
**Last Updated:** 2026-07-15 (enriched from a second, independent NotebookLM extraction pass — authorship, Data Act/Product Liability Directive coverage, Board questions framework, case studies, and key quotes added; see Log)  

---

## Source

**Full Citation (APA):** Ruizendaal, C., van Wendel de Joode, I., Besseling, L., Valkenburg, M., Hengst, J. A., Verhoeven, C., & Zaidi, B. (2025). *Navigating third party risk management in the digital and geopolitical era: Strategies for resilience and compliance*. PricewaterhouseCoopers Netherlands. [⚠ VERIFY #169 — filename suggests November 2025; no internal publication date confirmed]  
**Authors:** Casper Ruizendaal (Partner, Risk Consulting); Ilse van Wendel de Joode (Director, Digital Law & Commercial Contracting); Lean Besseling (Director, Risk Consulting); Marco Valkenburg (Senior Manager, Risk Consulting); Jan Anthonie Hengst (Manager, Risk Consulting); Caitlin Verhoeven (Senior Associate, Risk Consulting); Basmah Zaidi (Senior Associate, Risk Management) — confirmed via second extraction pass, 2026-07-15; not captured in the original intake.  
**Document Type:** Practitioner white paper (advisory/consulting)  
**Issuing Institution:** PwC Netherlands (PricewaterhouseCoopers, Netherlands practice)  
**Publication Date:** ⚠ VERIFY #169 — filename `20251112` suggests November 12, 2025; body text references DORA effective January 2025 and AI Act phasing; exact date not stated internally. Independently re-confirmed as unresolved by a second extraction pass, 2026-07-15 — treat as a standing flag, not a one-off.  
**URL / DOI:** PwC Netherlands website (⚠ VERIFY #169 for canonical URL)  

**Routing note:** This is a PwC Netherlands practitioner white paper, NOT an Indian regulatory instrument. Format B (Wiki Intake Note) applies. The document was considered for P3 primary relevance due to its FSB TPRM gap coverage.

---

## Executive Summary

PwC Netherlands maps the third-party risk management (TPRM) landscape as it has been transformed by five converging forces: digital dependency, regulatory proliferation, supply chain complexity, geopolitical fragmentation, and AI/technology advancement. The document introduces a "Good TPRM → Great TPRM" progression framework, analyses six common organisational TPRM pitfalls, and evaluates the EU's Digital Decade regulatory architecture (DORA, NIS2, DSA, AI Act, GDPR) as an integrated TPRM governance structure. It also surveys AI-enabled TPRM tools (LeAh, CREANCE.AI, DMS AI platform) that represent the emerging market for AI-assisted third-party due diligence. The document is directly relevant to P3 (BFSI JEIM) as it closes a gap identified in [[International_11]] (FSB TPRM — Tool 3.7 AI vendor exit strategy) by providing a practitioner-level implementation framework for the AI vendor governance obligations that FSB identifies as systemic risk mitigation requirements.

---

## Key Frameworks and Findings

### Five Converging Forces Reshaping TPRM

| Force | Description |
|---|---|
| **Digital Dependency** | Organisations critically dependent on third-party digital infrastructure; single-vendor concentration risk |
| **Regulatory Proliferation** | EU Digital Decade framework (DORA, NIS2, DSA, AI Act) creates layered, intersecting TPRM obligations |
| **Supply Chain Complexity** | Nth-party risk (sub-processors, cloud sub-dependencies) creates governance opacity |
| **Geopolitical Fragmentation** | Sanctions regimes, data localisation requirements, and vendor nationality risk |
| **AI/Technology Advancement** | AI integration in third-party services and in TPRM governance tooling itself |

### Good TPRM vs. Great TPRM Framework

| Dimension | Good TPRM | Great TPRM |
|---|---|---|
| Risk identification | Vendor inventory maintained | Dynamic, continuous discovery including nth parties |
| Assessment | Periodic questionnaire-based | Continuous monitoring + AI-assisted signal detection |
| Contractual protection | Standard T&Cs | Exit strategies, service continuity, AI vendor addenda |
| Concentration risk | Tracked | Actively managed with diversification requirements |
| Regulatory alignment | Single-framework compliance | Multi-framework (DORA + NIS2 + AI Act) integrated compliance |
| AI tools | None or limited | LeAh / CREANCE.AI / DMS AI for automated due diligence |

### EU Digital Decade Regulatory Architecture

| Regulation | Effective Date | TPRM Relevance |
|---|---|---|
| **DORA** (Digital Operational Resilience Act) | January 2025 | ICT third-party risk management; incident reporting; exit strategy requirements |
| **NIS2** (Network and Information Security Directive 2) | October 2024 | Supply chain security requirements; incident notification |
| **DSA** (Digital Services Act) | February 2024 | Platform accountability; algorithm transparency obligations |
| **AI Act** | August 2024 (in force); August 2026 (applies) | Third-party AI system obligations; GPAI provider requirements; ⚠ VERIFY #170 |
| **GDPR** | May 2018 (ongoing) | Data processor agreements; data subject rights in third-party processing |
| **Data Act** | Phasing in (per source, "over the next two years" from 2025) | Data portability and switching rights for data processing service providers; reduces vendor lock-in; strengthens user autonomy — **added 2026-07-15, missed in original intake** |
| **Product Liability Directive** | Not stated in source | Due diligence, contracts, monitoring, and incident response for suppliers of digital components; traceability and back-to-back contractual obligations — covered only in the source's Annex I action table, **added 2026-07-15, missed in original intake** |

Note: DORA and NIS2 create the most direct TPRM obligations; AI Act adds AI-system-specific third-party obligations for deployers of AI systems from external providers. The original intake captured five of the source's seven regulatory regimes (DORA, NIS2, DSA, AI Act, GDPR) and missed the Data Act and Product Liability Directive rows above — both are addressed substantively in the source's Annex I ("EU digital decade: Practical third-party risk actions").

### Five Board Questions for TPRM Oversight

Added 2026-07-15 — present in the source ("Setting the scene" section) but absent from the original intake. The white paper frames these as the board-level diagnostic for whether a TPRM strategy is adequate:

1. Are critical third-party relationships clearly identified?
2. Are there mechanisms for continuous monitoring of those relationships?
3. Are suppliers aligned with the organisation's cybersecurity standards?
4. Is the organisation prepared for geopolitical or regulatory shifts affecting third parties?
5. Is concentration risk being actively reduced?

This is structurally the same instrument type as [[Board_AI_Risk_Oversight_Checklist]] (this vault's own consulting template) applied to the TPRM/vendor-risk domain rather than AI governance broadly — a genuine cross-reference, not a coincidence, since TPRM and AI vendor governance overlap substantially. See Cross-Links below.

### Aggregation Risk (defined term, added 2026-07-15)

The source explicitly defines **aggregation risk** as "the cumulative exposure an organisation faces when multiple third parties rely on the same underlying service providers, technologies, or geographic regions" — distinct from, and more precise than, the "concentration risk" language the original intake used to cover this idea. Both terms now appear in this node; treat "aggregation risk" as the source's own more precise term.

### Six Common TPRM Pitfalls

1. **Siloed governance** — TPRM managed separately from enterprise risk, creating blind spots
2. **Assessment fatigue** — Over-reliance on questionnaires that third parties treat as checkbox exercises
3. **Concentration blindness** — Tracking individual vendors but not concentration exposure across the portfolio
4. **Nth-party opacity** — Sub-processor risks not visible in standard due diligence
5. **Exit strategy deficit** — Contractual exit provisions not operationally tested; AI vendor lock-in particularly acute
6. **Regulatory fragmentation** — Parallel compliance to DORA, NIS2, AI Act without integrated framework

### AI-Enabled TPRM Tools

| Tool | Function |
|---|---|
| **LeAh** | AI-assisted vendor risk assessment; natural language processing of third-party documentation |
| **CREANCE.AI** | Automated credit and counterparty risk assessment with AI signal processing |
| **DMS AI Platform** | Document management and third-party due diligence automation |

PwC's inclusion of these tools positions the white paper as a market-facing advisory document as well as a governance framework document. The AI-in-TPRM tooling section is relevant to P3's interest in AI governance in BFSI operations.

### Case Studies and Cited Incidents (added 2026-07-15)

Not captured in the original intake — the source uses four worked examples and two historical incidents to ground its framework, useful as citable practitioner evidence in consulting/teaching contexts:

- **Anonymised multinational corporation** — lacked effective linkages for third-party data; Business Contract Owners hesitant to engage with compliance tasks, producing communication gaps and inconsistent deliverable quality. Illustrates Pitfall #1 (siloed governance).
- **Multinational consumer goods organisation** — decentralised, manual ICT third-party onboarding under NIS2 pressure, resulting in governance gaps; PwC built an ICT TPRM framework using IBM OpenPages for centralised automated workflows.
- **Multinational organisation (unnamed sector)** — PwC NL implemented a TPRM operating model using multi-domain questionnaires, AI-driven adverse media scanning, and integrated sanctions databases to fix onboarding inefficiencies.
- **Global industrial manufacturer** — deployed PwC's "DMS" AI platform, including a "Screener" module (sanctions/adverse media) and an "Outreach Portal" module, to embed risk management directly into supplier onboarding.
- **Suez Canal blockage (2021)** — cited as the reference incident for how a single point of failure disrupts global trade routes and supply chains; supports the "Digital Dependency"/"Geopolitical Fragmentation" forces in the Five Converging Forces table above.
- **Schrems II judgment** (post-GDPR) — invalidated the EU–US Privacy Shield, forcing controllers dependent on U.S. providers to adopt alternative transfer safeguards; cited alongside GDPR's May 2018 entry into force as the historical precedent for "EU regulations assume continuous third-party oversight."
- **Geopolitical Risk Index (GPR)** — named as the framework PwC references for quantifying geopolitical exposure; paired with PwC's own "Quickscan" tool (a structured approach mapping geopolitical risks against a company's business model and existing controls) — the Quickscan tool was not in the original intake's AI-Enabled TPRM Tools table.

### Notable Quotes (added 2026-07-15)

- "Corporate integrity now appears to extend beyond a company's own actions and is increasingly assessed based on the conduct of the company's third parties."
- "The imperative now is not whether to act, but how swiftly to integrate a proactive and scalable TPRM strategy."
- "Geopolitical risks now materially influence where and how companies operate."
- "EU regulations now assume that companies exercise continuous oversight of their third parties."
- "Board-level visibility and measurable outcomes must define TPRM efforts."

---

## India Relevance and Governance Gap Analysis

This document directly closes the **FSB TPRM Tool 3.7 AI vendor exit strategy gap** identified in [[International_11]] (⚠V-FSB3/#138). The FSB identified AI vendor exit strategies as a critical but underdeveloped TPRM component; PwC provides the "Great TPRM" implementation architecture that operationalises this requirement.

**India BFSI TPRM gap analysis:**

1. **DORA benchmark vs. India:** DORA (effective January 2025) requires: mandatory ICT third-party contracts with exit provisions; ICT concentration risk reporting to regulators; ICT service provider register; operational resilience testing including third-party dependencies. India's equivalent — RBI's IT Framework for Banks (2016/updated) and Outsourcing Guidelines (2006/updated) — predates DORA by nearly two decades and does not address AI-specific vendor obligations, concentration risk quantification, or operational resilience testing requirements.

2. **AI vendor lock-in:** PwC's "Exit Strategy Deficit" pitfall (#5 above) is acutely relevant to Indian BFSI. Major Indian banks and NBFCs have deployed AI/ML systems from AWS, Google Cloud, Microsoft Azure, and Indian vendors (TCS, Infosys, Wipro) without disclosed exit strategies or service continuity provisions specific to AI model dependencies.

3. **NIS2 equivalent gap:** India has no NIS2 equivalent. CERT-In Directions (April 2022) address incident reporting but not supply chain security obligations or third-party security requirements at the TPRM level.

4. **AI Act deployer obligations (from August 2026):** Indian entities deploying EU-regulated AI systems as deployers (not just providers) will face AI Act third-party obligations when accessing EU markets or processing EU data. India's absence of equivalent domestic obligations creates an asymmetric compliance burden.

5. **Nth-party opacity:** RBI's Outsourcing Guidelines require due diligence of direct service providers; they do not address sub-processors or cloud sub-dependencies. This is the "Great TPRM" gap that PwC identifies as systemic.

Cross-reference: [[International_11]] (FSB TPRM systemic framework) and [[F042_IBM_Cost_Data_Breach_Report_2025]] (breach cost consequences of inadequate third-party AI governance).

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | TPRM regulatory architecture analysis; "Good → Great" framework as a maturity progression model; regulatory proliferation and its governance implications; AI-enabled TPRM tooling as emergent governance mechanism |
| P3 (BFSI JEIM) | **Primary** — closes FSB TPRM Tool 3.7 gap; provides India BFSI AI vendor governance benchmark; six pitfalls directly applicable to Indian BFSI TPRM audit; exit strategy deficit is a critical P3 finding |
| P4 (Doctrinal IJLIT) | DORA/NIS2/AI Act as comparative third-party liability framework; EU architecture vs. Indian outsourcing guideline regime |
| fsQCA | RC condition — EU regulatory commitment (DORA + AI Act deployer obligations) vs. India's absence provides a sharp RC calibration point; CC condition — concentration risk management as organisational governance capability indicator |

---

## Concept Links

- [[Accountability]] — DORA mandates documented ICT third-party registers, contracts, and exit strategy provisions; these operationalise accountability at the third-party governance level; PwC's "Great TPRM" framework extends accountability to nth-party dependencies
- [[Transparency]] — AI vendor documentation obligations under AI Act Art.13 (transparency obligations for high-risk AI systems); NIS2 incident transparency; "Good TPRM" → "Great TPRM" transition requires transparency on concentration exposure
- [[Governance_Capacity]] — AI-enabled TPRM tools (LeAh, CREANCE.AI) represent governance capacity augmentation; 89% lacking ML security tools (F044) and TPRM pitfall #1 (siloed governance) together indicate a governance capacity deficit that these tools address
- [[Governance_Debt]] — India's TPRM framework (2006 outsourcing guidelines) represents approximately 15–20 years of governance debt relative to DORA (2025); exit strategy deficit for AI vendors is a new governance debt accumulation accelerated by rapid AI deployment
- [[Regulatory_Parallelism]] — EU's five-regulation Digital Decade architecture (DORA/NIS2/DSA/AI Act/GDPR) itself creates regulatory parallelism within the EU; India's parallel regulatory silos (RBI/SEBI/IRDAI) each have separate (and less developed) TPRM frameworks without the EU's attempt at integration
- [[Institutional_Coherence]] — PwC identifies regulatory fragmentation (pitfall #6) as a primary TPRM governance challenge; EU's integrated Digital Decade architecture represents an attempt at institutional coherence across TPRM obligations — a model India's AI governance architecture currently lacks

---

## ⚠ VERIFY BEFORE PUBLISHING

- **V-B14-06 / #169 — Publication date — LOW.** Filename `20251112` suggests November 12, 2025, but no internal publication date is confirmed in the document body. Verify: access PwC Netherlands website for publication metadata; confirm date for APA citation.
- **V-B14-07 / #170 — EU regulatory effective dates — LOW.** Dates cited above (DORA January 2025; NIS2 October 2024; DSA February 2024; AI Act August 2024 / August 2026) are sourced from the PwC document and are consistent with training data. Verify: confirm AI Act Annex III phased application dates and GPAI CoP timeline (the document notes AI Act applies from August 2026, with GPAI CoP from August 2025).

---

## Cross-Links to Corpus

- [[Board_AI_Risk_Oversight_Checklist]] — added 2026-07-15. The source's "Five Board Questions for TPRM Oversight" (above) is structurally the same instrument as this vault's own board-level checklist template, applied to third-party/vendor risk rather than AI governance broadly. Worth a future cross-pollination pass: TPRM board questions could inform a vendor-risk variant or addendum to the checklist; not done in this pass to avoid scope creep on a single-document intake.
- [[International_11]] — FSB TPRM: Tool 3.7 AI vendor exit strategy gap; F045 directly addresses this gap at the implementation framework level
- [[F042_IBM_Cost_Data_Breach_Report_2025]] — IBM's Shadow AI premium (USD 670K) and 97% lacking AI access controls finding quantify the financial risk of TPRM governance failures at the AI vendor level
- [[F044_Microsoft_AI_Security_Risk_Assessment]] — Microsoft ML attack taxonomy provides the technical threat context for TPRM security assessments of AI vendors
- [[F043_MIT_AI_Risk_Mitigation_Taxonomy_2025]] — MIT taxonomy's Governance & Oversight category (30%) and Operational Process category (36%) map to PwC's "Great TPRM" framework; both documents point toward process-heavy, oversight-light current practice
- [[F036_NIST_NCCoE_Agent_Identity_Authorization]] — NIST's access delegation and inter-agent authentication standards are directly applicable to nth-party AI system governance gaps identified by PwC

---

## Log

- 2026-06-19: Node created (original intake).
- 2026-07-15: Enriched from a second, independent NotebookLM extraction pass of the same source document — user ran the document through NotebookLM and pasted the extraction unprompted, which surfaced that this document was already in the vault (duplicate catch, no new node created). Added: full author list (previously missing), Data Act and Product Liability Directive rows to the regulatory architecture table (previously missed), the Five Board Questions framework, the explicit "aggregation risk" definition, five case studies/cited incidents, five verbatim quotes, and a cross-link to [[Board_AI_Risk_Oversight_Checklist]]. Closed a bidirectional-linking gap: [[Governance_Capacity]] was missing its "Instances in Corpus" entry for F045 despite being listed in this node's own Concept Links section since 2026-06-19 — added in the same pass. No new VERIFY flags required — both uncertain items in the second extraction (publication date, page-number mapping) duplicate the existing #169/#170 flags rather than raising new ones.
