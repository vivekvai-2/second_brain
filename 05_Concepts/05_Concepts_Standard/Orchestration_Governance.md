---
type: Standard Concept
status: candidate
last_updated: 2026-08-09
tags:
  - type/concept-standard
  - status/candidate
  - concept-class/candidate
  - paper/p4
  - paper/p3
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/linkedin
  - content/carousel-ready
concept_class:
  - candidate
---

# **Orchestration Governance**

**Type:** Standard Concept (candidate class) **Status:** Candidate — Three-Instance Gate **PASSED**, see below **Created:** 2026-08-09
**Theoretical lineage:** Delegation and agency theory (principal–agent, but with the agent unable to hold intent); workflow and process governance; zero-trust architecture; forensic reconstruction
**Origin:** Practitioner content authored by Vivek, 2026-08 (Microsoft AI-native security architecture carousel) — formalised into a vault construct on 2026-08-09

---

## **Definition**

**One-sentence definition.** Orchestration Governance is the governance of the layer that decides *which* AI component runs, *in what sequence*, *on what inputs*, and *under whose authority* — as distinct from the governance of the models that reason and the agents that act.

**Full analytical definition.** In an agentic AI deployment, three things are separately governable: the **model** (what reasoned), the **agent** (what acted, with what permissions), and the **orchestration layer** — variously called the harness, the workflow engine, or the coordination plane — which sequences models and agents into a workflow and determines what runs when. Model governance has a mature apparatus (validation, versioning, model risk management, SR 11-7 and its successors). Agent governance has an emerging one (identity, delegated authority, least privilege, kill switches). **Orchestration governance has neither, in any jurisdiction examined in this corpus.** The construct names that gap and specifies what would fill it: approval of the workflow set, authority over changes to it, and reconstructability of orchestration decisions after the fact.

**Plain-language practitioner definition.** Models get validated. Agents get identities. Nobody approves the workflow that strings them together, nobody owns changes to it, and nobody can reconstruct months later why the system ran the sequence it ran.

---

## **The problem the concept solves**

[[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] is among the richest notes in this vault — Five Structural Breaks, a three-layer pre-deployment/runtime/post-deployment model, US–China convergence analysis, a nine-field agent system register. **None of its five breaks is the orchestration layer.** Break 2 (chained systems propagate errors) comes closest but is framed as a property of *agents in a chain* rather than of the *thing that constitutes the chain*. Break 4 (shared state destroys audit trails) is downstream of orchestration but treats state as the object.

The distinction matters because the governance answers differ:

| Layer | Governance question | Existing apparatus |
|---|---|---|
| **Model** | What reasoned, on what version, validated by whom? | Mature — model risk management, validation, versioning, change control |
| **Agent** | What authority does this actor hold, under whose account? | Emerging — NIST NCCoE agent identity, SPIFFE/SPIRE, ephemeral identity, least privilege |
| **Orchestration** | Who approved this workflow, who may change it, can the decision be reconstructed? | **None** |

An agent register tells you the agents exist. A model register tells you what version reasoned. Neither tells you that Agent 3 ran because Agent 1's confidence fell below a threshold set in a workflow definition that a platform engineer changed in a sprint six weeks ago.

---

## **Constitutive dimensions**

| Dimension | Diagnostic question | Failure mode when absent |
|---|---|---|
| **Workflow authorisation** | Who approved the set of workflows the orchestration layer is permitted to run? | Capability drift — the system can execute sequences nobody sanctioned |
| **Change authority** | Who may alter a workflow, under whose authority, with what record? | Silent policy change — the governing logic moves without a governance event |
| **Orchestration reconstructability** | Can it be established, months later, why this sequence ran on these inputs? | Unauditable causation — the outcome is attributable to no decision |
| **Delegation scope** | What is the standing grant of authority, as distinct from per-action approval? | Unbounded standing authority — one approval licenses indefinite action |

The third dimension is the one that connects this construct to [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]: orchestration decisions are precisely the class of artefact that no instrument in the corpus requires anyone to retain.

---

## **Three-Instance Gate — PASSED (2026-08-09)**

Per [[00_MOC/Workflow_Discipline_Protocol]] CDW-1, entry requires three distinct corpus instances **or** theoretical load-bearing in an active paper. Both limbs are satisfied. Each instance below is verified present in the vault.

| # | Node | What it contributes |
|---|---|---|
| **1** | [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]] | Names **"orchestration drift"** as one of five multi-agent system risks (alongside semantic misalignment, security and trust gaps, cascading effects, systemic complexity). **The corpus's only existing term for the phenomenon** — named in a WEF/Capgemini multi-stakeholder framework and then never developed anywhere in the vault. |
| **2** | [[05_Concepts/05_Concepts_Standard/Model_Risk]] — **SR 26-2** (Fed/OCC/FDIC, 17 Apr 2026, superseding SR 11-7) | **Explicitly carves generative and agentic AI out of model risk management scope** as "novel and rapidly evolving," directing institutions to govern them under "broader risk management and governance practices." The consequence is structural: an orchestrated agentic system sits **outside the independent-challenge function** that model validation provides. A mature supervisory regime has drawn the boundary such that orchestration falls in the gap — by considered judgment, not oversight. |
| **3** | [[06_Frameworks/SAIL_Secure_AI_Lifecycle]] | SAIL 3.18 **"Posture Drift"** and the treatment of **shadow agents**: the enterprise-security articulation of the same gap, arrived at from practice rather than regulation. Its action-control-vs-access-control pivot is orchestration governance in vendor vocabulary. |
| **4** | [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] | Six focus areas including **Access Delegation** and **Data Flow Tracking** — the closest any standards body comes, and it stops at the agent boundary. Identity and delegation are specified; *what sequence the delegated agents are run in, and who approved that sequence*, are not. Supplies the negative evidence: the most advanced federal standards effort on agentic governance does not reach the orchestration layer. |
| **5** | [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] | IMDA's Model AI Governance Framework for Agentic AI (~Jan 2026), the world's first framework dedicated to AI agents, with an L1–L4 autonomy scale and the "make humans **meaningfully** accountable" pillar. **Governs autonomy level, not workflow authorisation** — again stopping short. |

