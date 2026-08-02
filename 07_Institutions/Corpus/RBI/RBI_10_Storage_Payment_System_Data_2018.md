---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/rbi
---

# RBI_10 — Storage of Payment System Data (RBI/2017-18/153, DPSS.CO.OD.No.2785/06.08.005/2017-2018)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_10_Storage_Payment_System_Data_2018.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India, Department of Payment and Settlement Systems
**Document date:** 6 April 2018
**Pages:** Not independently paginated in this extraction (single-page circular plus FAQ)
**Domain:** [[03_Domains/Privacy_DataProtection]] | [[03_Domains/DPI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Storage of Payment System Data
**Type:** RBI Circular (binding directive)
**Target entities:** All authorised/approved Payment System Providers (per RBI FAQ clarification)
**Legal basis:** Section 10(2) read with Section 18 of the Payment and Settlement Systems Act, 2007
**Companion documents:** RBI FAQ clarification on Storage of Payment System Data (Common Man portal, dated 25 June 2019 per page metadata, post-circular)

**Primary source link:** https://www.rbi.org.in/Scripts/NotificationUser.aspx?Id=11244&Mode=0
**FAQ link:** https://www.rbi.org.in/commonman/english/scripts/FAQs.aspx?Id=2995

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** High — primary RBI notification, directly retrieved
**AI explicit:** No — general payment-data localisation directive, not AI-specific; relevant to AI governance only as a data-input constraint on AI-based credit/fraud/payment analytics
**Tier classification:** Tier B — technology-neutral data-localisation mandate with downstream relevance to AI/analytics systems built on payment data
**AI Governance Wiki relevance:** MEDIUM-HIGH — this is India's **earliest and strictest** data-localisation instrument in the corpus, predating DPDP by five years, and the clearest available illustration of the "sectoral regulator moved first, horizontal statute moved later" sequencing pattern

---

## Substantive Content

### Core mandate — full, not conditional, localisation
Unlike the DPDP Act's Rule 15 (permissive by default, restrictable only by future government notification — see [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]), this 2018 RBI circular mandates that the **entire data relating to payment systems operated by them, including end-to-end transaction details, be stored only in India** — a blanket, not conditions-based, localisation requirement. Compliance deadline was six months from issue (15 October 2018); System Audit Report certifying compliance was due to RBI by 31 December 2018.

### Scope confirmed via FAQ
The RBI's own FAQ clarification confirms the circular applies to all authorised/approved Payment System Providers — a broad sweep across the payments ecosystem (banks, NBFCs, card networks, wallets, UPI-linked intermediaries).

### Confirmed gap: no cross-reference to DPDP
Consistent with the finding already documented in [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] (no sectoral regulator circular cross-references DPDP compliance obligations), this 2018 circular and the 2023/2025 DPDP framework remain **parallel, non-cross-referencing regimes**. Notably, this is the reverse-direction case: the *sectoral* instrument predates and does not anticipate the *horizontal* statute (the opposite chronology to SEBI_9/10/RBI_6 discussed in MeitY_4's parallelism analysis, which were issued *during* DPDP's dormant period). This 2018 circular is the earliest-dated localisation instrument in the entire PRIS corpus.

---

## Analytical Significance for PRIS Research

### For P2 (DPI Governance) and Regulatory_Parallelism
This is the **strictest** localisation regime documented in the corpus — full mandatory in-India storage, with no conditions-based carve-out — a sharp structural contrast to DPDP's Rule 15 permissive-by-default model (see [[06_Frameworks/DPDP_Act_2023]]'s "Cross-Border Transfer: Comparative Regulatory Design" synthesis). This gives PRIS a genuine **intra-India comparative pair**: RBI's blanket localisation (2018, payments) vs. DPDP's conditions-based transfer regime (2023/2025, general personal data) — a cleaner within-jurisdiction contrast than the existing DPDP-vs-GDPR comparison, since both instruments here are Indian and the variation is purely regulator-driven rather than jurisdiction-driven.

### For Governance_Debt
An entity that is both a Payment System Provider (this circular) and a DPDP Significant Data Fiduciary (MeitY_8/MeitY_4) faces two non-harmonised, differently-calibrated data-residency regimes for overlapping data categories (payment transaction data is also personal data) — a direct, citable instance of the overlapping-audit-cycle Governance_Debt pattern already documented for BFSI entities.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (Rule 15 cross-border transfer contrast), [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] (parallel-regime confirmation)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]], [[05_Concepts/05_Concepts_Signature/Governance_Debt]]
**Related frameworks:** [[06_Frameworks/DPDP_Act_2023]] (intra-India localisation-model comparator)
**Related projects:** [[02_Projects/P2_DPI_JSIS]], [[02_Projects/P3_BFSI_JEIM]], [[08_Methods/fsQCA]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Screening corpus — high value as an intra-India localisation-model comparator
- **Wiki intake status:** Pending — Normal-High priority for S2/S5 update

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Thin_Node_Perplexity_Prompts_2026-08-02]] Privacy_DataProtection prompt.
