---
type: Signature Concept
status: active
last_updated: 2026-08-09
tags:
  - type/concept-signature
  - status/active
  - concept-class/signature
  - paper/p4-primary
  - paper/p3
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - engine/linkedin
  - content/carousel-ready
concept_class:
  - signature
linked_domains:
  - "[[03_Domains/AI_Governance]]"
  - "[[03_Domains/Cybersecurity_Governance]]"
  - "[[03_Domains/BFSI_Governance]]"
  - "[[03_Domains/Judicial_Governance]]"
linked_projects:
  - "[[02_Projects/P4_Doctrinal_IJLIT]]"
  - "[[02_Projects/P3_BFSI_JEIM]]"
---

# **Evidentiary Governance**

**Type:** Signature Concept **Status:** **ELEVATED to signature class 2026-08-09** (was: candidate, pending P4 execution) **Last Updated:** 2026-08-09

> ### Elevation record — 2026-08-09
>
> Elevated from candidate to signature class. The prior condition was "pending P4 execution," which was circular: the construct could not be used in P4 while held at candidate class, and could not be elevated until used. The substantive grounds now stand independently of P4:
>
> 1. **Gate passed with seven verified corpus instances**, not three — RBI_8, RBI_1, CERT_In_1, MeitY_4, International_22, DHC_1, CEA_3 — spanning four regulators, two jurisdictions, one judgment, and both BFSI and critical-infrastructure sectors.
> 2. **Its primary contribution candidate (OQ-EG-01) is no longer blocked.** BSA_1 exists; the crosswalk it called for has been performed and is written up at [[06_Frameworks/Evidentiary_Destination_Matrix]], which produced a publishable headline finding — the s.63(4) certificate-readiness column is empty across the entire Indian corpus.
> 3. **It has generated a downstream framework and a knowledge product** ([[06_Frameworks/Evidentiary_Destination_Matrix]], [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]) and supplies the artefact-class specification for a second concept ([[05_Concepts/05_Concepts_Standard/Orchestration_Governance]]). Generativity of that kind is the practical test of signature status.
> 4. **The naming collision that muddied it is resolved** (see Intersection section).
>
> **Reversible.** If P4 develops without this construct as its organising axis, demote to candidate and record the reason here. The elevation is a working judgment, not a commitment.
**Theoretical Lineage:** Forensic readiness (Tan 2001; Daubner et al. 2023); assurance-case and safety-case scholarship (ISO/IEC/IEEE 15026; Clymer et al. 2024); AI audit ecosystem (Raji et al. 2024; Goodman & Trehu 2023); institutional decoupling (Meyer & Rowan 1977); electronic-evidence doctrine (Bharatiya Sakshya Adhiniyam 2023, s.63 — ⚠ corpus node not yet created)

---

## **Definition**

**One-sentence definition.** Evidentiary Governance is the governance regime constituted by the artefacts a regulated entity is obliged to *generate and retain* — rather than the rules it is obliged to *follow* — and by the question of whether those artefacts are sufficient to reconstruct, independently verify, and where necessary legally prove what an automated system actually did.

**Full analytical definition.** Evidentiary Governance treats retained technical artefacts as the operative unit of AI accountability, positioned as a distinct analytical layer beneath policy (which declares intent) and control (which specifies mechanism). The construct holds that an obligation is only as enforceable as the artefact trail it generates, and that regulatory instruments can therefore be diagnosed along an *evidentiary* axis independent of their substantive content: what must be recorded, by whom, in what form, for how long, and to whose satisfaction. Its diagnostic power lies in separating three questions that governance scholarship routinely conflates — whether an obligation exists, whether it is complied with, and whether compliance is *demonstrable to a third party under adversarial conditions*.

**Plain-language practitioner definition.** Policies say what should happen. Controls say how. Evidence proves what actually did happen — and most organisations collect the first two and almost none of the third in a form that would survive an auditor, a regulator, or a court.

---

## **Problem the Concept Solves**

Four adjacent literatures each capture part of this territory and none captures the whole:

