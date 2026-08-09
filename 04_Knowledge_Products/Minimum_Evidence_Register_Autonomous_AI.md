---
type: Knowledge Product
status: active
last_updated: 2026-08-09
tags:
  - type/knowledge-product
  - status/active
  - engine/consulting
  - engine/knowledge-product
  - engine/teaching
  - engine/linkedin
  - paper/p4
  - content/checklist
  - content/carousel-ready
  - gate/open
---

# Minimum Evidence Register for Autonomous AI — and what Indian law actually requires

**Type:** Knowledge Product / practitioner artefact **Status:** Active — v1 **Created:** 2026-08-09
**Audience:** Board, CRO, CISO, GC, internal audit
**Origin:** Six-record register from Vivek's Microsoft AI-native security architecture carousel (2026-08), crosswalked here against binding and non-binding Indian instruments
**Called for by:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] §Reuse — "directly operational for the Board AI Risk Oversight Checklist and the Common Evidence Repository recommendation"

---

## The proposition

> If you cannot produce these six records, your governance is asserted, not demonstrated.

Six records. Each answers a question a board, an auditor, a regulator or a court will eventually ask about an autonomous or agentic AI deployment.

| # | Record | The question it answers |
|---|---|---|
| **1** | **Agent identity** | Which agents exist, and under whose account do they run? |
| **2** | **Model version** | What reasoned, and when did it last change? |
| **3** | **Delegation approval** | Who authorised the authority granted? |
| **4** | **Orchestration workflow** | What sequences may be run? |
| **5** | **Permitted actions** | Which systems may the agent modify? |
| **6** | **Runtime evidence** | Proof that the action taken matched the approval given |

---

## The crosswalk — what Indian instruments actually mandate

This is the part that makes the register a research artefact rather than a checklist. Coding: **✅** mandated; **◐** partially or by analogy; **❌** absent.

