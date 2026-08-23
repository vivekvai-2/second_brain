---
type: Signature Concept
tags:
  - type/concept-signature
  - status/active
  - paper/p3
  - paper/p4
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/linkedin
  - content/carousel-ready
---

# **Deontic Bifurcation**

**Type:** Signature Concept
**Status:** Active
**Last Updated:** 2026-07-14 (introduced from [[Cross_Institutional_Mandate_Comparison]] + [[Systemic_Regulatory_Governance]])
**Theoretical Lineage:** Institutional Grammar (Crawford & Ostrom 1995; Frantz & Siddiki 2021); regulatory governance (Baldwin, Cave & Lodge 2012); law-and-technology scholarship on soft-law/hard-law interaction

---

## **Definition**

Deontic Bifurcation is the structural coexistence, within a single jurisdiction, of highly coercive, binding statutory mandates (deontic operator "SHALL" / MUST) alongside flexible, principles-based voluntary guidelines (deontic operator "SHOULD" / MAY) that govern the same technological capabilities or organisational activities. The pattern systematically drives regulated enterprises to allocate compliance investment toward the coercive binding mandates while under-investing in the aspirational principles — producing rigid compliance at the expense of ethical or normative depth. Deontic Bifurcation is analytically distinct from ordinary regulatory pluralism because the binding and aspirational instruments are aimed at *the same regulated activity* by *the same or closely related regulators*, not at complementary policy layers.

## **Application in This Research**

Within [[fsQCA_Thesis_Chapter]], Deontic Bifurcation is a candidate structural condition explaining variance in the Structural Readiness (SR) score across the 10-case configuration set — jurisdictions with high Deontic Bifurcation (e.g., India) score lower on SR than jurisdictions with unified deontic architectures (e.g., EU under the AI Act). Within [[P3_BFSI_JEIM]], Deontic Bifurcation is the empirical mechanism explaining why Indian BFSI enterprises deprioritise RBI FREE-AI's aspirational Seven Sutras in favour of RBI Digital Lending Directions' binding accountability chain and SEBI Reg 16C's sole-responsibility clause — the same institution can issue "shall" and "should" instruments in close succession, and enterprises rationally weight compliance investment toward the "shall" instrument. Within [[P4_Doctrinal_IJLIT]], Deontic Bifurcation is the doctrinal signature of the polycentric Indian AI regulatory architecture and provides the empirical anchor for critiquing the assumption that principles-based frameworks alone can shape enterprise behaviour without paired sanction-bearing rules.

## **Boundary Conditions**

- Deontic Bifurcation requires the coexistence of binding and aspirational instruments *within a single regulatory space* (typically the same regulator, or two regulators governing the same activity). Ordinary hard-law + soft-law layering across distinct policy domains does not constitute Deontic Bifurcation.
- The construct is empirically identifiable through ADICO coding: presence of at least one instrument coded with a strong deontic operator (SHALL/MUST) plus at least one instrument coded with a weak deontic operator (SHOULD/MAY) governing the same regulated capability.
- Deontic Bifurcation is neutral on whether the binding instrument is well-designed; the pattern describes the *architectural coexistence*, not the substantive adequacy of either instrument.
- The pattern is not equivalent to [[Regulatory_Parallelism]]: parallelism describes uncoordinated *equal-weight* mandates from independent regulators; bifurcation describes *unequal-weight* mandates (one binding, one aspirational) in the same regulatory space.

## **Theoretical Positioning**

Deontic Bifurcation is grounded in Institutional Grammar (IG2) scholarship, which distinguishes deontic operators (SHALL, SHOULD, MAY, MUST NOT) as structurally distinct types of institutional statement rather than variations along a single continuum. The construct extends Ostrom's original ADICO framework (Crawford & Ostrom 1995) into a diagnostic instrument for identifying architectural patterns in polycentric regulatory systems. It draws on law-and-technology scholarship (Lessig 1999; Reidenberg 1998) on how legal architecture shapes compliance behaviour, and on regulatory governance theory (Baldwin, Cave & Lodge 2012) that identifies command-and-control regulation and principles-based regulation as substitute rather than complementary strategies. Within PRIS, Deontic Bifurcation performs a bridging function: it operationalises the qualitative observation that Indian AI governance is "layered" or "polycentric" into an ADICO-codeable, measurable architectural feature that generates predictable enterprise-side compliance-allocation behaviour.

