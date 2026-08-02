---
type: Standard Concept
tags:
  - type/concept-standard
  - status/active
  - paper/p3-primary
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - content/carousel-ready
---

# **Model Risk**

**Type:** Standard Concept
**Status:** Active — created 2026-08-02 (final sourcing pass)
**Theoretical Lineage:** Banking supervision; validation and assurance scholarship; three-lines-of-defence
**Why this note exists:** 69 referencing notes, no node — and several of the corpus's primary documents on it (SR 11-7, Sudjianto, Rao & Scepanovic, Tammenga) sat unwired to any concept

---

## **Definition**

Model risk is the potential for adverse consequence arising from decisions based on incorrect or misused model outputs. Two limbs, both in the supervisory definitions: **error** (the model is wrong) and **misuse** (the model is right but applied outside its validated purpose). Within PRIS the construct's analytical value is not the definition but the **boundary question** — whether AI and machine-learning systems fall inside existing model-risk frameworks or require a separate regime. Four major jurisdictions now answer that question differently and explicitly, which makes it one of the cleanest comparative findings available to this research programme.

## **⚠ The Corpus Contains a Superseded Instrument**

**SR 11-7 was superseded on 17 April 2026.** Every vault reference treating it as current guidance is now stale — see the list under *Instances in Corpus*.

**SR 26-2 — Revised Guidance on Model Risk Management**, Federal Reserve jointly with OCC and FDIC, 17 April 2026. https://www.federalreserve.gov/supervisionreg/srletters/SR2602.htm
Companions: OCC Bulletin 2026-13; FDIC FIL-15-2026.

Verbatim: it "supersedes and replaces SR letter 11-7… (issued April 4, 2011) and SR letter 21-8, Interagency Statement on Model Risk Management for Bank Systems Supporting Bank Secrecy Act/Anti-Money Laundering Compliance." Also rescinds OCC Bulletins 2011-12, 2021-19 and 1997-24, the Model Risk Management booklet of the Comptroller's Handbook, and FDIC FIL-22-2017.

Key changes:

- **Applicability** narrowed to organisations above **$30bn** total assets
- **Explicitly non-enforceable**: "the guidance does not set forth enforceable standards or prescriptive requirements; accordingly, non-compliance with this guidance alone will not result in supervisory criticism"
- **Three-pillar architecture retained** (development/implementation/use; validation/monitoring; governance/controls) with a **new dedicated third-party/vendor-model section**
- **Model definition tightened** to three cumulative criteria: applies statistical/economic/financial/mathematical theory; processes inputs into quantitative estimates; drives consequential decisions. Explicitly **excludes** simple arithmetic, deterministic rule-based processes, and spreadsheets without embedded statistical methods

## **The Boundary Question — four jurisdictions, four answers**

The most productive comparative material in this note.

| Jurisdiction | Instrument | Position on AI/ML |
|---|---|---|
| **US** | SR 26-2 (2026) | **Exclusion by carve-out.** Traditional statistical and **non-generative, non-agentic ML remain in scope**. **Generative AI and agentic AI are explicitly carved out** as "novel and rapidly evolving," to be governed under "broader risk management and governance practices" pending a promised Request for Information on AI-based models. The boundary is drawn at *generative/agentic vs everything else* — not at AI vs non-AI |
| **UK** | PRA SS1/23 (pub. 17 May 2023, effective 17 May 2024) | **Inclusion by default.** AI/ML appears as a sub-principle *within* the unified framework, applying "to the extent that it applies to the use of models more generally." Five principles: model identification and risk classification; governance; development/implementation/use; independent validation; model risk mitigants. Covers all model types including financial-reporting models and material deterministic quantitative methods |
| **EU** | ECB *Guide to Internal Models*, rev. 2025/2026 | **Middle path — inclusion with supplementary scrutiny.** First-ever dedicated ML section. Defines ML as "highly complex modelling techniques relying on many parameters, capable of capturing non-linearity, needing large datasets… sometimes processing unstructured data," and clarifies that "models based on linear or logistic regression do not qualify as ML for the purposes of the guide." Expectations across governance (ML risks integrated **across the three lines of defence**; staff trained to interpret ML outputs), internal controls (justify added complexity; ensure explainability; Internal Audit must explicitly cover ML models at higher frequency), and data/methodology. ⚠ Narrower scope than the others — Pillar 1 internal models only |
| **India** | draft circular + FREE-AI | **Bifurcated patchwork** — see below |

