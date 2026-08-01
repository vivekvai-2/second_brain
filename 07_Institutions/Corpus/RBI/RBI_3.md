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

# RBI_3 — Draft Circular: Regulatory Principles for Management of Model Risks in Credit

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_3.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India, Department of Regulation (DoR.STR.REC.)
**Document date:** Draft circular, 5 August 2024 (for comments — not yet confirmed as final)
**Pages:** 5
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Regulatory Principles for Management of Model Risks in Credit
**Type:** Draft Circular (for comments — status of finalisation ⚠ VERIFY BEFORE PUBLISHING)
**Target entities:** All Commercial Banks (incl. RRBs and LABs), all Primary (Urban) Co-operative Banks, all State/Central Co-operative Banks, all NBFCs (incl. HFCs), all All-India Financial Institutions
**Legal basis:** Sections 21, 35A, 56 of the Banking Regulation Act, 1949; Sections 45JA, 45L, 45M of the RBI Act, 1934; Sections 30A, 32, 33 of the National Housing Bank Act, 1987
**Companion documents:** [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (FREE-AI report's "AI System Governance Framework" recommendation closely parallels this draft's model risk principles, predating it by ~1 year)

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework, BFSI) and S6 (Implementation & Governance Artifacts)
**Jurisdiction:** India
**Confidence:** Medium — draft circular, not yet confirmed as finalised/binding
**AI explicit:** No (technology-neutral "credit risk model" definition, but explicitly captures any "quantitative method that applies statistical, economic, financial, or mathematical principles" — covers ML/AI credit models)
**Tier classification:** Tier B — technology-neutral with direct AI application
**AI Governance Wiki relevance:** MEDIUM — provides the model-governance baseline (model inventory, validation cadence, board oversight) that AI-specific frameworks (RBI_FREE_AI_2025) build upon for credit-scoring AI specifically.

---

## Substantive Content

### Scope definition (mandatory)
"Credit risk model" = any quantitative method applying statistical, economic, financial, or mathematical principles/assumptions to process data into outputs used for credit decisions, including credit scoring/borrower selection, loan pricing, risk analysis, loan loss provisioning, and economic capital estimation. This definition is broad enough to capture ML-based credit scoring models without naming AI/ML explicitly.

### Governance and oversight (mandatory, "shall")
- REs **shall** put in place a Board-approved policy on model risk management covering the entire model life cycle: governance/oversight commensurate with model materiality, development/selection processes, documentation, independent vetting/validation, change control, monitoring/reporting (including internal audit role), and third-party model usage.
- REs **shall** maintain a **Model Inventory** of all approved models (in-sourced or outsourced) with critical information.
- Deployment of individual credit models, and any subsequent changes to inputs/assumptions, **shall** require approval of the Risk Management Committee of the Board (RMCB) or a designated Sub-Committee.

### Model development and deployment principles (mandatory)
- Objectives, problem statements, and intended solutions must be clearly defined.
- Inputs/assumptions must ensure robustness.
- Detailed documentation required, including sensitivity of outputs to assumptions/inputs.
- Models must have scalability/flexibility for dynamic business conditions and interface with core banking/ALM/risk systems.
- **Outcomes "shall be consistent, unbiased, explainable and verifiable"** — this is the closest analogue in this document to AI-specific "fairness/explainability" requirements, applied here to credit models generally.
- Manual overrides of model outcomes must follow policy provisions and be documented in auditable form.
- For outsourced/third-party models: REs remain "ultimately responsible and accountable for the integrity and outcomes," and contracts must provide access to minimum technical documentation on design/configuration/operation.

### Model validation framework (mandatory)
- Independent vetting/validation process required, separate from model development/selection.
- Each model validated **before deployment** and **after material amendments**, with periodic review **at least annually**.
- External experts may be engaged for validation.
- Validation must review assumption validity, data accuracy, and data source reliability (text truncated at extraction boundary — further validation criteria not captured).

---

## Analytical Significance for PRIS Research

### For P3 (BFSI AI Governance Regulatory Parallelism, JEIM)
This draft (Aug 2024) predates the RBI FREE-AI Committee Report (2025) by roughly a year and establishes model-governance baselines — board-approved policy, model inventory, annual validation, explainability/auditability of outcomes — that FREE-AI's "AI System Governance Framework" recommendation (Section 4.4) appears to extend specifically to AI/agentic systems. This is evidence of **sequential layering within a single regulator** (RBI issuing successive, increasingly AI-specific model governance instruments) rather than cross-regulator parallelism — a useful contrast case to the MeitY/RBI convergence found in Batch 1.

### Coordination / Parallelism Pattern
Existing node: [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]]. Pattern: **Sequential convergence (intra-regulator)** — RBI_3 (2024, technology-neutral model risk) is a direct precursor to RBI_FREE_AI_2025's (2025) AI-specific model governance recommendations. Useful as a "before/after" pair for tracking regulatory evolution toward AI-explicit governance within one regulator.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]], [[07_Institutions/Corpus/RBI/RBI_1]]
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** —
**Related projects:** [[02_Projects/P3_BFSI_JEIM]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** —

---

## Coding Status

- **P3 NVivo:** Screening corpus (candidate — assess as precursor instrument for the BFSI AI governance evolution timeline)
- **Wiki intake status:** Pending

---

## Log

- 2026-06-14: Corpus node created. Batch 2. Cowork session. Source: RBI-DRAFT-MANAGEMENT-OF-MODEL-RISK-IN-CREDIT-05-08-24.pdf. ⚠ VERIFY: confirm whether this draft circular has since been finalised/issued as a binding Master Direction.
