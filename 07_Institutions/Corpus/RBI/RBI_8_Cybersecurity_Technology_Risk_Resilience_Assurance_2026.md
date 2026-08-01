---
type: corpus-node
node-id: RBI_8
institution: RBI
date: 2026-07-31
wiki-section: S2
tier: A
ai-explicit: false
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - institution/RBI
  - wiki-section/S2
  - tier/A
  - batch/ad-hoc-20260802
  - concept/Evidentiary_Governance
  - concept/Retention_Horizon_Divergence
  - concept/Regulatory_Parallelism
  - concept/Governance_Debt
  - concept/Institutional_Coherence
  - concept/Accountability
  - project/P3
  - project/P4
  - project/fsQCA
  - jurisdiction/india
---

# RBI_8 — Reserve Bank of India (Commercial Banks – Cybersecurity, Technology: Risk, Resilience and Assurance Framework) Directions, 2026

**Node ID:** RBI_8
**Institution:** Reserve Bank of India (RBI), Department of Supervision
**Document type:** Regulatory — Directions under Banking Regulation Act / RBI Act
**Date:** July 31, 2026
**Jurisdiction:** India
**Wiki Section:** S2 — India Regulatory
**Tier:** A (primary RBI regulatory instrument; verbatim quotes extracted from source PDF)
**Source PDF:** `RBI Cybersecurity Jul 26.pdf` (56 pages, 233 paragraphs)

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Reserve Bank of India (Commercial Banks – Cybersecurity, Technology: Risk, Resilience and Assurance Framework) Directions, 2026 |
| Issuing Authority | Reserve Bank of India, Department of Supervision (CSITEG) |
| Reference Number | RBI/DoS/2026-27/410; DoS.CO.CSITEG.4/31.01.015/2026-27 |
| Date | July 31, 2026 |
| Commencement | **Immediately upon issuance** (para 2) — no phase-in |
| Legal basis | Sections 27 and 35-A, Banking Regulation Act 1949; Reserve Bank of India Act 1934 |
| Scope | Commercial Banks — banking companies (excluding Small Finance Banks, Payments Banks, Local Area Banks), corresponding new banks, and State Bank of India, per s.5(c), (da), (nc) BR Act 1949 (para 3) |
| Foreign banks | Branch-mode foreign banks: Board references read as controlling/head office; **"comply or explain"** approach for Chapters II, III and others (para 4) |
| Supersedes | **Repeals** extant Cybersecurity Framework and IT Governance directions/instructions/guidelines applicable to Commercial Banks, per companion circular DoS.CO.PPG.66/11.01.005/2026-27 of the same date (para 230) |
| Structure | 8 chapters, 233 paragraphs |
| Signatory | N. Suganandh, Chief General Manager |
| AI relevance | **NIL — see S5.1.** Zero AI/ML provisions across 56 pages. Analytically significant as a null finding. |

---

## S2. Governance Context

RBI_8 is the **most recent primary RBI instrument in the corpus** and the most consequential for vault maintenance, because it repeals rather than supplements. It consolidates into a single instrument what was previously distributed across the Cybersecurity Framework circulars and the IT Governance Master Direction — the latter being [[07_Institutions/Corpus/RBI/RBI_1]], which must now be treated as superseded for Commercial Banks.

It sits alongside, and does not reference, three adjacent RBI instruments:

- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — Seven Sutras AI governance framework (principles-based)
- [[07_Institutions/Corpus/RBI/RBI_7]] — Digital Lending Directions 2025 (AI-explicit, credit assessment)
- [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] and the Commercial Banks Outsourcing Directions 2025, from which RBI_8 paras 126–135 are expressly carved out (Chapter V.Q preamble)

The carve-out is notable: RBI_8's third-party provisions apply **only** to IT/cybersecurity third-party arrangements *not* covered by the Managing Risks in Outsourcing Directions, 2025 — an explicit intra-RBI boundary-setting device, and the only such device in the instrument.