1. **AI audit scholarship** (Raji et al. 2024; Goodman & Trehu 2023, per [[04_Knowledge_Products/Wiki_Intake/F123_Sloane_Moss_Chowdhury_Hiring_Algorithms_Auditability_2021]] and [[04_Knowledge_Products/Wiki_Intake/Costanza_Chock_Who_Audits_the_Auditors_2022]]) theorises the *audit* as the accountability mechanism but leaves the evidentiary substrate audits depend upon undertheorised — it asks who audits, not what they audit against.
2. **Assurance- and safety-case scholarship** (ISO/IEC/IEEE 15026 lineage) subordinates evidence to argument: a safety case is explicitly "not simply a repository of evidence." Evidentiary Governance inverts this, treating the repository itself as the governable object.
3. **Forensic-readiness scholarship** (Tan 2001; Daubner et al. 2023) supplies the design logic — build systems that generate sound evidence — but is pre-AI and general-IS, with no engagement with probabilistic, non-deterministic systems or with AI-specific artefact classes.
4. **Documentation and disclosure norms** — model cards and datasheets, per [[04_Knowledge_Products/Wiki_Intake/F080_Mitchell_et_al_Model_Cards_for_Model_Reporting_2019]] and [[04_Knowledge_Products/Wiki_Intake/F081_Gebru_et_al_Datasheets_for_Datasets_2018]] — are point-in-time voluntary disclosures, not continuous retained records, and are therefore structurally incapable of answering "what did this system do on 14 March."

Evidentiary Governance unifies these by supplying a single analytical axis — artefact generation and retention — along which any instrument, whether Indian sectoral circular or EU horizontal regulation, can be coded and compared.

---

## **Constitutive Dimensions**

| Dimension | Diagnostic question | Corpus anchor |
|---|---|---|
| **Artefact specification** | Does the instrument name the artefact class to be retained, or only the obligation? | [[07_Institutions/Corpus/RBI/RBI_1]] §15 names audit/logging capability explicitly; most Indian AI instruments do not |
| **Retention horizon** | For how long, and does the period cohere with adjacent regimes? | See [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] — the dedicated sub-pattern |
| **Custody and integrity** | Are chain-of-custody, tamper-evidence, and localisation specified? | [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] §16.6 — India-resident storage, encryption, forensic-irretrievability wipe certification |
| **Evidentiary destination** | Is the artefact designed for supervisory inspection, or for adversarial legal proof? | Unresolved across the entire Indian corpus — see Open Questions |

The fourth dimension carries the construct's principal analytical weight and is the least addressed in the literature.

---

## **Three-Instance Gate — Status: PASSED (2026-08-02)**

Per [[00_MOC/Workflow_Discipline_Protocol]] CDW-1, entry requires three distinct primary-source corpus instances **or** theoretical load-bearing in an active paper. Both limbs are satisfied. Every node cited below was verified present in the vault on 2026-08-02; none is inferred.

| # | Corpus node | Evidentiary provision (verified in node text) |
|---|---|---|
| 0 | **[[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]]** | **Canonical instance (added 2026-08-02).** Para 95 — audit trails shall satisfy "regulatory and legal requirements," be sufficient "to facilitate the conduct of audits, serve as forensic evidence... and assist in dispute resolution, including for **non-repudiation** purposes." Definition 14 defines *digital forensics* as "the process used to acquire, preserve, analyse, and report on evidence using scientific methods that are demonstrably reliable, accurate, and repeatable," attributed to NIST. Para 220(5) requires CSOC capability for "clear attribution of actions including who did what, when and how, along with preservation of evidence." The most evidentially specified instrument in the corpus. |
| 1 | [[07_Institutions/Corpus/RBI/RBI_1]] | §15 — every IT application accessing critical/sensitive information must have audit/logging capability; audit trails must **support forensic evidence and dispute resolution**. ⚠ **Superseded for Commercial Banks** by RBI_8 para 95 (31 July 2026) — retained as the 2023 antecedent in the evidentiary time series, which now runs 2023 → 2026 with strengthening language at each step. |
| 2 | [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] | §16.6 — audit data India-resident, encrypted in transit/at rest, forensically wiped with irretrievability certification post-engagement, retained one year by default. A full custody regime for audit artefacts. |
| 3 | [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] | Rule 6 — minimum one-year retention of logs and personal data **specifically for breach investigation**; Seventh Schedule log-retention obligation. Evidentiary purpose stated on the face of the instrument. |
| 4 | [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] | Art. 33 (five-year subcontracting documentation) and Art. 47 + Annex V (ten-year machine-readable Declaration of Conformity retention). The comparative benchmark for specified artefact classes with stated horizons. |

