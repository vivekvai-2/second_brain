---
type: Corpus Node
status: draft-instrument
tags:
  - type/corpus-node
  - status/active
  - institution/rbi
  - paper/p3-primary
  - paper/p4
  - gate/open
  - engine/phd
---

# RBI_13 — Draft Circular: Regulatory Principles for Management of Model Risks in Credit (2024)

> ## ⚠ DUPLICATE ALERT — flagged 2026-08-09, not merged
>
> **This node and [[07_Institutions/Corpus/RBI/RBI_3]] are the same instrument.** Both are the Draft Circular *Regulatory Principles for Management of Model Risks in Credit*, **5 August 2024**, DOR.STR.REC./21.04.048/2024-25. RBI_3 was created earlier; RBI_13 was created 2026-08-02 during the model-risk sourcing pass without a duplicate check against RBI_3.
>
> This is a **duplicate-detection debt** instance in the sense recorded at [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (cf. the SEBI_16/SEBI_14 case resolved 2026-07-14). **Reported only, per the standing duplicate protocol — no merge performed.**
>
> **Resolution is Vivek's call, and a merge needs both:** RBI_13 carries better sourcing metadata (reference number, comment-period close, FIDC provenance caveat) and the [[05_Concepts/05_Concepts_Standard/Model_Risk]] linkage; **RBI_3** carries the legal-basis detail (BR Act ss.21/35A/56; RBI Act ss.45JA/45L/45M; NHB Act ss.30A/32/33) and the RBI_FREE_AI companion note.
>
> **Superseding instrument:** [[07_Institutions/Corpus/RBI/RBI_14_Draft_Guidance_Model_Risk_Management_2026]] (June 2026) is the general-purpose successor covering all models across eleven RE categories. ⚠ Its relationship to this 2024 credit-scoped draft is **not stated** in its text — whether RBI_14 supersedes, absorbs, or runs parallel is unresolved (⚠#337).

**Institution:** [[RBI]] | **Concept:** [[Model_Risk]] | **Added:** 2026-08-02 (model risk sourcing pass)

---

## Document Identity

- **Title:** Regulatory Principles for Management of Model Risks in Credit
- **Issuing body:** Reserve Bank of India, Department of Regulation
- **Reference:** DOR.STR.REC./21.04.048/2024-25
- **Date:** **5 August 2024** (draft); comment period closed 4 September 2024
- **Link:** https://www.fidcindia.org.in/wp-content/uploads/2024/08/RBI-DRAFT-MANAGEMENT-OF-MODEL-RISK-IN-CREDIT-05-08-24.pdf
- **Status:** ⚠ **DRAFT — finalisation unconfirmed.** No evidence located that this has been issued in binding form since August 2024. Verify against RBI's circulars index before citing as operative
- ⚠ **Provenance:** retrieved via an **FIDC-hosted copy**, not rbi.org.in. Verify against the RBI original

## Substantive Content

**Definition.** A credit risk model is "any quantitative method that applies statistical, economic, financial, or mathematical principles and assumptions to process data into an output to be used for credit decisions."

**Obligations on Regulated Entities:**

- Board-approved **model risk management policy** covering the entire model lifecycle
- A comprehensive **Model Inventory**
- **Independent validation** before deployment and **at least annually** thereafter
- Validation reporting to the **Risk Management Committee of the Board (RMCB)**
- Validation must review **"instances of bias or discrimination, if any"**

## Analytical Significance

**India's nearest equivalent to SR 26-2 / SS1/23 — and it is neither general-purpose nor in force.** The instrument is confined to **credit risk models**. It does not extend to market, operational or financial-reporting models, and so is not a general model-risk framework in the sense the US and UK instruments are. See [[Model_Risk]] for the full four-jurisdiction comparison.

**The bias clause is the AI hook.** Requiring validation to review "instances of bias or discrimination" imports an AI/ML-relevant concern into an otherwise conventional statistical-model instrument. Note what it does *not* do: it names bias without specifying a test — the same pattern recorded at [[Fairness]], where every Indian instrument names fairness and none states which criterion applies. **Consistent across two independent instruments now**, which strengthens that finding from an observation to a pattern.

**Two-track structure.** India's model-risk position is split across this draft (conventional models, credit-scoped, not in force) and [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (AI systems, cross-cutting, non-binding Committee recommendation). Neither track is both general-purpose and binding. That bifurcation is itself the finding, and it differs structurally from the US carve-out and the UK's unified inclusion.

**Deontic status for [[Deontic_Bifurcation]].** A draft instrument carries no deontic force at all while using fully mandatory language throughout — obligations drafted in the imperative that bind nobody. Distinct from the four bifurcation types already recorded (designed; emergent; delegated-across-documents; supervisory-expectation). Candidate fifth type: **prospective deontic** — mandatory text awaiting force. Compare the DPDP Rules' commencement structure and the [[DPB]] shell.

## Coding Notes (IG 2.0)

Good ADICO yield if coded: clear Attributes (Regulated Entities), mandatory Deontics, specified aIms (maintain inventory; validate annually; report to RMCB), Conditions (before deployment; at least annually). **Or-else absent** — as a draft it has no enforcement provision. Useful as a control case against [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] (same regulator, same period, complete ADICO with licence-condition Or-else) and [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (same regulator, recommendations, no Or-else). Three RBI instruments, three deontic states — a clean within-institution deontic gradient.

## Related Nodes

- [[05_Concepts/05_Concepts_Standard/Model_Risk]] — parent concept and the four-jurisdiction comparison
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — the AI-specific track (¶4.4.68 inventory; Rec. 24 audit framework)
- [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] — binding contrast case
- [[04_Knowledge_Products/Wiki_Intake/Fed_OCC_SR11-7_Model_Risk_Management_2011]] — ⚠ superseded 17 Apr 2026 by SR 26-2

## Linked Concepts

[[Model_Risk]] · [[Fairness]] · [[Assurance_Reuse_Gap]] · [[Governance_Debt]] · [[Deontic_Bifurcation]] · [[Accountability]]

## Linked Domains

[[BFSI_Governance]] · [[AI_Governance]]

---

_Back to [[RBI]] | [[Corpus_Index_MOC]]_
