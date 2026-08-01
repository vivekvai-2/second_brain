---
type: Corpus Node
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/sebi
  - theme/regulatory-sandbox
  - theme/fintech-experimentation
---

# SEBI_13 — Revised Framework for Regulatory Sandbox

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/SEBI/SEBI_13_Regulatory_Sandbox_Framework_2021.md`
**Institution:** [[07_Institutions/SEBI]]
**Issuing body:** Securities and Exchange Board of India, Information Technology Department
**Document date:** June 14, 2021 (SEBI/HO/ITD/ITD/CIR/P/2021/575)
**Pages:** 24
**Domain:** [[03_Domains/BFSI_Governance]] | [[03_Domains/AI_Governance]]

---

## Instrument Identity

**Full title:** Revised Framework for Regulatory Sandbox
**Type:** Circular (with Standard Operating Procedure annexures)
**Target entities:** All Stock Exchanges, Clearing Corporations, Depositories, and SEBI-registered intermediaries (entities registered under Section 12, SEBI Act 1992) seeking to test FinTech solutions
**Legal basis:** Section 11(1), SEBI Act 1992; Section 19, Depositories Act 1996. Underpinned by SEBI Regulatory Sandbox (Amendment) Regulations, 2020, which enables grant of relaxations/exemptions via limited certificates of registration.
**Companion documents:** Supersedes/revises original Regulatory Sandbox framework, circular SEBI/HO/MRD-1/CIR/P/2020/95 (June 5, 2020) — eligibility criteria revised "to enhance the reach."

---

## Analytical Classification

**Wiki section:** S6 (Implementation & Governance Artifacts — regulatory experimentation mechanisms)
**Jurisdiction:** India
**Confidence:** High — primary regulatory instrument, circular status
**AI explicit:** Partial — not an AI-specific framework; however, Annexure-1 application form (Stage-I) explicitly requires applicants to disclose "Usage of Artificial Intelligence and Machine Learning, if any" (item 3.2.b) as part of the technical solution summary, making this the regulatory gateway through which AI/ML-based securities-market FinTech solutions are sandboxed in India
**Tier classification:** Tier C — AI-adjacent governance (technology-neutral experimentation mechanism with an explicit AI/ML disclosure trigger)
**AI Governance Wiki relevance:** MEDIUM — provides the only formal "controlled experimentation" pathway in the Indian securities-market regulatory architecture through which AI/ML-driven FinTech tools can be tested on live users under regulatory supervision; directly relevant to any discussion of regulatory sandboxes as an AI-governance tool (a recurring theme in S6 implementation artifacts)

---

## Substantive Content

### Objective and Structure
The Regulatory Sandbox grants SEBI-regulated entities facilities and flexibilities to experiment with FinTech solutions in a live environment, on a limited set of real users, for a limited time frame. Testing proceeds in **two stages**:
- **Stage-I**: limited, identified users (cap set case-by-case by SEBI), each providing positive consent acknowledging risks.
- **Stage-II**: larger identified user set, available only after **minimum 90 days / three (3) months** in Stage-I (the document uses both figures — ⚠ VERIFY BEFORE PUBLISHING: para 4 states "minimum 90 days" while para 15 states "minimum three (3) months"; these are likely intended as equivalent but should be reconciled before citation).
- **Total sandbox duration** (Stage-I + Stage-II combined): maximum **12 months**, extendable on request and SEBI approval.

### Eligibility Criteria
Stage-I eligibility (6 criteria) requires: SEBI Section-12 registration (principal applicant bears sole responsibility even in partnerships); genuine need to test on real users (test-environment data alone insufficient) and genuine need for regulatory relaxation; alignment with the sandbox objective (new innovation or process improvement/inclusion); identifiable user/market benefits; testing readiness (developed test plans with success criteria); and a risk-management strategy with safeguards.

Stage-II eligibility (6 criteria) additionally requires: demonstrated adequate progress, documented review of Stage-I risks and mitigation steps, user feedback summary (including adverse feedback), and a proposed exit strategy for post-testing deployment.

### Mandatory vs. Relaxable Requirements (Annexure-3)
**Never relaxed**: fit-and-proper criteria; KYC principles; AML/CFT compliance; confidentiality of customer/user information; risk checks (price/order-value checks); handling of user moneys/assets beyond existing regulations.
**May be relaxed**: net worth, financial soundness, and track record of applicant; registration fees; technology risk management and outsourcing guidelines.

This mandatory/relaxable split is itself a governance-design artifact: SEBI pre-commits to an "investor-protection floor" (KYC/AML/confidentiality/risk-checks) that no sandbox relaxation can breach, while operational/financial-threshold requirements remain negotiable — a useful template for any "innovation sandbox with hard governance floors" design discussion.

### Process, Fees and Oversight
- Application via Annexure-1 (Stage-I) / Annexure-2 (Stage-II), signed by CEO or authorised officer/compliance officer, submitted to SEBI's IT Department (physical or via regulatorysandbox@sebi.gov.in).
- SEBI reviews and communicates suitability **preferably within 30 working days**.
- On approval, applicant pays a **token fee of ₹10,000** for a limited certificate of registration valid up to **12 months**.
- SEBI may consult its Committee on Financial and Regulatory Technologies (CFRT) or Regulatory Sandbox Sub-committee.
- **Monthly reporting** required during testing (KPIs, incident/fraud reports, remedial actions); **final report within 30 calendar days** of Stage-II completion; records retained for **3 years** post-exit.

### User Protections
Sandbox users retain the same protection rights as live-market participants except where specifically modified by the consent form and granted relaxations. Applicants must carry **liability/indemnity insurance** (coverage from start of testing to **3 months post-exit**), publish a grievance-redressal mechanism, and allow users SCORES access. Users retain an unconditional **right to revoke consent**.

### Exit, Withdrawal and Revocation
- **Exit strategy** (successful testing): user notification, broader-deployment plan, migration handling, and statement of regulatory changes needed for live launch.
- **Withdrawal strategy** (unsuccessful/discontinued testing or SEBI revocation): user notification; settlement/transfer of user positions and **refund of dues within 15 days** of withdrawal initiation.
- **Revocation grounds** (12 listed) include failure of risk mitigants, false/misleading disclosures, legal contraventions (India or abroad), reputational loss, liquidation, cybersecurity compromise, and non-cooperation with SEBI directions. Revocation triggers a notice-and-response process culminating in a speaking order, though SEBI may act immediately "in the interest of... the securities market" where satisfied of necessity.
- Violations facilitating KYC circumvention, privacy breaches, fraud/mis-selling, AML breaches, market-integrity risk, or IP theft can trigger **separate enforcement action** (debarment, monetary penalty, prosecution) beyond sandbox revocation — per the Annexure-1 enclosure undertaking.

---

## Analytical Significance for PRIS Research

### For AI Governance Wiki (S6) / P3 (BFSI AI Governance Regulatory Parallelism, JEIM)
This is SEBI's pre-existing, general-purpose "controlled experimentation" instrument — issued in 2021, before the current wave of AI-specific governance circulars ([[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_11]]). It establishes that India's securities regulator already had a sandbox mechanism explicitly capable of admitting AI/ML-based solutions (via the Annexure-1 disclosure item) nearly four years before SEBI's dedicated AI/ML reporting and board-accountability circulars. This is evidence of a **sequencing pattern**: general-purpose technology sandboxes preceding AI-specific substantive obligations — relevant to P3's narrative on how Indian BFSI regulators have evolved from technology-neutral to AI-explicit instruments over time. It also offers a possible institutional template for [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]: a "regulatory sandbox" model that other regulators (RBI, IRDAI) could adopt for AI-specific live-testing, reducing [[05_Concepts/05_Concepts_Signature/Governance_Debt]] associated with parallel, untested AI compliance obligations.

### Coordination / Parallelism Pattern
No direct corpus overlap identified — this is the first SEBI sandbox-mechanism node in the corpus. Distinguish from [[07_Institutions/Corpus/SEBI/SEBI_9]]/[[07_Institutions/Corpus/SEBI/SEBI_10]] (AI/ML reporting obligations for *already-deployed* systems) — SEBI_13 governs *pre-deployment experimentation*, a different point in the AI system lifecycle. Together these form a lifecycle pair worth noting in any S6 lifecycle-governance synthesis.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/SEBI/SEBI_9]] (AI/ML Reporting for MIIs — post-deployment counterpart), [[07_Institutions/Corpus/SEBI/SEBI_10]] (AI/ML Reporting for Mutual Funds), [[07_Institutions/Corpus/SEBI/SEBI_11]] (Board Memo on AI Responsibility Assignment)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (sandbox as a coordination/innovation-governance mechanism), [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (mandatory vs. relaxable requirements as a governance-debt design choice), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]], [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (sandbox as potential future venue for agentic AI live-testing)
**Related frameworks:** None yet in corpus
**Related projects:** [[02_Projects/P3_BFSI_JEIM]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** None identified directly — potentially relevant to AEGIS_OS if a future engagement involves SEBI-regulated entity AI pilots requiring sandbox routes.

---

## Coding Status

- **P3 NVivo:** Screening corpus — useful as lifecycle/sequencing context rather than direct AI-obligation evidence
- **Wiki intake status:** Pending

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session.
