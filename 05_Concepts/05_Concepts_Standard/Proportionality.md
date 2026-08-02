---
type: Standard Concept
tags:
  - type/concept-standard
  - status/active
  - paper/p3
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
---

# **Proportionality**

**Type:** Standard Concept
**Status:** Active — created 2026-08-02 (EA-principle cluster intake)
**Last Updated:** 2026-08-02
**Theoretical Lineage:** EU public law (suitability/necessity/balance); risk-based regulation; regulatory governance
**Role in fsQCA:** Structural — the calibration logic linking risk tier to obligation intensity; candidate RL (Regulatory Logic) property rather than an EA constituent

---

## **Definition**

Proportionality is defined here as the property of a regulatory regime whereby the intensity of imposed obligation varies with the magnitude of the risk the regulated activity presents, according to a stated and reviewable method. The classical legal test is tripartite — a measure must be *suitable* (capable of achieving a legitimate aim), *necessary* (no less restrictive means available), and *balanced* (proportionate stricto sensu). In AI governance this abstract test is operationalised almost everywhere as risk-tiering, and the substitution matters: tiering is a mechanism for delivering proportionality, not proportionality itself, and an instrument can tier without ever conducting the balance inquiry.

**Ontological placement.** Proportionality differs from the other four constructs created in this pass. Explainability, fairness, human oversight and contestability are properties of a *decision or system* and are candidate constituents of the EA outcome condition. Proportionality is a property of the *regulatory regime* — a second-order construct governing how the others are allocated. It therefore belongs analytically with the RL (Regulatory Logic) condition, not with EA. Recommend not folding it into the EA composite; doing so would mix levels of analysis and is the kind of error a configurational reviewer will identify immediately.

## **Application in This Research**

Within [[P4_Doctrinal_IJLIT]], proportionality is the normative standard against which India's instrument set is assessed: instruments that impose uniform obligations regardless of risk, or that tier without a stated method, fail the test in different ways and the distinction structures the diagnosis. Within [[fsQCA_Thesis_Chapter]], proportionality is already implicitly present in the RL condition — the existing [[Transparency]] note records that "risk-proportionality is a calibrated property of the Regulatory Logic (RL) condition." This note makes that explicit and supplies the measurement basis it lacked. Within [[Systemic_Regulatory_Governance]] and [[Regulatory_Parallelism]], proportionality supplies the criterion for distinguishing defensible regulatory differentiation from incoherent fragmentation — two regulators imposing different obligations on comparable risks is parallelism; imposing different obligations on genuinely different risks is proportionality working correctly. **That distinction is load-bearing for the whole parallelism argument and has not previously been formalised.**

## **Measurement & Calibration**

| Resource | What it gives |
|---|---|
| **RAND (Feb 2026), *The Science and Practice of Proportionality in AI Risk Regulation*** | The tripartite suitability/necessity/balance structure stated for the AI-regulation context: "EU measures must be suitable, necessary, and balanced" |
| **Atlantis Press, *Risk-Based and Proportionate Regulation of Generative AI*** | A comparative proportionality-assessment tool applying the tripartite test across two domains (cybersecurity vs disinformation); finds "proportionality effectiveness is limited by the quantifiability of the risk and the complexity of value tension." Methodologically the closest thing to a cross-case proportionality comparison located |
| **GIRAI "Proportionality and Do No Harm" thematic area** (IDRC/GIRAI methodology) | A fully specified, replicable coding protocol across three evidence categories: frameworks/mechanisms, government regulatory actions, non-state actor involvement. Directly transferable to case-level calibration |

**Recommended calibration for RL.** Score each case's regime on three items: (1) does it tier risk at all; (2) is the tiering method stated and reviewable; (3) does obligation intensity demonstrably vary across tiers. This yields a defensible 0–6 composite, and is consistent with GIRAI's three-category evidence structure without importing GIRAI's country-level weighting. The Atlantis Press finding — that proportionality effectiveness is bounded by risk quantifiability — should be recorded as a scope condition.

## **Regulatory Definitions (Operative Text)**

| Instrument | Locus | Operative text / status |
|---|---|---|
| **EU AI Act** | Structural, not a single article | Four-tier classification (unacceptable / high / limited / minimal). Recital 26: risk-based approach; the Act "introduces a proportionate risk-based approach to AI regulation, which imposes a gradual scheme of requirements and obligations depending on the level of risk posed to health, safety and fundamental rights" |
| | Art. 14(3) | Oversight measures "shall be commensurate with the risks, level of autonomy and context of use" — proportionality applied to a specific obligation |
| **UNESCO** | Meta-principle | Functions as a balancing principle across the ten principles: "The level of T&E should be appropriate to the context, as there may be tensions between T&E and other principles such as privacy, safety and security" |
| **NIST AI RMF** | Embedded | Delivered through risk-tiering language inside the Govern–Map–Measure–Manage functions; not a named trustworthiness characteristic |
| **OECD** | Embedded | Within "robustness, security and safety"; no standalone clause |
| **India — NCAIC** | Principle 2 of 8 | "Risk Proportionality (prohibited/high/medium/low-risk tiers)" — a four-tier structure that closely mirrors EU AI Act Art. 5 and the AI Act taxonomy. ⚠ The node itself flags that the degree of genuine adaptation vs direct transposition should be assessed before citing this as an Indian innovation |
| **India — SEBI** | — | SEBI's 2025 consultation signals a shift toward risk-tiered AI governance; not yet operative |
| **India — RBI** | — | FREE-AI differentiates by risk for agentic systems ("medium- and high-risk use cases") without defining tiers or a tiering method |