**Theoretical load-bearing:** the construct supplies the mechanism for [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]'s missing artefact class (orchestration decisions) and is a candidate section for [[02_Projects/P4_Doctrinal_IJLIT]].

---

## **The Indian position: nothing, and not by exclusion**

The comparative point is sharper than "India lags."

| Jurisdiction | Position on agentic/orchestration governance |
|---|---|
| **US** | **Excluded by considered judgment** — SR 26-2 places generative and agentic AI outside model risk scope pending a future Request for Information |
| **China** | **Included and being mandated** — CAC May 2026 agentic guidance calls for clear boundaries between actions an agent may take alone, those requiring user authorisation, and the user's own decisions; a mandatory national standard is in drafting (see [[06_Frameworks/China_AI_Governance]], [[04_Knowledge_Products/Wiki_Intake/F139_ConcordiaAI_State_of_AI_Safety_China_2026]]) |
| **Singapore** | **Addressed at the autonomy layer** — IMDA L1–L4 scale, voluntary, additive to two prior frameworks |
| **EU** | AI Act governs systems and providers; no orchestration-layer provision located |
| **India** | **Neither included nor excluded — the question has not been reached.** [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] covers "increasingly autonomous AI systems" in scope without operationalising action- or workflow-level authorisation. No Indian regulator has issued agent-specific guidance of any kind |

This is the framing worth developing: **the US decided to exclude, China decided to include, and India has not decided.** A regulatory-lag argument that does not depend on the India-lags-the-West narrative, because on this question the West is split and nobody is following anybody.

---

## **Where the Indian regulatory hooks would attach if anyone reached for them**

Not currently exercised — this is a doctrinal availability analysis, not a description of practice:

| Hook | Provision | What it could reach |
|---|---|---|
| **Non-delegable accountability** | [[07_Institutions/Corpus/SEBI/SEBI_14]] Reg 16C; [[07_Institutions/Corpus/RBI/RBI_7]] LSP due diligence; DPDP Rules Rule 13(3); CERT-In reporting duty on the entity | The entity answers for orchestrated outcomes regardless of which component executed. **Automation changes who executes; it does not change who answers.** |
| **Outsourcing / third-party** | [[07_Institutions/Corpus/RBI/RBI_2]]; [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]]; [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] regs 11–12 | A vendor-supplied orchestration layer is a third-party arrangement; CEA_3 binds vendors directly and requires a Bill of Materials, which would in principle have to enumerate orchestration components |
| **Change management** | CEA_3 reg 8(25) — version control, rollback, digital signature for OT updates | The nearest thing in Indian law to workflow-change control, drafted for software patches rather than for agent workflows |
| **Audit trail sufficiency** | [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] paras 93/95, 220(5) attribution — "who did what, when and how" | The strongest reconstructability language in Indian regulation. **It was written for human and system actors, and would have to be read onto orchestration decisions to reach them** |