**Theoretical load-bearing:** the construct is the organising axis for the [[02_Projects/P4_Doctrinal_IJLIT]] doctrinal critique and supplies the evidentiary calibration dimension for [[02_Projects/P3_BFSI_JEIM]].

---

## **Intersection with Signature Constructs**

**[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]** — Evidentiary Governance exposes parallelism at a layer the existing matrix does not reach. [[06_Frameworks/Cross_Regulator_Coordination_Pattern_Matrix]] documents parallelism in *rule design*; Evidentiary Governance documents it in *artefact specification*, where four Indian regulators independently mandate functionally equivalent logging without common artefact definitions, formats, or horizons.

**[[05_Concepts/05_Concepts_Signature/Governance_Debt]]** — supplies a new debt variant: *evidentiary-destination debt*, where an instrument mandates retention without specifying whether the retained artefact must satisfy supervisory inspection or legal admissibility, leaving the regulated entity to guess at the standard. ✅ **Naming collision resolved 2026-08-09** — Governance_Debt's variant (absence of primary source in the vault, a research-quality issue) has been renamed **Source-Verification Debt**; *evidentiary-destination debt* keeps this name unambiguously and is now operationalised in [[06_Frameworks/Evidentiary_Destination_Matrix]], which finds it universal across the Indian corpus: **not one instrument states what its retained artefacts are for.**

**[[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]** — the strongest coherence test available. Instruments may converge on principle (the Seven Sutras / IOSCO / SEBI convergence documented at [[07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025]]) while diverging completely on the artefacts that would evidence compliance. Principle-level coherence without artefact-level coherence is coherence that cannot be verified.

**[[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]]** — the closest existing PRIS construct and the necessary disambiguation. Assurance_Reuse_Gap concerns the *non-transferability of a produced artefact* across regulators. Evidentiary Governance concerns *whether the artefact is specified, generated and retained at all, and to what evidentiary standard*. The former presupposes the latter. Where both are absent, the enterprise carries duplicated audit cycles producing artefacts that would satisfy neither regulator adversarially.

---

## **Empirical Manifestation in the Indian Regulatory Space**

The Indian corpus displays a consistent asymmetry: **evidentiary obligations are specified with far greater precision in cybersecurity instruments than in AI-specific instruments.** CERT-In's audit-policy guidelines specify custody, localisation, encryption and destruction; [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] mandates data-lifecycle governance covering retention and deletion without specifying artefact classes, formats, or horizons for AI-specific records. [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] advances furthest at the principle level, naming "immutable audit trails" under Security by Design and "named ownership, immutable logging" under Accountability and Traceability — but as a non-binding framework it specifies no horizon and no custody regime.

The result is that India's most AI-explicit instruments are its least evidentially specified, while its most evidentially specified instruments are technology-neutral. This inverts the intuitive expectation and is a directly publishable finding.

**RBI_8 (31 July 2026) confirms the asymmetry at its sharpest.** The instrument that most fully specifies evidentiary obligations anywhere in the corpus — non-repudiation, NIST-sourced forensic definition, four-part attribution requirement — contains **zero** AI provisions across 56 pages (verified by full-text sweep: *artificial intelligence* 0, *machine learning* 0, *model risk* 0, *generative* 0, *automated decision* 0, bare token `AI` 0). The asymmetry is therefore not a lag that later instruments close; it is reproduced in the newest instrument available, by a regulator that had already published its own AI framework. This substantially strengthens the finding.

**But the asymmetry is a deontic artefact, not an absence — RBI_9 (2026-08-02 intake).** [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]], issued ~June 2026, reportedly covers **"logging, traceability and forensic readiness"** as a named AI control domain — the construct's own theoretical core, in an Indian financial regulator's own words, six weeks before RBI_8 omitted AI entirely.

