---
type: Corpus Node
node-id: RBI_16
institution: RBI
date: 2026-07
status: active
last_updated: 2026-08-09
wiki-section: S2
tier: B
ai-explicit: false
tags:
  - type/corpus-node
  - status/active
  - status/draft-instrument
  - engine/phd
  - jurisdiction/india
  - institution/rbi
  - tier/B
  - batch/ad-hoc-20260809
  - concept/Governance_Debt
  - concept/Decision_Infrastructure
  - concept/Retention_Horizon_Divergence
  - concept/Assurance_Reuse_Gap
  - project/p3
  - project/p4
---

# RBI_16 — Draft Guidance on Regulatory Expectations for Data Governance, 2026

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_16_Draft_Guidance_Data_Governance_2026.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India, **Department of Regulation** (DoR.ORG.REC.)
**Document date:** **July 2026 — exact day not stated** (placeholder: "July XX, 2026")
**Pages:** 20 pages; 6 chapters, 63 paragraphs
**Domain:** [[03_Domains/BFSI_Governance]]

---

## ⚠ Draft Status, and its sibling instrument

**This is a draft issued for consultation, not an operative instrument.** Identical markers to RBI_14: unfilled reference number (`DoR.ORG.REC.XXXX/XX-XX-XXXX/2026-27`) and unfilled date ("July XX, 2026").

**Same department, one month apart, same 11-category applicability clause, word for word.** [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] (June 2026 draft, DoR.ORG.REC.) and this document (July 2026 draft, same department code) list **identical** regulated-entity categories in para 4/para 3 respectively — Commercial Banks, SFBs, Payments Banks, Local Area Banks, RRBs, Urban and Rural Co-operative Banks, all four NBFC layers, the five AIFIs, ARCs, and CICs. **This is not incidental drafting reuse — it is evidence that DoR is issuing a coordinated multi-instrument governance-modernisation package to the same regulated population within a single quarter**, rather than two unrelated drafts. Treat RBI_14 and RBI_16 as companion instruments when assessing either one's scope or timing.

---

## Instrument Identity

**Full title:** Guidance on Regulatory Expectations for Data Governance
**Type:** **Guidance** — hortatory. Operative verb is "should" throughout (consistent with RBI_14's deontic profile, not independently re-verified paragraph-by-paragraph here)
**Legal basis:** Not stated in the text supplied
**International reference:** Basel Committee's **BCBS 239** — *Principles for effective risk data aggregation and risk reporting* — named explicitly (para 2) as a source the Guidance draws upon
**Reading rule:** Para 4 — read in conjunction with relevant RBI Directions; "the applicable Directions shall prevail" in case of inconsistency (identical formulation to RBI_14 para 5)

### Applicability — identical to RBI_14

Para 3 lists the same eleven RE categories as RBI_14 para 4, in the same order. See the note above.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) primary
**Jurisdiction:** India
**Confidence:** High for text and content; instrument status is draft
**AI explicit:** **No.** "Artificial Intelligence," "AI" and "Machine Learning" do not appear anywhere in the text supplied. The Introduction (para 1) gestures at the adjacent territory — "advanced analytics, and automated decision-making processes" as drivers of data volume/velocity/complexity — but the instrument itself is technology-neutral and applies to all RE data, not an AI-specific subset.
**Why it is in this corpus despite that:** [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] requires AI/ML models to meet data-quality standards — para 54(7) names data quality, non-representativeness, incompleteness, drift — **without specifying the governance architecture that would produce that data in the first place.** This document is that architecture: ownership, stewardship, custody, lineage, metadata, classification, SSOT, quality management, retention, and third-party data-sharing controls, issued by the same department roughly one month later. It is the corpus's most detailed primary-source treatment of the **data layer** that every AI/ML instrument in the corpus presupposes and none has specified.
**Tier classification:** **Tier B** — primary-source draft text, comprehensive, not yet operative
**AI Governance Wiki relevance:** **MEDIUM** — foundational-layer relevance to AI governance, not direct AI-governance content

---

## Substantive Content

### S3.1 Structure

| Chapter | Content | Paras |
|---|---|---|
| I | Preliminary — introduction, applicability, 15 definitions | 1–5 |
| II | Governance — DGF, Board, Board Committee (DGC), executive-level DGC, data risk management | 6–21 |
| III | Organisational Structure — Data Function, Data Owner, Data Steward, Data Custodian, roles mapping | 22–31 |
| IV | Data Lifecycle — origination/capture, processing/sharing/transformation, retention/archival/disposal | 32–42 |
| V | Data Architecture — SSOT, metadata and lineage, classification, quality management | 43–59 |
| VI | Third-Party Arrangements | 60–63 |

