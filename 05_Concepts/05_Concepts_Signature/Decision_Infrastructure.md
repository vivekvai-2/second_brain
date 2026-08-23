---
type: Signature Concept
status: candidate
last_updated: 2026-08-09
tags:
  - type/concept-signature
  - status/candidate
  - concept-class/candidate
  - paper/p3
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/linkedin
  - engine/knowledge-product
  - content/carousel-ready
  - content/thought-leadership
concept_class:
  - candidate
linked_domains:
  - "[[03_Domains/BFSI_Governance]]"
  - "[[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]"
  - "[[03_Domains/Healthcare_Governance]]"
  - "[[03_Domains/AI_Governance]]"
---

# **Decision Infrastructure**

**Type:** Signature Concept (candidate class) **Status:** Candidate — Three-Instance Gate **PASSED**; elevation to signature pending use in P3 or P4 **Created:** 2026-08-09
**Theoretical lineage:** Institutional theory (decoupling; Meyer & Rowan 1977); infrastructure studies (Star & Ruhleder — infrastructure as relational and visible on breakdown); sociotechnical systems; regulatory governance
**Origin:** *Decision Infrastructure Series, Release 0.1* — framework authored by Vivek, 2026-08. Formalised as a vault construct 2026-08-09.

---

## **Definition**

**One-sentence definition.** Decision Infrastructure is the chain through which an AI output becomes an institutional act — data → model → workflow → decision → action — and the claim the construct makes is that institutional risk is generated at the **handoffs**, not in the model.

**Full analytical definition.** Governance regimes for AI overwhelmingly take the *model* as their unit of assessment: validation, versioning, bias testing, explainability, model risk management. Decision Infrastructure holds that this unit is misplaced for institutional risk, because a model produces a recommendation whereas an institution produces a **decision that binds someone** — a loan refused, a patient escalated, a benefit denied, load redispatched. Between the two lie workflow integration, threshold configuration, escalation rules, override paths, and execution, and it is at these handoffs that accountability dissolves: the model was validated, the operator followed the workflow, the workflow was configured by someone else, and no one owns the outcome. The construct's diagnostic claim is that this failure is **sector-invariant** — the same structure recurs in banking, power, healthcare and public administration with different content and identical form.

**Plain-language practitioner definition.** The model is not the risk. The decision without control is.

---

## **The problem the concept solves**

The vault already documents the *symptom* from two directions and lacks the construct that connects them.

[[05_Concepts/05_Concepts_Signature/Governance_Debt]]'s **infrastructure-layer** sub-pattern (2026-08-02) records that ~~NPCI runs federated AI fraud scoring across UPI~~ *(refuted 2026-08-15, ⚠#361 — read as **NPCI's EFRM issuing ecosystem-level fraud alerts member banks are directed to prioritise**)* and Grid-India runs day-ahead demand forecasting on the national grid, with ~~**no governance instrument reaching either**~~ *(also restated: `RBI/DPSS/2024-25/123` **does** reach NPCI, from 1 Apr 2025, and carries no AI provision — **no AI instrument** reaching either)* — concluding that "India regulates AI at the regulator layer and not at the infrastructure-operator layer." That is an accurate catalogue of absence. It does not explain *why* the model is the wrong thing to have been regulating in the first place.

[[05_Concepts/05_Concepts_Standard/Model_Risk]] records the opposite move from the US side: SR 26-2 (Fed/OCC/FDIC, April 2026) **carves generative and agentic AI out of model risk scope entirely**, drawing the boundary at generative/agentic vs everything else. A mature supervisor concluded that the model-centred apparatus does not fit — without supplying a replacement unit.

Decision Infrastructure supplies the replacement unit. It is not a catalogue of gaps; it is a claim about **where the governable object actually sits**, and it generalises P3's BFSI-specific parallelism finding across sectors by identifying what those sectors share.

---

## **Constitutive dimensions — the five-stage chain and its four handoffs**

