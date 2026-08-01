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

# RBI_6 — Reserve Bank of India (All India Financial Institutions – Managing Risks in Outsourcing) Directions, 2025

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India, Department of Regulation
**Document date:** November 28, 2025 (RBI/DOR/2025-26/337, DOR.ORG.REC.No.256/21-04-158/2025-26)
**Pages:** 30
**Domain:** [[03_Domains/BFSI_Governance]] | [[03_Domains/AI_Governance]]

---

## Instrument Identity

**Full title:** Reserve Bank of India (All India Financial Institutions – Managing Risks in Outsourcing of Information Technology Services) Directions, 2025
**Type:** Master Direction
**Target entities:** All India Financial Institutions (AIFIs) only — explicitly defined as EXIM Bank, NABARD, NaBFID, NHB, and SIDBI. ⚠ VERIFY BEFORE PUBLISHING: this is a narrow, named-entity scope (5 institutions) — does NOT extend to scheduled commercial banks, NBFCs, or co-operative banks, which remain under [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction, Apr 2023).
**Legal basis:** Section 45L of the Reserve Bank of India Act, 1934
**Companion documents:** Repeals and supersedes prior outsourcing directions per circular DOR.RRC.REC.302/33-01-010/2025-26 (also dated Nov 28, 2025). Companion/parallel instrument to [[07_Institutions/Corpus/RBI/RBI_1]] (IT Governance Master Direction, Nov 2023) and [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction, Apr 2023) — the latter is the bank/NBFC equivalent of this AIFI-specific instrument.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S6 (Implementation & Governance Artifacts — cloud governance templates)
**Jurisdiction:** India
**Confidence:** High — primary regulation, Master Direction status under statutory power
**AI explicit:** Partial — not an AI-specific instrument, but Cloud Computing Services section (paras 60–61) directly governs AI/ML workload outsourcing infrastructure (IaaS/PaaS/SaaS), and IT-outsourcing risk controls apply to any AI vendor engagement by an AIFI
**Tier classification:** Tier B — technology-neutral IT-outsourcing regulation with direct AI-infrastructure application
**AI Governance Wiki relevance:** MEDIUM — provides the most current (Nov 2025) Indian regulatory template for cloud/CSP governance, which is directly reusable for AI vendor risk frameworks even though AIFIs are a small institutional set

---

## Substantive Content

### Scope and Coming Into Force
- Applies to **material outsourcing of IT services** by the five named AIFIs (EXIM Bank, NABARD, NaBFID, NHB, SIDBI).
- Directions come into force **immediately** upon issue (Nov 28, 2025).
- ⚠ VERIFY BEFORE PUBLISHING: Existing outsourcing arrangements must be reviewed and brought into compliance by **April 10, 2026** — this compliance deadline is now in the past relative to the current session date (2026-06-15); any future citation should note actual compliance status rather than treat this as a forward-looking deadline.

### Governance Framework (Mandatory)
- **Board-approved IT outsourcing policy** required, reviewed periodically.
- Defines tripartite governance: **Board/Board Committee** (overall responsibility, cannot be outsourced), **Senior Management** (implementation, risk assessment, monitoring), and the **IT Function/CISO** (technical due diligence, security configuration review).
- Outsourcing **does not diminish** the AIFI's own obligations to customers, regulators, or for confidentiality — accountability remains non-transferable (a recurring [[05_Concepts/05_Concepts_Standard/Accountability]] pattern across RBI instruments).

### Due Diligence (15-point framework)
Before onboarding any IT service provider, AIFIs **must** assess (illustrative, non-exhaustive per the Direction): financial soundness, technical competence, security track record, sub-contracting arrangements, business continuity capability, insurance cover, regulatory/legal compliance history, geographic concentration risk, and exit feasibility.

### Outsourcing Agreement — Minimum Contractual Clauses (24-point list)
Mandatory clauses include (selected, highest-relevance items):
- **Data localisation**: customer/business data arising from outsourced activity **must be stored in India** (cross-border processing permitted under conditions, but storage location requirement is explicit).
- **RBI audit access**: contracts must give RBI or its appointed agents the **right to access/inspect** the service provider's premises, systems, and records.
- Confidentiality and data protection obligations surviving contract termination.
- Sub-contracting restrictions — prior AIFI approval required for further sub-outsourcing.
- Right to conduct on-site inspections and obtain audit reports (including pooled/shared audits — see below).
- Termination rights without cause on reasonable notice, and clearly defined exit transition timelines.

### Monitoring, Audit and Reporting
- AIFIs must maintain a **central register** of all material outsourcing arrangements.
- **Pooled/shared audits** across multiple client institutions are explicitly permitted for common service providers — a practical [[05_Concepts/05_Concepts_Signature/Governance_Debt]] mitigation mechanism (reduces duplicative audit burden on shared CSPs/vendors).
- Internal audit and risk functions must periodically review outsourced arrangements as part of the regular audit plan.

### Business Continuity and Exit Strategy
- AIFIs must maintain **BCP/DR arrangements** covering outsourced IT services, tested periodically.
- A documented **exit strategy** is mandatory for every material outsourcing arrangement, including identified alternative arrangements and transition timelines — applies equally to cloud exit (see below).