## **Empirical Manifestation in the Indian AI Regulatory Space**

| Regulatory Space | Binding Instrument (SHALL) | Aspirational Instrument (SHOULD) | Enterprise Behaviour |
|---|---|---|---|
| **BFSI AI Governance — RBI** | [[07_Institutions/Corpus/RBI/RBI_7]] Digital Lending Directions 2025 (RU1 non-delegable credit AI accountability) | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] FREE-AI Framework 2025 (Seven Sutras) | Enterprises invest in binding LSP due-diligence programmes and largely ignore the Seven Sutras' voluntary architecture |
| **BFSI AI Governance — SEBI vs. National AI** | [[07_Institutions/Corpus/SEBI/SEBI_14]] Reg 16C sole-responsibility clause | MeitY IndiaAI Guidelines 2025/26 (voluntary ethical principles) | SEBI-registered intermediaries treat 16C as the operative rule; MeitY guidelines are boardroom paperwork only |
| **Telecom AI Enforcement vs. National Principles** | [[07_Institutions/Corpus/TRAI/TRAI_1]] UCC Spam Direction 2026 (mandatory AI/ML deployment + DLT sharing) | MeitY IndiaAI Guidelines 2025/26 (voluntary responsible AI principles) | Telecom access providers implement DLT enforcement infrastructure and disregard the aspirational national principles |
| **Data Protection Board vs. Sectoral AI** | [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] Rule 13(3) SDF algorithmic due diligence | [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] Seven Sutras (voluntary) for BFSI SDFs | SDF banks execute DPDP-mandated DPIAs; Seven Sutras remain uncalibrated to their operations |

## **Literature Anchors (2026-08-02 — Perplexity Deep Research)**

Sourced per [[Thin_Node_Perplexity_Prompts_2026-08-02]]. Zotero remains the authoritative reference store; logged here for quick reuse in drafting.

**IG/ADICO deontic-component theory:**
- Crawford, S. E. S., & Ostrom, E. (1995). A Grammar of Institutions. *American Political Science Review*, 89(3), 582–600. Foundational: defines the Deontic component as the modal holder for "may" (permitted), "must" (obliged), "must not" (forbidden); distinguishes rules (ADICO, with Or Else) from norms (ADIC, no Or Else) from shared strategies (AIC, no Deontic) — this presence/absence and type distinction is the direct theoretical root of "bifurcation" as this concept defines it.
- Frantz, C. K., & Siddiki, S. (2021). Institutional Grammar 2.0: A Specification for Encoding and Analyzing Institutional Design. *Public Administration*. DOI 10.1111/padm.12719. Extends Deontic to constitutive statements via an analogous "Modal" component (required vs. optional).
- Frantz, C. K., & Siddiki, S. IG 2.0 Codebook, v1.4 (newinstitutionalgrammar.org). Operational definition: Deontic "defines to what extent the action of an institutional statement is compelled, restrained, or discretionary" — precise operational language for this concept's SHALL/SHOULD coding scheme.
- Pieper, L. et al. (2023). The Use of Institutional Grammar 1.0 for Comparative Institutional Analysis. *International Journal of the Commons*. Tabulates Deontic values as "may, must, must not, should, should not" — one of the few sources explicitly including should/should not within the Deontic value set, directly supporting this concept's mandatory/advisory bifurcation coding.
- Basurto, X. et al. (2009). First empirical application of Crawford & Ostrom's grammar to two pieces of US legislation — methods precedent for coding mixed-deontic legislative/regulatory text at the statute level (as opposed to a single circular).