The corrected finding is therefore not that Indian AI instruments lack evidentiary specification and Indian evidentiary instruments lack AI. It is that **RBI possesses both vocabularies and has not combined them in binding text**: AI-with-forensic-readiness sits in a non-binding, apparently unpublished advisory; forensic-evidence-with-non-repudiation sits in the binding Directions, AI-free. This is [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] operating on the evidentiary axis, and it is a more precise and more publishable claim than the original asymmetry statement.

⚠ RBI_9 is Tier C — primary text not obtained, and the "forensic readiness" formulation is KPMG's characterisation rather than RBI's own heading (⚠ V-RBI9-3). **Confirm before building an argument on it.**

**CERT_In_3 (25 May 2026) supplies the same pattern from a different regulator.** It requires "evidence preservation" twice (§6.10, §10.1), audit logging for agentic AI (§12.14), and auditability for AI-assisted decisions (§12.10) — but is non-binding throughout, specifies no custody standard, no artefact format and no retention horizon. Artefact specification without evidentiary destination, precisely the fourth-dimension gap this construct predicts.

---

## **Operationalisation (IG 2.0 / ADICO)**

Full coding belongs in NVivo; this note records the construct-level coding scheme only.

| ADICO element | Evidentiary Governance operationalisation |
|---|---|
| **Attribute** | The entity obliged to generate and hold the artefact (provider, deployer, auditor, regulated entity) — distinct from the entity obliged to *perform* the governed act |
| **Deontic** | Strength of the retention obligation (SHALL / SHOULD / MAY), coded separately from the strength of the substantive obligation it evidences |
| **Aim** | Evidentiary destination — supervisory inspection, internal assurance, or adversarial legal proof |
| **Condition** | Triggering event for production (incident, scheduled audit, breach, regulator direction, court order) |
| **Or-else** | Consequence of non-retention or non-production, coded separately from the consequence of the underlying breach |

The *Aim* dimension is the novel coding contribution: existing ADICO applications in the vault do not distinguish evidentiary destination.

---

## **Judicial Test — the construct's first contact with a court (2026-08-02)**