---

## S3. Structural Overview

| Chapter | Content | Key paragraphs |
|---|---|---|
| I | Preliminary — short title, commencement, applicability, 40+ definitions | 1–6 |
| II | Role of the Board — Board-approved policies (annual review), ITSC, ACB oversight of IS Audit | 7–10 |
| III | IT Governance and Oversight — IT Governance Framework, InfoSec/Cyber policy, ITSC, IT Steering Committee, Information Security Committee, Head of IT, CISO, project management, IT architecture | 11–~40 |
| IV | Risk and resilience management | — |
| V | Controls — DLP, data migration, physical/environmental, capacity, secure configuration, network, application security lifecycle, **audit logs (J)**, patch/vulnerability/change, access control, teleworking, customer authentication, mail, removable media, **third-party (Q)**, cryptographic, STP, surveillance, threat defence, anti-phishing, **VAPT (W)**, **red teaming (X)**, BCP/DR, **incident response (Z)**, metrics, awareness, transaction monitoring, **forensics (EE)** | 93–211 |
| VI | Cyber Security Operations Centre — governance, capabilities, staff capabilities | 212–223 |
| VII | Information Systems Audit — ACB oversight, IS Audit Policy, separate IS Audit function, risk-based planning, continuous auditing | 224–229 |
| VIII | Repeal and other provisions | 230–233 |

---

## S4. Key Verbatim Quotes

**Definition 14 — Digital Forensics (Chapter I.C):**
> "'Digital Forensics' - The process used to acquire, preserve, analyse, and report on evidence using scientific methods that are demonstrably reliable, accurate, and repeatable. (Source: adapted from NIST Cloud Computing Forensic Science Challenges)"

**Para 93 (audit logging capability):**
> "The bank shall ensure that every IT application / system that can access or affect critical or sensitive information has necessary audit logging capabilities and provides audit trails."

**Para 95 (evidentiary purpose — the instrument's most significant provision for PRIS):**
> "The bank shall ensure that audit trails satisfy its business requirements, in addition to regulatory and legal requirements. The bank shall also ensure that audit trails are sufficiently detailed to facilitate the conduct of audits, serve as forensic evidence (the term 'forensics' refers to 'digital forensics' for the purpose of these Directions) when required, and assist in dispute resolution, including for non-repudiation purposes."

**Para 97 (retention — delegated, not specified):**
> "The bank shall consult all the stakeholders before finalising the scope, frequency, and storage of log collection."

**Para 182 (incident reporting — M1 pattern):**
> "The bank shall report cyber incidents within six hours of detection on DAKSH platform (Reserve Bank's Advanced Supervisory Monitoring System - https://daksh.rbi.org.in). The bank shall also pro-actively notify CERT-In regarding cyber incidents."

**Para 220(5) (CSOC attribution capability):**
> "establishing clear attribution of actions including who did what, when and how, along with preservation of evidence"

**Para 230 (repeal):**
> "With the issue of these Directions, the existing Directions, instructions, and guidelines relating to Cybersecurity Framework and IT Governance as applicable to Commercial Banks stand repealed, as communicated vide circular no. DoS.CO.PPG.66/11.01.005/2026-27 dated July 31, 2026."

---

## S5. Analytical Notes

### S5.1 — The AI null finding (primary analytical contribution)

RBI's flagship 2026 technology-risk framework for commercial banks contains **no AI-specific provision whatsoever**. Full-text sweep of the 56-page instrument returns: *artificial intelligence* 0, *machine learning* 0, *model risk* 0, *generative* 0, *automated decision* 0, and zero occurrences of the bare token `AI`. The only instance of "algorithm" (para 140) refers to cryptographic key length and cipher suites; the three occurrences of "analytics" are in the CSOC monitoring context.

This is analytically significant in three ways:

1. **It extends the RBI_1 null finding forward three years.** [[07_Institutions/Corpus/RBI/RBI_1]] (2023) was coded as a null finding — technology-neutral IT governance with zero AI-specific requirements. RBI_8 (2026) reproduces that posture in the instrument that replaces it, after RBI's own FREE-AI framework had already been published.
2. **It converts cross-regulator parallelism into intra-regulator parallelism.** The existing finding in [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]] is that RBI is the "silent party" relative to SEBI. RBI_8 shows RBI silent relative to *itself*: [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] and [[07_Institutions/Corpus/RBI/RBI_7]] govern AI explicitly, RBI_8 governs the technology estate those AI systems run on, and neither track cites the other. This is a stronger and more novel claim than the cross-regulator version.
3. **It is a deliberate architectural choice, not an oversight.** RBI_8 demonstrates fine-grained specificity elsewhere (six-hourly incident reporting, six-monthly VA, twelve-monthly PT, NIST-sourced forensic definitions). A regulator capable of that granularity that issues zero AI provisions in July 2026 is making a technology-neutrality choice, not omitting by inadvertence.

