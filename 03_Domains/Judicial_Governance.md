---
type: Domain
status: seeded
last_updated: 2026-08-02
tags:
  - type/domain
  - status/seeded
  - paper/p4
  - gate/open
  - engine/phd
  - engine/consulting
  - content/carousel-ready
---

# **Judicial Governance**

**Type:** Domain **Status:** Seeded — promoted from stub 2026-08-02; **not yet a full Domain synthesis** **Last Updated:** 2026-08-02

> **Status discipline.** The 2026-07-31 stub correctly recorded that this domain rests on a **single** corpus node and that a full synthesis on the model of [[03_Domains/DPI_Governance]] must wait for intake of the eCourts, CEPEJ and UK judicial-AI documents. That constraint stands. This promotion does two things only: it establishes the analytical axis the domain will be organised around, and it connects the judicial material to adjacent corpus nodes that were already carrying judicial-evidentiary content without being tagged to this domain. **No claim below rests on a document that has not been read into the vault.** The candidate-source table from the stub is preserved intact.
>
> **Update 2026-08-02 — second node, and a different kind.** [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] (Delhi High Court, 24 July 2026) is the domain's second corpus node and the first **adjudication** rather than guidance. The domain remains `seeded` rather than `active`: two nodes still do not support a full synthesis, and the intake queue below is unchanged. But the analytical axis stated below is now empirically supported rather than merely proposed — see §Dual Position, updated.

---

## **Core Synthesis**

Judicial Governance in the PRIS corpus is not primarily about courts adopting AI tools. Its analytical weight lies in the judiciary's dual position: it is simultaneously a **deployer** of AI systems subject to governance obligations, and the **forum** in which the evidentiary output of everyone else's AI systems is ultimately tested. These two roles pull in opposite directions and the corpus captures both.

As deployer, the judiciary is the only Indian institution to have published a self-audit of its own AI estate alongside a candid catalogue of its own failures — three documented Indian judicial AI-hallucination incidents, recorded in [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]]. No regulator in the corpus has done anything comparable for its own systems.

As forum, the judiciary is where [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] terminates. Every logging, retention and audit-trail obligation imposed by RBI, SEBI, CERT-In or MeitY is ultimately a bet about what will satisfy a court. The corpus currently contains that bet from the regulators' side and almost nothing from the court's side. Closing that asymmetry is this domain's reason for existing.

**The first data point from the court's side is now in, and it is stark.** In [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] the Delhi High Court determined what an LLM had and had not done **without a single retained system artefact before it** — no training-data manifest, no inference log, no retention record. It reconstructed model behaviour from the vendor's own published training cut-off dates set against the plaintiff's article publication dates, and on that basis held memorisation impossible (para 83). It then made **prompt design** an evidentiary standard, distinguishing the Munich *GEMA v. OpenAI* decision on the ground that ANI's prompts were adversarial where GEMA's were not (paras 104, 119).

The judgment contains no reference to the Bharatiya Sakshya Adhiniyam, no s.63 certification analysis, and no direction on preservation. India's first AI copyright case reached interlocutory disposal without any party or either Amicus raising the admissibility question at all. That silence is the domain's most important finding to date.

⚠ **DHC_1 is an interim order on an injunction application, expressly prima facie throughout, and appealable to a Division Bench** (para 274; ⚠ V-DHC1-1, appeal status unverified). Every claim in this domain note resting on it is provisional. It must not be cited as settled Indian law on AI training and copyright.

---

## **Organising Axis: Algorithmic Adjudication and Evidentiary Integrity**

`#concept-candidate/algorithmic-adjudication`

Staged inline per [[00_MOC/Workflow_Discipline_Protocol]] CDW-2 — the construct cannot clear the Three-Instance Gate on one corpus node and must not be given a standalone concept note until it can. Elevate when three distinct judicial-side primary sources have been intake.

The candidate construct: **judicial systems are being asked to adjudicate the outputs of automated systems at the same time as they adopt automated systems, without a settled evidentiary standard for either.** It has three provisional dimensions, each with existing corpus support:

| Dimension | Question | Current corpus support |
|---|---|---|
| **Judiciary as AI deployer** | What governs AI used *by* courts? | SCI_1 — nine-tool inventory, six-risk taxonomy, six ethical principles, role-differentiated obligations for institutions, lawyers and law clerks |
| **Judiciary as evidentiary forum** | What standard must AI-derived evidence meet? | **[[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]]** — first Indian adjudication; behaviour reconstructed from vendor metadata absent artefacts; prompt design made an evidentiary standard. ⚠ Structural gap persists: no Indian evidence-law instrument in the vault, and the judgment never engages BSA s.63 |
| **Judiciary as gap-filler** | What does a court do when the executive has not legislated? | DHC_1 para 4: *"the Courts are required to step in to fill the gap between advancing technologies and existing laws."* Decided the TDM question under existing s.52 while DPIIT was still consulting — see [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] §Inter-Branch |
| **Synthetic-media integrity** | How is fabricated evidence detected and governed upstream? | SCI_1 Ch. 4.C, plus MeitY's platform-side regime — see below |

---

