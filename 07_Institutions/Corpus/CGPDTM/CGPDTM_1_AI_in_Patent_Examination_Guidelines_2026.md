---
type: Corpus Node
node-id: CGPDTM_1
institution: CGPDTM
date: 2026-08-07
status: active
last_updated: 2026-08-23
wiki-section: S2
tier: A
ai-explicit: true
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/cgpdtm
  - institution/dpiit
  - tier/A
  - batch/desktop-20260823
  - concept/Deontic_Bifurcation
  - concept/Governance_Debt
  - concept/Regulatory_Parallelism
  - concept/Institutional_Coherence
  - concept/Human_Oversight
  - concept/Accountability
  - concept/Governance_Capacity
  - concept/Contestability_Redress
  - project/p1
  - project/p4
---

# CGPDTM_1 — Guidelines for the Use of Artificial Intelligence in Patent Examination Procedure

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/CGPDTM/CGPDTM_1_AI_in_Patent_Examination_Guidelines_2026.md`
**Institution:** [[07_Institutions/CGPDTM]]
**Issuing body:** Office of the Controller General of Patents, Designs and Trade Marks (O/o CGPDTM), under [[07_Institutions/DPIIT]], Ministry of Commerce and Industry ⚠ **VERIFY** — see ⚠#369
**Document date:** ⚠ **Not stated on the face of the document.** PDF creation metadata reads 7 August 2026, which is not a publication date. See ⚠#369
**Pages:** 16 pages (Guidelines proper, self-paginated "N of 16") + Annexure-I, 34 pages ("Page N of 34"). Annexure-II is referenced but **absent from the file** — see ⚠#370
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/Systemic_Regulatory_Governance]]

---

## ⚠ Scoping note — read before citing

**This instrument governs AI use *by the State*, not by regulated entities.** It binds Patent Office Examiners and Controllers in the discharge of their statutory and quasi-judicial functions. It creates no obligation for any applicant, patentee, or third party, and it is not a regulation of AI in the economy.

It is admitted to the corpus as **Tier A** nonetheless, on three grounds: (1) it is explicit, operative, AI-specific administrative law with SHALL-form obligations; (2) it is the first instrument in this corpus in which an Indian statutory authority regulates its own use of AI inside a quasi-judicial process, which is a distinct governance mode the corpus has otherwise captured only in white-paper form; (3) its deontic structure — hard duties on the individual officer, discretionary duties on the institution — is a clean new instance of the pattern tracked at [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]].

---

## Instrument Identity

**Full title:** Guidelines for the Use of Artificial Intelligence in Patent Examination Procedure
**Type:** Internal administrative guidelines / operating instruction. ⚠ No commencement clause, notification number, or in-force statement was found — see ⚠#371
**Target entities:** Examiners and Controllers of the Indian Patent Office; the "competent authority" of the O/o CGPDTM; the AI Governance Committee it contemplates
**Legal basis:** Not stated. The Guidelines are framed as governing the exercise of examination functions under the Patents Act, 1970, but cite no enabling provision. They cite [[07_Institutions/Corpus/NITI_Aayog/NITI_3]] (NITI Aayog, *Responsible AI #AIFORALL*, Parts 1 and 2) as background policy support
**Companion documents:** [[07_Institutions/Corpus/DPIIT/DPIIT_1]] — same ministry, adjacent subject (generative AI and copyright), **no cross-citation in either direction**

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework); secondary S6 (Implementation & Governance Artifacts — the safeguard table is directly reusable)
**Jurisdiction:** India
**Confidence:** High for content — full clean text extraction of the Guidelines and Annexure-I. **Medium for provenance** — undated, unnumbered, issuing authority inferred from an internal self-reference
**AI explicit:** Yes — AI is the entire subject matter
**Tier classification:** **Tier A** — explicit, operative AI-specific instruction, subject to the scoping note above
**AI Governance Wiki relevance:** **HIGH** — supplies the corpus's first worked example of a State body binding its own officers' AI use inside a rights-determining process, with a twelve-row use/risk/safeguard table that is directly transferable to enterprise practice.

---

## Substantive Content

### Structure

| § | Heading | Content |
|---|---|---|
| 1 | Introduction | Overview, Objective, Scope |
| 2 | Terminologies | Six definitions (2.1–2.6) |
| 3 | Limitations and risks, and the need for human oversight | Fourteen enumerated risks (3.1.1–3.1.14); §3.2 human oversight |
| 4 | Typical uses of AI in patent examination, potential risks and associated safeguards | Twelve numbered use-case rows |
| 5 | Prohibited Uses | Six prohibitions, (a)–(f) |
| 6 | Administrative Measures | Four measures; AI Governance Committee composition |
| Annexure-I | Illustrative examples | 34 pages of worked AI outputs with errors marked |
| Annexure-II | Checklist and declaration | ⚠ Referenced twice; **not present in the file** (⚠#370) |

### Definitions (§2)

Six terms are defined: **Artificial Intelligence** (a machine-based system generating predictions, recommendations, classifications, summaries or content from input data and prompts); **AI prompt**; **Generative Artificial Intelligence**; **AI tool**; **Public AI tools**; **Private AI tools**. The public/private split is the operative distinction in the instrument — it is what §5(a) turns on.

The AI definition is **outcome-based and notably broad**, capturing classification and summarisation systems, not merely generative ones. It does not track the OECD or EU AI Act formulations and contains no autonomy, adaptiveness, or inference-from-input elements.

### Scope (§1.3)

The Guidelines apply to AI use in patent examination tasks: **screening, classification, search, translation support, drafting support, technical comparison, and knowledge retrieval.**

### Risk taxonomy (§3.1)

Fourteen enumerated risks, of which the operationally distinctive ones are: profile sensitivity; prompt discipline; hallucination or fabrication; omission of critical detail; false pattern matching; loss of technical context; classification and search drift; over-breadth or over-narrowness; black-box opacity; confidentiality risk; misguidance; incomplete or outdated data; bias in training data and results; difficulty with complex patent language.

This is a **first-party regulator taxonomy of LLM failure modes** written for a document-intensive quasi-judicial function. It is materially more specific than the generic risk lists in the international framework nodes.

### Use/risk/safeguard table (§4)

Twelve rows, each with four columns: *S. No*, *Type of use*, *Possible benefits*, *Potential risks*, and enumerated safeguards. Uses run from IPC/CPC classification and prior-art search through claim-feature extraction, translation support, office-communication drafting, clarity and sufficiency assessment, to understanding case law.

The safeguard column is uniformly **SHALL**-form and converges on one rule: AI output is preliminary; the officer's own analysis and application of mind is determinative; nothing issues without personal satisfaction. Representative examples:

- On clarity objections: *"No clarity objection shall be issued unless the officer is personally satisfied as to its legal and technical basis."*
- On case law: *"No verbatim quote, ratio, paragraph, or legal proposition generated by AI shall be relied upon without checking the primary source."* Where AI output is found to contain fabricated, paraphrased or misattributed material, **it shall be discarded.**
- On novelty and inventive step: the final conclusion *"shall be based on the officer's own analysis and application of mind."*

The Guidelines also record a factual premise worth noting: the patent search databases the Office subscribes to **already contain in-built AI tools**, which the instrument classes as private AI tools offering better data security and better patent-context prompt comprehension. The instrument is therefore regularising an existing deployment, not authorising a new one.

### Prohibited uses (§5) — six, mandatory

| | Prohibition |
|---|---|
| (a) | Entering unpublished patent application contents, confidential office records, or internal deliberative material into **public** AI tools |
| (b) | Using AI as a substitute for the Examiner's or Controller's application of mind on substantive matters — novelty, inventive step, industrial applicability, sufficiency, clarity, unity of invention |
| (c) | Issuing office actions, FERs, hearing notices, decisions or other official communications solely on AI-generated output without adequate human oversight |
| (d) | Citing case law, prior art, scientific literature or other references suggested by AI without independent source verification from authentic sources |
| (e) | Using AI-generated content in official communications without review, correction and adoption by the concerned officer |
| (f) | Relying solely on AI for decision-making affecting rights of applicants/patentees or third parties, **especially in arriving at conclusions in cases involving opposing parties, for instance opposition proceedings** |

Prohibition (f) is the one to carry forward: it singles out **inter partes** proceedings for heightened treatment, which is a contestability-sensitive carve-out rather than a general accuracy concern.

### Administrative measures (§6) — four, all discretionary

The deontic register changes completely. Every institutional measure is **MAY**:

1. The competent authority **may prescribe** that material AI use in specified functions **shall be recorded** — tool name, nature of use, date of use, and anything else needed for supervision, audit or quality review. Such disclosure **may** be made available to stakeholders to improve confidence in the examination process.
2. The competent authority **may establish** a dedicated AI governance committee, entrusted with: review and approval of tools; categorisation of permitted and prohibited uses; prescription of safeguards and approval conditions; pilot studies; review of quality, errors, complaints or policy breaches; periodic revision of the Guidelines; and consultation with stakeholders and AI experts with demonstrable expertise in machine learning, NLP or LLM systems.
3. The competent authority **may take steps** for training and capacity building across six enumerated topics, including identification of hallucinations, unsupported claims and fabricated citations.
4. Where appropriate, the competent authority **may also provide** for independent audit, impact assessment, feedback mechanisms and incident reporting systems.

**Composition** is the one hard element: the AI Governance Committee of the O/o CGPDTM **shall comprise** examiner(s) and controller(s) from the Examination Division, officer(s) from the IT Office and from the QMS Division, nominated so as to cover the different technology groups. A committee whose existence is discretionary has a mandatory composition.

### Annexure-I

Thirty-four pages of worked illustrative examples, opening with AI-assisted IPC/CPC classification across multiple models and prompts, with **irrelevant classifications marked in red**. It is, in substance, a regulator-authored demonstration of model variance and error. Its closing line is explicit that the point of the exercise is to show *why extreme caution is required in using AI tools*. The Annexure expressly disclaims any intent to give prompt-engineering or model-training guidance.

---

## Analytical Significance for PRIS Research

### For P4 (Doctrinal, IJLIT)

This is a direct doctrinal object. An administrative authority exercising quasi-judicial power has, without statutory authorisation and without a commencement clause, issued SHALL-form constraints on how its officers may use AI in determinations that affect property rights. Three doctrinal questions follow, none answered on the face of the instrument: (i) what is the legal status of a determination made in breach of §5, and does breach go to jurisdiction, procedure, or neither; (ii) can an applicant or opponent invoke the Guidelines, given that Annexure-II's declaration mechanism is unread; (iii) does §5(f)'s singling out of opposition proceedings create a differential standard of review as between *ex parte* and *inter partes* matters. The instrument is unusually clean for this analysis because it is short, internally consistent, and free of the hedging that characterises the sectoral advisories.

### For P1 (SLR, Regulation & Governance)

Extends the corpus's institutional coverage to a **sixteenth** Indian body issuing AI-specific governance text, and — more usefully for the SLR's framing — to a governance *mode* the review is thin on: the State as AI user rather than AI regulator. Pairs with [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] and [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]].

### Coordination / Parallelism Pattern

**Parallelism, with a same-ministry twist.** [[07_Institutions/Corpus/DPIIT/DPIIT_1]] (December 2025) is DPIIT's working paper on generative AI and copyright. CGPDTM_1 is issued by DPIIT's own subordinate office on generative AI in patent examination. Same ministry, adjacent subject matter, roughly eight months apart, **zero cross-citation in either direction.** Existing parallelism instances in this corpus are inter-regulator; this one is *intra-ministerial*, which is a stronger form of the finding — coordination failure here cannot be attributed to institutional distance or absent statutory coordination mechanisms, since both bodies report into the same department. Recommend coding as a distinct sub-type on [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]].

Against [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]]: the Guidelines cite NITI Aayog's *Responsible AI* documents as their policy anchor but make no reference to the NCAIC framework. **Unpaired** — a national AI governance framework exists and this instrument does not reach for it.

### Deontic Bifurcation

The cleanest instance in the corpus to date. Duties on the **individual officer** are uniformly SHALL and are enforceable in the ordinary supervisory sense. Duties on the **institution** — logging, committee, training, audit, impact assessment, incident reporting — are uniformly MAY. The accountability architecture that would make the officer-level duties auditable is precisely the part left discretionary. Note the sharpest illustration: §6(1) makes *recording* of AI use conditional on the competent authority first choosing to prescribe it, so the evidentiary trail supporting every SHALL in §4 and §5 is optional at the institution's election.

This bears directly on the Deontic-Placement Debt pattern recorded at [[05_Concepts/05_Concepts_Signature/Governance_Debt]]: the pattern there is that binding force and AI coverage vary inversely across instruments. CGPDTM_1 shows the same inversion **within a single instrument**, across the individual/institution boundary.

### Evidentiary Governance

§6(1)'s optional log — tool name, nature of use, date of use — is a record-generation provision that is never made mandatory, and there is no retention period. Relevant to [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] and to [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]]: a fourth or later instance of an Indian instrument contemplating a record without specifying how long it is kept. ⚠ Confirm the instance count against the concept note before citing a number.

### Consulting Connection

**AEGIS_OS (🟡 open, non-defence scope only).** §5(b), §5(c) and §5(f) are, in substance, pre-execution authority constraints: a class of decisions that an AI system may inform but may not determine, with the boundary drawn by subject matter (substantive patentability) and by procedural posture (*inter partes*). That is the AEGIS_OS thesis stated by a government body in its own operating instruction. §6(1)'s tool/use/date log is a minimal audit-trail schema. Usable as a public-sector reference point in engagement material without disclosing anything client-side.

**PrivacyWeave (🟢 open).** §5(a) is a purpose-and-destination rule on confidential data — unpublished applications and internal deliberative material may not enter public AI tools — enforced, on the face of the instrument, by officer discipline alone. A worked example of exactly the control PrivacyWeave proposes to move to runtime.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/DPIIT/DPIIT_1]] · [[07_Institutions/Corpus/NITI_Aayog/NITI_3]] · [[07_Institutions/Corpus/NCAIC/NCAIC_1_AI_Governance_Framework_for_India_2025_26]] · [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]] · [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]]
**Related wiki intake notes:** [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Deontic_Bifurcation]] · [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] · [[05_Concepts/05_Concepts_Signature/Governance_Debt]] · [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] · [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] · [[05_Concepts/05_Concepts_Standard/Human_Oversight]] · [[05_Concepts/05_Concepts_Standard/Accountability]] · [[05_Concepts/05_Concepts_Standard/Contestability_Redress]] · [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] · [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]]
**Related frameworks:** [[06_Frameworks/IndiaAI_Framework]]
**Related projects:** [[02_Projects/P4_Doctrinal_IJLIT]] · [[02_Projects/P1_SLR_RG]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** AEGIS_OS · PrivacyWeave

---

## Coding Status

- **P3 NVivo:** Not applicable — non-BFSI, outside the P3 canonical corpus
- **P4 doctrinal:** Candidate primary source, high priority
- **Wiki intake status:** Pending

---

## Claims Flagged for Verification

- **⚠ #369 (HIGH).** The document carries **no date, no file or notification number, and no issuing authority block** on its face. Attribution to the O/o CGPDTM rests on a single internal self-reference in §6 ("The AI Governance Committee of the O/o CGPDTM shall comprise…") and on the Annexure-I running header. The date in this node's frontmatter (2026-08-07) is **PDF creation metadata, not a publication date**, and is used only so the node sorts correctly. **Do not cite a date, a reference number, or a formal issuing authority for this instrument until the source is located on the CGPDTM or IPO website.**
- **⚠ #370 (MEDIUM).** **Annexure-II (Checklist and declaration) is not in this file.** It is referenced in §4 and listed in the contents, but the document ends at "Page 34 of 34" of Annexure-I. The checklist and declaration are plausibly the instrument's actual accountability mechanism — the thing that would convert §5's prohibitions into a record. **This node makes no claim about their content.** Obtain and code separately.
- **⚠ #371 (MEDIUM).** **In-force status not determinable.** No commencement clause, effective date, or statement of application was found. The combination of the word "Guidelines" with pervasive SHALL-form drafting is consistent with an operative internal instruction, but that is an inference. Confirm before describing it as binding.
- **⚠ #372 (LOW).** The claim that the Guidelines cite no enabling statutory provision is an absence claim, drawn from a full-text extraction of the 16-page Guidelines and 34-page Annexure-I. It is well supported for **this file** but cannot speak to a covering notification or office order that may have accompanied the Guidelines and is not in the file. Ties to ⚠#369.

---

## Log

- 2026-08-23: Corpus node created from `Desktop/AI in Indian Patents.pdf`. Desktop intake batch. Full clean text extraction (Guidelines 16pp + Annexure-I 34pp); Annexure-II absent. New institution folder and institution note [[07_Institutions/CGPDTM]] created. Principal contributions: first state-as-AI-user instrument in the corpus with operative SHALL obligations; intra-ministerial parallelism instance against [[07_Institutions/Corpus/DPIIT/DPIIT_1]], a stronger form of the finding than the existing inter-regulator instances; within-instrument deontic bifurcation across the individual/institution boundary. Four flags (⚠#369–#372), one HIGH — all provenance, none content.
