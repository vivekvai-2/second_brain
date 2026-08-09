---
type: Corpus Node
node-id: CEA_3
institution: CEA
date: 2026-07-31
status: active
last_updated: 2026-08-09
wiki-section: S2
tier: A
ai-explicit: false
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/cea
  - institution/csirt-power
  - tier/A
  - batch/ad-hoc-20260809
  - concept/Evidentiary_Governance
  - concept/Retention_Horizon_Divergence
  - concept/Regulatory_Parallelism
  - concept/Governance_Debt
  - concept/Institutional_Coherence
  - concept/Assurance_Reuse_Gap
  - concept/Governance_Capacity
---

# CEA_3 — Central Electricity Authority (Cyber Security in Power Sector) Regulations, 2026

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026.md`
**Institution:** [[07_Institutions/CEA]]
**Issuing body:** Central Electricity Authority, Ministry of Power (Cyber Security Division)
**Document date:** Notified **31 July 2026**; Gazette of India, Extraordinary, Part III—Section 4, No. 484 (CG-DL-E-05082026-275218)
**Pages:** 38 Gazette pages (bilingual); 17 regulations across 10 chapters plus two Schedules
**Domain:** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

---

## Instrument Identity

**Full title:** Central Electricity Authority (Cyber Security in Power Sector) Regulations, 2026
**Type:** Binding subordinate regulation, gazetted
**Reference:** F. No. CEA-HY-91-19/8/2024-Cyber Security Division; signed Sharvan Kumar, Secretary
**Legal basis:** Sub-section (1) of section 177 read with clause (c) of section 73, Electricity Act, 2003 (36 of 2003)
**Commencement:** **1 April 2027.** Provided that regulations **5(9), 5(24), 5(33), 5(39), 6(2) and 6(7)** come into force on dates to be specified by the Authority through separate orders **with prior approval of the Central Government** — a staggered-commencement design isolating the six most cost-bearing obligations (24×7 Information Security Division; ISO 27001/TCC certification; mandatory personnel cyber-security courses; trusted-source IT procurement; OT perimeter security devices; trusted-source OT procurement).
**Procedural history:** Draft advertised in six newspaper dailies per s.177(3) r/w rule 3(2), Electricity (Procedure for Previous Publication) Rules, 2005; draft and notices made public **7 October 2025**; objections and suggestions considered. **MeitY concurrence recorded on the face of the instrument** for making these regulations in respect of cyber security for the power sector.
**Supersedes/relates to:** Notified successor to [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]] (draft, superseded by this notification); formalises into binding regulation the regime foreshadowed by [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]]

**Scope (reg 2):**
- All entities owning, operating or managing **Operational Technology** infrastructure associated with the interconnected power system, **and** their IT infrastructure physically or logically connected to such OT — existing and upcoming.
- **50 MW threshold** for generating companies, captive generating plants and organisations with Energy Storage Systems. Entities below 50 MW are *encouraged* (not required) to implement CERT-In's "15 Elemental Cyber Defense Controls for Micro, Small and Medium Enterprises."
- Power exchanges and OTC platforms — **except** regulations 6, 11 and 12.
- **Vendors** bound directly by regulations 11 and 12.
- "Entity" (reg 3(1)(w)) expressly includes gencos, captive plants, ESS organisations, transmission licensees, distribution licensees, NLDC, RLDCs, SLDCs, power exchanges and OTC platforms.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) — Critical Infrastructure / Power Sector
**Jurisdiction:** India
**Confidence:** High — full Gazette text, primary source
**AI explicit:** **No — zero AI provisions. See S5.1; this is the node's principal analytical contribution.**
**Tier classification:** **Tier A** — binding, gazetted, primary regulatory instrument (upgrade from CEA_2's Tier C draft status, as that node anticipated)
**AI Governance Wiki relevance:** **HIGH** — not for AI content, of which there is none, but because it is the corpus's cleanest instance of a mature regulator legislating comprehensively over a technology estate on which production ML is already running, with actual notice, and declining to address it.

---

## Substantive Content

### S3.1 Structural overview

| Chapter | Content | Regulations |
|---|---|---|
| I | Preliminary — short title, commencement, scope, 40 definitions | 1–3 |
| II | **Computer Security Incident Response Team – Power (CSIRT-Power)** — constitution, 14 enumerated functions | 4 |
| III | General cyber security requirements — 42 sub-clauses | 5 |
| IV | Additional requirements for OT-related entities — 9 sub-clauses | 6 |
| V | Functions of CISO and Information Security Division | 7 |
| VI | Cyber Security Policy — 33 mandated components | 8 |
| VII | Cyber Crisis Management Plan; entity responsibilities | 9–10 |
| VIII | **Cyber security requirements for vendors** | 11–12 |
| IX | Cyber security audit; CISO responsibilities | 13–14 |
| X | Self-audit; enforcement referral; power to relax | 15–17 |
| — | First Schedule (12 mandated retained document classes); Second Schedule (8 criteria for software updates requiring prior audit) | — |

### S3.2 CSIRT-Power — institutional architecture (Chapter II)

Defined at reg 3(1)(g) as "an organisation established by the Ministry of Power **as an extended arm of Indian Computer Emergency Response Team (CERT-In)**" for coordinating, reporting and responding to cyber security incidents in the power sector.

Reg 4(1) makes it the sector's **coordinating agency** for incident reporting and response and its **nodal agency** for analysis, prediction and prevention. Reg 4(1)(c) empowers it to collect from any entity: network architecture, asset details, logs, cyber forensic records, forensic images, policies and procedures, in the form and manner it specifies — with a proviso that sensitive data collected be protected, used only for cyber security purposes by designated government agencies, and **not disclosed to any third party without explicit communication to the concerned entity**.

Fourteen functions (reg 4(2)) include creating SOPs, security policies, sub-sector-specific benchmarks and controls in consultation with CERT-In, NCIIPC, sub-sectoral CSIRTs and Electricity Regulatory Commissions; vetting; and establishing **central and regional cyber security coordination forums** (reg 4(2)(m)). Reg 4(3) binds both entities *and vendors* to CSIRT-Power's directions. Reg 4(4) empowers the Authority to designate **sub-sectoral CSIRTs** for generation, transmission, distribution, grid operation and any other sub-sector.

### S3.3 CISO regime (regs 5(1)–(9), 7)

| Requirement | Provision |
|---|---|
| Designation | Regular employee, senior management level; **Alternate CISO** also required; both posts shall not be vacant simultaneously (5(2)) |
| Reporting line | Reports to **head of the entity**; where an entity (e.g. an SLDC) is not independent but part of a holding/parent company, it shall have a **separate CISO** reporting to the head of that holding/parent company (5(4)) |
| Tenure | Minimum **three years** (5(5)) |
| Ring-fencing | Role "ring fenced to the tasks of cyber security related matters only" (5(6)) |
| Public disclosure | CISO and Alternate CISO contact details in the **public domain**, updated, communicated to CSIRT-Power and all internal/external stakeholders (5(7)) |
| Training | Minimum **five man-days** cyber security training per financial year (5(8)) |
| Eligibility | **Citizen and resident of India**; engineering or equivalent degree from a recognised institute; **minimum fifteen years** experience in power sector or IT (7(1)) |

**Information Security Division (reg 5(9)):** dedicated, headed by the CISO, **within India**, operational **round the clock**; sufficient staffing; staff must hold valid certificates of domain-specific cyber security courses; five man-days annual power-sector cyber training; **minimum three-year tenure** for deployed staff. *Commencement deferred to a separate order.*

### S3.4 Incident reporting — the M1 pattern in a third sector

**Reg 7(3)(a):** cyber security incidents reported within **six hours** to **both CSIRT-Power and CERT-In**. Where an incident is concluded to be **cyber sabotage in critical systems**, reporting within **twenty-four hours**.

"Cyber sabotage" is separately defined at reg 3(1)(t) as "deliberate action to disrupt, damage or destroy the information systems, networks or data processed therein for malicious purpose." Note the deontic inversion: the *more severe* category carries the *longer* clock, presumably because the sabotage conclusion requires analysis the six-hour window cannot accommodate.

### S3.5 Evidentiary and retention architecture (regs 8(33), 7(3)(h)–(k); First Schedule)

The instrument specifies **seven distinct retention horizons in a single text** — the densest retention specification in the Indian corpus:

| Horizon | Record class | Provision |
|---|---|---|
| **Not older than one month** | Backup data of all critical systems; at least last two working backups available | 8(18), 8(33) |
| **180 days** | Logs of all ICT systems; logs of OT–IT interconnection; forensic records | 8(33)(h) |
| **365 days** | Logs associated with an incident, **including 180 days prior and 180 days post**, retained at least 365 days from occurrence | 8(33)(i) |
| **1 year** | Risk assessment, physical record of approval, and logs for each remote access to critical systems; risk assessment and approval for OT remote operation | 8(33)(b), (d) |
| **3 years** | Cyber security audit reports; self-audit reports | 8(33)(e), (g) |
| **4 years** | Certification audit reports | 8(33)(f) |
| **Life of asset** | FAT and SAT reports including cyber security requirement testing | 8(33)(c) |

**First Schedule** (via reg 7(3)(i)) places twelve document classes in the CISO's custody: Cyber Security Policy and its listed documents/procedures; Cyber Crisis Management Plan; Data Retention Policy and everything under it; ISO/IEC 27001 or Technical Criteria Certificate; asset register for cyber assets and critical systems; Cyber Risk Assessment and Mitigation Plan; Incident Response and Recovery Plan; Cyber Security Incident Reporting register; **Bill of Materials**; Business Continuity Plan; remote operation procedure; remote access procedure.

### S3.6 Assurance architecture — three audit cycles in one instrument

| Cycle | Frequency | Rotation rule |
|---|---|---|
| **Cyber security audit** (reg 13) | At least once per financial year, minimum 9 / maximum 15 months between consecutive audits (5(22)) | **No three consecutive audits by the same auditing agency or personnel** (5(22)); auditor must be CERT-In empanelled or MoP-designated (3(1)(p)) |
| **Certification audit** — ISO/IEC 27001 **or** Technical Criteria Certificate covering all critical systems (5(24)) | Per certification cycle | **No four consecutive audits by the same agency or personnel** (5(24)) |
| **Self-audit** (reg 15) | Every financial year | Entity may designate a board or senior-management member as responsible; non-compliances to be closed before the next year's self-audit |

Audit timelines (reg 13(3)): report within **six weeks** of commencement; **critical and high-risk** vulnerabilities addressed within **one month**; **medium and low** within **three months**; compensatory controls deployed until audit clearance. Closure report within **six months** of commencement (reg 14(1)).

**Escalation (regs 14, 15):** the **CISO – Ministry of Power** may demand any entity's audit closure report or compliance report at any time, seek written clarification, and — with prior Authority approval and prior notice — appoint a **third-party auditor at the entity's cost**. Where third-party findings vary from the closure report, the CISO-MoP may take further action.

### S3.7 Sovereignty and localisation

| Provision | Requirement |
|---|---|
| 5(19) | Sensitive information and data — **including cloud-hosted and historical** — stored encrypted, secured, and **resides within India only** |
| 6(3) | Control and operation of power system elements and exchange of information including real-time data over a dedicated channel isolated from the internet, **confined to national boundaries only**; cross-border entities may transmit only via dedicated separate communication system and **unidirectional gateway**, continuously monitored |
| 6(4) | Remote operation, if necessary, **within India**, prior approval of head or board, dedicated channel isolated from internet |
| 8(27) | Reference time source for OT systems shall be **terrestrial or India-specific satellite based and independent of the internet** |
| 7(1) | CISO and Alternate CISO shall be **citizens as well as residents of India** |
| 5(39), 6(7) | IT and OT equipment and services procured from **trusted sources** per Central Government orders (*both deferred to separate orders*) |
| 12(1) | For prosumer DERs, **vendor** must ensure applications, monitoring/control servers, real-time and historical data reside **exclusively within India** |

### S3.8 IT/OT separation (reg 6)

Reg 6(1) mandates **physical isolation** of OT from the internet *and* from IT systems. Where isolation from IT is not possible for business reasons, interconnection may be permitted with hardened logical separation, risk assessment, and approval of head or board — continuously monitored, with approvals and logs retained per the data retention policy. Reg 6(6) additionally requires the OT **communication system** to be isolated from the IT communication system. Reg 6(8) requires the OT environment to be segmented into **trust levels** by criticality, security requirements and risk assessment. Reg 8(28) requires identified IT↔OT data to flow through a separate channel and **unidirectional gateway**.

### S3.9 Vendor obligations — direct binding (Chapter VIII)

Reg 11 binds vendors to: provide documented and tested restoration procedures and recovery plans; ensure digitally signed or validated security patches for the **contract period or useful life, whichever is later**; provide integration documentation including third-party component patching; disclose **end of support / end of life** for software, hardware and systems including third-party-sourced items; provide a **Bill of Materials per CERT-In guidelines** covering all components including firmware in critical systems; **harden** hardware and software before supply; and establish a formal structured vulnerability-reporting process, furnishing vulnerabilities to **CSIRT-Power** through their disclosure programme.

Reg 12 extends to **prosumer Distributed Generation Resource** vendors — India-resident encrypted storage, mutual authentication and encryption for remote access and real-time data exchange with aggregators and distribution licensees, and trusted-source verification information. Commencement for existing prosumer DERs deferred to separate order.

### S3.10 Enforcement

The instrument contains **no penalty provision of its own**. Reg 16 routes enforcement outward: the CISO-MoP, after written clarification and examination, **may recommend** to the Central Government initiation of proceedings under the Information Technology Act, 2000, **or** file a petition before the Appropriate Commission for proceedings under **section 142 of the Electricity Act**. Reg 17 confers a general **power to relax** any provision on the Authority's own motion or on application, for reasons recorded in writing, to remove hardship for a class of persons.

---

## Analytical Significance for PRIS Research

### S5.1 — The AI null finding, at its strongest form in the corpus

A full-text sweep of the notified instrument returns **zero** occurrences of *artificial intelligence*, *machine learning*, *model risk*, *algorithm* (in any governance sense), *automated decision*, or the bare token `AI`, across 17 regulations, 40 definitions, 10 chapters and 2 Schedules. Reg 8's 33-component Cyber Security Policy specification — which reaches supply-chain risk, personnel risk, obsolescence phase-out, time-source selection and research collaboration — contains no AI or model-governance component.

This is the corpus's cleanest null finding, and materially stronger than the prior CEA_1/CEA_2 formulation, for three reasons:

1. **The regulator had actual, on-record notice.** [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] records Grid-India running production ML on the national grid, confirmed by the **Ministry of Power in a Rajya Sabha reply of 18 December 2023** — CEA's own parent ministry, on the record, more than two and a half years before this notification. The draft was published 7 October 2025 and objections were considered. This is not a regulator unaware of the technology.
2. **It is not a lag artefact.** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]] currently frames the power-sector gap as *technology-lag* rather than *coordination-failure*, on the basis that CEA's instruments "predate machine learning." **That framing does not survive this instrument.** CEA legislated afresh in 2026, with notice, after consultation, and did not extend the regime to AI. The domain's characterisation requires revision — see the Downstream Corrections block below.
3. **The instrument demonstrates fine-grained specificity elsewhere.** Six-hour and twenty-four-hour reporting clocks, 9–15-month audit windows, six-week report deadlines, one-month and three-month remediation clocks, seven retention horizons, auditor-rotation counts, a 50 MW applicability threshold, and a requirement that the OT time source be terrestrial or India-specific satellite. A regulator operating at that granularity that issues zero AI provisions is making a technology-neutrality choice, not omitting by inadvertence — the identical inference recorded at [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] §S5.1.

### S5.2 — Same-date, cross-sector convergence with RBI_8 (new finding)

**CEA_3 and [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] were both notified on 31 July 2026.** Two regulators, two critical sectors, one day. Both are binding, comprehensive technology-risk instruments. Both are evidentially dense. Both impose a **six-hour incident-reporting clock with a dual channel** (RBI: DAKSH + CERT-In; CEA: CSIRT-Power + CERT-In). **Both contain zero AI provisions.** Neither cites the other.

This is a stronger parallelism instance than any currently recorded in [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]], because same-day issuance forecloses the sequencing explanations (transposition lag, learning, diffusion) available for the corpus's other convergences. The most parsimonious reading is a shared exogenous driver — plausibly the same Mythos-class threat environment recorded at [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] §S5.2 as "coordination by common shock" — producing simultaneous, uncoordinated, structurally similar responses that are AI-silent in identical ways.

⚠ Same-day issuance is a strong observation but the causal claim is inferential. Neither instrument names a common trigger. Treat the convergence as documented and the mechanism as a hypothesis requiring a third instance.

### S5.3 — The retention inversion: CEA_3 against RBI_8 on the same date

[[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] records an **abdication variant** from RBI_8: an instrument mandating evidentiary sufficiency (para 95, including non-repudiation) while specifying **no retention period anywhere**, delegating scope, frequency and storage to bank-level stakeholder consultation (para 97).

CEA_3 does the exact opposite, on the same day, in the same jurisdiction: **seven enumerated horizons** (S3.5 above), a twelve-item mandatory custody schedule, and a data retention policy that is itself a mandated Cyber Security Policy component reviewed annually.

The two instruments therefore bracket the construct's full range within a single day of Indian regulatory output. This is unusually clean evidence that retention specification is a **discretionary drafting choice** rather than a function of instrument type, sector maturity, or drafting period — which is the sharpest available rebuttal to any reading of RBI_8's silence as a technical or temporal constraint.

CEA_3 also supplies a **first-party, binding 180-day log-retention figure**. Retention_Horizon_Divergence currently flags that the 180-day figure exists in the vault only as a secondhand cross-reference inside NCAIC_1, with the CERT-In 28 April 2022 Directions node still missing and the figure blocked for publication-track use. That block is now partially relieved: 180 days is available from a gazetted primary instrument, though from CEA rather than CERT-In. **The CERT-In 2022 Directions node gap remains open and should still be closed.**

### S5.4 — M1 upgraded from a two-regulator pattern to an N-regulator hub

[[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]] records the RBI↔CERT-In mandatory dual-channel reporting chain as **M1**, the corpus's one genuine coordination mechanism, and its Future Research item 2 asks explicitly "whether an equivalent mandatory-reporting-to-CERT-In clause exists in any SEBI or IRDAI instrument (would upgrade this from a two-regulator to an N-regulator coordination hub finding, with CERT-In as the common node)."

**Reg 7(3)(a) answers that question affirmatively from a sector the matrix does not yet cover.** CEA mandates six-hour reporting to CERT-In *and* to CSIRT-Power — and CSIRT-Power is itself constituted as "an extended arm of CERT-In" (reg 3(1)(g)). CERT-In is therefore the common node across **three** binding regulatory regimes (RBI, CEA, and via CERT_In_1's empanelment scheme, SEBI's audit chain), with CEA adding a sub-sectoral CSIRT layer beneath it.

This strengthens the *horizontal infrastructure coherence* limb of [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]'s two-layer model: CERT-In functions as shared incident-reporting and audit infrastructure across sectors, while the sectoral regulators above it continue to legislate without cross-reference. CEA_3 is now the third confirmed instance of that structure.

### S5.5 — MeitY concurrence: a rare affirmative coordination artefact

The preamble records that **"Ministry of Electronics and Information Technology has accorded its concurrence to make these regulations in respect of the Cyber Security for power sector."** Formal inter-ministerial concurrence recorded on the face of a sectoral instrument is rare in this corpus — the nearest comparators are [[07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025]]'s multi-ministry Sahyog architecture and [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]]'s two-ministry split administration.

Analytically this cuts both ways and the tension is worth preserving rather than resolving: MeitY concurred in an instrument that is comprehensively silent on AI, **while MeitY is simultaneously the ministry that issued the IndiaAI Governance Guidelines** ([[07_Institutions/Corpus/MeitY/MeitY_2]], 5 November 2025, confirmed on the ministerial record at [[07_Institutions/Corpus/Parliament/Parliament_2_Unstarred_Question_2988_Institutional_Framework_Auditing_AI_2026]]). Procedural coherence at the concurrence layer coexisted with substantive silence at the content layer. This is the coherence-in-form / incoherence-in-substance pattern (F094, F103, F121) appearing in an Indian inter-ministerial process rather than in a comparative guidelines survey.

### S5.6 — Institution-before-regulation: the instance closes, with a measurable gap

CEA_2 recorded CSIRT-Power's administrative inauguration (22 September 2024, per the Ministry of Power PIB release) preceding its regulatory formalisation as a second instance of the institution-before-regulation sequencing pattern. **That instance now closes:** CSIRT-Power is constituted in binding text on 31 July 2026, with fourteen enumerated functions and authority over entities and vendors.

**The gap is therefore measurable at approximately 22 months** — operational authority exercised administratively, formal authority conferred later. This is a completed cycle, and the only one in the corpus's four institution-before-regulation instances (CSIRT-Power, the AA regime/DEPA, Sahamati, BIS/ISO 42001 adoption) that can now be dated end-to-end. It is the direct counterpart to [[07_Institutions/Corpus/DPB/DPB_1_Establishment_and_Vacancy_2025_2026]], which is the inverse and worse: formal authority with no capacity. Together they bracket the sequencing pathology.

### S5.7 — ISO 27001 is mandated: a correction to the certification-recognition finding

Reg 5(24) requires entities to "ensure compliance with and acquire **ISO / IEC 27001 certificate or Technical Criteria Certificate** encompassing all critical systems," with a four-consecutive-audit rotation bar.

[[06_Frameworks/ISO_IEC_42001]] records as a finding that "No Indian regulator recognises certification as compliance evidence." **That statement is too broad and should be narrowed.** India does mandate a management-system certificate as a binding compliance obligation in the power sector — it is ISO 27001, not ISO 42001. The accurate finding is that no regulator anywhere recognises *ISO/IEC 42001* (the AI management-system standard) as compliance evidence, while ISO 27001 (the information-security standard) is mandated outright by at least one Indian sectoral regulator.

This **sharpens rather than weakens** the "certification without recognition" thesis flagged in that note as a standalone publishable paper: the contrast is now internal to India and internal to the ISO management-system family. The security standard is mandated; the AI standard is not recognised. The unit-of-certification mismatch argument (organisation-level standard vs system-level regulation) explains why — ISO 27001 governs an organisational security posture that maps onto CEA's entity-level obligations, whereas ISO 42001 would have to discharge system-level AI conformity obligations that do not exist in Indian law at all.

The **Technical Criteria Certificate** is separately notable: reg 3(1)(jj) defines it as issued by "a designated certification body **accredited** for ensuring conformance to cyber security standards specified by the Central Government" — a second Indian accreditation-of-certifiers regime, sitting alongside the unresolved NABCB/AIMS question at ⚠ #304.

### S5.8 — Assurance Reuse Gap: three cycles inside one instrument

[[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] currently documents a four-cycle Indian stack (DPDP SDF audit + SEBI CSCRF quarterly board review + RBI IT outsourcing audit + CERT-In cyber audit) with zero mutual recognition.

CEA_3 adds a **within-instrument** variant not previously recorded: a single regulation imposing three non-substitutable assurance cycles on the same entity over the same systems — annual cyber security audit (reg 13), ISO 27001/TCC certification audit (reg 5(24)), and annual self-audit (reg 15) — each with its own scope, cadence, rotation rule and retention horizon (3 / 4 / 3 years respectively), and **no provision permitting any one to satisfy any other**. Power-sector entities that are also Protected Systems additionally carry NCIIPC's validated control regime (reg 7(3)(d)).

This is structurally parallel to the MeitY_7 within-instrument governance-debt variant already recorded at [[05_Concepts/05_Concepts_Signature/Governance_Debt]], and extends the Assurance Reuse Gap from a cross-regulator to an intra-instrument phenomenon.

### S5.9 — Decision Infrastructure relevance

The instrument governs the technology estate — cyber assets, critical systems, OT/IT interconnection, perimeter devices, time synchronisation, supply chain — comprehensively, and says nothing about what the systems running on that estate *decide*. Grid-India's day-ahead demand forecasting and outage prioritisation are, under CEA_3, governed as **assets to be inventoried and secured**, not as **decisions to be validated, explained or attributed**.

That is precisely the model→workflow→decision→action gap the Decision Infrastructure framing identifies (see `Synthesis_Opportunities_and_Intake_20260809.md` §S3), and CEA_3 is now the binding-instrument evidence for the Power leg of that argument.

---

## Regulatory Units — selected

| RU | Obligation | Deontic | ADICO summary |
|---|---|---|---|
| RU1 | Six-hour incident reporting to CSIRT-Power and CERT-In (7(3)(a)) | SHALL | A=CISO; D=SHALL; I=report cyber security incident to CSIRT-Power and CERT-In; C=within six hours of incident |
| RU2 | Twenty-four-hour reporting for cyber sabotage in critical systems (7(3)(a) proviso) | SHALL | A=CISO; D=SHALL; I=report; C=incident concluded as cyber sabotage in critical system |
| RU3 | Sensitive data resides within India only (5(19)) | SHALL | A=entity; D=SHALL; I=store sensitive information/data encrypted, secured, resident in India; C=including cloud-hosted and historical data |
| RU4 | OT control and operation confined to national boundaries (6(3)) | SHALL | A=entity; D=SHALL; I=confine control, operation and information exchange to national boundaries over dedicated isolated channel; C=power system elements incl. real-time data |
| RU5 | Physical isolation of OT from internet and IT (6(1)) | SHALL | A=entity; D=SHALL; I=ensure physical isolation; C=OT system; **conditional relaxation on risk assessment + board approval** |
| RU6 | ISO 27001 or Technical Criteria Certificate for all critical systems (5(24)) | SHALL | A=entity; D=SHALL; I=comply with and acquire certificate; C=encompassing all critical systems; **commencement deferred** |
| RU7 | Annual cyber security audit, 9–15 month window, auditor rotation (5(22)) | SHALL | A=entity; D=SHALL; I=facilitate comprehensive audit; C=all critical systems; O=no three consecutive audits by same agency/personnel |
| RU8 | CISO ring-fenced to cyber security only, three-year minimum tenure (5(5), 5(6)) | SHALL | A=entity; D=SHALL; I=designate CISO for min. three years with role ring-fenced; C=all entities in scope |
| RU9 | Vendor Bill of Materials per CERT-In guidelines (11(5)) | SHALL | A=vendor; D=SHALL; I=provide BOM listing all components incl. firmware; C=components deployed in critical systems |
| RU10 | Vendor vulnerability disclosure to CSIRT-Power (11(7)) | SHALL | A=vendor; D=SHALL; I=establish formal reporting process and furnish vulnerabilities to CSIRT-Power; C=products and services supplied |
| RU11 | Sub-50 MW entities *encouraged* to adopt CERT-In MSME controls (2(1)(a) 2nd proviso) | **ENCOURAGED** | A=entity <50 MW; D=**hortatory**; I=implement 15 Elemental Cyber Defense Controls; C=below applicability threshold — the instrument's only non-binding clause and a candidate [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] instance |

**Deontic observation:** overwhelmingly SHALL-dense, consistent with RBI_8. RU11 is the single hortatory outlier, and it is structurally significant: it creates a **capacity-graded deontic boundary at 50 MW**, below which the entire regime becomes advisory. Whether the distributed-generation fleet below that threshold constitutes an aggregate systemic exposure is not addressed in the instrument.

---

## ⚠ VERIFY Flags

- **⚠ #309 (MEDIUM).** Source is a bilingual Gazette text extraction with significant Devanagari OCR corruption in the Hindi portion. All provisions cited in this node were taken from the **English text**, which extracted cleanly. Regulation and sub-clause numbers were individually checked against the English chapter structure, but the node has not been reconciled against the Hindi text; where the two diverge, the Gazette's own rules of construction govern. Confirm against the CEA-hosted PDF before quoting any provision verbatim in publication-track output.
- **⚠ #310 (MEDIUM).** The AI null finding rests on a term sweep of the extracted English text. Given the extraction quality caveat above, re-run the sweep against a clean CEA-hosted PDF before publishing the null finding as a headline claim. The finding is very likely robust — no AI-adjacent vocabulary appears anywhere in the 40 definitions or the 33-component Cyber Security Policy specification, where it would necessarily surface — but it is the node's principal contribution and warrants a clean confirmation.
- **⚠ #311 (MEDIUM).** The same-day convergence with RBI_8 (S5.2) is documented; the *common-shock mechanism* is inferred. Neither instrument names a trigger. Do not present the causal claim as established without a third same-period instance or direct evidence of a coordinating process.
- **⚠ #312 (LOW-MEDIUM).** Six regulations — 5(9), 5(24), 5(33), 5(39), 6(2), 6(7) — have **no commencement date**, deferred to separate Authority orders with prior Central Government approval. Any compliance-burden or capacity analysis must not treat these as in force on 1 April 2027. Their deferral is itself analytically interesting (they are the costliest obligations) and their eventual commencement dates should be tracked as a watch item.
- **⚠ #313 (LOW).** CSIRT-Power's September 2024 inauguration date is carried forward from CEA_2's PIB sourcing, not from this instrument, which does not recite it. The ~22-month sequencing gap at S5.6 depends on that external date.
- **⚠ #314 (LOW).** Reg 2(1)(a) proviso 2 cites CERT-In's "15 Elemental Cyber Defense Controls for Micro, Small and Medium Enterprises." **No corpus node exists for this document.** Create one before relying on the sub-50 MW hortatory regime's content.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]] | [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]] (superseded by this notification) | [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] | [[07_Institutions/Corpus/NCIIPC/NCIIPC_1_Guidelines_Protection_NCII_V2_2015]] | [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] (same-date comparator) | [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | [[07_Institutions/Corpus/MeitY/MeitY_2]] | [[07_Institutions/Corpus/DPB/DPB_1_Establishment_and_Vacancy_2025_2026]] | [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] | [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] | [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]]
**Related frameworks:** [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]] | [[06_Frameworks/ISO_IEC_42001]] | [[06_Frameworks/Manifestation_Evidence_Layer]]
**Related domains:** [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]] | [[03_Domains/Cybersecurity_Governance]] | [[03_Domains/AI_Governance]] | [[03_Domains/Systemic_Regulatory_Governance]]
**Related institutions:** [[07_Institutions/CEA]] | [[07_Institutions/Ministry_of_Power]] | [[07_Institutions/Grid_India]] | [[07_Institutions/CERT_IN]] | [[07_Institutions/NCIIPC]] | [[07_Institutions/MEITY]]
**Related projects:** [[02_Projects/P1_SLR_RG]] | [[02_Projects/P4_Doctrinal_IJLIT]] | [[02_Projects/fsQCA_Thesis_Chapter]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/Cross_Institutional_Mandate_Comparison]] | [[04_Knowledge_Products/Regulatory_Complexity_Handbook]]

---

## Coding Status

- **P3 NVivo:** Not applicable (non-BFSI sector) — but a high-yield **IG 2.0 / ADICO** target: 17 regulations with enumerated, deontic-explicit sub-clauses, reg 5 alone carrying 42 and reg 8 carrying 33.
- **Wiki intake status:** Pending — **High priority.** No existing Wiki section covers critical-infrastructure cyber governance; CEA_1 already flagged this as a structural gap.

---

## Log

- 2026-08-09: Corpus node created from full Gazette text supplied by Vivek (bilingual extraction; English text used throughout). **Not a duplicate** — CEA_2 is the 2025 *draft*; this is the notified instrument, and it closes CEA_2's standing "not confirmed as finalised/gazetted" status flag. Tier upgraded to A as CEA_2 anticipated. AI null finding verified by term sweep and recorded as the node's principal contribution, materially stronger than the CEA_1/CEA_2 formulation because the regulator legislated afresh with on-record notice of Grid-India's ML deployment. Four new findings recorded: same-date convergence with RBI_8 (S5.2); the retention-specification inversion against RBI_8 (S5.3); M1 upgraded to an N-regulator CERT-In hub, answering an open question in the Cross_Regulator matrix (S5.4); and the ISO 27001-is-mandated correction to [[06_Frameworks/ISO_IEC_42001]] (S5.7). Institution-before-regulation instance closed at ~22 months (S5.6). Six VERIFY flags (#309–#314), none HIGH.