| Stage | What it is | Handoff risk to the next stage |
|---|---|---|
| **Data** | Raw facts and signals | Provenance, representativeness, and currency of the inputs the model will treat as ground truth |
| **Model** | Patterns and predictions | **H1: model → workflow.** The recommendation's confidence, uncertainty and caveats are stripped as it enters a business process that expects a value |
| **Workflow** | Business process integration | **H2: workflow → decision.** Thresholds, routing and escalation rules — typically configured by engineering, not by risk — determine which recommendations become decisions |
| **Decision** | Recommendation or choice | **H3: decision → action.** Whether a human meaningfully intervened, and whether that intervention is distinguishable from a rubber stamp |
| **Action** | Administrative or operational effect | **H4: action → accountability.** Whether the executed act can be attributed to an approved authority and reconstructed afterwards |

**H2 carries the construct's analytical weight.** A threshold change is a policy change — it alters who gets credit, who gets escalated, whose outage is restored first — and it is almost never governed as one. It requires no model revalidation, generates no governance event, and leaves no approval trail. Vivek's own worked example: *"AI changes a borrower's risk score overnight. Risk: credit policy changes silently."*

---

## **Three-Instance Gate — PASSED (2026-08-09)**

Per [[00_MOC/Workflow_Discipline_Protocol]] CDW-1, entry requires three distinct primary-source corpus instances **or** theoretical load-bearing in an active paper. **Both limbs are satisfied.** Every node cited was verified present in the vault on 2026-08-09.

| # | Corpus node | Sector | What it instantiates |
|---|---|---|---|
| **1** | [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] + [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] | Power | **The construct's cleanest instance, and it is now binding-instrument evidence.** Grid-India runs day-ahead demand forecasting (ANN, XGBoost, 2–5% MAPE) on the national grid, confirmed by the Ministry of Power in a Rajya Sabha reply of 18 Dec 2023. CEA_3 (notified 31 Jul 2026) governs that technology estate **comprehensively** — cyber assets, critical systems, OT/IT separation, perimeter devices, supply chain, time synchronisation — across 17 regulations, and contains **zero provisions on what the systems running on that estate decide**. The forecasting model is governed as an asset to be inventoried and secured, not as a decision to be validated, explained or attributed. Estate governed; decisions ungoverned. |
| **2** | [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]] ✅ *primary-sourced 2026-08-15; ~~federated AI fraud scoring~~ **restated** — see ⚠#322* | BFSI / payments | **Ecosystem-level fraud alerts member banks are directed to prioritise**, i.e. a decision input crossing an institutional boundary; NPCI inside the cyber perimeter, outside every AI perimeter — a score produced by one operator that conditions decisions taken by many banks. No circular, policy paper, technical standard or framework reaches it. The decision (declining or flagging a transaction) is taken by a member bank on an input it did not generate and cannot inspect: **the handoff crosses an institutional boundary and no instrument follows it across.** ⚠ Evidence base is trade reporting and promotional material, not a primary instrument — see VERIFY #322. |
| **3** | [[07_Institutions/Corpus/ICMR/ICMR_1]] | Healthcare | Eight-principle ethical framework covering privacy, accountability, transparency and data governance, with **seven differentiated stakeholder categories** — the most detailed obligation mapping in the domestic corpus — and **no enforcement mechanism attached to any of them**, and no provision governing the point at which an AI recommendation becomes a clinical decision. Architecture without enforcement, at exactly the handoff the construct identifies. |
| **4** | [[07_Institutions/Corpus/SEBI/SEBI_14]] Reg 16C + [[07_Institutions/Corpus/RBI/RBI_7]] | BFSI | The **negative-space instance**, and the most analytically useful. Both instruments attach **non-delegable accountability** to the regulated entity for AI outputs — sole responsibility regardless of the tool's origin. Accountability is therefore fixed at the *entity* level while nothing governs the *chain* through which the output became a decision. The entity answers for an outcome produced by handoffs it is under no obligation to control, document, or be able to reconstruct. **This is Decision Infrastructure stated as a liability asymmetry.** |
| **5** | [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] (F020) | BFSI / credit | Automated decision-making in Indian credit scoring: privacy-by-design obligations under DPDP implemented **without corresponding algorithmic-accountability-by-design obligations** under RBI's framework. The input side of the chain is governed; the decision side is not. |

