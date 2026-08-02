---
type: Corpus Node
status: active
tags:
  - type/corpus-node
  - status/active
  - institution/rbi
  - paper/p2-primary
  - paper/p4
  - gate/open
  - engine/phd
---

# RBI_12 — ReBIT NBFC-AA API Specifications v2.0.0 and Adoption Strategy (2023)

**Institution:** [[RBI]] (via ReBIT, wholly-owned RBI subsidiary) | **Framework:** [[DEPA]] | **Added:** 2026-08-02 (DEPA sourcing pass)

Consolidated node — two instruments issued the same day, governing the same regime, per the PRIS evidence-reuse threshold.

---

## Document Identity

**(a) NBFC-Account Aggregator (AA) API Specification, Version 2.0.0**

- **Issuing body:** Reserve Bank Information Technology Private Limited (ReBIT), under RBI mandate per Master Direction para 9.2
- **Date:** 9 August 2023 (v2.0.0); supersedes v1.1 of 8 November 2019
- **Binding status:** Technical standard mandatory for ecosystem participants by delegation from a binding Master Direction — **binding in effect, delegated in form**
- **Link (canonical):** https://api.rebit.org.in/
- **Link (full text, Sahamati-hosted):** https://sahamati.org.in/wp-content/uploads/2025/10/2-API_Specifications_v2.0.0.pdf

**(b) NBFC-AA API Specification Adoption Strategy, Version 1.0.0**

- **Issuing body:** ReBIT
- **Date:** 9 August 2023
- **Link:** https://specifications.rebit.org.in/artefacts/NBFC-AA_API_Specification_Adoption_Strategy.pdf

## Substantive Content

**(a)** Specifies six functional flow categories across the AA / FIP / FIU role triad: account discovery and linking, consent flow, consent handle management, FI data flow, notification flow, and monitoring flow.

**(b)** The analytically important document. It establishes ReBIT's formal **API Governance Process** — change request intake → ReBIT analysis → stakeholder discussion → **RBI concurrence** → versioning → publication — and imposes compliance-tracking obligations on regulated entities: a **Plan of Action within 30 days** of a major version release, and **Adoption Progress Reports every 30 days** until the prior version is decommissioned.

## Analytical Significance

**Standard-setting as delegated regulation.** RBI does not specify the AA technical architecture itself; it licenses the entity type and delegates specification to a wholly-owned subsidiary, retaining a concurrence gate. The result is an instrument that is formally technical and substantively regulatory. For [[Deontic_Bifurcation]] this is a distinct architecture from the ones already recorded there: not mandatory-core-plus-advisory-annexure within one document, but **binding force acquired by delegation across documents** — the specification carries no deontic of its own and inherits enforceability from the Master Direction above it. Recommend coding as a third bifurcation type alongside designed and emergent.

**The 30-day reporting cadence is an assurance mechanism, not merely an implementation schedule.** Adoption Progress Reports every 30 days until decommission give the regulator continuous visibility of migration state across the ecosystem. Nothing comparable exists for any Indian AI instrument — [[Assurance_Reuse_Gap]] and [[Evidentiary_Governance]] both take this as a positive control: India has built continuous-assurance reporting where it chose to.

**Direct contrast for [[Governance_Debt]].** A data-format API specification in India carries versioned change control, a regulator concurrence gate, mandatory migration plans and 30-day progress reporting. AI model governance in the same sector carries a Committee report with no operative amendment ([[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]]). The asymmetry is not one of regulatory capability.

## Verification Notes

⚠ The v2.0.0 full text was retrieved via a **Sahamati-hosted** copy rather than ReBIT's own portal. Sahamati is now an RBI-recognised SRO, so the hosting is credible, but confirm against `api.rebit.org.in` before quoting the specification text in publication-track output.

## Related Nodes

- [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] — the delegating instrument (para 9.2)
- [[06_Frameworks/DEPA]] — parent framework
- [[07_Institutions/Corpus/Sahamati/Sahamati_1_SRO_Recognition_and_Grievance_Architecture_2026]] — SRO now holds delegated technical-standard authority alongside ReBIT; the division of labour between them is **not yet documented** and is an open question

## Linked Concepts

[[Assurance_Reuse_Gap]] · [[Evidentiary_Governance]] · [[Deontic_Bifurcation]] · [[Governance_Debt]] · [[Governance_Capacity]]

## Linked Domains

[[DPI_Governance]] · [[BFSI_Governance]]

---

_Back to [[RBI]] | [[Corpus_Index_MOC]]_
