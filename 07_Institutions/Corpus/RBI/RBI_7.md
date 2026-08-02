---
type: corpus-node
node-id: RBI_7
institution: RBI
date: 2025-05-08
wiki-section: S2
tier: A
ai-explicit: true
tags:
  - type/corpus-node
  - institution/RBI
  - wiki-section/S2
  - tier/A
  - batch/11
  - concept/Regulatory_Parallelism
  - concept/Governance_Debt
  - concept/Accountability
  - concept/Transparency
  - project/P3
  - project/P4
  - project/fsQCA
---

# RBI_7 — Reserve Bank of India (Digital Lending) Directions, 2025

**Node ID:** RBI_7  
**Institution:** Reserve Bank of India (RBI)  
**Document type:** Regulatory — Master Direction under Banking Regulation Act / RBI Act  
**Date:** May 8, 2025 (RBI/2025-26/36)  
**Jurisdiction:** India  
**Wiki Section:** S2 — India Regulatory  
**Tier:** A (primary RBI regulatory instrument; verbatim quotes extracted)  
**Source PDF:** RBI Digital Lending Regs.PDF

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Reserve Bank of India (Digital Lending) Directions, 2025 |
| Issuing Authority | Reserve Bank of India |
| Reference Number | RBI/2025-26/36 |
| Date | May 8, 2025 |
| Legal basis | Banking Regulation Act 1949; Reserve Bank of India Act 1934 |
| Scope | All Regulated Entities (REs) — scheduled commercial banks, co-operative banks, NBFCs, and their Loan Service Providers (LSPs) engaged in digital lending |
| Supersedes | Earlier digital lending guidelines (2022 framework) |
| AI relevance | Explicit: Chapter IV (Technology and Data Requirements) directly governs AI-driven creditworthiness assessment, training data, and LSP AI model oversight |

---

## S2. Governance Context

RBI_7 is the most recent primary RBI regulatory instrument in the corpus (May 2025), superseding the 2022 digital lending guidelines. It arrives after:

- **RBI_FREE_AI_2025** (November 2025) — Seven Sutras AI governance framework (principles-based, "should" language)
- **RBI_3** (Draft Circular Model Risk in Credit, August 2024) — unresolved draft as of Batch 11
- **RBI_2** (IT Outsourcing Master Direction, 2023) — technology-neutral third-party governance baseline

RBI_7 is operationally distinct from these: it is a **sector-specific, binding** direction that explicitly regulates AI/ML use in the context of digital credit assessment. Where RBI_FREE_AI_2025 is aspirational and principles-based, RBI_7 is operative and prescriptive.

**Parallelism significance:** RBI_7 regulates AI-driven credit assessment without cross-reference to SEBI_14's sole-responsibility-for-AI-outputs framework. A bank offering both lending (RBI_7 scope) and investment advisory (SEBI_14 scope) operates under two independent AI accountability regimes with no lex specialis mapping — extending Cluster C09 intra-SEBI convergence into the RBI lending domain.

---

## S3. Regulatory Units (RUs) — AI-Relevant