**Theoretical load-bearing.** The construct generalises [[02_Projects/P3_BFSI_JEIM]]'s BFSI-specific regulatory-parallelism finding by identifying the sector-invariant structure beneath it, and supplies [[02_Projects/P4_Doctrinal_IJLIT]] with a unit-of-governance argument (why the model is the wrong object) distinct from its existing fragmentation critique.

**Cross-sector scope is the point.** Four sectors — power, payments, healthcare, credit — with different regulators, different instruments, different risk vocabularies, and the identical structural gap. That breadth is what makes it a signature-class candidate rather than a BFSI sub-pattern.

---

## **Intersection with signature constructs**

**[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]].** Reframes what parallelism is *about*. The existing finding is that regulators issue functionally equivalent obligations over the same object without coordination. Decision Infrastructure suggests they have been coordinating-or-failing-to-coordinate over the **wrong object**: multiple regulators governing models in parallel, none governing decisions at all. Cross-regulator parallelism and the decision-layer gap are then the same phenomenon seen from two angles — horizontal duplication at the model layer, vertical absence at the decision layer.

**[[05_Concepts/05_Concepts_Signature/Governance_Debt]].** Supplies the explanation the infrastructure-layer sub-pattern lacks. That sub-pattern records that instruments do not reach infrastructure operators. Decision Infrastructure says *why that keeps happening*: instruments are drafted around entities and assets, and a decision chain is neither — it crosses systems, teams and sometimes institutions, so no drafting convention picks it up.

**[[05_Concepts/05_Concepts_Signature/Institutional_Coherence]].** A coherence test at a layer the two-layer model does not reach. India has horizontal infrastructure coherence (CERT-In as shared audit and reporting substrate) and vertical substantive incoherence (sectoral rule-making without cross-reference). Decision Infrastructure identifies a **third axis**: coherence *along the chain* within a single entity — whether the model owner, workflow owner, decision owner and action owner are governed by mutually consistent obligations. On current coding, no Indian instrument governs more than one of those roles.

**[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]].** The two are complements. Decision Infrastructure identifies *where* accountability dissolves; Evidentiary_Governance identifies *what artefact would have to exist* to prove it did not. The handoff points H1–H4 are precisely the junctures for which no instrument in the corpus specifies a retained artefact — see [[06_Frameworks/Evidentiary_Destination_Matrix]].

**[[05_Concepts/05_Concepts_Standard/Orchestration_Governance]].** The narrower sibling. Orchestration Governance is Decision Infrastructure applied to the specific case where the workflow layer is *itself* automated by an agentic harness. Decision Infrastructure is the general claim (the chain is the governable object); Orchestration Governance is the acute case (the chain composes itself at machine speed).

---

## **Sector-invariance table**

The claim that this is one pattern rather than four coincidences:

| Sector | The decision | The risk at the handoff | Accountability effect |
|---|---|---|---|
| **BFSI** | Approve or decline an SME loan | AI changes a borrower's risk score overnight | Credit policy changes silently; accountability becomes unclear |
| **Power** | Redispatch load; prioritise outage restoration | Predicted impact diverges from field reality | Public impact with no attributable decision-maker |
| **Healthcare** | Escalate to ICU; delay surgery | Clinical outcome varies from prediction | Responsibility blurred between clinician and system |
| **Public administration** | Benefit eligibility | Eligibility rules encoded in workflow, not in policy | Citizen has no decision to contest |
| **Pharma / manufacturing** | Manufacturing deviation disposition | Deviation classification determines regulatory consequence | Quality decision made by configuration |

Different risks. Same root cause: **governance failures occur in workflows, not in models.**

---

## **The Data stage gets its first dated, detailed primary-source instrument (2026-08-09)**

