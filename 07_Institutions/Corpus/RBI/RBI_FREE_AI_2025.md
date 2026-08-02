---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/rbi
---

# RBI_FREE_AI_2025 — Framework for Responsible and Ethical Enablement of Artificial Intelligence (FREE-AI) Committee Report

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_FREE_AI_2025.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India (FREE-AI Committee, constituted by RBI)
**Document date:** Released 13 August 2025
**Pages:** ~85 (Table of Contents extends to Annexure VI; not fully determinable from extraction)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]
**Link (confirmed 2026-08-02, direct RBI document repository):** https://rbidocs.rbi.org.in/rdocs/PublicationReport/Pdfs/FREEAIR130820250A24FF2D4578453F824C72ED9F5D5851.PDF

---

## Instrument Identity

**Full title:** Framework for Responsible and Ethical Enablement of Artificial Intelligence (FREE-AI) — Committee Report
**Type:** Committee Report / Advisory Framework (non-binding)
**Target entities:** Regulated Entities (REs) under RBI supervision — banks, NBFCs, Asset Reconstruction Companies (ARCs), All India Financial Institutions (AIFIs), Urban Co-operative Banks (UCBs)
**Legal basis:** Constituted by RBI; recommendations are advisory pending formal issuance as binding directions
**Companion documents:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (DPDP Rules 2025 — incorporated by reference for data lifecycle governance); [[07_Institutions/Corpus/RBI/RBI_1]] (IT Governance Master Direction); RBI Master Directions referenced in Annexure IV (AI-specific enhancements)

---

## Analytical Classification

**Wiki section:** S4 (Agentic AI Governance) — primary; also feeds S2 (India Regulatory Framework, BFSI)
**Jurisdiction:** India (BFSI sector)
**Confidence:** Medium (committee report / framework — not yet a binding Master Direction or Circular)
**AI explicit:** Yes
**Tier classification:** Tier A — explicit AI regulation/framework, though currently advisory rather than mandatory
**AI Governance Wiki relevance:** HIGH — first dedicated AI governance framework from an Indian prudential regulator; directly referenced by an existing Wiki Intake stub ([[04_Knowledge_Products/Wiki_Intake/RBI_FREEAI_MasterCircular]]) which previously pointed to this corpus node before it existed.

---

## Substantive Content

### Survey evidence base (Chapter 3.3)
Two RBI surveys underpin the report's recommendations:
- **Department of Supervision (DoS) survey**: 612 supervised entities (Feb–May 2025), covering ~90% of sector asset size. Only **20.80% (127 of 612)** entities reported using or developing AI systems.
- **FinTech Department (FTD) survey**: 76 entities (Jan–May 2025), with follow-up interactions with CTOs/CDOs of 55 of the 76 entities.
- Adoption skew: no AI usage reported by Tier 1 UCBs (deposits ≤ ₹100 crore); Tier 2/3 UCB adoption below 10%; only 27% of 171 surveyed NBFCs used AI; no adoption among ARCs.
- Of 583 AI applications in production/development: customer support (15.60%), credit underwriting (13.70%), sales/marketing (11.80%), cybersecurity (10.60%) were the largest categories — predominantly simple rule-based or moderately complex ML models; 35% of respondents used public cloud deployment.
- 67% of the 76 FTD-surveyed entities were exploring at least one Gen AI use case, mostly experimental (internal chatbots, employee productivity), with reluctance toward customer-facing Gen AI due to data sensitivity and explainability/bias concerns.
- Cited adoption barriers: AI talent gap, implementation cost, data quality, computing access, legal uncertainty.

### The Seven Sutras (guiding principles, Chapter 4.3)
The report frames its recommendations around seven principles for "Responsible and Ethical Enablement of AI" in finance (named "Sutras" — consistent with the parallel India AI Governance Guidelines' seven-sutra structure, see [[07_Institutions/Corpus/MeitY/MeitY_2]]). Full enumeration not captured in extraction — ⚠ VERIFY BEFORE PUBLISHING: confirm exact sutra names and wording against primary text before use in any deliverable, and check for overlap/divergence with the India AI Governance Guidelines' sutras (Trust, People First, Innovation over Restraint, Fairness & Equity, Accountability, Understandable by Design, Safety/Resilience/Sustainability).

### Key recommendations (Chapter 4.4, by pillar)

**Governance Pillar (mostly "Medium term" — recommended, not yet mandatory):**
- **Board-Approved AI Policy**: REs should establish a board-approved AI policy covering governance structure, accountability, risk appetite, operational safeguards, auditability, consumer protection measures, AI disclosures, model life cycle framework, and liability framework. Industry bodies should provide an indicative policy template for smaller entities.
- **Data Lifecycle Governance**: REs must establish data governance frameworks for collection, access, usage, retention, and deletion of data used in AI systems, ensuring compliance with "applicable legislations, such as the DPDP Act" — direct cross-reference to [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]].
- **AI System Governance Framework**: REs must implement model governance covering the full AI lifecycle (design, development, deployment, decommissioning), including model documentation, validation, and ongoing monitoring for model drift/degradation. For **autonomous AI systems capable of independent financial decision-making**, the report calls for stronger governance with **human oversight, especially for medium- and high-risk use cases** — this is the report's explicit agentic-AI governance provision.
- **Product Approval Process**: AI-enabled products/solutions must be brought within scope of institutional product approval frameworks, with AI-specific risk evaluations included.

