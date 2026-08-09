---
type: Framework
status: active
last_updated: 2026-08-09
tags:
  - type/framework
  - status/active
  - paper/p4-primary
  - paper/p3
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/consulting
  - content/wiki-entry
---

# Evidentiary Destination Matrix — Indian logging mandates against BSA s.63

**Type:** Framework / synthesis **Status:** Active — first pass **Created:** 2026-08-09
**Answers:** OQ-EG-01 in [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] (its self-declared *primary contribution candidate*) and OQ-JG-01 in [[03_Domains/Judicial_Governance]]
**Method specified by:** [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] Log — "systematically check RBI_8, CERT_In_2/3, SEBI's AI/ML reporting circulars, and DPDP's breach-notification retention rules against s.63(2)'s four conditions and s.63(4)'s certificate-signatory requirement"

---

## Why this matrix exists

[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] identifies four constitutive dimensions along which any instrument can be coded: artefact specification, retention horizon, custody and integrity, and **evidentiary destination**. The fourth carries the construct's principal analytical weight and was recorded as "unresolved across the entire Indian corpus."

That phrasing understated the problem. The dimension is not merely unresolved in the sense of *not yet coded*. It is unresolved in the sense that **no Indian regulatory instrument states what its retained artefacts are for** — whether they must satisfy a supervisor's inspection or a court's admissibility test. Those are different standards with different requirements, and an entity building a logging architecture cannot satisfy both by accident.

India has a terminal evidentiary standard: **Bharatiya Sakshya Adhiniyam, 2023, s.63**, in force since 1 July 2024, replacing Indian Evidence Act s.65B. Every electronic record offered in any Indian court or tribunal must clear it. This matrix asks, instrument by instrument, whether the artefacts India's regulators require entities to keep would clear it — and finds, on a first pass, that **not one instrument in the corpus was drafted with s.63 in view.**

---

## The standard being tested against

**BSA s.63(2) — four conditions** for a computer output to be admissible without the original:

| # | Condition |
|---|---|
| **(a)** | Regular use of the device for the relevant activity |
| **(b)** | Regular feeding of information into the device in the ordinary course of that activity |
| **(c)** | Proper operation throughout the material period — or, if not properly operating, that the improper operation did not affect the accuracy of the output |
| **(d)** | The output reproduces or is derived from information fed into the device in the ordinary course of the activity |

**BSA s.63(4) — mandatory certificate**, submitted **with the record at each instance of its production**, which must identify the record and describe the manner of production, describe the device, deal with the s.63(2) conditions, and be **signed by a person occupying a responsible official position** in relation to the operation of the device or the management of the activity, with an expert additionally able to attest. The **Schedule** prescribes the format: Part A by the producing party, Part B by a person with relevant technical expertise.

**The operative asymmetry.** s.63 is a *production-time* obligation running to a **named signatory**. Every Indian regulatory logging mandate in the corpus is a *retention-time* obligation running to an **institution**. Nothing connects them.

---

## The matrix

Coding: **✅** provision addresses the condition; **◐** partially or by implication; **❌** absent.