### S3.2 A four-role accountability chain, distinct from RBI_14's model-risk chain

Unlike RBI_14, which places accountability on the RE as a single undifferentiated entity, this instrument builds a **named four-role chain**: **Data Owner** (accountable per domain — business logic, classification, quality, SSOT designation), **Data Steward** (implements within the domain, "connecting business logic and rules with system designs"), **Data Custodian** (technical management — access controls, retention/disposal execution, BCP for data platforms), and a **Data Function** headed by an officer "not below the rank of Chief General Manager or equivalent" acting as central coordinator. Para 30 requires this mapped explicitly to "accountability... responsibility... points of consultation... escalation and decision-making" — a more granular role-separation model than any other instrument in the corpus, including RBI_14's Board/RMCB/Senior Management triad for model risk.

### S3.3 Single Source of Truth (SSOT) — a new construct for the corpus

Para 43: an RE must maintain SSOT for all data elements and **"ensure that no parallel or competing SSOT sources exist for the same data element."** SSOT designation and changes require **Data Governance Executive Committee approval**, reported to the Board Committee for information (para 45). Para 46 requires a **reconciliation mechanism** between SSOT and downstream data. This is the corpus's first explicit single-source-of-truth mandate and directly underwrites the reliability of any AI/ML model trained or run on RE data — a model validated under RBI_14 is only as good as the SSOT feeding it, and this document is the first to require that SSOT be singular and reconciled.

### S3.4 Metadata and lineage (Ch. V.B) — traceability from point of capture

Para 48 requires **foundational metadata at the point of capture**: source system, purpose of collection, data owner, classification, retention/usage terms. Para 51 requires metadata updates on transformation, including "relationship between source and transformed or derived data" and "purpose and nature of the transformation." This is a stronger point-of-origin lineage requirement than RBI_14 imposes on models themselves (RBI_14 para 22 requires model inventories to record "dependencies with upstream and downstream models," but says nothing about the data those models consume).

### S3.5 Retention — the softest abdication instance in the corpus

Para 41: "data retention period is justified by business, legal, regulatory, or audit requirements" — **no numeric period stated anywhere in 20 pages.** Para 42(B) requires disposal to be "secure, controlled, and verifiable," again with no period attached. See S5.2.

### S3.6 Third-party data-sharing (Ch. VI) — no explicit refusal clause

Paras 60–63 require: sharing only for "defined and approved purposes and by designated personnel"; access on a "need to know" basis; non-disclosure clauses; secure channels (encryption, authentication, auto-deletion, deduplication); **periodic audit of third-party systems "either by itself or through external auditors, including CERT-IN empanelled auditors."** Compare RBI_14 para 46(i), which requires independent validation of third-party *models* "**notwithstanding** any validation, certification, or assurance provided by the third-party provider" — an express refusal to accept vendor assurance. **This instrument contains no equivalent formulation for third-party *data*.** See S5.4.

---

## Analytical Significance for PRIS Research

### S5.1 — Decision Infrastructure's "Data" stage gets its first dated, detailed primary-source instrument