**Protection Pillar:**
- **Consumer Protection**: REs should establish a board-approved consumer protection framework prioritising transparency and fairness for AI-driven decisions (text truncated at extraction boundary — ⚠ VERIFY remaining detail against primary text).

**Capacity-building / ecosystem recommendations:**
- RBI may consider establishing a dedicated AI institute for sector-wide capacity development.
- Industry bodies (IBA, SROs) should establish frameworks for sharing AI use cases, lessons learned, and best practices.
- Regulators and industry bodies should introduce structured recognition/reward programs for responsible AI innovation with positive social impact.

### Distinguishing mandatory vs. recommended
The report is explicitly framed as **advisory** — recommendations use "should" throughout (e.g., "REs should establish a board-approved AI policy") rather than "shall." No mandatory disclosure regime, enforcement trigger, or supervisory reporting obligation is established by this document itself. ⚠ VERIFY BEFORE PUBLISHING — confirm whether any RBI Master Direction has since converted any of these "should" recommendations into binding "shall" requirements (Annexure IV references "AI Specific Enhancements in RBI Master Directions" but full text not captured in extraction).

---

## Analytical Significance for PRIS Research

### For P3 (BFSI AI Governance Regulatory Parallelism, JEIM) and fsQCA
This is a **primary instrument** for P3/fsQCA — per the existing Wiki Intake stub, fsQCA working RL (regulatory leadership/legitimacy?) score = 0.33, characterised as an "advisory-dominant architecture." The report's explicit incorporation of DPDP (MeitY) and its silence on SEBI/IRDAI cross-references is direct evidence of the **Regulatory Parallelism** construct: RBI governs AI in BFSI without coordination mechanisms to SEBI (which separately regulates AI/ML disclosure for market intermediaries — see SEBI_9, SEBI_10, SEBI_11) or IRDAI (insurance AI — currently no corpus node, gap identified in vault structure).

### Coordination / Parallelism Pattern
Existing nodes: [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (Convergence — explicit incorporation by reference for data lifecycle); [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_11]] (Parallelism — no cross-reference found in extracted text between RBI FREE-AI and SEBI AI/ML reporting circulars, despite both governing AI use by regulated financial entities).

**Upstream convergence**: [[07_Institutions/Corpus/MeitY/MeitY_2]] (India AI Governance Guidelines) explicitly states its seven cross-sectoral "sutras" were adapted from this report's Seven Sutras — a named instance of sectoral-to-cross-sectoral policy diffusion. This is the strongest Institutional Coherence signal identified in Batch 1.