[[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] (Delhi High Court, 24 July 2026) is the first Indian judicial determination on LLM training and copyright, and it supplies two findings that the construct did not anticipate.

**1. Where no evidentiary layer exists, a court reconstructs from vendor metadata.** The output claim was decided without a training-data manifest, inference logs, retention record, or anything else from the defendant's systems. The Court reasoned from **published training cut-off dates** against article publication dates and concluded that memorisation was impossible (para 83). The dispositive evidence of what a model did was a date the vendor had published about itself.

This is the construct's fourth dimension — evidentiary destination — resolving itself by default. No instrument required the artefacts to exist, so none did, so the court used what was left. The rights-holder could not test the assertion because there was nothing to test it against.

**2. Prompt design is now an evidentiary standard in Indian law.** Para 104 introduces **adversarial prompting** as a legal category, with academic citation: prompts are "carefully designed inputs that manipulate model outputs." The Court distinguished *GEMA v. OpenAI* (Munich Regional Court, 11 Nov 2025 — which found memorisation) precisely on this ground: GEMA's prompts were non-adversarial, ANI's used the word "exactly" (para 119).

The consequence is that **the method of interrogating a system now bears on the weight of the resulting evidence**. This is a new dimension for the construct and it sits outside the existing four: not what artefact is retained, for how long, in whose custody, or to what end — but *how the system was questioned to produce the artefact in the first place*. No instrument in the corpus addresses how prompt-elicited evidence should be captured, logged, timestamped or authenticated. Add as a candidate fifth dimension — **interrogation provenance** — pending a second instance.

**3. The admissibility question was never engaged.** The judgment contains no reference to the Bharatiya Sakshya Adhiniyam, no s.63 certification analysis, no direction on preservation. **OQ-EG-01 is not merely unanswered: India's first AI copyright case reached final interlocutory disposal without any party or either Amicus raising it.** That is stronger evidence of the gap than the gap itself.

⚠ Interim order, expressly prima facie, appealable — see DHC_1 status caveat and ⚠ V-DHC1-1.

---

## **Open Research Questions**

**OQ-EG-01 (primary contribution candidate).** Would artefacts generated to satisfy EU AI Act Art. 12 logging or ISO/IEC 42001 documented-information requirements satisfy the certification conditions for electronic-record admissibility under Bharatiya Sakshya Adhiniyam s.63(4)? The technical-standards literature and the evidence-law literature do not currently speak to each other.

> ✅ **BLOCKER CLEARED 2026-08-09.** The original flag read: *"no BSA corpus node exists in the vault — s.63 provisions cited here derive from external Deep Research (2026-08-02), not from vault primary-source intake. A BSA_1 corpus node must be created before this question is used in any publication-track output."* **That node exists** — [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]], created 2026-08-02, the same day this flag was written. The flag was never updated. **OQ-EG-01 is unblocked.**
>
> BSA_1's own Log specifies the next step, still not done: *"systematically check RBI_8, CERT_In_2/3, SEBI's AI/ML reporting circulars, and DPDP's breach-notification retention rules against s.63(2)'s four conditions and s.63(4)'s certificate-signatory requirement."* **Add [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] to that list** — as the corpus's most artefact-specified instrument it is the strongest test case, and its silence on admissibility is the most telling.

**OQ-EG-02.** Are Indian sectoral logging mandates (RBI, SEBI, CERT-In) designed with eventual litigation use in mind, or purely for supervisory purposes? Neither [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] nor the SEBI AI instruments reference evidentiary or admissibility standards anywhere in the coded corpus.

**OQ-EG-03.** How do the BSA s.63(2) conditions — regular use, proper operation, ordinary course of business, carried forward from Indian Evidence Act s.65B — apply to probabilistic, non-deterministic systems whose defining property is that identical inputs need not produce identical outputs?

**OQ-EG-04.** What chain-of-custody standard should apply to model weights, inference logs, and prompt/output pairs? No instrument in the corpus, Indian or international, addresses this.

**OQ-EG-05 (new, 2026-08-02).** Should prompt provenance be a governed artefact class? [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] makes the adversarial or non-adversarial character of a prompt determinative of evidentiary weight, while no instrument specifies how prompts and their outputs are to be captured, timestamped or authenticated. A litigant's screenshot is currently the entire evidentiary record.

**OQ-EG-06 (new, 2026-08-02).** Where a regulated entity is required to retain nothing, does the evidentiary burden shift *de facto* to vendor-published metadata — and what governance consequences follow from a defendant's own published claims about its systems becoming the dispositive evidence about those systems?

---

## **Provenance and Correction Record**

> ⚠ **The content side of this correction was not closed until 2026-08-09.** The vault was corrected on 2026-08-02; the carousel carrying the false attribution kept circulating for a further week because nothing linked the corrected concept back to the artefact. Logged as **C-01** in [[11_Content/Content_Correction_Register]], which now exists as the reverse index for exactly this failure mode. Check it before republishing any practitioner artefact.

The construct originated in practitioner content drafted 2026-08-01 and was verified against external Deep Research on 2026-08-02. **One material correction was applied at intake:** the originating draft attributed a "Digital Forensics Artifact Catalog" to NIST. No such NIST publication exists. NIST's actual outputs in this space are CFTT (forensic *tool* reliability testing), CFReDS (reference test datasets), and SP 800-86 (2006, unsuperseded — a four-phase forensic *process* guide: collection, examination, analysis, reporting). The community-maintained ForensicArtifacts/Artifact Definitions repository is the nearest artefact catalogue and has no institutional relationship to NIST. **The forensics-to-AI-oversight structural analogy does not depend on the NIST attribution and survives its removal.** Any downstream content reusing this construct must not repeat the original attribution.