**Why this matters beyond taxonomy.** The US carve-out is the sharpest available evidence for [[Agentic_AI_Governance]]: the most developed model-risk regime in the world has looked at agentic AI and declined to govern it under model risk, explicitly, in 2026. That is not oversight — it is a considered jurisdictional judgment that agentic systems are not models in the relevant sense. It also bears on [[Human_Oversight]]: a system placed outside model validation is outside the independent-challenge structure that validation provides.

## **India — no equivalent exists, and the absence has structure**

**RBI Draft Circular, "Regulatory Principles for Management of Model Risks in Credit"** — DOR.STR.REC./21.04.048/2024-25, **5 August 2024**; comments closed 4 September 2024. **⚠ Still draft; finalisation unconfirmed.**

Defines a credit risk model as "any quantitative method that applies statistical, economic, financial, or mathematical principles and assumptions to process data into an output to be used for credit decisions." Requires: Board-approved model risk management policy across the full lifecycle; comprehensive **Model Inventory**; independent validation before deployment and **at least annually**; validation reporting to the **Risk Management Committee of the Board**; and review of "instances of bias or discrimination, if any" — an AI-relevant provision inside a credit-scoped instrument.

**Critical limitation: credit risk models only.** Not a general-purpose framework across market, operational or financial-reporting models the way SR 26-2 and SS1/23 are.

**RBI FREE-AI Committee Report** supplies the AI-specific layer, non-bindingly. ¶4.4.68 mandates REs "maintain a comprehensive inventory of AI systems in use across their operations" — fields specified (model type incl. ML/deep learning/NLP/GenAI; use cases; dependencies incl. third-party providers; risk categorisation High/Medium/Low; grievances record), **updated semi-annually**, available for supervisory inspection. **Recommendation 24** establishes an **AI Audit Framework**: internal audit for all AI applications, third-party audit for high-risk use cases, biennial review of the framework itself.

**The confirmed finding, stated precisely:** India has **no single, general-purpose, binding instrument equivalent to SR 26-2 or SS1/23**. What exists is (a) a **draft**, **credit-scoped** circular on traditional statistical model risk, and (b) a **non-binding Committee Report** extending model-governance language to AI. Three structural differences from the US and UK: neither instrument is general-purpose; the AI-specific extension is committee-recommendation status rather than supervisory guidance; and unlike the US carve-out, FREE-AI's language ("including both conventional AI models and increasingly autonomous AI systems") signals **inclusion** for advanced AI — structurally closer to the UK posture, without SS1/23's force.

**A rare positive for India.** On the *inclusion* question India is aligned with the UK and ahead of the US, which has explicitly excluded the fastest-moving category. India's problem here is bindingness, not conceptual scope — a more precise diagnosis than the corpus's usual framing and worth stating in [[P3_BFSI_JEIM]].

## **Three Lines of Defence**

**Schuett, J.**, *Three lines of defense against risks from AI*, **AI & Society** (Springer), DOI 10.1007/s00146-023-01811-0, 74 citations — the strongest peer-reviewed source connecting 3LoD to AI. Maps four actors (governing body; management as first and second lines; internal audit/external assurance as third), with first line = AI research/product teams, second = complementary risk expertise providing monitoring and challenge, third = independent assurance to the board.

Corroborated at regulatory level: the ECB requires ML risks be integrated "across the three lines of defence" — the clearest **regulatory-primary** 3LoD-AI statement located, not merely academic.

Counter-position, for balance: practitioner commentary argues linear 3LoD "was designed for static, process-driven environments" and proposes merging first and second lines into embedded governance teams, with the third line auditing operational controls and governance telemetry rather than process compliance. ⚠ Non-peer-reviewed; useful only as a foil to the Schuett/Wharton/ECB consensus.

## **Literature — note the direction of the evidence**

⚠ **The strongest peer-reviewed source argues *against* the structural-insufficiency thesis.** Maheshwari, A., *Generative Artificial Intelligence in Model Risk Management*, **Journal of Risk Model Validation**, 16 March 2026 — "extends SR 11-7 principles to Generative AI through behavioral and semantic validation," introducing prompt-variance, stability and human-alignment as quantitative proxies, and concluding via a sanctions-screening case study that **GenAI improves precision and auditability under existing governance**. Conclusion: existing frameworks *can* be extended.