### Group/Conglomerate and Offshore Outsourcing
- Intra-group outsourcing (e.g., to a group IT-services entity) is permitted but subject to the **same due diligence and contractual standards** as third-party outsourcing — no group-entity carve-out.
- Offshore (cross-border) outsourcing permitted subject to: data localisation requirements (India-stored copies), legal enforceability of RBI's audit/inspection rights in the offshore jurisdiction, and country-risk assessment of the offshore location.

### Outsourcing of Security Operations Centre (SOC) Services
Five **additional** requirements beyond the general framework apply specifically to SOC outsourcing — including enhanced monitoring of the SOC provider's access privileges, incident-escalation SLAs to the AIFI's own CISO, and restrictions on SOC providers sub-contracting monitoring functions further. (⚠ VERIFY BEFORE PUBLISHING — the five specific SOC requirements should be re-confirmed against paras if this becomes a citation point for cyber-resilience work, given overlap with [[07_Institutions/Corpus/CERT_In/CERT_2]] and [[07_Institutions/Corpus/CERT_In/CERT_4]].)

### Cloud Computing Services (Section E.4, paras 60–61) — Highest Reuse Value
- Explicit coverage of **IaaS, PaaS, and SaaS** models.
- Mandates a **Board-approved cloud adoption/governance policy** distinct from the general IT outsourcing policy.
- **CSP selection** must be risk-based, considering concentration risk (avoiding over-reliance on a single CSP), jurisdiction of data storage/processing, and the CSP's own sub-processor chain.
- **Identity and Access Management (IAM)** controls mandatory, including **multi-factor authentication (MFA)** for privileged access to cloud environments.
- References **NIST SP 800-210** (General Access Control Guidance for Cloud Systems) as a benchmark — the first explicit NIST cloud-security standard citation observed in an RBI AIFI-facing instrument in this corpus.
- **Cloud exit strategy** required as a distinct sub-component of the general exit-strategy obligation — covers data portability, de-provisioning, and migration to an alternative CSP or in-house infrastructure.

---

## Analytical Significance for PRIS Research

### For P3 (BFSI AI Governance Regulatory Parallelism, JEIM)
This instrument is structurally near-identical to [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction for banks/NBFCs, Apr 2023) but issued ~2.5 years later for a narrower institutional population (5 AIFIs vs. all banks/NBFCs/co-operative banks). This is direct evidence of RBI's **template-replication regulatory style**: rather than amending RBI_2's scope to cover AIFIs, RBI issued a parallel, near-duplicate Master Direction. This is a useful within-regulator (not cross-regulator) instance of [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — same risk domain, same control architecture, segmented by institutional category rather than coordinated under one instrument. The Cloud Computing Services section (paras 60–61) is the most current RBI articulation of cloud/CSP governance expectations and is directly transferable to any AI-infrastructure outsourcing analysis for P3's BFSI corpus.

### Coordination / Parallelism Pattern
**Existing node:** [[07_Institutions/Corpus/RBI/RBI_2]] (RBI IT Outsourcing Master Direction, Apr 2023, banks/NBFCs).
**Pattern:** Convergence with segmentation — RBI_6 replicates RBI_2's governance architecture (Board/Senior Management/IT Function roles, due diligence framework, exit strategy, audit-access clauses) almost clause-for-clause but issued as a **separate instrument for a separate institutional category** (AIFIs) rather than as an amendment extending RBI_2's scope. This is a "parallel-but-coherent" pattern — distinguishable from cross-regulator duplication (which RBI_2/SEBI/IRDAI comparisons typically show) because both instruments originate from the same regulator and are internally consistent in design.

### Possible link to RBI_5 ⚠VERIFY flag #31
[[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]]'s open ⚠VERIFY flag (#31 in [[Corpus_Index_MOC]]) notes a reference to a "new framework for financial services outsourcing... in the pipeline." ⚠ VERIFY BEFORE PUBLISHING: RBI_6 is a **candidate but not confirmed** resolution of this flag — RBI_5 concerns NBFC operational risk management (broader scope), while RBI_6 is scoped specifically to AIFI **IT** outsourcing only. These may be two distinct instruments responding to the same underlying RBI policy direction (post-2023 consolidation of outsourcing-risk frameworks across institutional categories), or RBI_5's reference may point to a still-unissued, broader-scope instrument. Do not assert RBI_6 as the answer to flag #31 without checking RBI_5's source text for the exact framing of "in the pipeline."

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_1]] (IT Governance Master Direction — Board/Senior Management governance architecture parallel), [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction — direct structural template this instrument replicates for AIFIs), [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] (possible — unconfirmed — link via ⚠VERIFY flag #31)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]], [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (pooled audit provision as a governance-debt mitigation mechanism), [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (cloud/CSP IAM and MFA controls directly applicable to agentic AI infrastructure governance)
**Related frameworks:** [[06_Frameworks/RBI_Free_AI]] (cloud governance provisions complement FREE-AI's infrastructure-risk recommendations)
**Related projects:** [[02_Projects/P3_BFSI_JEIM]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** None identified — AIFI scope (5 named DFIs) falls outside current AEGIS_OS/PrivacyWeave engagement profiles, though the Cloud Computing Services template (paras 60–61) is reusable reference material for any BFSI cloud-governance advisory.

---

## Coding Status

- **P3 NVivo:** Screening corpus — candidate for canonical inclusion as a within-regulator parallelism instance; cloud governance section (paras 60–61) is high-value evidence
- **Wiki intake status:** Pending

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session.