| Instrument | Retention specified | s.63(2)(a) regular use | (b) regular feeding | (c) proper operation | (d) faithful derivation | **s.63(4) certificate-readiness** | Stated destination |
|---|---|---|---|---|---|---|---|
| [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] | ✅ **Seven horizons**, 180-day logs, 365-day incident logs, First Schedule custody list | ◐ asset register records configuration and use (reg 5(25)) | ◐ logging enabled at ESP (reg 5(37)) | ◐ change management + version control + rollback (reg 8(25)) | ❌ | ❌ **No certificate, no signatory, no production procedure** | ❌ Unstated |
| [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | ❌ **None** (para 97 delegates) | ◐ | ✅ para 93 logging capability on every system accessing critical/sensitive info | ◐ | ◐ para 220(5) attribution: who did what, when, how | ❌ | ◐ **Closest in the corpus** — para 95 names "forensic evidence," "dispute resolution," "non-repudiation" |
| [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] | ✅ 1 year default | ◐ | ◐ | ◐ | ❌ | ❌ | ◐ Supervisory/audit — custody regime is strong (§16.6) but destination is inspection, not proof |
| [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | ❌ "secure retention," no period | ❌ | ◐ §12.14 agentic audit logging | ❌ | ❌ | ❌ | ❌ Requires "evidence preservation" (§6.10, §10.1) **without defining what the evidence is for** |
| [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] | ✅ 1 year minimum (Rule 6, Seventh Schedule) | ❌ | ◐ | ❌ | ❌ | ❌ | ◐ **Stated on the face of the instrument** — "for breach investigation." Investigation, not adjudication |
| SEBI AI/ML reporting circulars ([[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]], [[07_Institutions/Corpus/SEBI/SEBI_17]]) | ❌ | ❌ | ◐ inventory reporting | ❌ | ❌ | ❌ | ❌ Regulatory reporting only |
| [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] | ✅ 5 yr (Art. 33), 10 yr (Art. 47 + Annex V) | ❌ | ❌ | ❌ | ❌ | ◐ **Declaration of Conformity is a signed instrument** — the nearest functional analogue to a s.63 certificate anywhere in the corpus, though for a different purpose | ✅ Market-surveillance / conformity |

### What the matrix shows

**1. The certificate column is empty.** Not one Indian instrument — binding or advisory, AI-specific or technology-neutral, 2019 or 2026 — requires an entity to be able to produce a s.63(4)-compliant certificate for any artefact it is required to retain. No instrument names a responsible signatory for evidentiary production. No instrument references the Schedule format. **This is the finding.**

**2. Retention and admissibility are not correlated.** CEA_3 is the corpus's most retention-dense instrument and scores no better on certificate-readiness than SEBI's circulars, which specify no retention at all. Specifying *how long* to keep something is independent of specifying *whether it can be proved*.

**3. s.63(2)(d) is unaddressed everywhere.** The requirement that output "reproduces or is derived from information fed into the device in the ordinary course" is the condition most obviously strained by probabilistic systems, and **no Indian instrument engages it at all** — not even the AI-explicit ones.

**4. RBI_8 comes closest and still fails.** Para 95's "forensic evidence… dispute resolution… non-repudiation" is the only place in the Indian corpus where an instrument names an adversarial destination. But it pairs that with para 97's total retention abdication — an instrument that names the destination and then declines to specify the horizon that would make reaching it possible. The corpus's best evidentiary drafting is internally self-defeating.

**5. Destination, where stated at all, is supervisory.** DPDP Rules say "breach investigation." CERT-In says audit. Only RBI_8 gestures at proof. **No Indian instrument tells a regulated entity that its logs may one day have to survive cross-examination.**

---

## The generative-AI problem s.63 was not drafted for

BSA_1 records that s.63's conditions "map awkwardly onto generative AI systems whose outputs are non-deterministic by design." That understates a structural mismatch worth setting out precisely, because it is the paper's theoretical core:

| s.63(2) condition | Assumption it encodes | Why a generative system strains it |
|---|---|---|
| (a) regular use | The device performs a stable, identifiable activity | A general-purpose model performs indefinitely many activities; "the relevant activity" may not be individuable |
| (b) regular feeding in the ordinary course | Inputs are business records entering a system of record | Prompts are not fed "in the ordinary course of an activity" in the bookkeeping sense the provision inherits from s.65B and its 1872 ancestry |
| (c) proper operation | Malfunction is detectable and bounded; correct operation produces correct output | A model operating exactly as designed can produce a false output. **Hallucination is not malfunction.** The condition has no purchase on the failure mode that matters |
| (d) faithful derivation | Output is traceable to input by a reproducible process | Identical inputs need not produce identical outputs. Derivation is real but not reproducible, which is the sense the condition assumes |

Condition (c) is the sharpest. s.63(2)(c) contemplates a device that is either working or not working, and provides a saving clause for the latter. It has no category for a device that is working perfectly and producing something untrue. **The statute's implicit theory of machine error is deterministic, and generative AI's characteristic error is not.**

⚠ This is an analytical reading of the statute against the technology, not a proposition supported by Indian case law — **there is none**, which is itself the point (see below).

---

## The judicial confirmation

[[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] (Delhi High Court, 24 July 2026), India's first judicial determination on LLM training and copyright, reached final interlocutory disposal **without any party, either Amicus, or the Court invoking s.63 or submitting a certificate for any AI-generated artefact** — across 21 hearings and six intervenors. The Court instead reconstructed model behaviour from the **vendor's own published training cut-off dates** (para 83).

The sequence is worth stating plainly, because it is the argument in miniature:

1. No instrument required the artefacts to exist.
2. So they did not exist.
3. So the court used what was left — a date the defendant had published about itself.
4. And the rights-holder had nothing to test that against.

BSA_1 confirms this is a genuine gap rather than an artefact of prior corpus coverage: s.63 was in force from 1 July 2024, throughout the entire proceeding, and was never raised.

**The stronger version of the finding:** it is not that Indian AI governance fails a test set by evidence law. It is that **the two bodies of law have not yet met**, and the first case where they should have met passed without either side noticing.

---

## Contribution claim (for P4)

The defensible claim, stated conservatively:

> India has built, across five regulators and seven years, an increasingly dense set of obligations to *retain* technical artefacts, and has not once specified what those artefacts must be *capable of proving*. The country's terminal evidentiary standard — BSA s.63, in force since July 2024 — imposes a production-time certification requirement running to a named signatory that no regulatory logging mandate anticipates. Where the two regimes should have met, in India's first AI copyright case, neither party raised the question.

This is a **doctrinal gap-identification** contribution, not an empirical or theoretical one. It is defensible because every limb is documentary: the instruments are coded, the statute is coded, the judgment is coded, and the absence is checkable by anyone with the same corpus.

**What it is not.** It is not a claim that Indian AI systems' outputs are inadmissible — no court has held that, and the s.63(4) certificate can in principle be produced retrospectively by a responsible official "to the best of knowledge and belief." The claim is about **design**: regimes that mandate retention without certification-readiness leave the entity to discover the requirement at the worst possible moment.

---

## Open questions this matrix does not close

**OQ-EDM-01.** Can a s.63(4) certificate be validly given for a generative-AI output at all, given condition (c)'s deterministic theory of error? No Indian authority. The nearest analogue is expert-evidence practice for statistical and forensic-science outputs — a literature this corpus has not yet touched.

**OQ-EDM-02.** Does the Part B "person with relevant technical expertise" requirement in the Schedule create a de facto expert-witness obligation for any entity producing AI-system records? If so, the compliance cost of evidentiary readiness is materially higher than the retention obligations imply, and no instrument has priced it.

**OQ-EDM-03.** Would an EU AI Act Art. 12 log, or an ISO/IEC 42001 documented-information record, satisfy s.63(2)? This is OQ-EG-01's original comparative form and is now answerable — the artefacts are specified in International_22 and the standard is coded in [[06_Frameworks/ISO_IEC_42001]]. **Not attempted in this pass.**

**OQ-EDM-04.** Do any Indian regulators' *inspection* powers (RBI's supervisory access, CERT-In's collection powers under CEA_3 reg 4(1)(c)) produce records that would themselves need s.63 certification when relied on in enforcement proceedings? The regulator faces the same problem as the regulated entity, and no instrument addresses it.

---

## ⚠ VERIFY

- **⚠ #315 (MEDIUM).** The matrix's per-condition coding is a **first-pass analytical read**, performed from corpus nodes rather than from a fresh reading of each primary instrument against s.63. The ❌ column for s.63(4) certificate-readiness is high-confidence (an instrument either mentions evidentiary certification or it does not, and none does). The ◐ codings for s.63(2)(a)–(d) are interpretive and should be re-derived from primary text before publication.
- **⚠ #316 (MEDIUM).** s.63(2) and s.63(4) text is taken from [[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]], which was itself sourced via Perplexity Deep Research against the MHA Gazette PDF and India Code Schedule rather than by direct primary reading. Verify the statutory text before quoting.
- **⚠ #317 (LOW-MEDIUM).** SEBI row is coded from SEBI_9/SEBI_10/SEBI_17 as summarised in their nodes; SEBI_15 (CSCRF) has not been read against s.63 and may contain logging provisions that would change that row.
- **⚠ #318 (LOW).** The generative-AI/s.63 mismatch analysis is the author's reading of the statute against the technology. No Indian judicial or academic authority supports or contradicts it, because none was located. Present as argument, not as settled doctrine.

---

## Linked Corpus Nodes

[[07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023]] | [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] | [[07_Institutions/Corpus/CEA/CEA_3_Cyber_Security_Power_Sector_Regulations_2026]] | [[07_Institutions/Corpus/RBI/RBI_8_Cybersecurity_Technology_Risk_Resilience_Assurance_2026]] | [[07_Institutions/Corpus/CERT_In/CERT_In_1_Comprehensive_Cyber_Security_Audit_Policy_Guidelines_2025]] | [[07_Institutions/Corpus/CERT_In/CERT_In_3_Blueprint_AI_Assisted_Exploitation_2026]] | [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] | [[07_Institutions/Corpus/SEBI/SEBI_9]] | [[07_Institutions/Corpus/SEBI/SEBI_10]] | [[07_Institutions/Corpus/SEBI/SEBI_17]] | [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]]

## Linked Concepts

[[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] (parent construct — this matrix operationalises its fourth dimension) | [[05_Concepts/05_Concepts_Standard/Retention_Horizon_Divergence]] | [[05_Concepts/05_Concepts_Standard/Assurance_Reuse_Gap]] | [[05_Concepts/05_Concepts_Signature/Governance_Debt]] | [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]

## Linked Domains

[[03_Domains/Judicial_Governance]] | [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]] | [[03_Domains/Cybersecurity_Governance]] | [[03_Domains/Power_Grid_Critical_Infrastructure_Governance]]

## Linked Projects

[[02_Projects/P4_Doctrinal_IJLIT]] (primary) | [[02_Projects/P3_BFSI_JEIM]] | [[02_Projects/fsQCA_Thesis_Chapter]]

## Linked Knowledge Products

[[04_Knowledge_Products/AI_Governance_Wiki]] | [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]] | [[04_Knowledge_Products/Minimum_Evidence_Register_Autonomous_AI]]

---

## Log

- 2026-08-09: Framework created, closing OQ-EG-01's method step as specified in BSA_1's own Log. Seven instruments coded against s.63(2)(a)–(d) and s.63(4). **Headline finding: the certificate-readiness column is empty across the entire Indian corpus.** Secondary findings: retention density and admissibility-readiness are uncorrelated (CEA_3 vs SEBI); s.63(2)(d) unaddressed everywhere; RBI_8 alone names an adversarial destination and pairs it with total retention abdication. Generative-AI/s.63 structural mismatch set out at the condition level, with s.63(2)(c)'s deterministic theory of error identified as the sharpest point. DHC_1 recorded as judicial confirmation that the two bodies of law have not yet met. Four new open questions (OQ-EDM-01 to -04); four VERIFY flags (#315–#318).