### **Replacement NIST anchor — verified 2026-08-02**

A genuine, citable NIST-to-India evidentiary transmission exists and should be used in place of the withdrawn attribution. [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] Definition 14 imports a digital-forensics definition into binding Indian banking regulation, expressly attributed to *NIST Cloud Computing Forensic Science Challenges*. This is stronger than the original claim in every respect that matters: it is an actual instrument, actually citing NIST, actually binding, actually Indian, and dated 31 July 2026.

⚠ Confirm the underlying source is NISTIR 8006 before publication-track citation — RBI names the report title without a NISTIR number and says "adapted from," not "reproduced" (⚠ V-RBI8-2).

---

## **Reuse Across the Five Output Pockets**

- **Research (R):** organising axis for [[02_Projects/P4_Doctrinal_IJLIT]]; evidentiary calibration dimension for [[02_Projects/P3_BFSI_JEIM]] and [[02_Projects/fsQCA_Thesis_Chapter]].
- **Consulting (C):** directly operational for [[10_Consulting/Board_AI_Risk_Oversight_Checklist]] and the Common Evidence Repository recommendation already carried in Assurance_Reuse_Gap.
- **Thought Leadership (TL):** the policy → control → evidence → assurance → trust ladder is carousel-ready; see [[11_Content/ADP_Keynote_2026]] for audience fit.
- **Knowledge Product (KP):** fills an identified evidentiary gap in [[04_Knowledge_Products/AI_Governance_Wiki]] and [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]].

---

## **Distinguished From**

**Governance age / temporal validity** ([[04_Knowledge_Products/Wiki_Intake/F142_Azimi_Temporal_Validity_Governance_Age_2026]], 2026) — **the closest external construct, and genuinely distinct.** Both concern representational correspondence between governance instruments and the systems they govern. They differ in **target** and **time-direction**:

| | Evidentiary Governance | Governance age |
|---|---|---|
| Asks | Can the retained artefact **prove**, adversarially and retrospectively, what the system **did**? | Does the artefact still accurately **describe** what the system currently **is**? |
| Direction | Retrospective — proof of past conduct | Present-state — accuracy of current description |
| Test | Admissibility, custody, non-repudiation, third-party verification | Correspondence between representation and system reality |
| Fails when | The artefact exists but cannot be certified, retained long enough, or independently verified | The artefact is impeccable and describes a system that has since changed |