### S5.2 — Evidentiary provisions strengthen on supersession

Para 95 is the successor to RBI_1 §15 and is materially stronger. RBI_1 required that audit trails "support forensic evidence and dispute resolution." RBI_8 adds: satisfaction of "regulatory and legal requirements"; sufficiency "to facilitate the conduct of audits"; and — new — "non-repudiation purposes." Combined with the definition of digital forensics at Definition 14 and the CSOC attribution requirement at para 220(5), RBI_8 is the corpus's **most evidentially specified instrument**, Indian or international, at the operational layer.

Para 220(5) is worth isolating: "who did what, when and how, along with preservation of evidence" is a four-part reconstruction requirement written into binding regulation. It maps directly onto the diagnostic questions in [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]].

### S5.3 — A verified NIST-to-India evidentiary transmission

Definition 14 attributes its digital-forensics definition to *NIST Cloud Computing Forensic Science Challenges* (NISTIR 8006). This is the corpus's **first verified instance of an Indian financial regulator importing a NIST forensic-science definition into binding text**. It is a genuine, citable NIST-to-Indian-regulation evidentiary link, and should be used in place of the unsupportable "NIST Digital Forensics Artifact Catalog" attribution corrected at [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] §Provenance.

⚠ Cross-check NISTIR 8006 as the underlying source before publication-track citation — RBI names the report title, not the NISTIR number, and says "adapted from," not "reproduced."

### S5.4 — Retention abdication

Para 97 requires stakeholder consultation on "the scope, frequency, and storage of log collection" and specifies **no retention period anywhere in the instrument**. India's newest and most detailed banking cybersecurity Direction delegates the retention horizon wholly to the regulated entity. This is a new variant for [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]]: not divergence *between* regulators, but *abdication* by one — an instrument that mandates evidentiary sufficiency (para 95) without mandating the retention period that would make it achievable.

### S5.5 — M1 coordination pattern, re-enacted and hardened

Para 182 re-enacts the M1 pattern (separate regulatory reporting channels for one event) with two hardenings over the RBI_1 §27(d) formulation: a **six-hour** clock from detection, and a **named platform** (DAKSH). The CERT-In leg remains "pro-actively notify," retaining the asymmetry already recorded at [[06_Frameworks/Manifestation_Evidence_Layer]] — RBI specifies its own channel precisely and its peer's loosely. Paras 185 and 188 add CERT-In coordination and cyber-drill participation; para 184 adds IDRBT/IB-CART threat-intelligence sharing as permissive ("may").

This connects to the capacity-without-deployment governance-debt instance logged at [[07_Institutions/Corpus/International/International_15]] — DAKSH is now named in binding text with a hard clock, strengthening the argument that India's incident-reporting fragmentation is a governance-will rather than technical-capacity problem.

---

## S6. Regulatory Units — selected, evidentiary and governance layers