### Consulting Connection
**AEGIS_OS**: The report's call for "strong governance before deploying autonomous AI systems... capable of acting independently in financial decision-making," including human oversight for medium/high-risk use cases, is directly relevant to AEGIS_OS's runtime decision enforcement / authority-binding value proposition for agentic AI in regulated financial contexts.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]], [[07_Institutions/Corpus/RBI/RBI_1]], [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_11]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]], [[05_Concepts/05_Concepts_Signature/Governance_Debt]], [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]], [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** [[07_Institutions/Corpus/MeitY/MeitY_2]] (India AI Governance Guidelines — parallel seven-sutra structure)
**Related projects:** [[02_Projects/P3_BFSI_JEIM]], [[02_Projects/P4_Doctrinal_IJLIT]], [[02_Projects/fsQCA_Thesis_Chapter]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** AEGIS_OS (agentic AI / autonomous decision-making governance provisions)

---

## Coding Status

- **P3 NVivo:** In canonical corpus (per existing Wiki Intake stub: "Instrument node built in Corpus" — this session completes that reference) — confirm RU count in next NVivo pass
- **Wiki intake status:** Pending — existing stub at [[04_Knowledge_Products/Wiki_Intake/RBI_FREEAI_MasterCircular]] should be updated to reflect this node now exists

---

## Operationalizing Recommendations — Not Yet Notified (confirmed 2026-08-02)

The FREE-AI Report recommends amendments to seven existing RBI instruments rather than announcing new standalone circulars. **No separate RBI circular formally implementing any of these amendments has been located as an independently confirmed primary document as of this search** — treat as Committee recommendations only, not yet operative regulatory change:

- RBI Guidelines on Outsourcing of Financial Services (algorithmic bias/accountability clauses for vendors)
- Cyber Security Framework in Banks (AI-specific risks: model poisoning, adversarial attacks)
- RBI (Digital Lending) Directions, 2025 (disclosure of AI-driven credit assessments, fairness audits)
- Master Circular on Customer Service in Banks, 2015 (AI-usage disclosure, customer contestability of AI decisions)
- Fraud Risk Management Master Direction (AI-based early-warning fraud signals)
- Master Direction on IT Governance, Risk, Controls and Assurance Practices ([[07_Institutions/Corpus/RBI/RBI_1]]) (autonomous AI system access controls)
- Master Direction on Outsourcing of IT Services ([[07_Institutions/Corpus/RBI/RBI_2]]) (AI-specific risk disclosure by service providers)

This is itself an analytically useful finding: FREE-AI is a foundational-document stage instrument (Sutras + strategic pillars + 26 recommendations), not yet a binding amendment cycle — any PRIS analysis citing "RBI's FREE-AI obligations" as currently binding must specify that these are Committee recommendations pending implementation, structurally analogous to the DPDP "enacted but not operative" pattern already documented in [[06_Frameworks/DPDP_Act_2023]], though for a non-binding report rather than a statute.

## Confirmed Coordination Gap (2026-08-02)

**No joint RBI-SEBI-IRDAI statement specifically on AI governance was located.** The closest coordination-pattern evidence is structural/parallel rather than jointly issued: regulatory sandbox frameworks exist independently at RBI (Enabling Framework for Regulatory Sandbox, August 2019, updated February 2024), SEBI, and IRDAI, with RBI's Inter-operable Regulatory Sandbox (IoRS) — designed for products spanning more than one financial regulator's remit — as the single closest primary cross-regulator mechanism, though it is general fintech-focused rather than AI-specific. An ORF comparative analysis explicitly recommends an "overarching uniform regulatory framework" precisely because no such joint AI/fintech governance coordination body currently exists among RBI, SEBI, IRDAI, and IFSCA. This absence is a direct, citable strengthening of the existing [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] argument: FREE-AI (RBI), the SEBI AI/ML circulars, and IRDAI's Working Group ([[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]]) each proceed structurally siloed by regulator, with no coordinating mechanism.

### AI System Governance — inventory and audit provisions (added 2026-08-02, model-risk pass)

**¶4.4.68 — AI system inventory.** REs must "maintain a comprehensive inventory of AI systems in use across their operations," with specified fields: AI Models and Algorithms (model type — ML, deep learning, NLP, GenAI); Use Cases; Dependencies including third-party providers; Risk Categorisation (High/Medium/Low); Grievances record. **Updated semi-annually** and available for supervisory inspection.

**Recommendation 24 — AI Audit Framework.** Internal audit for all AI applications; **third-party audit for high-risk use cases**; biennial review of the audit framework itself.

**Governance scope, verbatim:** "AI system governance refers to the structured oversight of AI models and systems, including both conventional AI models and increasingly autonomous AI systems… REs must implement appropriate governance mechanisms across the entire AI model lifecycle, covering model design, development, deployment, and decommissioning."

**Comparative significance.** That scope language signals **inclusion** of autonomous/agentic systems within model governance — the opposite of the US position, where SR 26-2 (17 Apr 2026) **explicitly carves generative and agentic AI out** of model risk management as "novel and rapidly evolving." On the conceptual-scope question India is aligned with the UK's PRA SS1/23 and **ahead of the US**, which has excluded the fastest-moving category. India's deficit here is bindingness, not scope — a more precise diagnosis than the corpus's default framing. See [[05_Concepts/05_Concepts_Standard/Model_Risk]] for the full four-jurisdiction comparison, and [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]] for the conventional-model track.

## Log

- 2026-06-14: Corpus node created. Batch 1. Cowork session. Source: FREE-AI Committee Report.pdf. Note: this fills a previously broken wikilink referenced by [[04_Knowledge_Products/Wiki_Intake/RBI_FREEAI_MasterCircular]].
- 2026-08-02: Perplexity Deep Research re-verification per [[Thin_Node_Perplexity_Prompts_2026-08-02]] BFSI_Governance prompt. Replaced secondary-hosted link with confirmed direct rbi.org.in repository link. Added operationalizing-recommendations list (7 target instruments, none yet independently confirmed as amended) and the confirmed RBI/SEBI/IRDAI non-coordination finding.