Every instance in the Three-Instance Gate above evidences the **Model**, **Workflow** or **Decision** stages of the chain, or the handoffs between them. None reached the **Data** stage itself — the construct's own prescriptive section (below) is explicit that none of its five requirements are drawn from an existing instrument.

[[07_Institutions/Corpus/RBI/RBI_16_Draft_Guidance_Data_Governance_2026]] (draft, July 2026) is the first to close part of that gap. It requires: foundational metadata at the point of capture — source system, purpose, owner, classification (para 48); a **single, non-competing Source of Truth** for every data element, with a mandated reconciliation mechanism against downstream data (paras 43–46); and metadata updates on every transformation, recording "relationship between source and transformed or derived data" (para 51). Read together with [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] (which governs the Model stage in comparable detail), the corpus now has dated, primary-source, instrument-level evidence for **two of five stages** — Data and Model — issued by the same department one month apart.

**This sharpens the construct's central claim rather than weakening it.** The two instruments do not cite each other (see [[05_Concepts/05_Concepts_Signature/Governance_Debt]]'s new Uncited-Adjacency Debt sub-pattern), and neither reaches the **Model → Workflow handoff (H1)** or beyond. Two adjacent stages are now governed in isolation from each other and from everything downstream — data governed, model governed, the handoff between them and everything after it (workflow, decision, action) exactly as ungoverned as before. The instances **narrow** the construct's applicability (it can no longer claim the Data stage is wholly unaddressed in India) while **strengthening** its diagnostic claim (governance stops precisely at each stage's boundary and does not follow the chain across it).

## **What would have to be governed**

The construct's prescriptive content, kept deliberately short because it is the least evidenced part:

1. **Handoff ownership** — a named owner for each of H1–H4, distinct from the model owner
2. **Threshold change control** — configuration changes that alter decision outcomes treated as policy changes, with approval and record
3. **Decision provenance** — the ability to reconstruct which model version, which threshold, which workflow and which human action produced a specific institutional act
4. **Intervention evidence** — records distinguishing meaningful human intervention from rubber-stamping (connects to [[05_Concepts/05_Concepts_Standard/Human_Oversight]]'s nominal/effective boundary)
5. **Cross-boundary attribution** — where a decision input is produced by another institution (NPCI), an obligation that follows the input across the boundary

⚠ None of these is drawn from an existing instrument. They are derived from the construct, not observed — flagged accordingly at VERIFY #323.

---

## **Reuse across the output pockets**

- **Research (R):** generalising frame for [[02_Projects/P3_BFSI_JEIM]]; unit-of-governance argument for [[02_Projects/P4_Doctrinal_IJLIT]]; the sector-invariance table is a clean comparative figure. A cross-sector paper on decision-layer governance absence has no direct competitor located in the corpus.
- **Consulting (C):** the five-stage chain is a diagnostic instrument — walk a client's actual deployment through data → model → workflow → decision → action and identify who owns each handoff. Directly usable for AEGIS_OS and PrivacyWeave scoping, both of which are runtime-enforcement products addressing H3/H4.
- **Thought leadership (TL):** Release 0.1 is written and published; see [[11_Content/Content_Correction_Register]] W-03 for the caveat to carry.
- **Knowledge product (KP):** cross-sector chapter candidate for [[04_Knowledge_Products/Regulatory_Complexity_Handbook]]; the diagnostic belongs in [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]].

---

## **Open research questions**

**OQ-DI-01.** Is the model-as-unit-of-governance choice a drafting artefact (models are nameable and inspectable; chains are not) or a deliberate scope limitation? SR 26-2's carve-out is evidence that at least one supervisor considered the question and declined to extend.

**OQ-DI-02.** Does any jurisdiction govern a decision chain rather than a model or a system? The EU AI Act's "AI system" unit is closer than India's but still an artefact, not a process. **Not yet checked** — this is the single most important comparative gap for the construct's novelty claim.

**OQ-DI-03.** Where a decision input crosses an institutional boundary (NPCI → member bank), does any Indian instrument follow the obligation across? Account Aggregator (RBI_11, DEPA) is the nearest architecture with an explicit cross-institutional data-flow governance model and should be checked as a possible counter-example.

