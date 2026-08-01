---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/sebi
---

# SEBI_14 — Securities and Exchange Board of India (Intermediaries) (Amendment) Regulations, 2025

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/SEBI/SEBI_14.md`
**Institution:** [[07_Institutions/SEBI]]
**Issuing body:** Securities and Exchange Board of India
**Document date:** February 6, 2025 (notified); published Gazette of India Extraordinary February 10, 2025 (No. 92)
**Pages:** Not determinable from gazette extract
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Securities and Exchange Board of India (Intermediaries) (Amendment) Regulations, 2025
**Notification reference:** F.No. SEBI/LAD-NRO/GN/2025/226
**Type:** Statutory Amendment Regulation (amendment to principal Regulations of 2008)
**Target entities:** All registered persons under SEBI (Intermediaries) Regulations, 2008 — stock brokers, sub-brokers, investment advisers, portfolio managers, merchant bankers, research analysts, and all other SEBI-registered intermediary categories
**Legal basis:** Sections 11(1) and 30 of the Securities and Exchange Board of India Act, 1992, read with SEBI (Intermediaries) Regulations, 2008
**Companion documents:** [[07_Institutions/Corpus/SEBI/SEBI_11]] (Board Memo: AI Responsibility Assignment 2024–25), [[07_Institutions/Corpus/SEBI/SEBI_9]] (AI/ML Reporting for MIIs, Jan 2019), [[07_Institutions/Corpus/SEBI/SEBI_10]] (AI/ML Reporting for Mutual Funds, May 2019)

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S4 (Agentic AI Governance)
**Jurisdiction:** India
**Confidence:** High — primary gazette notification; binding statutory regulation
**AI explicit:** Yes
**Tier classification:** Tier A — Explicit AI regulation: sole-responsibility obligation for AI/ML tool outputs is named and imposed by statute
**AI Governance Wiki relevance:** HIGH — First binding statutory regulation in the Indian securities market specifically governing AI/ML tool usage; elevates SEBI_11 Board-memo-level AI responsibility assignment to the force of law

---

## Substantive Content

### Amendment Structure

Chapter IIIB — "Usage of Artificial Intelligence" is inserted into SEBI (Intermediaries) Regulations, 2008, after the existing Chapter IIIA. The chapter consists of a single operative regulation: Regulation 16C.

### Regulation 16C — Full Operative Text (reconstructed)

Every registered person who uses "AI and ML tools and techniques" for carrying out its activities shall be **solely responsible** for:

| Obligation | Scope |
|---|---|
| (a) Privacy, security and integrity of data | Investor data and stakeholder data processed through or by AI/ML tools |
| (b) AI outputs | All outputs derived from use of AI and ML tools and techniques — no caveat for third-party AI vendors |
| (c) Legal compliance | Compliance with all applicable laws in the context of AI/ML tool usage |

**Enforcement:** Board may take action under **Chapter V** of the Intermediaries Regulations for violations of Regulation 16C. Chapter V governs enquiry and action against intermediaries (suspension, cancellation, penalties).

### Definition of "AI and ML Tools and Techniques"

Defined broadly within the regulation to include **any application, software, or executable system** that uses artificial intelligence or machine learning techniques. No exclusion for general-purpose tools, third-party SaaS, or embedded AI functionality in market infrastructure.

### Mandatory Nature

"Shall be solely responsible" — unambiguously mandatory. Carve-outs: none expressed. The sole-responsibility framing explicitly precludes diffusion of liability across AI vendors or service providers.

### Significance of "Solely Responsible"

The word "solely" is operationally significant: it forecloses any liability-sharing argument between a SEBI-registered intermediary and its AI vendor. Whether an intermediary uses a proprietary model, a licensed third-party API (e.g., LLM), or embedded AI in its trading/compliance software, the intermediary bears full regulatory accountability for the output.

### Relationship to Predecessor Instruments

| Predecessor | Nature | Shift |
|---|---|---|
| SEBI_9 (Jan 2019) | Circular — AI/ML reporting obligation for MIIs | Advisory-level, reporting-only |
| SEBI_10 (May 2019) | Circular — AI/ML reporting for mutual funds | Advisory-level, reporting-only |
| SEBI_11 (2024–25) | Board Memo — AI responsibility assignment | Board-level resolution, pre-statutory |
| **SEBI_14 (Feb 2025)** | **Statutory regulation — binding Amendment** | **Full statutory force; sole responsibility; enforcement via Chapter V** |

SEBI_14 represents the completion of a six-year regulatory arc: from voluntary-disclosure circulars (2019) through board-resolution framing (2024) to binding statutory obligation (2025).

---

## Analytical Significance for PRIS Research

### For P3 — BFSI AI Governance / Regulatory Parallelism (JEIM)

SEBI_14 is the strongest single instrument for the **Regulatory Parallelism** thesis in the Indian BFSI corpus. It confirms that SEBI has now enacted a binding AI accountability obligation (sole responsibility for outputs + data integrity) without cross-referencing or coordinating with RBI's contemporaneous AI governance work (RBI_FREE_AI_2025, RBI_3). Both regulators are now imposing AI-specific accountability obligations on entities that are frequently dual-regulated (e.g., non-banking entities with SEBI and RBI registration). The absence of any reference to RBI's FREE-AI Committee or MeitY's IndiaAI framework in SEBI_14 is itself evidence of parallelism rather than convergence.

### For P4 — Doctrinal (IJLIT)

The sole-responsibility clause (Reg. 16C) is the first Indian financial regulation to resolve the **AI accountability gap** doctrinally — it does so by simple attribution (the regulated entity is solely responsible) rather than algorithmic auditing, explainability mandates, or model validation requirements. This is a distinct doctrinal approach from the EU AI Act (risk-tier obligations) and NIST (lifecycle process requirements). The minimalism of the provision — one regulation, three clauses, no technical standards — is itself analytically significant.

### For P1 — SLR (Regulation & Governance)

Provides the India-securities-sector data point in the global survey of binding AI regulations. Paired with RBI_FREE_AI_2025 (RBI) and MeitY_4 (DPDP Act), confirms that India's AI governance is now multi-regulator, sector-specific, and lacking a central coordination mechanism — a key SLR finding.

### For fsQCA — Regulatory Configurations for Trustworthy AI

SEBI_14 adds a configuration variable for the India case: **binding sector-specific AI accountability regulation enacted without coordination mechanism**. Supports the "parallelism without coherence" configurational pathway in the truth table.

### Coordination / Parallelism Pattern

**Instruments in scope of same BFSI AI governance space:** SEBI_14 ↔ [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] / [[07_Institutions/Corpus/RBI/RBI_3]]
**Pattern: Parallelism** — Two regulators (SEBI and RBI) have now each enacted AI-specific governance obligations for overlapping BFSI entities (dual-registered NBFCs, FPIs, MFs), through different instruments, with no explicit cross-reference or coordination. SEBI uses "solely responsible for outputs"; RBI's FREE-AI framework uses a different accountability architecture (model validation, Board-approved policy, RMCB). Neither instrument references the other. This is a textbook instance of [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]].

### Consulting Connection

Relevant to **AEGIS_OS** (runtime decision enforcement layer): Regulation 16C's sole-responsibility-for-AI-outputs clause creates a concrete compliance driver for pre-execution AI governance tooling — the regulated entity must be able to demonstrate control over outputs, which AEGIS_OS is designed to enable. Also relevant to **PrivacyWeave** (DPDP purpose enforcement): the data privacy/security obligation in Reg. 16C(a) creates a direct interface with DPDP Act 2023 compliance requirements.

---

## Connections

**Related corpus nodes:**
- [[07_Institutions/Corpus/SEBI/SEBI_9]] — AI/ML Reporting for MIIs (2019) — predecessor instrument, Cluster C09
- [[07_Institutions/Corpus/SEBI/SEBI_10]] — AI/ML Reporting for Mutual Funds (2019) — predecessor instrument
- [[07_Institutions/Corpus/SEBI/SEBI_11]] — AI Responsibility Assignment (2024–25) — direct antecedent Board memo
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — RBI FREE-AI Committee Report — parallelism counterpart
- [[07_Institutions/Corpus/RBI/RBI_3]] — RBI Draft Model Risk Credit Circular — domain overlap (AI output accountability)
- [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — DPDP Rules, 2025 — data privacy obligations interface (Reg. 16C(a))
- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — proposed coordination body, absence relevant

**Related concepts:**
- [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — primary instantiation: SEBI binding AI obligation enacted without RBI coordination
- [[05_Concepts/05_Concepts_Signature/Governance_Debt]] — compliance burden on dual-regulated entities holding both SEBI and RBI registration
- [[05_Concepts/05_Concepts_Standard/Accountability]] — sole-responsibility clause as accountability mechanism
- [[05_Concepts/05_Concepts_Standard/Transparency]] — not addressed in this instrument (no explainability or disclosure requirement)

**Related projects:**
- [[02_Projects/P3_BFSI_JEIM]]
- [[02_Projects/P4_Doctrinal_IJLIT]]
- [[02_Projects/P1_SLR_RG]]
- [[02_Projects/fsQCA_Thesis_Chapter]]

**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

**Related consulting:** AEGIS_OS (runtime governance), PrivacyWeave (DPDP interface)

---

## Coding Status

- **P3 NVivo:** Canonical corpus — add to SEBI sub-corpus; primary RUs are Reg. 16C(a)/(b)/(c) and sole-responsibility clause
- **Wiki intake status:** Pending

---

## Log

- 2026-06-18: Corpus node created. Batch 4 (Policy Dump intake). Cowork session.