The two are independent: an instrument can be perfectly current in its description and still unprovable ([[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] — seven retention horizons, zero certificate-readiness), or perfectly provable while describing a configuration that no longer exists.

**A boundary condition worth keeping:** governance age presupposes a representation to become inaccurate. Where an instrument makes no claim about a system at all — CEA_3 says nothing about the ML running on the grid — the failure is prior and different, and belongs to [[05_Concepts/05_Concepts_Signature/Decision_Infrastructure]] rather than to either construct here.

**[[06_Frameworks/Manifestation_Evidence_Layer]]** — no relationship despite the similar name. That framework is the P3 empirical evidence layer (SOM Tables S17–S21) documenting how cross-regulator coordination patterns M1–M5 *manifest*; "evidence" there means research evidence for a coordination claim. Evidentiary Governance concerns evidence as a *regulated artefact class*. The two must not be conflated in drafting.

---

## **Instances in Corpus**

- [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] — **canonical instance**; paras 93/95/97, Definition 14, para 220(5)
- [[07_Institutions/Corpus/RBI/RBI_1]] — §15 audit trails for forensic evidence and dispute resolution (2023 antecedent; superseded for Commercial Banks)
- [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] — §16.6 audit-data custody regime
- [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — Rule 6 breach-investigation retention
- [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] — Arts. 33, 47 + Annex V retention horizons
- [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] — **judicial instance**: model behaviour reconstructed from vendor-published training dates absent any retained artefact; prompt design made an evidentiary standard; BSA never engaged
- [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] — evidence preservation (§6.10, §10.1); agentic audit logging (§12.14); auditability (§12.10); **no custody standard, no horizon**
- [[07_Institutions/Corpus/RBI/RBI_9_AI_Accelerated_Cyber_Threats_Advisory_2026]] — "logging, traceability and forensic readiness" as a named domain ⚠ Tier C
- [[07_Institutions/Corpus/IRDAI/IRDAI_2_Working_Group_AI_Governance_2026]] — pre- and post-deployment AI audit framework mandated, due ~18 Sep 2026 (watch item)
- [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] — immutable audit trails at principle level, unspecified at operational level
- [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] — Ch. 4.C evidence tampering and deepfakes; the corpus's only judicial-side evidentiary treatment
- (2026-08-09) [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] — **the corpus's most completely specified instrument on the first two constitutive dimensions.** *Artefact specification:* a **First Schedule** naming twelve mandatory retained document classes (Cyber Security Policy and its procedures, Cyber Crisis Management Plan, Data Retention Policy, ISO 27001/TCC certificate, asset register, Cyber Risk Assessment and Mitigation Plan, Incident Response and Recovery Plan, incident register, **Bill of Materials**, Business Continuity Plan, remote operation procedure, remote access procedure) placed in the CISO's custody by reg 7(3)(i). *Retention horizon:* **seven distinct periods** (see [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] §Inversion). *Custody and integrity:* India-resident encrypted storage (reg 5(19)), access restricted to authorised persons under a defined access-control procedure, forensic records retained 180 days and incident-associated logs 365 days spanning ±180 days around the event (reg 8(33)(h)–(i)). Notified the **same day** as RBI_8 and specifying everything RBI_8 delegates — the sharpest available demonstration that the fourth dimension's absence elsewhere is elective. *Evidentiary destination:* still unresolved here too — the instrument nowhere states whether retained artefacts must satisfy supervisory inspection or adversarial legal proof, and does not engage the Bharatiya Sakshya Adhiniyam. **The construct's fourth-dimension gap therefore survives even the corpus's best-specified instrument**, which is a stronger form of the OQ-EG-01 finding than the Indian AI instruments alone supply.

---

- **(2026-08-23 — a record contemplated but never mandated, and no retention period)** [[07_Institutions/Corpus/CGPDTM/CGPDTM_1_AI_in_Patent_Examination_Guidelines_2026]] §6(1) — the competent authority **may prescribe** that material AI use be recorded (tool name, nature of use, date of use, anything else needed for supervision, audit or quality review), and such disclosure **may** be made available to stakeholders. Neither the record nor its disclosure is mandatory, and **no retention period is specified**. Relevant to [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] as a further Indian instrument contemplating a record without stating how long it is kept — ⚠ confirm the running instance count against that note before citing a number. Note also ⚠#370: **Annexure-II (Checklist and declaration) is absent from the source file** and is plausibly the instrument's actual evidentiary mechanism; this entry makes no claim about it.

## **Log**

- 2026-08-02: Concept created at candidate class. Three-Instance Gate passed against four verified corpus nodes. NIST attribution error corrected at intake (see Provenance). BSA corpus-node gap flagged as blocking for OQ-EG-01. Naming collision with the existing *evidentiary debt* variant in [[05_Concepts/05_Concepts_Signature/Governance_Debt]] flagged for resolution at next indexing pass.
- 2026-08-02 (later, ad-hoc intake): [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] intake on day of issuance materially strengthens the construct. Para 95 replaces RBI_1 §15 as canonical instance; Definition 14 supplies a verified NIST anchor replacing the withdrawn attribution; para 220(5) supplies a binding four-part reconstruction requirement; para 97 supplies the retention-abdication case. Empirical Manifestation section updated — the AI/evidentiary asymmetry is reproduced, not closed, by the newest instrument. **Gate now stands at five verified corpus nodes.**

---

*Back to [[_Concepts_MOC]]*
