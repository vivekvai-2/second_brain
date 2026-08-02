---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/meity
---

# MeitY_8 — Digital Personal Data Protection Act, 2023

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023.md`
**Institution:** [[07_Institutions/MEITY]]
**Issuing body:** Parliament of India (Ministry of Law and Justice, Legislative Department, for the Gazette notification); administered by MeitY
**Document date:** Act No. 22 of 2023 — Presidential assent and Gazette notification 11 August 2023. Commencement (Section 1(2)) staggered via Notification G.S.R. 843(E), 13 November 2025.
**Pages:** Not independently paginated in this extraction; 44 sections across 9 chapters plus a penalty Schedule (per companion framework synthesis)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/DPI_Governance]] | [[03_Domains/Privacy_DataProtection]]

---

## Instrument Identity

**Full title:** The Digital Personal Data Protection Act, 2023 (Act No. 22 of 2023)
**Type:** Binding primary statute
**Target entities:** Data Fiduciaries and Data Processors processing digital personal data within India, and processing outside India connected to offering goods/services to Data Principals in India; the Data Protection Board of India as the constituted enforcement body
**Legal basis:** Enacted by Parliament; Presidential assent 11 August 2023
**Companion documents (constitutive instruments, not separately noded — folded in here per PRIS evidence-reuse threshold):**
- **Commencement Notification G.S.R. 843(E)** (MeitY, 13 November 2025, Gazette of India Extraordinary Part II Section 3(i)) — brought into force: s.1(2), s.2 (definitions), ss.18–26 (Data Protection Board establishment/composition/functions), s.35, ss.38–43, s.44(1)/(3) (RTI Act and TRAI Act consequential amendments), effective immediately on publication; s.6(9) and s.27(1)(d) (Consent Manager registration duty and Board's power to penalise Consent Manager breaches) effective 13 November 2026; all remaining substantive provisions (ss.3–5, 6(1)–(8)/(10), 7–17, 27 except (1)(d), 28–34, 36, 37, 44(2)) effective 13 May 2027.
- **DPB Establishment Notification G.S.R. 844(E)** (MeitY, 13 November 2025, under s.18(1)/(3) of the Act) — formally constitutes the Data Protection Board of India with effect from the date of Gazette publication; fixes the Board's head office in the National Capital Region. Signed by Ajit Kumar, Joint Secretary (F. No. AA-11038/1/2025-CL&ES).
- **DPDP Rules, 2025 (Final, G.S.R. 846(E), 13 November 2025)** — subordinate legislation under s.40; already coded as the canonical corpus node [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]. This node (MeitY_8) is retained specifically for the primary Act text and its two constitutive commencement/establishment notifications, which MeitY_4 does not separately extract.
- **Standing Committee 48th Report ("Citizens' Data Security and Privacy")** — pre-enactment legislative-history document; coded separately as [[07_Institutions/Corpus/Parliament/Parliament_1_Standing_Committee_48th_Report_2023]] since it examines the 2022 Bill draft, not the final Act, and originates from a distinct institution (Lok Sabha Committee, not MeitY).

**Primary source link:** https://www.meity.gov.in/static/uploads/2024/06/2bf1f0e9f04e6fb4f8fef35e82c42aa5.pdf (MeitY-hosted Act text) | https://www.meity.gov.in/content/digital-personal-data-protection-act-2023 (MeitY landing page)
**Commencement notification link:** https://www.meity.gov.in/static/uploads/2025/11/c56ceae6c383460ca69577428d36828b.pdf
**DPB establishment notification link:** https://www.meity.gov.in/static/uploads/2025/11/cc217843dc3bcb37b2b05bcc3b4e031f.pdf

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) — primary; feeds S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** High — primary statute, Gazette-verified, cross-confirmed against two independent primary-source notifications (commencement and Board establishment)
**AI explicit:** No — technology-neutral personal-data statute; AI-relevant only through downstream Rules (Rule 13(3) algorithmic-software due diligence, already coded in MeitY_4)
**Tier classification:** Tier B — general data-protection regime with indirect AI-governance relevance via constraining data inputs to AI training/deployment
**AI Governance Wiki relevance:** HIGH — this is the enabling statute for the entire DPDP regime; the Rules (MeitY_4) cannot be read without it

---

## Substantive Content

### Structure
44 sections across 9 chapters plus a penalty Schedule: I Preliminary; II Obligations of Data Fiduciary; III Rights and Duties of Data Principal; IV Special Provisions; V Data Protection Board of India; VI Powers, Functions and Procedure of the Board; VII Appeal and Alternate Dispute Resolution; VIII Penalties and Adjudication; IX Miscellaneous. (Full section-by-section obligation architecture — consent standard, Significant Data Fiduciary duties, cross-border transfer blacklist model, penalty Schedule — is already synthesised in the companion framework node [[06_Frameworks/DPDP_Act_2023]]; this Corpus Node records the instrument facts and the two constitutive notifications that operationalised it, which is the gap this intake closes.)

### Commencement architecture — three distinct instruments, easily conflated
A precise reading requires distinguishing three separate Gazette actions, all bearing dates in the same November 2025 window:
1. **G.S.R. 843(E)** — the Act's own s.1(2) commencement notification (which *sections* of the Act come into force, and when)
2. **G.S.R. 844(E)** — the DPB establishment notification (constitutes the Board itself, under s.18)
3. **G.S.R. 846(E)** — the DPDP Rules, 2025 (subordinate legislation under s.40, already coded in MeitY_4)

Treating these as one event risks misdating which specific obligation (statutory section vs. subordinate rule vs. institutional constitution) is actually live at any given point — a distinction the framework note's "staggered commencement" analysis depends on getting right.

### Data Protection Board of India — constitution
The Board is established with effect from the date of Gazette publication (13 November 2025), with its head office fixed in the National Capital Region. As of the most recent confirmed search (May 2026), Chairperson/Member appointments were still under a Search-cum-Selection process (per a MeitY Personnel-I recruitment notice dated 6 May 2026) — i.e., the Board exists as a legal entity before it is fully staffed, consistent with the framework node's "stand up the regulator before activating the regime" sequencing finding.

### Confirmed gap: no sectoral cross-referencing circular
No RBI, SEBI, or IRDAI circular explicitly invoking DPDP compliance obligations has been issued as of the most recent search (post-14 November 2025 Rules notification). Sectoral instruments (RBI IT Governance Master Direction, Digital Payment Security Controls 2024, Digital Lending Directions 2025; CERT-In Directions 2022) continue to operate in parallel to, rather than by cross-reference to, the DPDP Act. This is a **confirmed negative finding**, not a search gap — it strengthens rather than weakens the existing [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] argument: sectoral regulators are not coordinating with the central data-protection statute even after its institutional machinery went live.

### Items sourced but not independently verified — flagged, not intaken
- **"Explanatory Note on Draft Digital Personal Data Protection Rules, 2025"** (MeitY, referenced 3 January 2025) — direct PDF URL not independently confirmed; treat as pending verification before citing.
- **DPBI Chairperson/Member recruitment notice** (6 May 2026) — administrative proforma only; noted above for the staffing-timeline point but not separately coded as a corpus node (low standalone reuse value per PRIS ontology rule on evidence thresholds).
- **Draft DPDP Rules, 2025** (3 January 2025, G.S.R. 02(E)) — superseded by the final Rules already coded in MeitY_4; not separately noded.

---

## Analytical Significance for PRIS Research

### For P2 (DPI Governance, JSIS) and the Governance_Debt argument
The three-notification commencement structure (Act-section commencement, Board establishment, Rules notification — all dated within days of each other in November 2025, following a 27-month dormancy from August 2023 assent) is itself the clearest documentary evidence in the corpus of the "enacted but not operative" pattern the framework node already argues. This node supplies the primary-source citations (G.S.R. 843(E), G.S.R. 844(E)) that the framework synthesis previously asserted from secondary description.

### For Regulatory_Parallelism
The confirmed absence of any sectoral (RBI/SEBI/IRDAI) circular cross-referencing DPDP post-commencement is a documented **unpaired/non-coordinated** data point — sectoral regulators built their own algorithm/data-adjacent obligations (RBI_6, SEBI_9/10/11) during DPDP's dormant period and have not revisited or cross-referenced them now that DPDP's institutional machinery is live.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (subordinate Rules — canonical), [[07_Institutions/Corpus/Parliament/Parliament_1_Standing_Committee_48th_Report_2023]] (pre-enactment legislative history), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]], [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]] (parallelism comparators)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Governance_Debt]], [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (institution-before-obligation sequencing), [[05_Concepts/05_Concepts_Standard/Accountability]]
**Related frameworks:** [[06_Frameworks/DPDP_Act_2023]] (parent framework/synthesis node — this Corpus Node supplies its primary-source grounding)
**Related projects:** [[02_Projects/P2_DPI_JSIS]], [[02_Projects/P3_BFSI_JEIM]], [[08_Methods/fsQCA]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Screening corpus — high priority; closes a previously flagged gap (framework node had zero corpus-node grounding for the Act itself, only for its subordinate Rules)
- **Wiki intake status:** Pending — HIGH priority for S2 update

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Thin_Node_Perplexity_Prompts_2026-08-02]] DPDP prompt. Closes the "framework has 1 evidence link" gap flagged in the 2026-08-02 thin-node audit. Institutes the distinction between the Act's own commencement notification (G.S.R. 843(E)) and the Rules notification (G.S.R. 846(E), already in MeitY_4) — previously conflated risk noted and resolved here.