**Soft-law/hard-law hybrid instrument-design theory:**
- SSRN working paper (30 November 2024), *Theoretical Foundations of Soft Law*, citing Medić (2024): "soft law instruments often coexist with binding rules, creating a hybrid regulatory environment" — direct theoretical framing of deontic bifurcation at the instrument-design level, independent of the IG/ADICO tradition.
- Reconnect Blog (6 October 2023), review of EU soft-law scholarship: bindingness and normativity are not necessarily correlated — supports treating deontic bifurcation as a spectrum rather than a binary.
- University of Amsterdam working paper, *The European Commission's Soft Law Instruments*: explicit linguistic marker — "'shall/will' language is likely to correspond to instruments intended to have legally binding effects, whereas conditional 'should' language...suggests non-binding provisions" — a citable methodological precedent for using deontic modality as a proxy for bindingness, directly supporting this concept's empirical coding method.

**NLP/computational deontic-modality coding (methods precedent for scaling the coding):**
- *Artificial Intelligence and Law* (Springer, DOI-bearing, contract-focused): ML classification of contract sentences by deontic modality, noting "obligation" is identified by must/shall, "permission" by may — the linguistic-marker method this concept's ADICO coding already uses, confirmed at computational scale (for contracts, not yet regulatory instruments — see gap below).
- Boginskaya, O. (2022). Corpus-based study of deontic modality ("shall, should, must, may") in international legal instruments — direct precedent for corpus-based coding of exactly these four markers.

### Confirmed Gaps — both are genuine original-contribution opportunities

