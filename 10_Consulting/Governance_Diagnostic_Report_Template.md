---
type: Consulting Template
tags:
  - type/consulting-template
  - status/active
  - engine/consulting
  - engine/knowledge-product
  - content/checklist
---

# Governance Diagnostic Report — Template

**Type:** Consulting Deliverable Template
**Status:** Active
**Created:** 2026-07-15
**Use for:** Paid diagnostic engagements — e.g. the "BFSI AI Governance Diagnostic Report" ([[BFSI_AI_Governance_Handbook]]) and "Governance Debt Assessment" ([[Regulatory_Complexity_Handbook]]) already named as consulting deliverables in the vault.
**Anchors on:** [[Regulatory_Parallelism]], [[Governance_Debt]], [[Institutional_Coherence]], [[Deontic_Bifurcation]], [[Assurance_Reuse_Gap]]

---

## Purpose

A structured diagnostic instrument for assessing how much of a client's compliance burden is Governance Debt rather than substantive risk management — and where their governance architecture is coherent versus fragmented. Every section below is a fill-in-the-blank scaffold built from constructs already validated against the 18-instrument RBI/SEBI/CERT-In/MeitY/IRDAI corpus in [[Cross_Institutional_Mandate_Comparison]]. Do not re-derive the diagnostic logic per engagement — instantiate it against the client's specific regulatory stack.

---

## 1. Regulatory Architecture Map

List every regulator, statute, and binding/aspirational instrument the client is subject to. Model on the Instrument Inventory table in [[Cross_Institutional_Mandate_Comparison]] §3.

| Regulator | Instrument | Legal Force (Binding/Aspirational/Draft) | Regulated Function | Enforcement Status |
|---|---|---|---|---|
| | | | | |

**Output:** a one-page regulatory footprint the client has usually never seen assembled in one place. This alone is often the first value delivered.

---

## 2. Parallelism Diagnostic

Run every pair of overlapping instruments identified in Section 1 through this seven-dimension checklist (source: [[Regulatory_Parallelism]] operationalisation logic).

| Diagnostic Dimension | Instrument A | Instrument B | Parallelism Confirmed? |
|---|---|---|---|
| 1. Independent issuance? | | | |
| 2. Functionally equivalent capabilities governed? | | | |
| 3. Explicit cross-reference between instruments? | | | |
| 4. Can a single control satisfy both? | | | |
| 5. Separate evidence/audit trails required? | | | |
| 6. Is substantive protection multiplied (not just paperwork)? | | | |
| 7. Is governance work multiplied? | | | |

**Classification rule:** Parallelism is confirmed when dimensions 1, 2, 5, 7 = Yes and dimensions 3, 4, 6 = No. Repeat per instrument pair; log every confirmed pair.

---

## 3. Governance Debt Quantification

Classify each confirmed Parallelism instance against the variant taxonomy documented in [[Governance_Debt]]:

| Variant | Definition (one line) | Present in this client? | Estimated Compliance Effort Impact |
|---|---|---|---|
| Unresolved-duplication | Two live instruments cover the same obligation with no reconciliation | | |
| Regulatory-uncertainty | An unfinalised draft the client must nonetheless track and prepare for | | |
| Evidentiary | Compliance expectation circulating in practitioner literature, unconfirmed against primary source | | |
| Aspiration-without-instrument | A named strategic commitment with no operative regulatory instrument behind it | | |
| Standards-transposition | An international standard exists; India-specific transposition is missing or lagging | | |
| Assurance Reuse Gap | An audit/DPIA/attestation produced for Regulator A cannot discharge the equivalent obligation to Regulator B | | |

**Output:** a scored Governance Debt profile — count of instances, weighted by compliance-effort impact (Low/Moderate/High per [[Governance_Debt]] rationale conventions).

---

## 4. Institutional Coherence Scorecard

Rate the client's governance architecture — not the regulators' — against the five dimensions from [[Cross_Institutional_Mandate_Comparison]] §9. This section is architecturally reversed from the regulator-level assessment: it asks whether the *client's own* governance function has built compensating coherence where the regulatory environment has none.

| Dimension | Rating (Low/Moderate/High) | Evidence |
|---|---|---|
| Clear internal role allocation across compliance/risk/legal/tech | | |
| Consistent internal terminology for AI/ML/algorithmic systems | | |
| Interoperable internal reporting (single incident triggers one internal process, not three) | | |
| Shared assurance / reusable audit artefacts across regulatory obligations | | |
| Coordinated escalation and enforcement response | | |

---

## 5. Recommendations (Three Levels)

Mirror the recommendation architecture used in [[Cross_Institutional_Mandate_Comparison]] §12 — diagnostics are more credible when they show awareness of what the client cannot fix (institutional level) versus what they can (enterprise level).

### Institutional level (context only — not actionable by client)
- Note any structural coordination gaps the client is exposed to but cannot remedy (e.g. absence of a cross-regulator coordination body).

### Enterprise level (actionable — this is the paid deliverable's core value)
1. Unified Controls Framework opportunities — where one control can be engineered to discharge multiple regulators' obligations simultaneously.
2. Common Evidence Repository opportunities — where audit/assurance artefacts can be centralised for reuse.
3. Runtime enforcement opportunities — where a technical control (cf. AEGIS OS / PrivacyWeave pattern in [[Inbound_Pipeline_Index]]) could convert passive paper compliance into active enforcement.

### Board level
- A one-slide summary translating Sections 2–4 into a board-legible risk statement, formatted for direct reuse in [[Executive_Board_Briefing_Deck_Template]].

---

## Engagement Notes

- **Typical scope:** single sector, single client entity, 3–6 week diagnostic window.
- **Pricing anchor:** position as a fixed-fee diagnostic, not time-and-materials — the checklist structure is what makes fixed-fee pricing defensible.
- **Upsell path:** diagnostic → workshop ([[Workshop_Masterclass_Curriculum_Template]]) → advisory retainer.
- **Confidentiality:** client-specific instances of Sections 2–4 stay in the client deliverable only. Do not log client names in vault concept "Instances in Corpus" sections — those are reserved for published/public regulatory corpus evidence.

---

## Linked Vault Nodes

**Signature Concepts:** [[Regulatory_Parallelism]], [[Governance_Debt]], [[Institutional_Coherence]], [[Deontic_Bifurcation]], [[Assurance_Reuse_Gap]]

**Knowledge Products:** [[BFSI_AI_Governance_Handbook]], [[Regulatory_Complexity_Handbook]], [[Cross_Institutional_Mandate_Comparison]]

**Domains:** [[BFSI_Governance]], [[AI_Governance]]

**Consulting:** [[Consulting_Deliverable_Templates_Index]], [[Inbound_Pipeline_Index]]

---

_Back to [[Consulting_Deliverable_Templates_Index]]_