**OQ-DI-04.** Can the four handoffs be operationalised for IG 2.0 / ADICO coding — i.e. is there an ADICO statement form that captures a handoff rather than an actor's obligation? If not, the construct may resist the vault's primary coding method, which is a methodological constraint worth knowing early.

---

## **⚠ VERIFY**

- **✅ ⚠#322 — CLOSED 2026-08-15, with the instance restated.** [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]] now exists, built on three primary NPCI documents. **But primary sourcing did not support the instance as written.** The claim inherited from Governance_Debt — *"NPCI runs federated AI fraud scoring across UPI"* — is **not evidenced**: no NPCI document describes federated learning, and the Best Practices document's AI/ML exhortation is addressed to **member banks**, not to NPCI's EFRM system (⚠#361). The only NPCI AI system named as live or piloted is the **UPI Help Assistant**, a grievance-resolution SLM — not fraud scoring.
  **The restated instance, which the gate does not need weakened:** NPCI's EFRM produces **ecosystem-level fraud alerts that member banks are directed to act on with priority** — a decision input crossing an institutional boundary — while NPCI sits **inside** a binding cyber-resilience perimeter (`RBI/DPSS/2024-25/123`, Large Non-Bank PSO, from 1 Apr 2025) and **outside every AI-governance perimeter**, because RBI's AI instruments bind Regulated Entities and NPCI is a PSO, not an RE. **Whether the input was produced by a model or a rule engine does not change the accountability structure — which is the construct's own argument.** The instance is stronger for being narrowed: it no longer depends on an unverified technical characterisation.
- **~~⚠ #322 (MEDIUM).~~** *(original)* The NPCI instance rests on trade reporting and promotional material, **not on a primary instrument or a corpus node** — [[07_Institutions/NPCI]] is an institution file, and no NPCI corpus node exists. It is the weakest of the five gate instances. **Create an NPCI corpus node, or drop this instance and rely on the other four**, before the gate is cited in publication-track output. The gate passes without it.
- **⚠ #323 (MEDIUM).** The five prescriptive requirements ("What would have to be governed") are **derived from the construct, not observed in any instrument.** Present as proposal, never as a description of existing obligations.
- **⚠ #324 (MEDIUM).** OQ-DI-02 is unanswered and is load-bearing for the novelty claim. If a jurisdiction does govern decision chains as such, the contribution reduces from "identifies an ungoverned layer" to "documents India's absence of a governance form that exists elsewhere" — still publishable, materially weaker. **Check before framing any abstract around novelty.**
- **⚠ #325 (LOW).** Healthcare and pharma rows in the sector-invariance table draw on the originating Release 0.1 framework's worked examples. ICMR_1 supports the healthcare row; **the pharma/manufacturing-deviation row has no corpus support** and should be dropped or sourced before external use.

---

## **Instances in Corpus**

- [[07_Institutions/Corpus/RBI/RBI_16_Draft_Guidance_Data_Governance_2026]] + [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] — the construct's first dated, detailed primary-source instrument-level evidence at the **Data** stage (RBI_16) read alongside the **Model** stage (RBI_14): two adjacent stages now governed, in isolation from each other and from everything downstream. See dedicated section above.
- [[07_Institutions/Corpus/RBI/RBI_15_Utkarsh_2.0_Medium_Term_Strategy_2023_25]] — background dating evidence only, not a governance instance. Vision 1 item 17 ("Adoption of emerging SupTech solutions for effective supervision") is the earliest dated institutional signal in the corpus (Dec 2022) that RBI intended to move toward automated supervision tooling, but carries no operational or deontic content — the strategic-intent bullet exists years before any instrument that could be assessed against H1–H4.
- [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] + [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] — estate governed comprehensively, decisions ungoverned; the construct's binding-instrument evidence
- [[07_Institutions/Corpus/ICMR/ICMR_1]] — seven stakeholder categories, no enforcement, nothing at the recommendation→decision handoff
- [[07_Institutions/Corpus/SEBI/SEBI_14]] / [[07_Institutions/Corpus/RBI/RBI_7]] — non-delegable entity accountability over an ungoverned chain; the liability asymmetry
- [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] — DPDP input-side obligations without RBI decision-side obligations
- [[04_Knowledge_Products/Wiki_Intake/MoHFW_1_SAHI_Healthcare_AI_Strategy_2026]] — national healthcare AI strategy with no instrument reaching deployment decisions
- [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]] — cross-institutional fraud alerting; binding cyber perimeter, no AI perimeter ✅ ⚠#322 closed

