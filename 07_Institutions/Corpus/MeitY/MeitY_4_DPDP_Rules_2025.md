---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/meity
---

# MeitY_4 — Digital Personal Data Protection Rules, 2025

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025.md`
**Institution:** [[07_Institutions/MEITY]]
**Issuing body:** Ministry of Electronics and Information Technology, Government of India
**Document date:** November 13, 2025 (G.S.R. 846(E), Gazette of India Extraordinary, Part II, Section 3(i), No. 760); draft published January 3, 2025 (G.S.R. 02(E)); corrigendum issued December 10, 2025 (G.S.R. 892(E), minor textual corrections only)
**Pages:** 41 (Gazette notification, Hindi + English, 23 rules + 7 Schedules)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/DPI_Governance]]

---

## Instrument Identity

**Full title:** Digital Personal Data Protection Rules, 2025
**Type:** Subordinate legislation (Rules) under Section 40(1) and (2) of the Digital Personal Data Protection Act, 2023 (22 of 2023)
**Target entities:** All Data Fiduciaries, Data Processors, Consent Managers, and "Significant Data Fiduciaries" processing digital personal data in India, plus the Data Protection Board of India (institutional rules for its constitution and functioning)
**Legal basis:** Section 40, sub-sections (1) and (2), Digital Personal Data Protection Act, 2023
**Companion documents:** Operationalises [[06_Frameworks/DPDP_Act_2023]] (framework node, confirmed extant) under s.40. The Act itself, plus its commencement (G.S.R. 843(E)) and DPB-establishment (G.S.R. 844(E)) notifications, are now separately coded at [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] (2026-08-02 intake — closes the gap this flag identified).

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) — primary; also feeds S5 (Data, Privacy & Security) and S4 (Agentic AI Governance, via Significant Data Fiduciary algorithmic-audit provisions)
**Jurisdiction:** India
**Confidence:** High — primary subordinate legislation, gazetted
**AI explicit:** Partial — not an AI-specific instrument, but Rule 13(3) (Significant Data Fiduciary obligation to verify that "algorithmic software" used for hosting/processing personal data does not pose a risk to Data Principal rights) is a direct, explicit AI/algorithmic-governance hook within India's general data protection framework
**Tier classification:** Tier B — technology-neutral data protection regime with explicit algorithmic-governance application for Significant Data Fiduciaries
**AI Governance Wiki relevance:** HIGH — DPDP Rules 2025 is the operational backbone of India's data protection regime and a foundational reference for any AI governance discussion involving personal data processing, consent architecture, children's data, cross-border transfer, or algorithmic accountability in India

---

## Substantive Content

### Commencement — Staggered, Multi-Tier (⚠ VERIFY BEFORE PUBLISHING — critical for currency)
The Rules do **not** come into force uniformly:
- **Rules 1, 2, 17–21** (short title/definitions; Board constitution, Chairperson/Member appointment, salary, meeting procedure, digital-office functioning, staffing) — in force from **date of gazette publication (November 13, 2025)**.
- **Rule 4** (Consent Manager registration) — in force **one year** after publication, i.e., **November 13, 2026**.
- **Rules 3, 5–16, 22, 23** (notice requirements, government processing standards, security safeguards, breach notification, retention/erasure, children's data, Significant Data Fiduciary obligations, Data Principal rights, cross-border transfer, research exemption, Appellate Tribunal, information-calling powers) — in force **eighteen months** after publication, i.e., **May 13, 2027**.
⚠ As of the current session date (2026-06-15), the substantive operational obligations (breach notification, security safeguards, children's consent, SDF obligations) are **not yet in force** — only the institutional/Board-constitution provisions are live. Any practitioner-facing commentary must distinguish "rules notified" from "rules in force."

### Notice and Consent Architecture (Rule 3, Rules 10–11)
- Notice to Data Principals must be **standalone/independently understandable**, in clear and plain language, and must itemise: the specific personal data categories, the specified purpose(s), and the goods/services/uses enabled — plus a direct communication link for withdrawal of consent (with **ease of withdrawal comparable to ease of giving consent**), exercise of rights, and complaints to the Board.
- **Children's data (Rule 10)**: Data Fiduciaries must obtain **verifiable parental consent** before processing a child's personal data, with due diligence to confirm the consenting adult's identity/age via (a) reliable details already held, or (b) voluntarily provided identity/age details or a virtual token issued by an "authorised entity" (including Digital Locker service providers). Four detailed illustrations (Cases 1–4) cover registered vs. unregistered parent scenarios.
- **Persons with disability with lawful guardians (Rule 11)**: Data Fiduciaries must verify the guardian's appointment by a court, designated authority (under RPwD Act 2016 §15), or local-level committee (under National Trust Act 1999 §13).
- **Children's data exemptions (Rule 12, Fourth Schedule)**: Sections 9(1) and 9(3) of the Act (parental consent / no tracking-advertising-to-children) **do not apply** to: clinical establishments/mental health establishments/healthcare professionals (health-service processing only); allied healthcare professionals; educational institutions (educational activity/safety tracking); crèche/childcare providers (safety tracking); transport providers for such institutions (location tracking during transit). Also exempted by *purpose*: statutory functions in a child's interest, subsidy/benefit provision, email-only account creation, real-time location for safety, ad-blocking for child welfare, and age-verification processing itself.

### Consent Managers (Rule 4, First Schedule)
- Registration requires: Indian incorporation, **net worth ≥ ₹2 crore**, sound financials/management, "fit and proper" directors/KMP, MoA/AoA provisions locking in Part B obligations (amendable only with Board approval), and independent certification of platform conformity to Board-published data protection standards.
- Consent Manager obligations (Part B, 13 items): enable direct or routed consent flows between Data Principal and onboarded Data Fiduciaries (with worked examples involving banks B1/B2); ensure shared data is unreadable to the Consent Manager itself; maintain consent/notice/sharing records for **≥7 years**; provide machine-readable record access; act in a **fiduciary capacity**; avoid conflicts of interest with Data Fiduciaries (including via director/KMP financial interests); publish ownership/shareholding (>2% threshold) transparency; maintain audit mechanisms; no sub-contracting of obligations; control of the registered company cannot be transferred without Board approval.

**Architectural lineage (added 2026-08-02, DEPA sourcing pass).** Rule 4 and the First Schedule are not a novel design — they are [[06_Frameworks/DEPA]]'s consent-manager architecture in statutory form. The data-blindness requirement, the fiduciary-capacity duty, the conflict-of-interest bar, and the machine-readable record-access obligation all restate constraints already operating on RBI-licensed Account Aggregators since 2016 (see [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]]) and on ABDM's HIE-CM in health. MeitY did not design a consent manager; it generalised one that two sectoral regulators had already been running.

**⚠ Rule 4 has an unstaffed registrar (added 2026-08-02).** Rule 4 commences **13 November 2026** and Consent Manager registration is with the **Data Protection Board**. As of 31 July 2026 the Board has **no appointed Chairperson and no appointed Members** — applications were invited 6 May 2026 and the Search-cum-Selection Committees remain at the stage of soliciting names. **An unstaffed Board cannot register anyone.** This supplies a mechanism by which the DPDP consent-manager regime may remain inoperative past its own commencement date, and the same dependency governs every substantive obligation commencing 13 May 2027, all of which are Board-enforced. See [[DPB]] and [[07_Institutions/Corpus/DPB/DPB_1_Establishment_and_Vacancy_2025_2026]].

**Chiasmus for P2/P4.** The DPDP consent-manager regime is **statutorily enacted but not operative** — Rule 4 commences 13 November 2026 and registration has not opened. The AA consent-manager regime is **operative but never statutorily enacted as such** — it runs on 2016 NBFC licensing plus a NITI Aayog document its own authors labelled a draft. India currently has two consent-manager regimes, each missing precisely the half the other has. Recorded in full at [[06_Frameworks/DEPA]].

### State Processing for Subsidies/Benefits (Rule 5, Second Schedule)
Processing by the State/instrumentalities for providing subsidies, benefits, services, certificates, licences or permits (under law, policy, or using public funds — each separately defined, including reference to Consolidated Fund of India/State and local-authority funds) must follow Second Schedule standards: lawfulness, purpose limitation, data minimisation, accuracy, retention limits, reasonable security safeguards, Data Principal intimation (with contact info and rights-exercise link), and accountability of the determining entity.

### Security Safeguards and Breach Notification (Rules 6–7)
- **Minimum security safeguards**: encryption/obfuscation/masking/virtual tokens; access controls to computer resources; logging/monitoring/review for unauthorised-access detection; continuity measures (e.g., backups); **minimum 1-year retention of logs and personal data** for breach investigation (unless other law requires longer); contractual security provisions with Data Processors; appropriate technical/organisational measures.
- **Breach notification to Data Principals**: "without delay" — description (nature/extent/timing), consequences, mitigation measures, protective steps the principal can take, and DPO/responsible-person contact.
- **Breach notification to the Board**: immediate description (nature/extent/timing/location/likely impact), followed within **72 hours** (or Board-extended period, on written request) by: updated/detailed information, broad facts on causes/circumstances, mitigation measures, findings on the breaching party, remedial measures, and a report on Data Principal intimations. ⚠ VERIFY BEFORE PUBLISHING — the 72-hour figure is a notification-timeline claim per Section 8 flagging rules; confirm against final Act/Rules text if cited in any deadline-sensitive output (note also this Rule is not yet in force per commencement analysis above).

### Retention and Erasure (Rule 8, Third Schedule, examples)
- General rule: erase personal data once the specified purpose is no longer being served (subject to legal retention requirements), with **≥48-hour prior notice** to the Data Principal before erasure.
- **Class-specific 3-year retention exceptions** (Third Schedule) — triggered by **inactivity** (3 years from last Data Principal contact for the specified purpose/rights exercise, or from DPDP Rules 2025 commencement, whichever is later) for:
  - E-commerce entities with **≥2 crore registered users in India**
  - Online gaming intermediaries with **≥50 lakh registered users in India**
  - Social media intermediaries with **≥2 crore registered users in India**
  Exceptions to erasure: account-access and virtual-token/wallet-access functions remain.
- General processing-log retention: **minimum 1 year** from date of processing (Seventh Schedule purposes), independent of the above.

### Significant Data Fiduciary (SDF) Obligations (Rule 13)
- Annual (12-monthly) **Data Protection Impact Assessment (DPIA) and audit**, with significant-observations report to the Board.
- Due diligence that **algorithmic software** used for hosting/display/uploading/modification/publishing/transmission/storage/updating/sharing of personal data does not pose a risk to Data Principal rights — **the corpus's clearest explicit linkage between India's general data protection regime and algorithmic/AI accountability**.
- Data localisation: SDFs must ensure that Central-Government-specified personal data (on recommendation of a MeitY-led committee) and associated traffic data **are not transferred outside India** — a targeted, committee-driven localisation mechanism (not a blanket data-localisation mandate). ⚠ VERIFY BEFORE PUBLISHING — distinguish this targeted SDF localisation power from broader "data localisation" claims sometimes made about DPDP; the general cross-border transfer rule (Rule 15) is permissive subject to government-specified conditions, not a blanket ban.

### Cross-Border Data Transfer (Rule 15)
Personal data **may be transferred outside India**, subject to Central Government-specified requirements (general or special order) regarding data made available to foreign States or persons/entities/agencies under their control. This is a **conditions-based, not prohibition-based**, framework — notable contrast to stricter data-localisation regimes (e.g., RBI payment-data localisation). ⚠ VERIFY BEFORE PUBLISHING if comparing to RBI/other sectoral localisation rules — avoid "blanket localisation" framing for DPDP generally.

### Research/Archiving/Statistical Exemption (Rule 16)
DPDP Act provisions do not apply to personal data processing necessary for research, archiving, or statistical purposes, provided Second Schedule standards (lawfulness, purpose limitation, minimisation, accuracy, retention limits, security, accountability) are met.

### Data Protection Board of India — Institutional Architecture (Rules 17–23, Fifth–Seventh Schedules)
- **Chairperson/Members**: appointed via Search-cum-Selection Committees (Cabinet Secretary-chaired for Chairperson; MeitY Secretary-chaired for other Members); salary **₹4,50,000/month (Chairperson)**, **₹4,00,000/month (Members)**, consolidated, no house/car — pay-matrix Level 17/15 equivalence for allowances; no pension/gratuity for Board service.
- **Functioning**: Board operates as a **"digital office"** — proceedings may be conducted via techno-legal measures without requiring physical presence, while retaining summons/oath powers. One-third quorum; Chairperson casting vote; conflict-of-interest recusal; emergency-action provisions (7-day retrospective ratification); **inquiries under Section 27 to be completed within 6 months**, extendable by up to 3 months at a time with recorded reasons.
- **Appellate Tribunal**: digital filing; fee parity with TRAI Act 1997 appeals (waivable by Tribunal Chairperson); not bound by CPC 1908, guided by natural justice; also functions as digital office.
- **Information-calling powers (Rule 23, Seventh Schedule)**: Central Government may require Data Fiduciaries/intermediaries to furnish information for (i) sovereignty/integrity/state-security purposes (via designated officer), (ii) performance of statutory functions/disclosure obligations (via "person authorised under applicable law"), and (iii) SDF-notification assessments (via MeitY Secretary-designated officer). Non-disclosure to affected Data Principals can be mandated where disclosure would prejudice sovereignty/security.

---

## Analytical Significance for PRIS Research

### For P2 (DPI Governance, JSIS)
DPDP Rules 2025 is the central operational instrument for P2's regulatory-architecture analysis of Indian digital governance. The staggered commencement schedule (institutional provisions live now; substantive obligations — breach notification, children's consent, SDF audits — not until May 2027) is itself a finding: it demonstrates a **sequenced institutional-capacity-building approach** — the Board is constituted and operational 18 months before the obligations it will enforce become binding, suggesting a deliberate "stand up the regulator before activating the regime" sequencing. This is directly relevant to P2's analysis of DPI governance institution-building sequencing (cf. UIDAI, NPCI precedents).

### For AI Governance Wiki (S2, S4, S5)
Rule 13(3)'s algorithmic-software due-diligence requirement for Significant Data Fiduciaries is the **first explicit "algorithm-aware" obligation** in this corpus's MeitY/data-protection track — it sits alongside SEBI's AI/ML reporting circulars ([[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]]) and RBI's cloud-governance provisions ([[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]]) as evidence of a **convergent pattern**: India's sectoral and cross-sectoral regulators are each independently inserting algorithm/AI-specific due-diligence clauses into otherwise technology-neutral instruments, without a unifying cross-regulator AI statute. This is strong evidence for [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] at the cross-regulator level — SEBI (securities AI/ML reporting), RBI (cloud/algorithmic outsourcing risk), and MeitY (SDF algorithmic audit) are each building parallel, non-coordinated algorithm-governance hooks into sector-specific or general frameworks.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]].
**Pattern:** **Parallelism** — each instrument independently creates an algorithm/AI-accountability obligation (SEBI: AI/ML reporting for MIIs/MFs; RBI: algorithmic risk in cloud-outsourced IT for AIFIs; MeitY: SDF algorithmic-software due diligence for personal-data processing) within its own jurisdictional silo, with no cross-referencing or harmonisation mechanism visible across these instruments. This is a candidate finding for P3's regulatory-parallelism argument: **the absence of an explicit AI law in India has produced convergent-but-uncoordinated algorithmic-governance insertions across sectoral regulators**, each anchored to that regulator's pre-existing technology-risk framework (IT outsourcing, AI/ML system reporting, data protection).

### Governance Debt
The DPDP Rules' Consent Manager framework, retention-schedule complexity (general rule + three Schedule-specific inactivity-based regimes + Seventh Schedule log-retention), and SDF dual obligations (DPIA/audit **and** algorithmic due diligence **and** data-localisation compliance) represent a significant compliance-architecture build for any entity that is simultaneously an SDF under DPDP **and** subject to SEBI/RBI/IRDAI algorithm-governance obligations — a direct [[05_Concepts/05_Concepts_Signature/Governance_Debt]] instance: a large BFSI entity could face DPDP SDF algorithmic-audit obligations, RBI IT-outsourcing/cloud-governance audits, and SEBI AI/ML reporting — three overlapping but non-harmonised audit/assessment cycles.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] (cloud/algorithmic governance parallel), [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]] (AI/ML reporting parallels), [[07_Institutions/Corpus/SEBI/SEBI_11]] (AI accountability assignment parallel)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (cross-regulator algorithmic-governance convergence), [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (overlapping SDF/AIFI/MII audit cycles), [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] (Board-first sequencing as a coherence-building design), [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (Board institution-building), [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (SDF algorithmic due diligence)
**Related frameworks:** [[06_Frameworks/DPDP_Act_2023]] (confirmed extant — this Rules node operationalises it under s.40; see also [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] for the Act's own corpus node)
**Related projects:** [[02_Projects/P2_DPI_JSIS]] (primary), [[02_Projects/P3_BFSI_JEIM]] (SDF/BFSI overlap), [[08_Methods/fsQCA]] (DPDP as a configurational element in comparative regulatory analysis)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** **PrivacyWeave** — directly relevant; PrivacyWeave's DPDP purpose-limitation enforcement positioning aligns closely with Rule 3 (notice/consent architecture), Rule 8 (retention/erasure), and the Consent Manager framework (Rule 4) — this node should be flagged to the PrivacyWeave engagement team as a primary reference for Rules 3, 4, and 8 specifically.

---

## Coding Status

- **P3 NVivo:** Screening corpus — high priority for canonical inclusion; Rule 13(3) algorithmic due-diligence clause is a key cross-regulator parallelism data point
- **Wiki intake status:** Pending — HIGH priority for S2 update

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session.
- 2026-07-31: **Duplicate resolved.** MeitY_1 (created earlier, Batch 1, 2026-06-14) cited the identical Gazette notification (G.S.R. 846(E), 13 November 2025) — same instrument. This node (MeitY_4) is retained as canonical, being substantially more granularly extracted (full rule-by-rule breakdown, exact figures, existing Regulatory_Parallelism/Governance_Debt cross-links to SEBI_9/10/11 and RBI_6). MeitY_1 additionally covered the December 2025 corrigendum, which has been folded into this node's record below. MeitY_1 converted to a redirect stub; all vault references repointed here.

**Corrigendum note (folded in from MeitY_1):** A corrigendum to the notified Rules was issued 10 December 2025 (G.S.R. 892(E)) — minor typographical corrections only, to pages 24, 29, 32, 34, 38 of the Rules. No substantive change.
- 2026-08-02: Companion-documents flag resolved. The Act's own corpus node ([[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]]) and the parent framework node ([[06_Frameworks/DPDP_Act_2023]]) are both confirmed extant; cross-links updated accordingly.