| RU | Obligation | Deontic | ADICO summary |
|---|---|---|---|
| RU1 | Audit logging capability on every system accessing critical/sensitive information (para 93) | SHALL | A=bank; D=SHALL; I=ensure audit logging capability and audit trails; C=every IT application/system accessing or affecting critical or sensitive information |
| RU2 | Audit trails sufficient as forensic evidence and for non-repudiation (para 95) | SHALL | A=bank; D=SHALL; I=ensure audit trails sufficiently detailed for audit, forensic evidence, dispute resolution, non-repudiation; C=business, regulatory and legal requirements |
| RU3 | Log retention scope/frequency/storage set by stakeholder consultation (para 97) | SHALL | A=bank; D=SHALL; I=consult stakeholders before finalising scope, frequency, storage of log collection; C=unspecified; **O=absent** |
| RU4 | Six-hour incident reporting on DAKSH + CERT-In notification (para 182) | SHALL | A=bank; D=SHALL; I=report on DAKSH within 6 hours of detection, pro-actively notify CERT-In; C=cyber incident detected |
| RU5 | CSOC attribution and evidence preservation (para 220(5)) | SHALL | A=bank (via CSOC); D=SHALL; I=establish clear attribution — who did what, when, how — with preservation of evidence; C=CSOC monitoring systems |
| RU6 | CISO independence from IT function (para 27) | SHALL | A=bank; D=SHALL; I=designate senior executive as CISO with no direct reporting to Head of IT and no business targets; C=all commercial banks |
| RU7 | VA six-monthly, PT twelve-monthly for critical/DMZ customer-interface systems (para 151) | SHALL | A=bank; D=SHALL; I=conduct VA ≥ every 6 months, PT ≥ every 12 months; C=critical information systems and/or DMZ with customer interface |
| RU8 | Red teaming (para 162) | **MAY** | A=bank; D=MAY; I=conduct red teaming exercises; C=discretionary — a deontic outlier in an otherwise SHALL-dense instrument |
| RU9 | Accountability for security in outsourced/partner arrangements (para 127) | SHALL | A=bank; D=SHALL; I=be accountable for management and assurance on security risks in outsourced and partner arrangements; C=non-delegable |

**Deontic observation:** the instrument is overwhelmingly SHALL-dense. RU8 (red teaming, MAY) is the clearest discretionary outlier and a candidate instance for [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] within a single instrument.

---

## S7. Concept Linkages