| RU# | Provision | Deontic | Key Obligation | ADICO elements |
|---|---|---|---|---|
| RU1 | Due diligence on Loan Service Providers (LSPs) | SHALL | REs must conduct due diligence on LSPs, including assessment of AI/ML systems used for creditworthiness determination | A=RE; D=SHALL; I=conduct LSP due diligence including AI model assessment; C=before onboarding/periodic review |
| RU2 | Creditworthiness assessment governance | SHALL | AI-driven credit scoring and lending decisions must meet data governance standards; basis of AI-assisted decisions must be supportable | A=RE/LSP; D=SHALL; I=document AI credit model basis; C=RBI supervisory oversight |
| RU3 | Data collection standards for AI | SHALL | Collection, usage, and sharing of customer data with third parties governed; training data provenance must comply with applicable frameworks | A=RE/LSP; D=SHALL; I=implement data collection/sharing standards; C=AI training data used in creditworthiness assessment |
| RU4 | Storage security for AI training/operational data | SHALL | Data storage security requirements apply to all data used in AI credit assessment, including model training datasets | A=RE/LSP; D=SHALL; I=implement storage security controls; C=data used in digital lending AI systems |
| RU5 | Comprehensive privacy policy | SHALL | All digital lending platforms using AI must maintain a comprehensive privacy policy explaining AI use of customer data in credit decisions | A=RE (digital lending platform); D=SHALL; I=publish comprehensive privacy policy; C=AI-assisted lending |
| RU6 | Default Loss Guarantee (DLG) arrangement governance | SHALL | DLG arrangements where AI models inform guarantee decisions face regulatory scrutiny; RE retains accountability for AI-informed DLG decisions | A=RE; D=SHALL; I=retain accountability for AI-informed DLG outcomes; C=DLG arrangements using AI credit assessment |

---

## S4. Key Verbatim Quotes

> "Due diligence requirements with respect to Loan Service Providers (LSPs)." — RBI/2025-26/36, May 8, 2025

> "Assessing the borrower's creditworthiness." — RBI Digital Lending Directions 2025

> "Collection, usage and sharing of data with third parties." — RBI Digital Lending Directions 2025

> "Storage of data security requirements." — RBI Digital Lending Directions 2025

> "Comprehensive privacy policy requirement for all platforms." — RBI Digital Lending Directions 2025

---

## S5. Analytical Notes

**RBI_7 vs. RBI_FREE_AI_2025 — deontic gap:**

RBI_FREE_AI_2025 uses "should" language throughout (Seven Sutras are aspirational principles). RBI_7 uses "shall" — it is a binding Master Direction. This creates a bifurcated RBI AI governance landscape:

| Instrument | Modality | Domain | Deontic |
|---|---|---|---|
| RBI_FREE_AI_2025 | Principles-based | Broad AI governance across BFSI | Should (voluntary) |
| RBI_7 | Rules-based | Digital lending AI specifically | Shall (binding) |
| RBI_3 | Draft circular | Model risk in credit | Pending |

For fsQCA: India's BFSI AI governance now has an *intra-RBI* deontic configuration: binding sector-specific (digital lending) + aspirational general principles. This complicates the binary "principles-based vs. rules-based" calibration and may require a graduated calibration.

**LSP due diligence chain:**
RU1 creates a vendor accountability chain for AI credit models: the RE is responsible for the LSP's AI creditworthiness model, regardless of whether the RE built it. This is structurally parallel to SEBI_14's sole-responsibility clause (RE accountable for AI tools used, including third-party tools) — the two instruments converge on the accountability-attribution pattern without cross-reference.

**Credit AI and DPDP Act:**
RU3 (data collection/sharing standards) and RU5 (privacy policy) operate alongside but without explicit reference to the DPDP Act 2023 / DPDP Rules 2025 (MeitY_4). A consumer whose AI-driven loan application is rejected faces: (a) RBI_7 data governance protections; (b) DPDP Act consent/notice protections; and (c) no statutory right to AI explanation (unlike EU AI Act per HCJP/International_12). The DPDP-RBI_7 interaction is not mapped in either instrument — a lex specialis gap. (⚠V-RBI7-3)

---

## S6. Concept Linkages