[[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]]'s five-stage chain (Data → Model → Workflow → Decision → Action) has, until now, been evidenced almost entirely at the Model, Workflow and Decision stages — the construct's own "What would have to be governed" section (⚠#323) notes its prescriptions are derived, not observed. **This document is observed, primary-source, dated evidence at the Data stage specifically**: provenance requirements at capture (para 35), SSOT singularity (para 43), lineage through transformation (para 51), and classification tied to downstream risk (para 52–55). It does not reach the Model→Workflow handoff (H1) or beyond, but it is the strongest evidence yet that at least one stage of the chain has a dedicated Indian instrument, once RBI_16 and RBI_14 are read together as a stack: RBI_16 governs the data a model consumes; RBI_14 governs the model itself; neither reaches the workflow, decision or action stages. **The gap the construct identifies is now sharper, not weaker** — two instruments cover two of five stages in detail, and the remaining three (workflow, decision, action) remain as ungoverned as before.

### S5.2 — Retention Horizon Divergence: a fourth RBI abdication instance, and the softest yet

[[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] records three RBI/CERT-In/SEBI 2026 instruments that specify operational clocks precisely while stating no retention period (RBI_8, CERT_In_3, SEBI_18). **RBI_16 extends the pattern to a fourth instrument, and is the softest version recorded**: it does not even pair the silence with a strong sufficiency mandate (contrast RBI_8 para 95's forensic-evidence standard). It states only that the period should be "justified" by unspecified business/legal/regulatory/audit requirements — a standard with no test, no default, and no consequence for a wrong answer. Read against RBI_14's ten-year model-record retention (S5.7 in that node), RBI now holds, within a single department and a single quarter, instruments spanning the entire range from the corpus's most specific retention mandate (RBI_14) to among its least specific (RBI_16).

### S5.3 — Governance Debt: the coordinated-package finding cuts against the "uncoordinated regulator" framing in one specific respect

Much of [[05_Concepts/05_Concepts_Signature/Governance_Debt]]'s evidence base is *cross-regulator* incoherence. RBI_14 and RBI_16 being companion instruments from the same department in the same quarter is a case of apparent **intra-regulator coordination** — a data-governance instrument and a model-risk instrument that reference no other regulator, but also do not cross-reference *each other* despite governing adjacent layers of the same technical stack. RBI_16 nowhere cites RBI_14, and RBI_14 nowhere cites this document by name. **The debt is not duplication here — it is an uncited adjacency**: two instruments from the same department, same quarter, same regulated population, governing sequential stages of the same pipeline, without a stated relationship between them.

### S5.4 — Assurance Reuse Gap: a within-RBI contrast between data assurance and model assurance

[[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]]'s four-way typology (operative credit / architectural credit / express refusal / silence) currently places RBI_14 para 46(i) in the express-refusal category — the corpus's only instance of a regulator affirmatively declining to accept third-party assurance. **RBI_16's third-party data-sharing chapter (60–63) sits in the silence category by comparison**: audit of third-party systems is required, but there is no "notwithstanding any assurance provided" formulation. **The same department, in instruments issued a month apart, treats third-party model assurance and third-party data assurance differently** — an express refusal for one, ordinary oversight language for the other. Whether this is a considered distinction (models carry different risk than data-sharing arrangements) or an unconsidered drafting inconsistency cannot be determined from the text; either way it is now a recorded within-regulator divergence, not merely a cross-regulator one.

---

## ⚠ VERIFY Flags

- **⚠ #345 (LOW-MEDIUM).** Whether RBI_14 and RBI_16 are formally linked as a single consultation package, or are independent drafts that happen to share a department code and applicability clause, is not stated in either text. Confirm against RBI's consultation-paper index if it becomes available.
- **⚠ #346 (LOW).** Deontic profile ("should" throughout, no SHALL) is assumed by analogy to RBI_14's confirmed pattern and RBI_16's own para 4 inconsistency-rule language, but was not independently verified paragraph-by-paragraph across all 63 paragraphs of this document. Verify before citing a specific paragraph's deontic strength.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] (companion instrument — see Draft Status note) | [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | [[07_Institutions/Corpus/SEBI/SEBI_18_AI_Vulnerability_Detection_Advisory_2026]] | [[04_Knowledge_Products/Wiki_Intake/Martins_Mamede_Correia_BCBS_239_Master_Data_2022]] (F066 — the BCBS 239 implementation-layer companion this instrument's para 2 citation connects to)
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] | [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] | [[05_Concepts/05_Concepts_Standard/Model_Risk]]
**Related domains:** [[03_Domains/BFSI_Governance]]
**Related institutions:** [[07_Institutions/RBI]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] (medium — data-layer foundation for AI governance findings) | [[02_Projects/P4_Doctrinal_IJLIT]] (medium — intra-regulator uncited-adjacency finding)

---

## Coding Status

- **P3 NVivo:** Medium priority. Not AI-explicit, but structurally load-bearing for AI-governance findings via RBI_14.
- **IG 2.0 / ADICO:** Not attempted in this pass — deontic profile assumed by analogy, not independently coded.
- **Wiki intake status:** Complete, medium priority.

---

## Log

- 2026-08-09: Corpus node created from full draft text supplied by Vivek. **Not a duplicate** — no prior node for this instrument existed; distinct from RBI_14 in subject (data governance vs model risk) and date placeholder (July vs June 2026), though the two share department code and an identical applicability clause, recorded as a companion-instrument finding rather than a duplicate. Four findings recorded: this is the corpus's first detailed primary-source instrument for Decision_Infrastructure's Data stage (S5.1); a fourth and softest RBI retention-abdication instance (S5.2); an intra-regulator "uncited adjacency" variant of Governance_Debt distinct from the cross-regulator duplication evidence dominating that construct (S5.3); and a within-RBI divergence between express refusal of third-party model assurance (RBI_14) and ordinary oversight language for third-party data assurance (RBI_16), recorded at Assurance_Reuse_Gap (S5.4). Two VERIFY flags (#345–#346).
