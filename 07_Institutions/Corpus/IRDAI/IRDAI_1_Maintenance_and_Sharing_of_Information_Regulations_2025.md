---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/irdai
---

# IRDAI_1 — IRDAI (Maintenance of Information by the Regulated Entities and Sharing of Information by the Authority) Regulations, 2025 [Secondary Commentary]

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025.md`
**Institution:** [[07_Institutions/IRDAI]] ⚠ VERIFY BEFORE PUBLISHING — confirm `07_Institutions/IRDAI.md` institution file exists; this is the **first IRDAI corpus node**, so an IRDAI institution file and folder may need to be created as part of this batch's indexing pass.
**Issuing body:** Document is a third-party/consultancy explainer ("India's Insurance Industry's Data Governance Mandate — Latest IRDAI Compliance Requirement") describing a regulation issued by the Insurance Regulatory and Development Authority of India
**Document date:** Source regulation cited as "IRDAI (Maintenance of Information by the Regulated Entities and Sharing of Information by the Authority) Regulations, 2025" (gazette notification referenced via IRDAI document portal, documentId=6540652); the commentary document itself cites access dates of January 14–15, 2025. ⚠ VERIFY BEFORE PUBLISHING — exact gazette notification date/number for the underlying Regulations is NOT stated in this document; only a portal URL is given.
**Pages:** 9 (secondary commentary/whitepaper, not the primary gazette text)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]] | [[03_Domains/DPI_Governance]]

---

## Instrument Identity

**Full title (of underlying regulation, as cited):** Insurance Regulatory and Development Authority of India (Maintenance of Information by the Regulated Entities and Sharing of Information by the Authority) Regulations, 2025
**Type:** ⚠ This corpus node is built from a **secondary commentary/consultancy whitepaper**, not the primary regulatory text. The underlying instrument is subordinate legislation/regulations issued by IRDAI under the Insurance Act, 1938 (Section 20 of the Insurance Act, 1938 is cited as the basis for public-interest information sharing).
**Target entities:** All IRDAI-regulated entities — insurance companies, brokers, agents, and other regulated intermediaries
**Legal basis:** Insurance Act, 1938 (Section 20 cited for public-use information sharing); broader regulatory authority of IRDAI under the IRDA Act, 1999 (not explicitly cited in source document — ⚠ VERIFY)
**Companion documents:** Source document cross-references India's DPDP Act, 2023 and DPDP Rules, 2025 ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]]) as a compliance baseline for regulated entities acting as "significant data fiduciaries." Primary gazette notification available at IRDAI document portal (documentId=6540652) — **not retrieved**; this node is based solely on the secondary commentary.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** LOW-MEDIUM — ⚠ VERIFY BEFORE PUBLISHING: this document is a **secondary/derivative commentary** (consultancy-style explainer with citations to IBEF, JSTOR, Deloitte for sector-context framing), not the primary regulatory text. All specific regulatory content (Regulation 6 "compass of purpose," data localisation mandate, Board-approved data governance architecture requirement, penalty provisions) is reported **at second hand** and should be cross-verified against the primary gazette notification (IRDAI documentId=6540652) before being cited in any publication-track output.
**AI explicit:** NO — the regulation itself, as described, is a data governance/information-maintenance framework with no explicit AI/ML provisions. The source document's Section 1 (sector-context narrative) mentions AI/ML and blockchain adoption in underwriting, claims processing, and fraud detection as a **market trend observation**, not a regulatory requirement — do not conflate this contextual framing with the regulation's actual scope.
**Tier classification:** Tier C — AI-adjacent governance (general data governance/information-sharing framework for the insurance sector, with AI/ML referenced only as sectoral context, not as a regulated activity)
**AI Governance Wiki relevance:** MEDIUM — establishes IRDAI as a participant in India's cross-regulator data-governance/localisation pattern (alongside DPDP Rules 2025 and RBI data-localisation provisions); also the first corpus entry for IRDAI, opening a previously empty institutional track relevant to P3/P4 BFSI comparative work, though substantive AI-governance content is currently thin and second-hand.

---

## Substantive Content

### Reported Purpose and Scope (per secondary source)
The Regulations are described as establishing a comprehensive framework for (a) maintenance of information by regulated entities (insurers, brokers, agents) and (b) sharing of information by IRDAI with stakeholders. Five stated aims (as paraphrased in the source): standardising collection/storage/sharing of data to enhance transparency; ensuring accurate/timely records accessible to IRDAI and the public for oversight; facilitating data sharing with regulators/policymakers/public for analytics-driven decision-making; improving accountability/efficiency in insurer reporting; and encouraging risk management/compliance aligned with international standards.

### "Regulation 6 — Compass of Purpose" (as cited)
The source attributes to "Regulation 6" a purpose-specification provision: information may be sought for legal/regulatory functions by Indian regulators, public authorities (government, judiciary, law enforcement), and international supervisory bodies, and additionally for public use under Section 20 of the Insurance Act, 1938 or other applicable laws. ⚠ VERIFY BEFORE PUBLISHING — the specific numbering ("Regulation 6") and exact wording should be confirmed against the primary gazette text before use in any ADICO/Institutional Grammar coding exercise, as secondary paraphrase is unreliable for clause-level analysis.

### Data Governance Architecture (as described)
- **Board-approved data governance framework** required for regulated entities — structurally parallel to DPDP Rules 2025's emphasis on Board-approved policies for Significant Data Fiduciaries ([[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]], Rule 13) and RBI's Board-approved IT outsourcing/cloud policies ([[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]]).
- **Data localisation**: source states "all data should be stored and maintained in Indian data centres to promote data localisation, protecting data sovereignty, and increasing cybersecurity." ⚠ VERIFY BEFORE PUBLISHING — this is reported as a **general/blanket localisation requirement** for insurance-sector data, which would represent a **stricter** localisation posture than DPDP Rules 2025's targeted, government-specified SDF localisation (Rule 13(4)) or DPDP's conditions-based cross-border transfer regime (Rule 15). Given the secondary nature of this source, the "all data" framing must be checked against the primary regulation before any cross-instrument localisation comparison is published — it is plausible the primary text contains narrower scoping (e.g., specific data categories) that the commentary has generalised.
- **Data classification, data lineage, and data mapping** are referenced as components of the maintenance framework, with records to be mapped by domain/department/function with defined access and responsibilities (dashboard-based).

### Reporting and Information-Sharing Obligations (as described)
- **Regular reporting** (monthly/quarterly/annual) on financial status, claims, underwriting, and solvency, via IRDAI-defined forms/templates.
- **Data sharing for regulatory oversight**, with manner/timelines to be specified by IRDAI; used for solvency, corporate governance, and operational-standards monitoring.
- **Aggregated/anonymised data sharing** with policymakers, industry participants, and research bodies for sector-development purposes.
- **Public access**: non-confidential data (financial health, claim settlement ratios, customer satisfaction metrics) may be made publicly available by IRDAI.
- **Inter-regulator sharing**: IRDAI may share information with SEBI, RBI, and other regulators where there is overlapping concern (e.g., listed insurers) — an explicit cross-regulator data-sharing channel, relevant to [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] discussions of inter-regulator coordination (or its absence) in India's financial-sector governance.

### Compliance, Penalties, and Monitoring (as described)
- IRDAI empowered to impose **penalties or corrective action** for non-compliance, ranging from fines to suspension of operations or licence revocation, "depending on the severity of non-compliance." ⚠ VERIFY BEFORE PUBLISHING — no specific penalty quanta, tiers, or procedural (notice-and-hearing) safeguards are described in the source; this is a generic enforcement-powers statement that should not be cited as a specific penalty schedule.
- IRDAI to conduct **continuous oversight** and periodically evaluate/update guidelines for emerging challenges/technological advancements.

### Departmental Impact Mapping (Section 3 of source)
The source provides a department-by-department compliance-impact map (Operations, Underwriting, Investments, Risk Management, Compliance, Customer Service, Marketing, Sales) — each requiring enhanced data accuracy, audit trails, reporting systems, and staff training. This is **consultancy-framing content** (practitioner advisory in tone) rather than regulatory text, but it is useful as an illustration of how Indian compliance advisors are operationalising data-governance regulations for insurer clients — potentially relevant to P3/P4's practitioner-translation analysis of how abstract regulatory text becomes departmental compliance programmes.

---

## Analytical Significance for PRIS Research

### For P3/P4 (BFSI AI Governance Regulatory Parallelism)
This is the **first IRDAI entry** in the corpus, opening the third major BFSI-regulator track alongside RBI and SEBI. Even allowing for the secondary-source caveats, the reported structure — Board-approved data governance policy, data localisation, structured reporting to the regulator, inter-regulator data-sharing channels, and a generic enforcement-powers clause — is **structurally congruent** with both DPDP Rules 2025 (MeitY) and RBI's outsourcing/cloud directions (RBI_6), reinforcing the [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] thesis: India's BFSI regulators (RBI, SEBI, IRDAI) and its general data-protection regulator (DPDP Board) are independently converging on a common "Board-approved governance policy + localisation + structured regulatory reporting + enforcement powers" template, each via its own sectoral instrument. IRDAI_1 should be treated as a **provisional/low-confidence data point** for this pattern pending primary-source verification — but the pattern itself (if confirmed) would extend the parallelism finding across all three major financial-sector regulators plus the horizontal data-protection regulator.

### For Institutional Coherence / Governance Capacity
The explicit inter-regulator data-sharing provision (IRDAI ↔ SEBI/RBI for overlapping concerns, e.g., listed insurers) is a rare **affirmative coordination mechanism** in the corpus — most other instruments are silent on inter-regulator data flows. If confirmed against the primary text, this could be a positive [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] data point (an instance of regulators building bridges rather than operating in silos), in contrast to the largely uncoordinated "parallelism" pattern seen elsewhere (e.g., MeitY_4's algorithmic-due-diligence provisions vis-à-vis SEBI/RBI equivalents, which show no cross-referencing).

### Methodological Note — Secondary Source Limitation
⚠ VERIFY BEFORE PUBLISHING (corpus-wide methodological flag): This is the **first node in the corpus built from a secondary/consultancy commentary rather than a primary legal/regulatory text**. If the primary IRDAI (Maintenance of Information...) Regulations, 2025 gazette notification can be obtained (IRDAI documentId=6540652, per source footnote), a future session should retrieve it and either supersede or substantially supplement this node — particularly for any claims intended for ADICO/Institutional Grammar coding, fsQCA configurational variables, or direct quotation in publication-track outputs. Until then, this node should be tagged as **"secondary source — pending primary verification"** in any P3/P4 evidence table.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (Board-approved governance policy, SDF obligations, cross-border transfer conditions), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (Board-approved IT/cloud policy, India data-storage requirement, RBI audit-access rights).
**Pattern:** Convergent template across MeitY/RBI/IRDAI — Board-approved data/IT governance policy + India-based data storage/localisation + structured regulatory reporting + regulator enforcement/audit powers — each instrument independent, sector-specific, with IRDAI's instrument additionally featuring an explicit (if generic) inter-regulator data-sharing clause. Strengthens the cross-regulator [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] evidence base, subject to the primary-source verification caveat above.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (data governance/localisation/Board-policy parallel; explicitly cross-referenced by the source document itself re: SDF compliance), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (data localisation/Board-policy/audit-access parallel)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (cross-regulator data-governance template convergence), [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (explicit inter-regulator data-sharing provision — tentative positive instance), [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]] (public-disclosure provisions for non-confidential data), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** None yet in `06_Frameworks` — IRDAI is a new institutional track; no framework synthesis yet
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] (new BFSI regulator track), [[02_Projects/P4...]] (BFSI doctrinal — insurance-sector data governance)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S2/S5 — pending primary-source upgrade)
**Related consulting:** **PrivacyWeave** — the IRDAI regulation's reported alignment with DPDP SDF obligations (explicitly cross-referenced in the source) may be relevant to PrivacyWeave engagements involving insurance-sector clients; flag as provisional pending primary verification.

---

## Coding Status

- **P3 NVivo:** Provisional inclusion only — tag as "secondary source, pending primary verification" before any quotation-level coding
- **Wiki intake status:** Pending — LOW-MEDIUM priority until primary gazette text obtained; opens new IRDAI institutional section in S2

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session. First IRDAI corpus entry — new institution folder `07_Institutions/Corpus/IRDAI/` created. Flagged throughout as based on secondary/consultancy commentary; primary IRDAI gazette notification (documentId=6540652) not retrieved this session.