RBI_8 para 220(5) is the most interesting of these: a four-part reconstruction requirement in binding text that, on its face, would cover an orchestration decision — if anyone argued it. Nobody has.

---

## **Intersection with Signature Constructs**

*Required by [[00_MOC/Workflow_Discipline_Protocol]] CDW-3.*

**[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]].** Orchestration Governance exposes a form of parallelism the existing matrix cannot reach, because there is nothing to be parallel *about*. The corpus's parallelism instances are cases of multiple regulators governing the same object independently. Here the object is governed by **nobody, anywhere** — the US having excluded it by considered judgment (SR 26-2), China including it, India not having reached it. This is the limiting case: parallelism presupposes at least two instruments; orchestration has none.

**[[05_Concepts/05_Concepts_Signature/Governance_Debt]].** Supplies a variant distinct from those catalogued: **composition debt**. The corpus's debt variants arise from duplication (two mandates, one capability) or silence (no mandate, one capability). Composition debt arises where each *component* of a system is governed — the model by validation regimes, the agent by identity frameworks — and the *composition* of those governed components is not, so an entity can be fully compliant at every layer and still unable to account for what its system did. Compliance at the parts does not aggregate to accountability for the whole.

**[[05_Concepts/05_Concepts_Signature/Institutional_Coherence]].** A test the construct fails cleanly on Dimension 3 (obligation consistency): model governance, agent identity standards and orchestration all use different units of assessment — the model version, the actor identity, and the workflow instance respectively — with no instrument reconciling them. An entity cannot map an agent-identity record onto a model-validation record onto an orchestration decision, because no framework defines the join.

**[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]].** The tightest intersection. Orchestration Governance names a specific **artefact class** — workflow definitions, approval trails, delegation grants, orchestration execution logs — that Evidentiary_Governance's artefact-specification dimension predicts should be named by instruments and finds is not. RBI_8 para 220(5) ("who did what, when and how, along with preservation of evidence") is the only binding Indian text that would reach an orchestration decision on its natural reading, and no one has argued it. See OQ-OG-02.

---

## **Distinguished from adjacent constructs**