## **Cross-Domain Thread: Synthetic Media and Evidentiary Integrity**

This is the domain's most developed thread and the one that already spans three domains without having been assembled anywhere. SCI_1's own cross-links flag it as an unbuilt synthesis; this note assembles it.

The judiciary approaches synthetic media from the **courtroom-admissibility** angle — Chapter 4.C of the White Paper treats evidence tampering and deepfakes as a category of AI risk to adjudication. MeitY approaches the identical phenomenon from the **platform-content** angle: [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] on synthetically generated information labelling, [[07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025]] on non-consensual intimate imagery takedown with its 36-hour and 24-hour removal pathways, and [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] on severity-gated first-originator traceability.

The two regimes govern the same artefacts for different purposes and do not reference each other. MeitY's provenance-and-takedown machinery is designed to remove content; the judiciary's concern is whether content that was *not* removed can be authenticated when it arrives as evidence. **A labelling regime optimised for platform moderation is not automatically a provenance regime adequate for adjudication** — labels can be stripped, takedown destroys the artefact, and neither instrument specifies preservation for evidentiary purposes. This is [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] operating across the executive–judicial boundary rather than between sectoral regulators, and it is a novel extension of that construct.

---

## **Institutional Significance**

SCI_1 is the corpus's first instrument issued by the judiciary rather than by an executive ministry or statutory regulator. This matters for [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]]: the judiciary constitutes a fifth independent AI-governance-instrument-issuing institution alongside MeitY, the financial regulators, CERT-In and NCAIC — one that answers to none of them and coordinates with none of them.

The White Paper is also the only corpus instrument extending AI governance obligations to **junior research staff** (law clerks), with explicit reference to professional misconduct. Set against NCAIC's RACI model and CERT-In's maker-checker sign-off structure, this gives three distinct institutional approaches to distributing AI accountability across hierarchical actor categories — a comparison worth building for [[02_Projects/P4_Doctrinal_IJLIT]].

---

## **Known Structural Gap — Resolved 2026-08-02**