1. **No peer-reviewed article in *Regulation & Governance* or *Law & Policy* was found under an explicit "hybrid instrument" or "differentiated regulation" title combining binding-rule-plus-soft-guidance analysis with a confirmed DOI** — available material is SSRN/blog-level or EU-soft-law-specific. A targeted direct journal-issue search is needed before concluding this gap is real rather than a search-round artifact, but as of this pass, no such article exists.
2. **No large-scale NLP deontic-modality study has been applied to a corpus of regulatory instruments** (as opposed to contracts) — the confirmed AI & Law article is contract-focused. This is directly actionable: PRIS's own ADICO-coded corpus (18 binding instruments, 450 requirement units per [[03_Domains/BFSI_Governance]]) could be the basis for exactly this kind of study, positioning PRIS's method as filling a confirmed literature gap rather than merely applying an existing one.
3. **No peer-reviewed academic paper analyzing an RBI, SEBI, or MeitY instrument through an explicit deontic-mixing/"mandatory-core-plus-advisory-annexure" lens was found.** This is the single strongest original-contribution gap identified across the entire 2026-08-02 sourcing pass: the best available evidence is SEBI's **own regulatory taxonomy**, not academic literature — SEBI formally distinguishes binding "Master Circulars" from non-binding "Advisory/Guidance Circulars" (visible on sebi.gov.in's Guidelines for Research Analysts page), which is itself strong primary evidence that Indian financial regulators design deontic bifurcation deliberately into their instrument architecture, rather than it emerging as an unintended side effect of uncoordinated rulemaking. This nuance is worth folding into the concept's Definition/Theoretical Positioning: SEBI's Master-vs-Advisory split suggests bifurcation can be a **designed** feature (SEBI's own taxonomy) as well as an **emergent** one (the RBI FREE-AI/RBI_7 pairing already documented below) — a distinction this concept note does not yet make explicit.

## **Instances in Corpus**

- (Batch 15 continuation — canonical grounding) [[07_Institutions/Corpus/RBI/RBI_7]] + [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] pair — the sharpest single-regulator instance of Deontic Bifurcation in the corpus: RBI issues a binding "shall" direction on digital lending AI accountability (May 2025) and, in the same regulatory period, publishes an aspirational "should" committee report on general AI governance (August 2025). Enterprises rationally allocate compliance investment to the binding instrument.
- (Batch 15 continuation) [[07_Institutions/Corpus/SEBI/SEBI_14]] + IndiaAI Guidelines pair — Reg 16C's binding sole-responsibility clause coexists with MeitY's aspirational national AI principles; SEBI-registered intermediaries treat the two as operationally unrelated.
- (Batch 15 continuation) [[07_Institutions/Corpus/TRAI/TRAI_1]] + IndiaAI Guidelines pair — TRAI's binding DLT-based enforcement direction coexists with MeitY's voluntary responsible AI principles; the binding instrument dominates telecom-sector behaviour.
- (Batch 15 continuation) [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] Rule 13(3) + [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] pair — horizontal binding data-protection algorithmic due diligence coexists with sectoral aspirational AI governance for SDF banks.
- (2026-08-02 — **Designed, not merely emergent, bifurcation**) SEBI's own regulatory taxonomy formally distinguishes binding **Master Circulars** from non-binding **Advisory/Guidance Circulars** (per sebi.gov.in's Guidelines for Research Analysts page; see also Cyril Amarchand Mangaldas FIG Paper No. 22, 26 June 2023, analyzing SEBI's June 2023 Master Circular consolidation). Unlike the RBI_7/RBI_FREE_AI_2025 pairing (two separately-timed instruments that happen to bifurcate), this is a case where the regulator has **built the SHALL/SHOULD split into its own instrument-issuing taxonomy** — the strongest available evidence that Deontic Bifurcation in Indian financial regulation is at least partly a deliberate architectural choice, not solely an artefact of uncoordinated multi-instrument issuance. No peer-reviewed academic treatment of this taxonomy through a deontic-mixing lens was located — flagged as the strongest original-contribution gap in this concept's literature base (see Literature Anchors above).

- **(2026-08-23 — bifurcation *within* a single instrument, across the individual/institution boundary)** [[07_Institutions/Corpus/CGPDTM/CGPDTM_1_AI_in_Patent_Examination_Guidelines_2026]] — every existing instance in this list pairs *two* instruments (one binding, one aspirational). CGPDTM_1 produces the same inversion inside one document: duties on the individual Examiner or Controller are uniformly **SHALL** (twelve use-case safeguard sets, six prohibitions in §5), while every institutional measure in §6 is **MAY** — use-logging, the AI Governance Committee, training, independent audit, impact assessment, incident reporting. §6(1) is the sharpest illustration: recording of AI use is conditional on the competent authority first choosing to prescribe it, so the evidentiary trail that would make every §4 and §5 SHALL auditable is optional at the institution's election. The committee's *composition* is mandatory while its *existence* is not. **Suggests the concept has an intra-instrument variant that the current pair-based coding cannot capture.**

See [[Corpus_Index_MOC]] for full node index.

## **Future Reuse Opportunities**

- Develop a *Deontic Bifurcation Diagnostic Instrument* for practitioner and board-level use, mapping a regulated enterprise's applicable instruments onto the SHALL/SHOULD grid and identifying compliance-allocation asymmetries.
- Extend fsQCA calibration by treating Deontic Bifurcation as an independent structural variable within the SR condition, testing whether jurisdictions with unified deontic architectures (EU) versus bifurcated architectures (India, US federal-state, Japan) generate different governance-legitimacy outcomes.
- Design an academic paper (target: *Regulation & Governance* or *Public Administration*) arguing that principles-based AI ethics frameworks in isolation produce Deontic Bifurcation and are therefore self-defeating unless paired with binding sanction-bearing rules.
- Translate into LinkedIn thought-leadership content on why "voluntary AI ethics guidelines don't work" — the practitioner-facing implication of Deontic Bifurcation.

## **Linked Projects**

[[P3_BFSI_JEIM]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## **Linked Domains**

[[AI_Governance]]

[[BFSI_Governance]]

[[Systemic_Regulatory_Governance]]

## **Linked Signature Concepts**

[[Regulatory_Parallelism]]

[[Governance_Debt]]

[[Institutional_Coherence]]

## **Linked Standard Concepts**

[[Accountability]]

[[Legitimacy]]

[[Assurance_Reuse_Gap]]

## **Linked Methods**

[[Institutional_Grammar_IG2]]

[[fsQCA]]

---

_Back to [[_Concepts_MOC]]_