**Finding:** India's only articulated risk-tiering scheme sits in a non-binding framework (NCAIC) and appears to be substantially transposed from the EU AI Act. Its binding instruments gesture at risk differentiation without specifying tiers or method. On the three-item calibration above, every Indian binding instrument scores at item (1) partially and at items (2) and (3) not at all.

## **Measurement Risk**

Two strong critiques, both directed at the EU AI Act's own proportionality claims — which matters, because the AI Act is the benchmark against which India is being assessed throughout P4. If the benchmark's proportionality is itself unmethodical, the comparison must be framed accordingly.

- **Rangone (2025)**, *European Journal of Risk Regulation*: the AI Act's risk assessment is conducted "ex-ante at legislative level," not on "real and practical scenarios"; "the text does not provide a general methodology to assess risks," which "does not favour the residuality and the proportionality of rules, risks both under and over inclusion." ⚠ Perplexity returned a truncated Cambridge URL; verify before citing.
- **Stanford Law School Policy Paper No. 101 (Oct 2024)**: "important provisions of the AI Act do not follow a truly risk-based approach," citing lack of risk-benefit analysis, limited reliance on empirical evidence, and absence of case-by-case risk classification. ⚠ Truncated URL; verify.

The honest framing for P4: the EU AI Act is more *specified* than India's instruments but not necessarily more *proportionate*, because specification without a risk-assessment methodology is tiering rather than proportionality. That framing is more defensible than a simple EU-good/India-lagging comparison and is likely to read better to a European reviewer.

## **Boundary Conditions**

- Proportionality is a regime property, not a system property; do not fold it into EA.
- Risk-tiering is a mechanism for delivering proportionality, not proportionality itself. An instrument may tier without conducting suitability, necessity or balance inquiries — code these separately.
- Proportionality bounded by risk quantifiability (Atlantis Press): where risk cannot be quantified, proportionality assessment degrades into assertion. Relevant to agentic AI, where risk quantification is weakest.

## **Literature Anchors**

- RAND Corporation (2026). *The Science and Practice of Proportionality in AI Risk Regulation.* External Publication EP71258.
- *Risk-Based and Proportionate Regulation of Generative AI.* Atlantis Press conference proceedings.
- IDRC / Global Index on Responsible AI. *Proportionality and Do No Harm* thematic area methodology.
- Rangone, N. (2025). *Risks Without Rights? The EU AI Act's Approach.* European Journal of Risk Regulation.
- Stanford Law School (2024). *Policy Paper No. 101: Truly Risk-Based Regulation of Artificial Intelligence.*

## **Instances in Corpus**

- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — Risk Proportionality as Principle 2; four-tier scheme with an EU-transposition caveat already flagged in the node.
- [[04_Knowledge_Products/Wiki_Intake/F124_Viljanen_Parviainen_AI_Regulatory_Strata_2022]] — regulatory strata as layered proportionality; the closest theoretical treatment in the corpus. Previously unwired.
- [[07_Institutions/Corpus/International/International_18_UNESCO_Recommendation_Ethics_AI_2021]] — proportionality as a balancing meta-principle across competing values.
- [[07_Institutions/Corpus/International/International_28_EIOPA_Opinion_AI_Governance_Insurance_2025]] — proportionality applied to insurance supervision; interpretive layering on the binding AI Act.
- [[07_Institutions/Corpus/International/International_29_IAIS_Application_Paper_AI_Supervision_2025]] — "existing ICPs suffice, no new standards" is itself a proportionality judgement, and an unusually explicit one.
- [[07_Institutions/Corpus/RBI/RBI_5_Operational_Risk_Management_Resilience_NBFC_Guidance_2024]] — proportionality in Indian operational-risk supervision, outside the AI context; the domestic baseline against which AI-specific proportionality can be compared.
- [[04_Knowledge_Products/Wiki_Intake/Tammenga_AI_3LoD_Banks_2020]] and [[04_Knowledge_Products/Wiki_Intake/AgenticRisks_Enterprise_Wide_Agentic_AI_Risk_Controls_2025]] — risk-proportionate control allocation across three-lines architectures.
- [[04_Knowledge_Products/Wiki_Intake/F040_ELI_Guiding_Principles_ADM_EU]] — proportionality in administrative ADM.
- [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] — tiered obligations by intermediary size/significance; a pre-AI Indian precedent for risk-differentiated regulation and a useful demonstration that India *can* tier when it chooses to. Previously fully isolated.

## **Future Reuse Opportunities**

- The parallelism/proportionality distinction — differential obligations across regulators are defensible when risks differ and incoherent when they do not — sharpens [[Regulatory_Parallelism]] materially and should be written back into that note as a boundary condition.
- MeitY_7's tiering precedent is a strong rejoinder to any claim that Indian regulators lack the capacity for risk-differentiated regulation; the capacity exists and was not applied to AI. That is a [[Governance_Capacity]] finding, not a capability gap.
- "Specification is not proportionality" is a defensible contrarian line for practitioner content, and it inoculates P4 against the charge of uncritical EU-benchmarking.

## **Linked Projects**

[[P4_Doctrinal_IJLIT]]

[[P3_BFSI_JEIM]]

[[fsQCA_Thesis_Chapter]]

## **Linked Domains**

[[AI_Governance]]

[[Systemic_Regulatory_Governance]]

[[BFSI_Governance]]

## **Linked Standard Concepts**

[[Human_Oversight]]

[[Fairness]]

[[Explainability]]

[[Contestability_Redress]]

[[Governance_Capacity]]

## **Linked Signature Concepts**

[[Regulatory_Parallelism]]

[[Institutional_Coherence]]

[[Governance_Debt]]

## **Linked Frameworks**

[[EU_AI_Act]]

[[UNESCO_Recommendations]]

[[NIST_AI_RMF]]

## **Linked Methods**

[[fsQCA]]

---

_Back to [[_Concepts_MOC]]_
