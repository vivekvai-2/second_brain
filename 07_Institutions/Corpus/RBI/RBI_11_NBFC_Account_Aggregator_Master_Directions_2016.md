---
type: Corpus Node
status: active
tags:
  - type/corpus-node
  - status/active
  - institution/rbi
  - paper/p2-primary
  - paper/p3
  - paper/p4
  - gate/open
  - engine/phd
---

# RBI_11 — Master Direction: NBFC – Account Aggregator (Reserve Bank) Directions, 2016

**Institution:** [[RBI]] | **Framework:** [[DEPA]] | **Added:** 2026-08-02 (DEPA sourcing pass)

---

## Document Identity

- **Title:** Master Direction – Non-Banking Financial Company – Account Aggregator (Reserve Bank) Directions, 2016
- **Issuing body:** Reserve Bank of India, Department of Non-Banking Regulation
- **Original reference:** Circular No. RBI/DNBR/2016-17/46; Master Direction DNBR.PD.009/03.10.119/2016-17
- **Original date:** 2 September 2016
- **Binding status:** **Binding** — licensing conditions for a regulated NBFC category
- **Current status:** Live consolidated Master Direction, amended nine times: 9 Nov 2017; 23 Feb 2018; 22 Nov 2019; 5 Oct 2021; 23 Nov 2022; 29 Dec 2022; 10 Nov 2023; 22 Feb 2024; **6 Sep 2024** (most recent)
- **Link:** https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=10598

⚠ **Citation hazard.** RBI hosts this as a single dynamically updated page; amendments are folded into the same URL and there is no separately published consolidated version. **Date-stamp every retrieval.** Any quotation must record the retrieval date or it is unverifiable at a later reading.

## Substantive Content

The Directions create the Account Aggregator as a licensed NBFC category whose sole permitted business is consent-brokered retrieval and presentation of a customer's financial information from Financial Information Providers to Financial Information Users. The defining constraint is **data-blindness**: the AA may move data it is not permitted to read, store or use. Paragraph 9.2 delegates technical specification to ReBIT (see [[07_Institutions/Corpus/RBI/RBI_12_ReBIT_AA_API_Specifications_2023]]).

**6 September 2024 amendment** — the most substantial:

- New Paragraph 1A permanently places NBFC-AAs in the **Base Layer** of RBI's Scale Based Regulation structure
- Mandates adoption of RBI's *Guidance Note on Operational Risk Management and Operational Resilience* (30 April 2024) — links this regime to [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]]
- Replaces the NBFC Ombudsman Scheme 2018 with the **Reserve Bank – Integrated Ombudsman Scheme, 2021** — this is the statutory tier of the four-tier AA grievance chain
- Requires at least one director with bank/NBFC experience
- Clarifies Risk Management Committee formation at Board or executive level
- Adds disclosure requirements under Annex VII of the NBFC Scale Based Regulation Directions, 2023

**5 October 2021 amendment:** Dividend Payout Ratio definition; FATF non-compliant jurisdiction investment restrictions with a 20% voting-power cap.

## Analytical Significance

**Sequencing.** These Directions **predate the DEPA framework document by four years**. The regulatory instrument came first; the architectural rationale was published afterwards by a different body. This inverts the ordinary policy-to-regulation sequence and is a third instance of the "institution before regulation" pattern already recorded for CSIRT-Power in [[Power_Grid_Critical_Infrastructure_Governance]] — with a stronger form here, since the regulation preceded not just the institution but the stated policy.

**No AI provision.** The Directions govern data movement and say nothing about automated decision-making by FIUs consuming that data. An AA can lawfully deliver a complete financial profile to an FIU that runs an unregulated credit model on it. The consent layer is governed; the inference layer is not. This is the precise seam where [[Records_Rules_Asymmetry]] and [[Governance_Debt]] operate, and it is directly usable in [[P3_BFSI_JEIM]]. **(Added 2026-08-02)** The doctrine that governs this seam elsewhere is now in the corpus: under CJEU *SCHUFA* ([[07_Institutions/Corpus/International/International_36_CJEU_SCHUFA_C634_21]]) a credit agency's probability value is itself regulated automated decision-making where a third party draws strongly on it. India has no equivalent — [[DPDP_Act_2023]] contains no ADM provision. The AA regime governs the movement of data and nothing governs the inference drawn from it, and that gap now has a named foreign doctrine to measure it against rather than being asserted in the abstract. See [[GDPR]].

**Ombudsman integration.** The 2024 amendment's substitution of the Integrated Ombudsman Scheme 2021 is what makes tier 3 of the AA redress chain statutory rather than contractual. Compare [[Contestability_Redress]]: this same statutory ombudsman infrastructure exists and has *not* been extended to AI-assisted decisions.

## Coding Notes (IG 2.0)

Strong candidate for ADICO extraction — a licensing instrument with clear Attributes (NBFC-AA), mostly mandatory Deontics, and enforceable Or-else via licence conditions. Contrast against [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]], whose recommendations lack any Or-else. Useful as a within-institution deontic control: same regulator, same period, binding on data-sharing and advisory on AI.

## Related Nodes

- [[06_Frameworks/DEPA]] — parent framework
- [[07_Institutions/Corpus/RBI/RBI_12_ReBIT_AA_API_Specifications_2023]] — the technical standard delegated under para 9.2
- [[07_Institutions/Corpus/Sahamati/Sahamati_1_SRO_Recognition_and_Grievance_Architecture_2026]] — the SRO layer above these Directions
- [[07_Institutions/Corpus/RBI/RBI_10_Storage_Payment_System_Data_2018]] — the other RBI data-governance instrument predating DPDP
- [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — statutory Consent Manager regime built on this model

## Linked Concepts

[[Contestability_Redress]] · [[Institutional_Coherence]] · [[Governance_Debt]] · [[Accountability]] · [[Records_Rules_Asymmetry]]

## Linked Domains

[[DPI_Governance]] · [[BFSI_Governance]] · [[Privacy_DataProtection]]

---

_Back to [[RBI]] | [[Corpus_Index_MOC]]_