| Concept | Evidence from RBI_7 |
|---|---|
| [[Regulatory_Parallelism]] | RBI_7's AI accountability chain for digital lending (LSP due diligence = RE accountability) co-exists with SEBI_14's sole-responsibility clause without cross-reference; both apply to dual-regulated entities (NBFCs with both lending and securities operations). Extends the P3 corpus's parallelism finding into the digital credit domain — the most operationally urgent 2025 BFSI AI governance instrument. |
| [[Governance_Debt]] | May 2025 binding instrument creates a new compliance layer for all digital lending REs and their LSPs. Until RBI_3 (Model Risk in Credit draft) is finalised, dual-regulated entities must navigate both the binding RBI_7 LSP-AI due diligence framework AND the unresolved RBI_3 model-validation principles — regulatory-uncertainty governance debt persists alongside the operative RBI_7 obligations. |
| [[Accountability]] | RU1 (LSP due diligence) + RU6 (DLG retention) = explicitly named accountability chain: RE cannot transfer AI credit decision accountability to LSP vendor. Structurally parallel to SEBI_14 Reg.16C sole-responsibility. Together these two 2025 instruments (RBI_7 and SEBI_14) represent RBI and SEBI independently converging on the same accountability-attribution design for AI tools — parallelism in accountability architecture itself. |
| [[Transparency]] | RU5 (comprehensive privacy policy explaining AI use in credit decisions) = regulator-mandated user-facing transparency for AI-assisted lending. Does not rise to the EU AI Act standard of a statutory consumer right to AI explanation (HCJP finding, International_12) — privacy policy disclosure vs. legally actionable explanation right. |

---

## S7. Project Relevance

| Project | Relevance |
|---|---|
| P3 (BFSI — JEIM) | Core corpus: most recent (May 2025) binding RBI instrument for AI in digital lending; extends the BFSI AI governance timeline to 2025; strengthens the RBI accountability-architecture analysis alongside SEBI_14 |
| P4 (Doctrinal — IJLIT) | LSP due diligence chain (RU1) and DLG accountability retention (RU6) provide new ADICO-codeable deontic obligations for doctrinal analysis; RBI_7 vs. SEBI_14 parallel accountability architectures is a P4 comparative design contribution |
| fsQCA | India BFSI configurational evidence: RBI_7's binding sector-specific rules (digital lending) alongside RBI_FREE_AI_2025's voluntary general principles — a within-India intra-regulator deontic configuration not previously documented in the corpus |

---

## S8. ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-RBI7-1 | Confirm RBI_7 supersedes all prior digital lending guidelines (2022 framework) or only partially amends | rbi.org.in → Notifications → Master Directions 2025 |
| ⚠V-RBI7-2 | Chapter IV Technology and Data Requirements — confirm exact section numbering and whether AI is named explicitly or implied through "technology systems" | Primary text: RBI/2025-26/36 |
| ⚠V-RBI7-3 | DPDP Act interface: does RBI_7 explicitly reference DPDP Act 2023 / DPDP Rules 2025 for the data collection/sharing obligations (RU3), or are these independent tracks? | Primary text; also cross-check MeitY_4 (DPDP Rules 2025) for any RBI cross-reference |
| ⚠V-RBI7-4 | LSP AI due diligence: does RBI_7 specify that AI/ML systems used by LSPs must meet any minimum standards (e.g., explainability, fairness) or is the due diligence obligation technology-neutral? | Primary text Chapter on LSP governance |

---

## Backlinks

← [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (Seven Sutras — aspirational companion to RBI_7's binding obligations)  
← [[07_Institutions/Corpus/RBI/RBI_2]] (IT Outsourcing Master Direction — technology-neutral third-party baseline; RBI_7 adds AI-specific LSP layer)  
← [[07_Institutions/Corpus/RBI/RBI_3]] (Draft Model Risk in Credit — pending finalisation; unresolved alongside RBI_7)  
← [[07_Institutions/Corpus/SEBI/SEBI_14]] (Parallel sole-responsibility architecture for AI tools — no cross-reference)  
← [[04_Knowledge_Products/Wiki_Intake/International_12_HCJP_Legal_AI_BFSI_2025]] (EU AI Act consumer right to explanation — gap comparator for RBI_7 RU5)  
← [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]  
← [[05_Concepts/05_Concepts_Standard/Accountability]]  
← [[05_Concepts/05_Concepts_Standard/Transparency]]