| Record | Nearest Indian obligation | Coding | Gap |
|---|---|---|---|
| **1. Agent identity** | None located in any Indian instrument. [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]]'s nine-field agent system register is a **vault construct, not a legal requirement**. Closest: [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] reg 5(25) cyber asset register — an *asset* register, which would capture the software but not the agent as an actor with delegated authority | ❌ | **No Indian instrument requires an agent register.** The record most specific to agentic deployment is the one with no legal hook at all |
| **2. Model version** | [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]] (draft, unfinalised); [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (principles, non-binding). **[[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] — the binding instrument for commercial banks — has zero AI provisions**, so no model-versioning obligation reaches them through it. CEA_3 reg 8(25) requires version control and rollback for software updates generally | ◐ | Model versioning is required of Indian banks **only through a draft circular and a principles framework**, neither binding. The binding instrument is silent |
| **3. Delegation approval** | None. This is the [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] gap in its purest form — no Indian instrument requires a record of what standing authority was granted to an automated actor, by whom | ❌ | Complete absence |
| **4. Orchestration workflow** | None. CEA_3 reg 8(25) change management is the nearest analogue and is drafted for patches, not agent workflows | ❌ | Complete absence |
| **5. Permitted actions** | [[07_Institutions/Corpus/RBI/RBI_7]] LSP due diligence and [[07_Institutions/Corpus/SEBI/SEBI_14]] Reg 16C attach **accountability** for outputs, without requiring a record of what the system was **permitted** to do. CEA_3 reg 8(11) access control (authentication, authorisation, accounting) governs *human and system access*, not agent action scope | ◐ | Accountability without permission-scoping: the entity answers for actions it is under no obligation to have bounded in advance |
| **6. Runtime evidence** | **The one strong hook.** RBI_8 para 93 (logging capability on every system accessing critical/sensitive information), para 95 (audit trails sufficient as forensic evidence, dispute resolution, **non-repudiation**), para 220(5) (**attribution: who did what, when and how, with preservation of evidence**). CEA_3 regs 8(33)(h)–(i) supply the retention horizons RBI_8 omits (180-day logs, 365-day incident logs) | ✅ / ◐ | Strongest in the corpus — but **technology-neutral**. Would have to be *read onto* agent actions; no instrument says it applies to them, and nobody has argued it |

### What the crosswalk shows

**Four of six records have no Indian legal hook at all.** Records 1, 3 and 4 — agent identity, delegation approval, orchestration workflow — are precisely the records that distinguish autonomous deployment from conventional automation, and precisely the ones no instrument mentions.

**The two partial hooks run in opposite directions.** Record 5 has accountability without permission-scoping (you answer for it, but needn't have bounded it). Record 6 has evidentiary capability without AI-specificity (the logging duty exists, but was written for a different kind of actor).

**RBI_8 para 220(5) is the sleeping provision.** "Clear attribution of actions including who did what, when and how, along with preservation of evidence" is binding text that would, on its natural reading, cover an agent action and an orchestration decision. It has never been argued to. See [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] OQ-OG-02 — if it does reach, India's gap is interpretive rather than legislative, which is a materially more useful finding.

> ⚠ **State this as the finding, not as a compliance requirement.** The six records are a *governance proposal*, not a description of Indian legal obligations. Any board deck or carousel reusing this must not imply the records are required — see [[11_Content/Content_Correction_Register]] W-02.

---

## The board-facing version

What each record protects against, in terms a board will act on:

| Record | Board question it answers | Exposure if absent |
|---|---|---|
| Agent identity | "How many autonomous systems are running, and who owns them?" | Shadow agents; no denominator for risk |
| Model version | "Has the thing making these decisions changed?" | Silent capability drift; no baseline for incident analysis |
| Delegation approval | "Who said this system could do that?" | Authority exercised without a decision-maker |
| Orchestration workflow | "What sequences can it run without asking anyone?" | Capability the organisation never sanctioned |
| Permitted actions | "What can it change?" | Unbounded blast radius |
| Runtime evidence | "Can we prove what it actually did?" | Assertions the organisation cannot substantiate under challenge |

**The framing that lands:** boards will not audit the architecture. They will audit the evidence.

---

## Relationship to the maturity ladder

The register sits at the third rung of the ladder developed in [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]:

| Rung | What it does | Typical artefact |
|---|---|---|
| **Policies** | Declare what should happen | AI policy, risk register, SOPs |
| **Controls** | Define how it will happen | Access control, approval gates |
| **Evidence** | **Prove what actually happened** | **← this register** |
| **Assurance** | Independently verify | Audit, third-party evaluation |
| **Trust** | Build stakeholder confidence | Certification, disclosure |

Most regulated organisations hold rungs 1 and 2 and almost nothing at rung 3 in a form that would survive an auditor, a regulator, or a court. The [[06_Frameworks/Evidentiary_Destination_Matrix]] shows why that gap persists: **no Indian instrument specifies what retained evidence is for**, so nothing forces rung 3 into a provable form.

---

## Admissibility overlay

A record that exists is not the same as a record that can be proved. Under [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]], any of these six records offered in an Indian court needs a **s.63(4) certificate** — identifying the record and the manner of its production, describing the device, addressing the four s.63(2) conditions, and **signed by a person occupying a responsible official position**, with Part B of the Schedule completed by someone with relevant technical expertise.

**No Indian regulatory instrument requires an entity to be capable of producing that certificate for any retained artefact.** For an organisation actually building this register, the practical consequence is a seventh, unglamorous requirement:

> **7. A named signatory** — a person in a responsible official position who can, at production time, attest to how each record was produced and to the proper operation of the system that produced it.

That person does not currently exist in any Indian AI governance framework, and identifying them is the cheapest thing on this list.

---

## Consulting application

**Diagnostic use.** Walk a client's actual agentic deployment through the six records and score presence/absence. Expect four absent. The value is not the score — it is that records 1, 3 and 4 usually surface deployments nobody at board level knew were autonomous.

**Product mapping.** [[10_Consulting/AEGIS_OS_Inbound]] addresses records 3, 5 and 6 directly (authority binding, pre-execution enforcement, tamper-evident audit trail); [[10_Consulting/PrivacyWeave_Inbound]] addresses record 6 for data access specifically. Both are runtime-layer products, which is consistent with records 3–6 all being runtime artefacts.

**What to avoid.** Do not present the register as a compliance requirement. The honest and more persuasive framing is: *these are the six records a regulator or court would need, four of them are not required by any Indian instrument, and that gap is yours to close before someone asks.*

---

## ⚠ VERIFY

- **⚠ #326 (MEDIUM).** The crosswalk's ❌ codings assert **absence across the Indian corpus**, based on the instruments coded in this vault rather than an exhaustive search of Indian regulatory material. High confidence for records 1, 3 and 4 (agent registers and delegation records would be conspicuous if they existed) but confirm against IRDAI's forthcoming WG-AI recommendations (due ~18 Sep 2026) and SEBI_15 CSCRF before publishing the absence claim.
- **⚠ #327 (LOW-MEDIUM).** The six records originate in practitioner content, not in any standard or instrument. They are defensible as a proposal and are **not** an established framework. Do not attribute them to Microsoft — Microsoft published the engineering architecture; the evidence register is Vivek's own construction on top of it.
- **⚠ #328 (LOW).** RBI_13 is a **draft** circular. Record 2's ◐ coding depends on it; if RBI_13 is never finalised, model versioning has no binding Indian hook for commercial banks at all, and record 2 moves to ❌.

---

## Cross-Links

**Concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] | [[05_Concepts/05_Concepts_Standard/Orchestration_Governance]] | [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] | [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] | [[05_Concepts/05_Concepts_Standard/Human_Oversight]] | [[05_Concepts/05_Concepts_Standard/Accountability]]
**Frameworks:** [[06_Frameworks/Evidentiary_Destination_Matrix]] | [[06_Frameworks/RBI_Free_AI]] | [[06_Frameworks/ISO_IEC_42001]]
**Corpus nodes:** [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] | [[07_Institutions/Corpus/RBI/RBI_7]] | [[07_Institutions/Corpus/SEBI/SEBI_14]] | [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]]
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]]
**Consulting:** [[10_Consulting/Board_AI_Risk_Oversight_Checklist]] | [[10_Consulting/AEGIS_OS_Inbound]] | [[10_Consulting/PrivacyWeave_Inbound]] | [[10_Consulting/Agentic_AI_Security_Diagnostic_Template]]
**Content:** [[11_Content/Content_Correction_Register]] W-02

---

## Log

- 2026-08-09: Created from the six-record register in Vivek's Microsoft-architecture carousel, crosswalked against Indian instruments for the first time. **Headline: four of six records have no Indian legal hook.** Records 1, 3 and 4 — agent identity, delegation approval, orchestration workflow — are the ones that distinguish autonomous from conventional deployment and are entirely absent. Record 6 has the only strong hook (RBI_8 paras 93/95/220(5)) and it is technology-neutral. A seventh requirement — a named s.63(4) signatory — added from the admissibility overlay; it exists in no Indian AI framework and is the cheapest gap to close. Three VERIFY flags (#326–#328).