✅ **[[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] now exists in the vault.** The Bharatiya Sakshya Adhiniyam 2023 came into force on 1 July 2024, repealing the Indian Evidence Act 1872; its s.63 governs admissibility of electronic records and carries a mandatory certification requirement (Schedule, Parts A and B). Primary text confirmed via the official MHA-hosted Gazette PDF and the India Code Schedule PDF. This was the single most important missing document for this domain and for OQ-EG-01 in [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] — the domain can now progress past this blocker.

**Immediate next step (not yet done):** systematically check RBI_8, CERT_In_2/3, SEBI's AI/ML reporting circulars, and DPDP's breach-notification retention rules against s.63(2)'s four conditions and s.63(4)'s certificate-signatory requirement — see BSA_1's own "Analytical Significance" section for the preliminary read (most regulatory logging obligations appear to specify retention but not certification-readiness, on current coding).

---

## **Candidate Sources — Link-Verified 2026-08-02, Not Yet Read/Coded**

Item 1 (BSA) is now fully intaken — see [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] above. Items 2–6 have had their links independently verified as live and current (2026-08-02) but their content has still not been read or coded into the vault — this table tracks link-verification status, not intake status.

| Priority | Document | Issuing Body | Date | Source | Status |
|---|---|---|---|---|---|
| ~~1~~ | ~~Bharatiya Sakshya Adhiniyam, 2023 — s.63 and Schedule~~ | Parliament of India | In force 1 July 2024 | India Code | ✅ **Intaken** — [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] |
| 2 | Artificial Intelligence (AI) Guidance for Judicial Office Holders | Courts and Tribunals Judiciary, UK | 31 October 2025 (confirmed: supersedes Apr 2025, which superseded Dec 2023) | https://www.judiciary.uk/guidance-and-resources/artificial-intelligence-ai-judicial-guidance-october-2025/ | Link verified live; not yet read/coded |
| 3 | European Ethical Charter on the Use of AI in Judicial Systems | CEPEJ, Council of Europe | 3–4 December 2018 | https://rm.coe.int/ethical-charter-en-for-publication-4-december-2018/16808f699c | Link verified live; not yet read/coded |
| 4 | Vision Document for Phase III of eCourts Project | e-Committee, Supreme Court of India / DoJ | 26 November 2022 (per e-Committee's own listing; note the then-CJI accepted it 23 September 2022 — two dates in play, not a discrepancy, just acceptance-vs-publication) | https://ecommitteesci.gov.in/document/vision-document-for-phase-iii-of-ecourts-project/ | Link verified live; not yet read/coded |
| 5 | Policy and Action Plan Document, Phase II (eCourts) | e-Committee, Supreme Court of India | 8 January 2014 | https://ecommitteesci.gov.in/document/policy-and-action-plan-document-phase-ii/ | Link verified live; not yet read/coded |
| 6 | Policy and Action Plan Document, Phase I (eCourts) | e-Committee, Supreme Court of India | 1 August 2005 | https://ecommitteesci.gov.in/document/policy-and-action-plan-document/ | Link verified live; not yet read/coded |

**Standing cautions (unchanged).** No standalone official policy PDF exists for SUPACE — do not cite a SUPACE "policy document" without confirming one exists. No unified US federal judicial-AI policy instrument exists comparable to the UK or CEPEJ documents; US judicial AI governance is fragmented across circuit and district local rules.

---

## **Open Research Questions**

**OQ-JG-01 (no longer blocking — BSA_1 now intaken, 2026-08-02).** Do artefacts generated under Indian regulatory logging mandates satisfy BSA s.63(4) certification requirements? **Sharpened 2026-08-02:** DHC_1 shows the question is not merely unanswered but unasked — it did not arise across 21 hearings, six intervenors and two Amici. Now analytically tractable — see [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] for the preliminary read against RBI/CERT-In/SEBI logging provisions (not yet systematically completed).

**OQ-JG-05 (new, 2026-08-02).** Where a court must determine what an AI system did and no artefacts were retained, what evidentiary sources does it fall back on, and with what reliability? DHC_1's answer was vendor-published training dates. Is that generalisable, and what happens when a vendor's published claims are themselves contested?

**OQ-JG-06 (new, 2026-08-02).** Should prompt provenance be a governed artefact class? DHC_1 makes the adversarial character of a prompt determinative of evidentiary weight while no instrument specifies how prompts and outputs are to be captured or authenticated. Shared with [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] OQ-EG-05.

**OQ-JG-02.** Does MeitY's synthetic-media labelling and takedown regime preserve or destroy the provenance information a court would need for authentication? The instruments are silent; the answer determines whether the two regimes are complementary or actively in tension.

**OQ-JG-03.** How do the s.63(2) conditions carried over from s.65B — regular use, proper operation, ordinary course of business — apply to generative systems whose outputs are non-deterministic by design?

**OQ-JG-04.** Is the judiciary's willingness to publish its own AI failure catalogue (three documented hallucination incidents) replicable by regulators for their own systems, and if not, what explains the asymmetry in institutional candour?

---

## **Linked Projects**

[[02_Projects/P4_Doctrinal_IJLIT]] — primary; evidentiary and admissibility argument
[[02_Projects/P1_SLR_RG]] — SCI_1's 13-jurisdiction survey as comparative literature map
[[02_Projects/P5_AI_Ethics]] — hallucination incidents as documented ethical failure cases

## **Linked Domains**

[[03_Domains/AI_Governance]] | [[03_Domains/Privacy_DataProtection]] | [[03_Domains/International_Comparators]]

## **Linked Signature Concepts**

[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] — the judiciary is where this construct terminates
[[05_Concepts/05_Concepts_Signature/Institutional_Coherence]] — judiciary as a fifth independent instrument-issuing institution
[[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] — extended across the executive–judicial boundary via the synthetic-media thread

## **Linked Standard Concepts**

[[05_Concepts/05_Concepts_Standard/Accountability]] — role-differentiated obligations across institutions, lawyers, law clerks
[[05_Concepts/05_Concepts_Standard/Transparency]] — disclosure and audit-trail recommendations
[[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] — hallucination as documented failure mode

## **Linked Institutions**

[[07_Institutions/DHC]] | [[07_Institutions/SCI]] | [[07_Institutions/MEITY]] | [[07_Institutions/DPIIT]]

## **Linked Corpus Nodes**

[[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] (evidentiary standard — added 2026-08-02, closes prior blocking gap) | [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] (first adjudication) | [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]] (anchor) | [[07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025]] | [[07_Institutions/Corpus/MeitY/MeitY_6_SOP_NCII_Takedown_2025]] | [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] | [[04_Knowledge_Products/Wiki_Intake/F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]]

## **Future Reuse Opportunities**

- Build the synthetic-media integrity thread into a standalone comparative analysis — it is publishable in its own right and currently unclaimed in the literature.
- Adapt SCI_1's lawyer and law-clerk guideline sets as a template for professional-services AI-use policy in consulting engagements.
- Develop the three-way accountability-distribution comparison (judiciary / NCAIC RACI / CERT-In maker-checker) as a teaching case.
- Use the judicial hallucination catalogue as practitioner-facing content on generative-AI risk in regulated professional contexts.

---

## **Log**

- 2026-08-02: Promoted stub → seeded. Organising axis established (algorithmic adjudication and evidentiary integrity, staged inline per CDW-2). Synthetic-media cross-domain thread assembled from SCI_1 + MeitY_5/6/7 — a synthesis SCI_1's own cross-links had flagged as unbuilt. BSA corpus-node gap added as priority-1 blocking intake. **Not a full Domain synthesis** — that remains gated on the intake queue above.
- 2026-08-02 (later same day): Perplexity Deep Research verification pass (per [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]]) closed the priority-1 blocking gap — [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] now exists. DHC_1's V-DHC1-1 appeal-status flag resolved (no Division Bench appeal filed/decided as of verification). Candidate-source links for items 2–6 (UK judicial guidance, CEPEJ, three eCourts documents) all confirmed live — content still not read/coded. Still **not a full Domain synthesis**, but the single most important structural blocker is now cleared.

---

*Back to [[Domains_MOC]]*