On the other side: an IJFMR paper (2026) finds "substantial discrepancies among traditional MRM frameworks" for ML (⚠ verify indexing rigour); and CRISIL's *MRM in Times of AI* (June 2023) states it most bluntly — "traditional or existing model risk management frameworks are plainly insufficient to handle them" (⚠ industry white paper, not peer-reviewed).

**Handle this honestly.** The sharpest statement of structural insufficiency is non-peer-reviewed; the peer-reviewed source concludes the opposite. Any P3 claim that traditional MRM is structurally inadequate for AI must acknowledge that the best-quality evidence currently cuts the other way — and the US carve-out of generative/agentic AI is arguably stronger evidence for insufficiency than any of the papers, since it is a regulator acting on the belief rather than an author asserting it.

Also: Heß, V.L. et al. (2025), systematic review of 46 studies mapping ML across credit, market and liquidity risk — peer-reviewed, 42 citations; application mapping rather than adequacy argument.

## **Instances in Corpus — ⚠ stale references to flag**

- [[04_Knowledge_Products/Wiki_Intake/Fed_OCC_SR11-7_Model_Risk_Management_2011]] — **SUPERSEDED 17 Apr 2026.** Retain for historical/citation purposes; do not cite as current guidance
- Five further notes reference SR 11-7 and need a currency check before use: [[04_Knowledge_Products/Wiki_Intake/Kurshan_Shen_Chen_AI_Model_Governance_2020]], [[04_Knowledge_Products/Wiki_Intake/Tammenga_AI_3LoD_Banks_2020]], [[04_Knowledge_Products/Wiki_Intake/F085_Sudjianto_Zhang_Model_Validation_Practice_Banking_2024]], [[04_Knowledge_Products/Wiki_Intake/McLemore_Mihov_AI_Operational_Losses_2025]], [[Institutional_Coherence]]
- [[04_Knowledge_Products/Wiki_Intake/Rao_Scepanovic_AI_Model_Risk_Catalog_2025]] — AI model risk catalogue
- [[04_Knowledge_Products/Wiki_Intake/Schuett_Three_Lines_Defense_AI_2023]] — the 3LoD-AI anchor, previously unwired
- [[04_Knowledge_Products/Wiki_Intake/MindForge_MAS_AI_Risk_Management_Executive_Handbook]] and [[07_Institutions/Corpus/International/International_34_MAS_FEAT_Veritas_AI_MRM]] — the MAS AI MRM Information Paper (5 Dec 2024), advisory
- [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]] — India's nearest equivalent, credit-scoped and still draft
- [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] — ¶4.4.68 AI inventory; Recommendation 24 AI Audit Framework

## **Confirmed Absences**

- **No HKMA, BoJ or BSP instrument equivalent to the MAS AI MRM paper was located.** ⚠ Stated as a search finding, not an exhaustive audit — these regulators may use "AI governance" rather than "model risk management" terminology. Verify against each regulator's own index before asserting.
- No Indian general-purpose model-risk instrument.

## **Linked Projects**

[[P3_BFSI_JEIM]] · [[P4_Doctrinal_IJLIT]] · [[fsQCA_Thesis_Chapter]]

## **Linked Domains**

[[BFSI_Governance]] · [[AI_Governance]] · [[International_Comparators]]

## **Linked Standard Concepts**

[[Explainability]] · [[Fairness]] · [[Human_Oversight]] · [[Agentic_AI_Governance]] · [[Accountability]] · [[Transparency]] · [[Proportionality]]

## **Linked Signature Concepts**

[[Assurance_Reuse_Gap]] · [[Governance_Debt]] · [[Evidentiary_Governance]] · [[Deontic_Bifurcation]]

## **Linked Frameworks**

[[RBI_Free_AI]] · [[Singapore_AI_Governance]] · [[ISO_IEC_42001]] · [[EU_AI_Act]]

## **Linked Methods**

[[Comparative_Regulatory_Analysis]] — the four-jurisdiction boundary comparison is a worked example of functional comparison across differing binding force

---

_Back to [[_Concepts_MOC]]_