## **Feeds Into**

[[04_Knowledge_Products/Regulatory_Complexity_Handbook]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]] | [[04_Knowledge_Products/AI_Governance_Wiki]]

## **Linked Signature Concepts**

[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] | [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]

## **Linked Standard Concepts**

[[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Standard/Human_Oversight]] | [[05_Concepts/05_Concepts_Standard/Model_Risk]] | [[05_Concepts/05_Concepts_Standard/Contestability_Redress]]

## **Linked Domains**

[[03_Domains/BFSI_Governance]] | [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]] | [[03_Domains/Healthcare_Governance]] | [[03_Domains/AI_Governance]] | [[03_Domains/Systemic_Regulatory_Governance]]

## **Linked Projects**

[[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/P4_Doctrinal_IJLIT]] | [[02_Projects/fsQCA_Thesis_Chapter]]

## **Linked Methods**

[[08_Methods/Institutional_Grammar_IG2]] — see OQ-DI-04

## **Linked Consulting**

[[10_Consulting/AEGIS_OS_Inbound]] | [[10_Consulting/PrivacyWeave_Inbound]] | [[10_Consulting/Governance_Diagnostic_Report_Template]]

---

## **Log**

- 2026-08-09: Concept created at candidate class from Vivek's *Decision Infrastructure Series, Release 0.1*, formalised as a vault construct. **Three-Instance Gate passed against five instances across four sectors** (power, payments, healthcare, credit) — cross-sector breadth is the basis for signature-class candidacy rather than a BFSI sub-pattern. CEA_3, intaken the same day, supplies the power leg as binding-instrument evidence: an instrument governing the grid's technology estate across 17 regulations with nothing on what the systems decide. SEBI_14/RBI_7 recorded as the negative-space instance — non-delegable entity accountability over a chain no instrument governs. Positioned against Governance_Debt's infrastructure-layer sub-pattern (which catalogues the absence) as the construct that explains it, and against SR 26-2 (which vacates the model unit without replacing it). Four VERIFY flags (#322–#325); **#322 (NPCI instance is non-primary) and #324 (novelty claim unchecked) are the two to resolve before external use.**
- 2026-08-09 (later, same day): [[07_Institutions/Corpus/RBI/RBI_16_Draft_Guidance_Data_Governance_2026]] intaken and read against [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] — the construct's first dated, primary-source instrument-level evidence at the **Data** stage, closing part of the gap the construct's own prescriptive section had flagged as entirely derived rather than observed. Narrows the construct's applicability (Data stage is no longer wholly unaddressed) while strengthening its diagnostic claim (two adjacent stages governed in isolation, H1 handoff and everything after it still untouched). RBI_15 (Utkarsh 2.0) also added the same day as background dating evidence only, explicitly not counted toward the gate.

- 2026-08-15: **⚠#322 closed** by creation of `NPCI_1`, and **instance 2 restated**. Primary sourcing refuted the "federated AI fraud scoring" characterisation the instance had inherited from Governance_Debt; the replacement — cross-institutional fraud alerting inside a cyber perimeter and outside every AI perimeter — is narrower, primary-sourced, and does not rest on an unverified technical claim. New flags ⚠#361–#365. **Gate integrity note:** instance 2 was carried for six days on a claim no primary source supported. It survived because the *structural* argument never depended on the technical detail — but the detail was stated as fact.
