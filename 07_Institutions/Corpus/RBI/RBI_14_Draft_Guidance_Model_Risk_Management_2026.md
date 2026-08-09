---
type: Corpus Node
node-id: RBI_14
institution: RBI
date: 2026-06
status: active
last_updated: 2026-08-09
wiki-section: S2
tier: B
ai-explicit: true
tags:
  - type/corpus-node
  - status/active
  - status/draft-instrument
  - engine/phd
  - jurisdiction/india
  - institution/rbi
  - tier/B
  - batch/ad-hoc-20260809
  - concept/Model_Risk
  - concept/Human_Oversight
  - concept/Assurance_Reuse_Gap
  - concept/Deontic_Bifurcation
  - concept/Explainability
  - concept/Agentic_AI_Governance
  - concept/Retention_Horizon_Divergence
  - concept/Governance_Debt
  - project/p3
  - project/p4
  - project/fsQCA
---

# RBI_14 — Draft Guidance on Regulatory Principles for Model Risk Management, 2026

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026.md`
**Institution:** [[07_Institutions/RBI]]
**Issuing body:** Reserve Bank of India, **Department of Regulation** (DoR.ORG.REC.)
**Document date:** **June 2026 — exact day not stated in the document** (see Draft Status below)
**Pages:** 16 pages; 64 paragraphs across 6 chapters
**Domain:** [[03_Domains/BFSI_Governance]] | [[03_Domains/AI_Governance]]

---

## ⚠ Draft Status — and a flag it resolves

> **This is a draft issued for public consultation, not an operative instrument.** Two markers on the face of the document confirm it:
>
> - **Reference number is an unfilled placeholder:** `DoR.ORG.REC.XXXX/XX-XX-XXXX/2026-27`
> - **Date is an unfilled placeholder:** "June xx, 2026"
> - Para 64 states: *"The final Guidance on 'Regulatory Principles for Model Risk Management', following public consultation, would supersede Chapter-3 on Credit Risk Models of the 'Guidance Note on Credit Risk Management, dated October 12, 2002."*
>
> ### ✅ This closes ⚠ #306
>
> [[04_Knowledge_Products/Wiki_Intake/F140_Joshi_Preventing_AI_Assisted_Cyber_Attacks_ISC2_Keynote_2026]] cited "RBI Guidance DOR.ORG.REC.XXXX/2026-27" for its slides 11–15, and this vault flagged that at ⚠ #306 as an *"unfilled placeholder citation… treat as unconfirmed / possibly illustrative or drafted-ahead-of-issuance material, not a verified RBI instrument."*
>
> **The flag was wrong about the source and right about the status.** The placeholder is not the deck author's error — it is in the RBI draft itself, because the circular number has not yet been assigned. F140 was accurately reproducing a real draft. Its substantive content (three lines of defence, risk tiering, 10-year inventory retention, explainability thresholds, prompt-injection safeguards, kill-switches, customer disclosure with human-agent option) is confirmed against this primary text and can now be traced to named paragraphs. **#306 closed; the "possibly illustrative" characterisation is withdrawn.**

---

## Instrument Identity

**Full title:** Guidance on Regulatory Principles for Model Risk Management, 2026
**Type:** **Guidance** — hortatory throughout. The operative verb is **"should"** in every substantive paragraph; "shall" does not appear as an obligation-creating term. Contrast [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]], which is SHALL-dense
**Legal basis:** Not stated in the extracted text — no enabling section cited (contrast RBI_3/RBI_13's explicit BR Act s.21/35A/56 and RBI Act s.45JA/45L/45M basis). ⚠ #334
**Supersedes on finalisation:** Chapter 3 (Credit Risk Models) of the **Guidance Note on Credit Risk Management, 12 October 2002**
**Forward reference:** Para 2 cites **"paragraph I.10 of Utkarsh 2029"** and states that *"further requirements, if any, applicable to AI models may be issued later"* — a named future-instrument signal. **Utkarsh 2029 does not exist in this vault** (⚠ #335)
**Reading rule:** Para 5 — to be read with relevant RBI Directions; **"In case of any inconsistency, the applicable Directions shall prevail"**

### Applicability — the broadest of any AI-adjacent RBI instrument in the corpus

Para 4 lists **eleven** regulated-entity categories:

| # | Category |
|---|---|
| i | Commercial Banks (including Foreign Banks) — banking companies, corresponding new banks, SBI |
| ii–iv | Small Finance Banks; Payments Banks; Local Area Banks |
| v | Regional Rural Banks |
| vi–vii | Urban Co-operative Banks; Rural Co-operative Banks (State and Central) |
| viii | NBFCs — **all four layers**: Base, Middle, Upper, Top |
| ix | All-India Financial Institutions — EXIM Bank, NABARD, NaBFID, NHB, SIDBI |
| x | Asset Reconstruction Companies |
| xi | Credit Information Companies |

**Analytically significant.** RBI_8 (binding, 31 Jul 2026) applies to Commercial Banks only, expressly excluding SFBs, Payments Banks and Local Area Banks. RBI_14 (hortatory, June 2026) reaches all of them plus co-operatives, all NBFC layers, AIFIs, ARCs and CICs. **The instrument with the widest perimeter is the one with the weakest deontic force** — see S5.2.

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) primary; S6 (Implementation & Governance Artifacts) secondary
**Jurisdiction:** India
**Confidence:** High for text and content; **the instrument's own status is draft**
**AI explicit:** **Yes — emphatically.** Chapter V.B is a dedicated AI/ML chapter (paras 49–63) naming foundational models, frontier models, generative AI, hallucination, prompt injection, adversarial inputs, red-teaming, data drift, concept drift, automation bias
**Tier classification:** **Tier B** — primary-source draft text, comprehensive, not yet operative. Upgrade to A on notification
**AI Governance Wiki relevance:** **HIGH** — the most AI-specified Indian financial-sector instrument in the corpus by a considerable margin, and the document that most directly refutes the vault's standing "India has no general-purpose model-risk instrument" finding

---

## Substantive Content

### S3.1 Structure

| Chapter | Content | Paras |
|---|---|---|
| I | Preliminary — introduction, applicability (11 RE categories), 8 definitions | 1–7 |
| II | Governance — MRMF, Board, RMCB, Senior Management | 8–13 |
| III | Model Risk Management — tiering, inventory, consumer protection | 14–25 |
| IV | Model Lifecycle — selection/development, validation, approval, deployment/monitoring, change management, BCM/decommissioning | 26–44 |
| V | Specific Models — **A. Third-Party Models (45–48); B. AI/ML Models (49–63)** | 45–63 |
| VI | Other Provisions — supersession | 64 |

### S3.2 The model definition — deliberately expansive

Para 7(3) defines a model by **function, not by label**:

> "…incorporates data, applies theoretical, empirical, or judgement-based assumptions (input component), uses statistical, mathematical, economic, financial, or such other cognitive techniques (**including Artificial Intelligence (AI) / Machine Learning (ML)**) to analyse, interpret relationships and process inputs (processing component) and produce results that are used for business or any other operations and decision making (output component). It includes algorithms, analytics, interfaces, applications, decision-based rules, and other computational tools which, by virtue of their use, have a material impact on decision-making in various business processes, **irrespective of whether such tools are recognised as models by the RE**."

The accompanying **illustration** is the sharpest drafting in the document: a spreadsheet loan-pricing calculator is "only a basic mathematical tool" — until the RE uses it to derive lending rates, at which point it takes inputs (borrower type, tenor, credit score, collateral), applies processing logic (rate grids, risk-weighted spreads, margin formulas) and produces an output that drives business decisions, and **"then it should be considered as a model."**

**This is a functional, use-based definition that closes the self-classification loophole.** An RE cannot escape the framework by declining to call something a model.

### S3.3 The Model Risk definition — and the temporal limb

Para 7(7) defines model risk as arising from three sources:

| Limb | Content |
|---|---|
| (i) **Model errors** | Inappropriate specification, incorrect parameterisation, flawed hypotheses/assumptions, computational errors, inaccurate/inappropriate/incomplete data, inadequate controls, inadequate validation |
| (ii) **Misapplication** | Improper or unintended usage; misinterpretation of outputs |
| (iii) **Time-suitability issues** | **"models becoming less fit / unsuitable over time"** |

**Limb (iii) is a constitutive element of model risk in an Indian regulatory definition, and it is temporal.** See S5.5 — this bears directly on [[04_Knowledge_Products/Wiki_Intake/F142_Azimi_Temporal_Validity_Governance_Age_2026]], intaken the same day.

### S3.4 Governance architecture

**Accountability (para 8):** *"An RE is accountable for the outcomes of all models used by it, irrespective of whether the models are developed internally, sourced from third-parties, or a combination thereof."* Restated for third-party models at para 45. This is the **non-delegable accountability** formulation already recorded across [[07_Institutions/Corpus/SEBI/SEBI_14]] Reg 16C, [[07_Institutions/Corpus/RBI/RBI_7]] and DPDP Rule 13(3).

| Body | Duties |
|---|---|
| **Board** (11) | Approve and periodically review the MRMF; approve risk appetite and tolerance for model risk, **forward-looking and informed by scenario analysis / stress testing**; approve model-risk policies including tiering |
| **RMCB** (12) | Review validation reports for **'high'-tier models and approve their deployment**; review tiering reports at least annually; **oversee models approved with exceptions, third-party models, and models involving AI**; review breach reports |
| **Senior Management** (13) | Operationalise MRMF; implement tiering; maintain inventory and documentation; periodic policy review, report to RMCB |

**Three lines of defence (para 15):** model owners (1st), independent model risk management and validation function (2nd), independent internal audit (3rd) — explicit.

### S3.5 Risk tiering, inventory, retention

**Tiering (paras 17–20).** Reviewed at least annually or on triggers. Drives validation intensity/frequency/method, approval route (high-tier → RMCB), controls, monitoring scope, inventory detail, and BCP. Based on **materiality** (significance to business, financial/operational impact, consumer implications) and **complexity** (difficulty of oversight, unstructured data, explainability challenges).

**Para 20 is a well-drafted anti-gaming clause:** *"the RE should ensure that the integration of multiple factors does not result in one factor offsetting or diluting the other… a low complexity should not result in a disproportionate reduction of the overall risk tiering of a highly material model."*

**Inventory (paras 21–24).** Must cover active, inactive, under-development and decommissioned models. **"It should ensure that no model is used, relied upon, or deployed unless it is part of inventory."** Minimum fields: owners, developers, validators, approvers; risk tier; intended use; **dependencies with upstream and downstream models**; key observations from validation, monitoring and audit.

**Retention (paras 23–24):** decommissioned models retained in inventory for **at least ten years** from decommissioning or from ceasing to serve as backup/benchmark, whichever is later, or longer if law requires. Documentation retention aligned to the same period.

**Consumer protection (para 25):** *"An RE should not use any model that harms consumer"* — an unusually blunt substantive prohibition in a document otherwise written in process terms. Grievance redressal must cover consumer-facing models.

### S3.6 Lifecycle

| Stage | Key provisions |
|---|---|
| **Selection/development (26–28)** | Document rationale, objectives, scope **before** development; weigh costs including *"fairness, ethical considerations, and biasness"*; structured development process; data (empirical **or synthetic**) per RE data governance |
| **Validation (29–33)** | **Independent validation by the RE** for all models including third-party; conducted **prior to and after deployment**, following modification, on internal or external triggers, and periodically; covers inputs, conceptual/design soundness, performance, alignment with intended use; **validation reports to RMCB within three months of completion** |
| **Approval (34–35)** | Approval structure with exception approvals, thresholds, remediation timelines; documented rationale |
| **Deployment/monitoring (36–37)** | Deployment coordinated with IT and data functions; **outputs replicated and stable in production**; ongoing monitoring of all deployed models; **models approved with exceptions subject to enhanced RMCB monitoring** |
| **Change management (38–42)** | Structured process; controlled, enterprise-level implementation with recovery mechanisms; **documented impact assessment before any change**, including continued suitability for intended use; comprehensive change/version/approval log; **RE must define what constitutes a material change, breach of which re-initiates validation and approval** |
| **BCM/decommissioning (43–44)** | Continuity planning within overall BCP — model unavailability, performance degradation, failure; fallback via manual intervention, substitution, back-up; stakeholders informed of decommissioning for enterprise-wide transition |

### S3.7 Third-party models (Chapter V.A) — an explicit refusal of cross-recognition

Para 46(i) requires third-party models to be subject to:

> "independent validation by the RE in accordance with paragraphs 29 to 33 **notwithstanding any validation, certification, or assurance provided by the third-party provider**"

and (ii) **enhanced RMCB oversight irrespective of risk tier**.

Para 47: pre-acquisition due diligence on provider credibility, methodological soundness, limitations, data suitability and quality.

Para 48: contracts must provide **access to minimum technical documentation** sufficient to validate the model per the RE's MRMF; **audit rights for the RE and its supervisory authority**, directly or through external experts; and continuity and exit arrangements.

### S3.8 AI/ML models (Chapter V.B) — the most AI-specified Indian financial text in the corpus

**Risk management (49–57).**

- **49:** define scope of AI/ML models **including foundational and frontier AI models**; additional controls commensurate with impact on customers, operations, financial outcomes
- **50:** deploy only where commensurate risk can be effectively managed
- **51:** where a third-party provider does not disclose adequate information, identify the resulting risks and mitigate, **"such as limiting the usage"**
- **52:** for AI risk tiering, additionally consider **"the extent of reliance and the level of autonomy placed on the model outputs for decision-making"**
- **53:** for material third-party AI models, datasets and dependencies — consider **concentration risk from a limited number of model providers, supply chain risk, limitations in independent validation, and changes in model behaviour or capabilities resulting from provider-driven updates**
- **54(1):** define **explainability and transparency thresholds** for all AI models; higher thresholds for material decision-making or significant customer/operational impact. Where **full explainability is not achievable** — enhanced validation and testing, mechanisms to verify and corroborate outputs before use, frequent validation, continuous monitoring, **usage restrictions**, compensating controls
- **54(2):** control boundaries via system-level controls or model design to mitigate **hallucination**, particularly for generative models and where outputs drive customer interaction or decision-making
- **54(3):** identify bias and discriminatory outputs; **fairness assessment**; mitigants including recalibration or redesign; for complex models consider **constraining complexity (e.g. regularisation) and limiting feature selection**
- **54(4):** no overfitting; out-of-sample and varied-scenario performance assessment
- **54(5):** no reliance on **spurious correlations or unintended relationships**
- **54(6):** outputs under similar inputs should not exhibit **excessive or unexplained variation**; manage stochastic behaviour and model uncertainty via **confidence scores and probability outputs**
- **54(7):** data risks — quality, non-representativeness, incompleteness, **breach of intellectual property rights**; **data drift and concept drift monitored and addressed on an ongoing basis**
- **55:** structured challenge processes **including red-teaming or equivalent**, particularly for customer-interaction or generative models
- **56:** enhanced controls for models with **dynamic or automatic updates** — *"defining a clear scope of what can be updated automatically, strict justifications for enabling automatic updates, enhanced data quality checks, and more stringent and frequent monitoring"*
- **57:** enhanced documentation for AI models given complexity, **self-adapting nature** and training-data reliance, to enable **traceability, reproducibility, and auditability**

**Deployment controls (58–59).** Access controls against unauthorised access/use/modification; cyber safeguards; controls for external interfaces, APIs and integration pipelines. For customer-facing models including generative AI: controls against **prompt injection and adversarial inputs**, **limitations on session and context persistence**, **anomalous usage detection**; **disclosure that the user is interacting with an AI/ML system, with its limitations**; and **an option to switch to human assistance on request**.

**Human oversight (60–63).**

- **60:** robust human oversight for AI models **including automated decision-making use cases**, with mitigants including (i) **human-in-command arrangements** (human-in-the-loop / human-on-the-loop / other), (ii) **override, suspension, or deactivation mechanisms including kill-switch arrangements**, (iii) periodic human review of model outputs and model-driven decisions to identify anomalies
- **61:** oversight must consider **automation bias, over-reliance on model outputs, and decision fatigue**
- **62:** oversight personnel must possess **adequate expertise and understanding of model functioning** and be **able to effectively challenge, override, or escalate**
- **63:** oversight arrangements — **including decisions, interventions, overrides, incidents and near misses** — periodically reviewed and strengthened based on experience

---

## Analytical Significance for PRIS Research

### S5.1 — India now has a general-purpose model-risk instrument. The vault says it does not.

[[05_Concepts/05_Concepts_Standard/Model_Risk]] records as a **confirmed finding**: *"India has no single, general-purpose, binding instrument equivalent to SR 26-2 or SS1/23. What exists is (a) a draft, credit-scoped circular on traditional statistical model risk, and (b) a non-binding Committee Report,"* and lists under Confirmed Absences: *"No Indian general-purpose model-risk instrument."*

**RBI_14 requires that to be rewritten.** It is general-purpose (all models, all RE types), comprehensive (governance, tiering, inventory, full lifecycle, third-party, AI/ML, human oversight), and materially more AI-specified than SR 26-2 — which *excludes* generative and agentic AI — or SS1/23.

The precise corrected finding: **India now has a general-purpose model-risk instrument that is more AI-inclusive than the US or UK equivalents, and it is hortatory and in draft.** The vault's existing diagnosis — *"India's problem here is bindingness, not conceptual scope"* — was correct in substance and is now confirmed by a much stronger instance than the credit-scoped draft it was based on.

### S5.2 — Deontic-Placement Debt: the pattern is now three-for-three

[[05_Concepts/05_Concepts_Signature/Governance_Debt]] §Deontic-Placement Debt records RBI placing AI content in a hortatory instrument while the binding instrument on the same subject omits it, using RBI_9 (June 2026 advisory) → RBI_8 (31 July 2026 Directions, AI-silent).

**RBI_14 is a third data point in the same quarter, and it makes the pattern systematic rather than incidental:**

| Instrument | Date | Deontic force | AI content | Perimeter |
|---|---|---|---|---|
| [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | June 2026 | Advisory, apparently unpublished | **AI-explicit** | REs |
| **RBI_14 (this node)** | June 2026 | **Draft Guidance — "should"** | **AI-explicit, dedicated chapter** | **11 RE categories — the widest** |
| [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | 31 July 2026 | **Binding Directions — "shall", in force on issuance** | **Zero AI provisions** | Commercial Banks only |

Within roughly six weeks, RBI produced two AI-explicit non-binding instruments and one AI-silent binding one. **The instrument with the strongest deontic force has the narrowest perimeter and no AI content; the instruments with the widest perimeter and richest AI content have the weakest force.** That is a systematic inverse relationship between bindingness and AI coverage within a single regulator in a single quarter, and it is a materially stronger claim than the two-instrument version.

It is also a clean [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] instance with an explicit forward reference: para 2's *"further requirements, if any, applicable to AI models may be issued later"* is the regulator stating that binding AI requirements remain deferred.

### S5.3 — Human oversight: the largest India/EU specification gap in the corpus is closed

[[05_Concepts/05_Concepts_Standard/Human_Oversight]] records a **specification-gap finding**: the EU AI Act devotes four paragraphs and five enumerated sub-conditions to human oversight while *"the two Indian instruments that address it use a single unelaborated noun phrase each,"* and concludes this is *"the largest India/EU gap of any construct in the EA cluster — larger than fairness, larger than explainability."*

**Paras 60–63 close that gap, and on one dimension exceed Art. 14(4):**

| EU AI Act Art. 14(4) | RBI_14 equivalent |
|---|---|
| (a) capacity to understand the system's capacities and limitations | **62** — personnel possess "adequate expertise and understanding of model functioning" |
| (b) awareness of and countermeasures against automation bias | **61** — "automation bias, over reliance on model outputs and **decision fatigue**" |
| (c) ability to correctly interpret output | **60(iii)** — periodic human review of outputs and model-driven decisions to identify anomalies |
| (d) ability to decide not to use, override, or reverse | **60(ii)** — override, suspension, or deactivation |
| (e) ability to intervene or halt (stop function) | **60(ii)** — **kill-switch arrangements** |
| — | **60(i)** — human-in-command taxonomy (HITL / HOTL / other) — **no Art. 14(4) equivalent** |
| — | **63** — oversight arrangements including **interventions, overrides, incidents and near misses** periodically reviewed and strengthened — **a learning loop Art. 14(4) does not require** |

**Decision fatigue and the near-miss learning loop are not in Art. 14(4).** On specification density for human oversight, this draft is at parity with the EU AI Act and arguably ahead.

**The correction to record is precise:** the specification gap was real when measured against RBI FREE-AI and NCAIC_1. It does not survive RBI_14. What survives is the **bindingness** gap — Art. 14 is binding law; this is draft guidance. That is the same diagnosis S5.1 reaches independently, from a different construct, which is a useful convergence.

⚠ Consequence for the D4 fsQCA calibration: the bespoke Art. 14(4) five-item coding scheme would now score India substantially higher than the note assumes, **if instrument text is what is being coded**. Whether a draft counts is a calibration decision that must be made explicitly, not by default.

### S5.4 — Assurance Reuse Gap: refusal of cross-recognition, in regulatory text

[[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] documents non-cross-recognition largely as an **absence** — regulators do not provide for reuse of assurance artefacts across regimes, and the gap is inferred from silence.

**Para 46(i) is not silence. It is an express refusal:** third-party models require independent validation by the RE *"notwithstanding any validation, certification, or assurance provided by the third-party provider."*

This is the corpus's **first instance of a regulator affirmatively excluding reliance on external assurance in the instrument text**, rather than merely failing to permit it. It converts the construct's central claim from an inference about regulatory silence to a documented regulatory choice, and it is considerably harder to argue away. Para 48's requirement that contracts secure audit rights *for the RE and its supervisory authority* reinforces the same posture: assurance must be re-performable by the accountable party and its regulator, not accepted from the vendor.

Note the tension with the vendor-side reality captured at [[06_Frameworks/ISO_IEC_42001]]: a market in AI management-system certificates is expanding, and the regulator that matters for Indian BFSI has pre-emptively declined to treat such certificates as discharging validation.

### S5.5 — Temporal validity appears in Indian regulatory text, the same day F142 argues it is under-theorised

[[04_Knowledge_Products/Wiki_Intake/F142_Azimi_Temporal_Validity_Governance_Age_2026]] (intaken 2026-08-09) argues that **temporal validity** is an under-theorised dimension of governance and that governance instruments treat time as an administrative scheduling variable rather than a theoretical dimension.

RBI_14 para 7(7)(iii) makes **"time-suitability issues (models becoming less fit / unsuitable over time)"** one of three constitutive limbs of the definition of model risk — not a review-scheduling provision, but part of what model risk *is*. Para 54(7) requires **data drift and concept drift** to be monitored and addressed on an ongoing basis. Para 40 requires a documented impact assessment before any change including **"the continued suitability of the model for its intended use."** Para 56 imposes enhanced controls on **dynamic or automatic updates**.

**This is a partial counter-instance to F142's gap claim, and a valuable one.** RBI is not merely scheduling reviews; it names temporal degradation as a risk category and requires continuous monitoring of the specific mechanisms (drift) by which representational correspondence decays. F142's claim survives in modified form — RBI names the phenomenon without theorising *representational correspondence* as such, and the paper's distinction between compliance and representational accuracy is not present — but the claim that regulators treat time only as an administrative variable does not hold against this text. **Record in F142 rather than leaving its gap claim unqualified.**

### S5.6 — Decision Infrastructure: a partial counter-instance

[[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] (created 2026-08-09) argues that governance takes the model as its unit and does not reach the chain through which an output becomes an institutional act.

**Para 22 requires the model inventory to record "dependencies with upstream and downstream models."** That is chain-awareness in regulatory text, and the construct should acknowledge it. Para 36 (deployment coordinated with IT and data functions; outputs replicated and stable in production) and para 39 (changes implemented "at enterprise level") reach further toward the workflow layer than any other Indian instrument in the corpus.

**What it still does not do:** it governs dependencies *between models*, not the handoffs from model to workflow to decision to action. There is no requirement to record who configured a threshold, no treatment of a threshold change as a policy change, and no decision-provenance obligation. **The construct's H2 handoff (workflow → decision) remains ungoverned; H1 (model → workflow) is now partially reached.** Record as a boundary refinement, not a refutation.

### S5.7 — Retention: a 10-year horizon from a fourth regulator-instrument

Para 23's **ten-year retention for decommissioned models** (from decommissioning or from ceasing to serve as backup/benchmark, whichever is later) is a new entry for [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]], and it matches the EU AI Act Art. 47 ten-year Declaration-of-Conformity horizon at the top of the corpus spread. Para 24 aligns documentation retention to the same period.

Note the intra-RBI incoherence this creates: RBI_8 (binding, July 2026) specifies **no retention period at all** while RBI_14 (guidance, June 2026) specifies ten years for model records. The same regulator, six weeks apart, at opposite ends of the construct's range — reinforcing the [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] finding that retention specification is a drafting choice rather than a constraint.

### S5.8 — Agentic AI: named, but obliquely

Para 52 requires AI risk tiering to consider **"the extent of reliance and the level of autonomy placed on the model outputs for decision-making"** — autonomy as a tiering dimension, structurally similar to IMDA's L1–L4 scale ([[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]]). Para 49 names **foundational and frontier AI models**. Para 57 refers to models' **"self-adapting nature."** Para 56 governs **automatic updates**, requiring a defined scope of what may update without human action.

**But there is no agent, no orchestration, no delegation grant, and no multi-agent provision.** Para 56 is the nearest thing in Indian regulation to workflow authorisation and it is scoped to model self-updating, not to agent workflows. For [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] this is a near-miss worth recording: RBI has the autonomy vocabulary and applies it to *how much weight a model's output carries*, not to *what an autonomous actor is permitted to do*.

---

## Regulatory Units — selected

| RU | Obligation | Deontic | ADICO summary |
|---|---|---|---|
| RU1 | RE accountable for outcomes of all models, however sourced (8, 45) | **SHOULD** (framed as a statement of accountability) | A=RE; D=is accountable; I=outcomes of all models; C=internal, third-party or hybrid |
| RU2 | Board-approved MRMF covering all models including AI/ML (9) | SHOULD | A=RE; D=SHOULD; I=put in place Board-approved MRMF; C=all models regardless of source |
| RU3 | No model used or deployed unless in inventory (21) | SHOULD | A=RE; D=SHOULD; I=ensure no model used, relied upon or deployed; C=unless part of inventory |
| RU4 | Independent validation of third-party models notwithstanding vendor certification (46(i)) | SHOULD | A=RE; D=SHOULD; I=independently validate; C=third-party models; **O=absent**; explicitly non-substitutable by vendor assurance |
| RU5 | 10-year retention of decommissioned models in inventory (23) | SHOULD | A=RE; D=SHOULD; I=retain in inventory ≥10 years; C=from decommissioning or cessation as backup/benchmark, whichever later |
| RU6 | High-tier models require RMCB approval before deployment (12(1), 18(ii)) | SHOULD | A=RMCB; D=SHOULD; I=review validation report and approve deployment; C=models tiered 'high' or equivalent |
| RU7 | Explainability thresholds defined; enhanced controls where full explainability unachievable (54(1)) | SHOULD | A=RE; D=SHOULD; I=define thresholds, apply higher for material decisions, apply compensating controls incl. usage restrictions; C=all AI models |
| RU8 | Kill-switch / override / suspension mechanisms (60(ii)) | SHOULD | A=RE; D=SHOULD; I=establish override, suspension, deactivation incl. kill-switch; C=AI models incl. automated decision-making |
| RU9 | Customer disclosure of AI interaction with option to switch to human (59(ii)–(iii)) | SHOULD | A=RE; D=SHOULD; I=disclose AI interaction and limitations; provide human-assistance option; C=models interfacing with customers or external users |
| RU10 | RE should not use any model that harms consumer (25) | SHOULD | A=RE; D=SHOULD NOT; I=use a model that harms consumer; C=unconditional — the document's only absolute prohibition |

**Deontic observation.** Uniformly **SHOULD**. There is no SHALL, no penalty, no reporting obligation to RBI, and no supervisory consequence stated anywhere in 64 paragraphs. Para 5's inconsistency rule (*"the applicable Directions shall prevail"*) positions the whole document as subordinate to binding instruments. **RU10 is the only prohibition and it is also the least operationalised** — "harms consumer" is undefined, with no threshold, test or process attached.

---

## ⚠ VERIFY Flags

- **⚠ #334 (MEDIUM).** **No legal basis is cited anywhere in the extracted text.** RBI_3/RBI_13 (the 2024 credit-scoped draft) expressly invoked BR Act ss.21, 35A, 56 and RBI Act ss.45JA, 45L, 45M. This document invokes nothing. Whether that is a draft artefact or a deliberate signal that the instrument is issued as non-statutory guidance is material to its eventual force — confirm against the final notification.
- **⚠ #335 (MEDIUM).** Para 2 cites **"paragraph I.10 of Utkarsh 2029"** as the source of a commitment that further AI-model requirements may follow. **Utkarsh 2029 is not in this vault.** It is RBI's medium-term strategy framework and is the named forward-reference for binding Indian AI model regulation. **Source it** — it is the closest thing the corpus has to a dated signal of RBI's AI regulatory roadmap.
- **⚠ #336 (MEDIUM).** Draft status: reference number and date are unfilled placeholders, and para 64 confirms public consultation is pending. **Do not cite as operative.** Track for notification; on notification this becomes Tier A and the Model_Risk correction at S5.1 strengthens further.
- **⚠ #337 (LOW-MEDIUM).** The document supersedes only **Chapter 3 of the 2002 Credit Risk Management Guidance Note** on finalisation. Its relationship to the **2024 credit-scoped draft** ([[07_Institutions/Corpus/RBI/RBI_3]] / [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]]) is **not stated**. Whether RBI_14 supersedes, absorbs, or runs parallel to that draft is unresolved and affects how the 2024 draft should be treated in the corpus.
- **⚠ #338 (LOW).** Source is a text extraction with Devanagari header corruption in the masthead. All provisions cited were read from the English body, which extracted cleanly. Paragraph numbers were checked against the table of contents. Verify against the RBI-hosted PDF before quoting verbatim.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] (binding, AI-silent — the deontic contrast) | [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] | [[07_Institutions/Corpus/RBI/RBI_7]] | [[07_Institutions/Corpus/RBI/RBI_3]] and [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]] (the 2024 credit-scoped predecessor — **note these two nodes duplicate each other**, see the Log) | [[07_Institutions/Corpus/SEBI/SEBI_14]] | [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] | [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]]
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Model_Risk]] | [[05_Concepts/05_Concepts_Standard/Human_Oversight]] | [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] | [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Standard/Explainability]] | [[05_Concepts/05_Concepts_Standard/Fairness]] | [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] | [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Standard/Contestability_Redress]]
**Related frameworks:** [[06_Frameworks/RBI_Free_AI]] | [[06_Frameworks/EU_AI_Act]] | [[06_Frameworks/ISO_IEC_42001]] | [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]]
**Related intake notes:** [[04_Knowledge_Products/Wiki_Intake/F140_Joshi_Preventing_AI_Assisted_Cyber_Attacks_ISC2_Keynote_2026]] (⚠#306 closed by this node) | [[04_Knowledge_Products/Wiki_Intake/F142_Azimi_Temporal_Validity_Governance_Age_2026]] (partial counter-instance)
**Related domains:** [[03_Domains/BFSI_Governance]] | [[03_Domains/AI_Governance]]
**Related institutions:** [[07_Institutions/RBI]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]] (**high** — general-purpose, AI-explicit, 11-category perimeter) | [[02_Projects/P4_Doctrinal_IJLIT]] (**high** — the bindingness/scope inversion) | [[02_Projects/fsQCA_Thesis_Chapter]] (EA/RL calibration affected — see S5.3)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]] | [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]

---

## Coding Status

- **P3 NVivo:** **High-priority addition.** General-purpose, AI-explicit, widest RE perimeter in the corpus. 64 enumerated paragraphs, deontically uniform (SHOULD) — a clean comparator against RBI_8's SHALL-density for deontic analysis.
- **IG 2.0 / ADICO:** high-yield. Note the **absent Or-else** across all 64 paragraphs — a striking uniform feature for coding.
- **Wiki intake status:** Pending — High priority.

---

## Log

- 2026-08-09: Corpus node created from full draft text supplied by Vivek. **Not a duplicate** — distinct from the 2024 credit-scoped draft in scope (all models vs credit models), date (June 2026 vs 5 Aug 2024), department code (DoR.ORG.REC vs DoR.STR.REC) and supersession target (2002 Credit Risk Guidance Note Ch.3). ✅ **Closes ⚠#306** — the "unfilled placeholder citation" flagged on F140 is in the RBI draft itself, not an error by the deck author; the "possibly illustrative" characterisation is withdrawn. Six findings recorded: **India now has a general-purpose model-risk instrument, contradicting [[05_Concepts/05_Concepts_Standard/Model_Risk]]'s Confirmed Absences** (S5.1); the Deontic-Placement Debt pattern becomes three-for-three within one quarter, with an **inverse relationship between deontic force and AI coverage** (S5.2); the **largest India/EU specification gap in the corpus — human oversight — is closed and on two dimensions exceeded** (S5.3); **the corpus's first express regulatory refusal of third-party assurance reuse** (S5.4); **temporal validity appears in Indian regulatory text** as a constitutive limb of the model-risk definition, a partial counter-instance to F142 intaken the same day (S5.5); and **partial chain-awareness** via upstream/downstream model dependencies, refining rather than refuting [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] (S5.6). Five VERIFY flags (#334–#338).
- 2026-08-09 (**vault-quality finding, not about this document**): duplicate-check for this node surfaced that **[[07_Institutions/Corpus/RBI/RBI_3]] and [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]] are the same instrument** — both the Draft Circular *Regulatory Principles for Management of Model Risks in Credit*, 5 August 2024, DOR.STR.REC./21.04.048/2024-25. RBI_3 was created earlier; RBI_13 was created 2026-08-02 during the model-risk sourcing pass without a duplicate check against RBI_3. This is a **duplicate-detection debt** instance in the sense recorded at [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (cf. SEBI_16/SEBI_14). **Flagged, not merged** — per the standing duplicate protocol, reported only. Resolution is Vivek's call: RBI_13 carries better sourcing metadata and the Model_Risk linkage; RBI_3 carries the legal-basis detail and the RBI_FREE_AI companion note. A merge would need both.