| Concept | Linkage |
|---|---|
| [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | **New canonical anchor.** Paras 93/95/97, Definition 14, and para 220(5) together make RBI_8 the corpus's most evidentially specified instrument. Para 95 supersedes RBI_1 §15 as the canonical instance. Para 97 supplies the artefact-specification-without-retention-horizon case that the construct's fourth dimension predicts. |
| [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | New **abdication variant** — evidentiary sufficiency mandated (para 95), retention horizon delegated entirely to the bank (para 97). Distinct from inter-regulator divergence. |
| [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | **Intra-regulator parallelism** — RBI_8's total AI silence alongside RBI_FREE_AI_2025 and RBI_7, with no cross-reference in either direction. A novel extension: parallelism previously coded only across regulators. |
| [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | Two instances: (i) the AI-silence gap means commercial banks operating AI systems have no AI-specific technology-risk controls in the governing instrument, only technology-neutral ones; (ii) para 97's absent retention horizon transfers a compliance-design burden to the regulated entity. |
| [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | Negative instance at the intra-institutional level — RBI's principle-layer coherence (Seven Sutras) is not carried into its operative technology-risk instrument. |
| [[05_Concepts/05_Concepts_Standard/Accountability]] | RU9 (para 127) non-delegable accountability for outsourced security, consistent with the SEBI_14 / RBI_7 / IOSCO convergence at [[07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025]]. |
| [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] | Chapter VII IS Audit and the CERT-In empanelled-auditor reference (para ~137) add a fourth non-cross-recognising audit cycle for entities also subject to DPDP SDF audit, SEBI CSCRF and CERT-In cyber audit. |

---

## S8. Project Relevance

| Project | Relevance |
|---|---|
| [[02_Projects/P3_BFSI_JEIM]] | **High.** Supersedes a screening-corpus node (RBI_1); supplies the intra-regulator parallelism finding; adds nine codeable RUs. P3's RBI baseline must be re-cut against RBI_8. |
| [[02_Projects/P4_Doctrinal_IJLIT]] | **High.** Para 95 non-repudiation language and Definition 14 are the strongest doctrinal anchors in the corpus for the evidentiary argument. The AI-silence finding supports the fragmentation critique. |
| [[02_Projects/fsQCA_Thesis_Chapter]] | Medium. Affects RL/EA calibration for the India case — binding, immediate-effect, SHALL-dense, but AI-silent. |
| [[08_Methods/Institutional_Grammar_IG2]] | High-yield ADICO target — 233 enumerated, deontic-explicit paragraphs. |

---

## S9. ⚠ VERIFY Flags

- **⚠ V-RBI8-1 (HIGH, blocking for RBI_1).** The precise scope of the para 230 repeal depends on companion circular **DoS.CO.PPG.66/11.01.005/2026-27 (31 July 2026)**, which lists the repealed instruments and is **not in the vault**. Whether [[07_Institutions/Corpus/RBI/RBI_1]] is repealed in full, in part, or only as to Commercial Banks cannot be confirmed without it. RBI_1 has been flagged, not rewritten, pending this. **Obtain the companion circular.**
- **⚠ V-RBI8-2 (MEDIUM).** Definition 14 cites "NIST Cloud Computing Forensic Science Challenges" by title without a NISTIR number and says "adapted from." Confirm against NISTIR 8006 before quoting the lineage in publication-track output.
- **⚠ V-RBI8-3 (MEDIUM).** RBI_1 remains applicable to entities outside the Commercial Banks definition (Small Finance Banks, Payments Banks, Local Area Banks, NBFCs, co-operative banks). The corpus must not treat RBI_1 as globally repealed. Scope of continuing applicability to be confirmed with V-RBI8-1.
- **⚠ V-RBI8-4 (LOW).** Chapter IV was not read paragraph-by-paragraph in this intake pass; the structural summary at S3 for that chapter is derived from the table of contents. Complete on next pass before any Chapter IV claim is made.
- **⚠ V-RBI8-5 (LOW).** Source is a text-extracted PDF with Devanagari header artefacts. Paragraph numbers and quotes were verified individually; the 233-paragraph count is derived from the final numbered paragraph and should be confirmed against the RBI website version.

---

## Backlinks

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_1]] (superseded — see V-RBI8-1) | [[07_Institutions/Corpus/RBI/RBI_2]] | [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]] | [[07_Institutions/Corpus/RBI/RBI_7]] | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] | [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] | [[07_Institutions/Corpus/International/International_15]] | [[07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]]
**Related frameworks:** [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]] | [[06_Frameworks/Manifestation_Evidence_Layer]] | [[06_Frameworks/RBI_Free_AI]]
**Related domains:** [[03_Domains/BFSI_Governance]] | [[03_Domains/Cybersecurity_Governance]] | [[03_Domains/AI_Governance]]
**Related institutions:** [[07_Institutions/RBI]] | [[07_Institutions/CERT_IN]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/P4_Doctrinal_IJLIT]] | [[02_Projects/fsQCA_Thesis_Chapter]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]] | [[04_Knowledge_Products/Cross_Institutional_Mandate_Comparison]]

---

## Log

- 2026-08-02: Node created from source PDF (56pp) on day of ad-hoc intake, two days after issuance. AI null finding verified by full-text term sweep (six AI-related terms, all zero). Evidentiary provisions (paras 93/95/97, Def. 14, para 220(5)) extracted verbatim. Repeal flagged as blocking for RBI_1 pending companion circular DoS.CO.PPG.66/11.01.005/2026-27. Chapter IV not yet read at paragraph level (V-RBI8-4).