| Construct | Difference |
|---|---|
| [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | The parent. Governs agents as decision-makers (identity, authority, kill switch). Orchestration Governance governs the layer that *composes* them. An agent register can be complete while the workflow set is entirely ungoverned |
| [[05_Concepts/05_Concepts_Standard/Model_Risk]] | Governs the reasoning component. SR 26-2 expressly excludes agentic systems, which is precisely how orchestration ends up ungoverned |
| [[05_Concepts/05_Concepts_Standard/Human_Oversight]] | Concerns whether a human can intervene. Orchestration Governance concerns whether the *grant of authority* was approved and is reconstructable — see the delegation-as-control-point section in that note |
| [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | Concerns whether retained artefacts can prove what happened. Orchestration Governance identifies a **specific artefact class** — workflow definitions and approval trails — that no instrument requires anyone to retain |

---

## **Minimum orchestration evidence set**

The artefacts that would have to exist for the third dimension to be satisfiable. Cross-walked against Indian instruments in [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]:

1. **Workflow definition register** — what sequences may be run
2. **Workflow approval trail** — who authorised each, when, under what authority
3. **Change log with authority attribution** — who altered a workflow, on whose approval
4. **Delegation grant record** — what standing authority was conferred, to which agent, by whom, with what scope and expiry
5. **Orchestration execution log** — which sequence ran, on which inputs, at what time
6. **Reconstruction capability** — the ability to bind the above into an account of a specific past decision

---

## **Reuse across the output pockets**

- **Research (R):** candidate section for [[02_Projects/P4_Doctrinal_IJLIT]]; supplies the mechanism for the Evidentiary_Governance artefact gap; the US-excludes / China-includes / India-undecided table is a clean comparative figure
- **Consulting (C):** the six-artefact set above is a direct diagnostic for AEGIS_OS scoping — the product's authority-binding and pre-execution enforcement address dimensions 1, 2 and 4
- **Thought leadership (TL):** the origin carousel is written; see [[11_Content/Content_Correction_Register]] W-02 for the caveat to carry (the six records map to almost nothing in binding Indian law — state that as the finding rather than implying the records are required)
- **Knowledge product (KP):** fills an identified S4 gap in [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## **Open questions**

**OQ-OG-01.** Is orchestration a genuinely distinct governable layer, or a composition of model and agent governance that decomposes without remainder? The strongest evidence for distinctness is SR 26-2: a mature supervisor drew a boundary that leaves it ungoverned, which implies it was not already covered.

**OQ-OG-02.** Does RBI_8 para 220(5)'s "who did what, when and how" reach an orchestration decision on its natural reading? If yes, India has an unexercised binding hook and the gap is interpretive rather than legislative — a materially different and more useful finding.

**OQ-OG-03.** Do the China CAC agentic guidance and the drafting mandatory standard address workflow authorisation specifically, or only per-action user authorisation? Primary texts not in the corpus (URLs in F139's sourcing leads).

**OQ-OG-04.** Is "orchestration drift" (F037) the same phenomenon as SAIL's "posture drift," or two distinct failure modes with a shared name?

---

## **⚠ VERIFY**

- **⚠ #319 (MEDIUM).** The claim that **no jurisdiction governs the orchestration layer** rests on the absence of located provisions across the instruments in this corpus, not on an exhaustive search. Absence of evidence is weak evidence of absence at this scale. Before publishing, run a targeted check of the EU AI Act GPAI provisions, NIST AI 600-1, and the China CAC guidance for workflow-authorisation language.
- **⚠ #320 (MEDIUM).** The Microsoft AI-native security reference architecture (Signals → Context → Models → Harness → Agents → Actuators) is the construct's originating source and **is not in the corpus as a node.** The six-layer taxonomy and the "humans remain in control" statement are quoted from the practitioner carousel, not from a primary Microsoft document. **Create a Wiki Intake node for the Microsoft architecture before citing the layer taxonomy in publication-track output.**
- **⚠ #321 (LOW).** SR 26-2's carve-out scope is taken from [[05_Concepts/05_Concepts_Standard/Model_Risk]]'s summary rather than from the supervisory letter itself. Confirm the exclusion language before building the US-excludes limb of the comparative table on it.

---

## **Instances in Corpus**

- [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]] — "orchestration drift" named, undeveloped
- [[05_Concepts/05_Concepts_Standard/Model_Risk]] / SR 26-2 — agentic AI carved out of model risk scope; the boundary that creates the gap
- [[06_Frameworks/SAIL_Secure_AI_Lifecycle]] — posture drift, shadow agents, action control vs access control
- [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] — access delegation and data-flow tracking, stopping at the agent boundary
- [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]] — autonomy tiers without workflow authorisation
- [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices]] — "Preserve Coordination Trust" as a foundational principle; the closest existing vault language
- [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] — para 220(5) as the unexercised Indian hook

## **Linked Concepts**

[[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | [[05_Concepts/05_Concepts_Standard/Model_Risk]] | [[05_Concepts/05_Concepts_Standard/Human_Oversight]] | [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Standard/Accountability]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]]

## **Linked Frameworks**

[[06_Frameworks/SAIL_Secure_AI_Lifecycle]] | [[06_Frameworks/China_AI_Governance]] | [[06_Frameworks/Singapore_AI_Governance]] | [[06_Frameworks/NIST_AI_RMF]] | [[06_Frameworks/RBI_Free_AI]] | [[06_Frameworks/Evidentiary_Destination_Matrix]]

## **Linked Domains**

[[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]] | [[03_Domains/Cybersecurity_Governance]]

## **Linked Projects**

[[02_Projects/P4_Doctrinal_IJLIT]] | [[02_Projects/P3_BFSI_JEIM]]

## **Linked Consulting**

[[10_Consulting/AEGIS_OS_Inbound]] | [[10_Consulting/PrivacyWeave_Inbound]]

---

## **Log**

- 2026-08-09: Concept created at candidate class from Vivek's own Microsoft-architecture carousel, formalised as a vault construct. Three-Instance Gate passed against five verified nodes (F037, SR 26-2 via Model_Risk, SAIL, F036, International_35), two of which supply the gap as *negative* evidence — the most advanced agent-governance efforts stop at the agent boundary. Comparative position established: US excludes by judgment (SR 26-2), China includes and is mandating, Singapore addresses autonomy not workflow, India has not reached the question. Four Indian doctrinal hooks identified as available but unexercised, RBI_8 para 220(5) the strongest. Three VERIFY flags (#319–#321); **#320 is the one to act on — the originating Microsoft architecture has no corpus node.**
