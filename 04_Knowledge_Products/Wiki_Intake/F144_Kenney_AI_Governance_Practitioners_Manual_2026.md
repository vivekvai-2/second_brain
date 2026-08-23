---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - batch/desktop-20260823
  - concept/Governance_Debt
  - concept/Regulatory_Parallelism
  - concept/Accountability
  - project/p1
  - project/p4
---

# AI Governance Practitioner's Manual (Kenney) — Intake Note

**Source:** Noah M. Kenney / Digital 520 (independent consultancy, United States)
**Year:** 2026
**Full title:** The AI Governance Practitioner's Manual: Law, Privacy, Security, and Compliance for Every Role — First Edition
**File ID:** F144
**Zotero key:** [to be added manually]
**Wiki section(s):** S6 (Implementation & Governance Artifacts) — primary; S2 (India Regulatory Framework) and S3 (International Regulatory Context) — secondary, by way of what it omits
**Confidence:** Medium — self-published practitioner reference by a single author; no peer review, no institutional imprimatur. Its own factual apparatus is unusually explicit, which makes it testable, and it fails one test (Finding 4)
**Jurisdiction:** Global, with a pronounced US/EU centre of gravity

---

## Classification

**Document type:** Practitioner reference work / self-published professional manual
**Length and structure:** 300 pages; 46 chapters in nine parts, plus ten appendices (A–J) forming a "Reference Desk"
**Primary audience:** Multiple, and explicitly so — the manual is indexed by role rather than by subject. Parts II–VII address executives and governance leaders, lawyers, privacy professionals, engineers and data scientists, security professionals, and compliance officers and auditors in turn
**AI explicit:** Yes
**Stated currency:** Through August 2026, including legislation in force from July 2026

---

## 3–5 Reusable Findings

1. **Role-indexed architecture with per-role reading paths** (feeds S6). The manual's organising decision is to index by audience rather than subject, on the stated reasoning that an AI governance practitioner is simultaneously advising on privacy, consumer protection, civil rights, sectoral regulation, cybersecurity, IP and horizontal AI regimes, and that no single professional owns all of that terrain. Part I is a common foundation everyone reads; Parts II–VII are role-specific; Part VIII holds cross-cutting domain playbooks (healthcare, financial services, government, generative AI, autonomous agents). Chapters are written to be entered out of sequence, each opening with a "Who this chapter is for" statement and cross-referencing rather than assuming linear reading. This is a directly borrowable structure for the [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]], which currently indexes by subject.

2. **The structured regulatory entry template** (feeds S6, and S9 on methodology). Every law and standard surveyed is rendered in an identical seven-part schema: name and citation, then a metadata line giving *Jurisdiction / Effective / Regulator / Scope*; then **Applicability** (who and what it reaches, including thresholds), **Core obligations**, **Penalties and enforcement**, **Recent developments**, and a **Stack lens** locating where in the author's five-layer model the obligation actually bites. Higher-stakes entries add a *Practitioner note* and a *Common failure pattern*. The stated purpose is direct cross-regime comparability on any single dimension — penalty exposure, breach timing, automated-decisioning rights, sensitive-data treatment, fairness obligations, vendor flow-down. **This is worth a deliberate comparison against Format A** in [[04_Knowledge_Products/Wiki_Intake/PRIS_Cowork_Context]]: the schemas overlap substantially, and Kenney's *Common failure pattern* field has no Format A equivalent.

3. **India coverage is data-protection-only — the sectoral AI layer is absent** (feeds S2, S3). India appears as §20.6, a single structured entry covering the DPDP Act 2023 and its anticipated Rules. A term sweep of the full 128,544-word text extraction returns **zero occurrences** of *RBI*, *Reserve Bank*, *SEBI*, *IRDAI*, *MeitY*, *NITI*, *CERT-In*, *Aadhaar*, or *UPI* (⚠#377). The entire object of P3 and P4 — India's sectoral, multi-regulator AI governance layer — is therefore invisible in a 300-page practitioner manual claiming August 2026 currency. **This is the note's most useful finding for PRIS**, and it is a citable one: it evidences that the Indian sectoral layer is not merely under-coordinated domestically but under-represented in the practitioner literature that shapes how multinationals actually build compliance programmes. Pairs with [[04_Knowledge_Products/Wiki_Intake/F121_Correa_Kluge_Worldwide_AI_Ethics_200_Guidelines_2023]] on Anglosphere over-representation.

4. **A verifiable currency failure on the DPDP Rules** (feeds S2). The India entry describes the Rules as *"anticipated 2026"*, states that *"final Rules and Board operationalization remain the central 2026 milestone for India practitioners"*, and advises staging compliance builds against the Rules timeline. The entry is marked *"Verified: August 2026."* The Digital Personal Data Protection Rules, 2025 were in fact **notified on 13 November 2025** (G.S.R. 846(E), Gazette of India Extraordinary Part II §3(i) No. 760), per [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] — roughly nine months before the manual's stated verification date. The manual's own methodology section asserts that every structured entry carries a *Primary sources* line "verified against primary sources as of August 2026." **The apparatus is stated and the entry fails it.** This is a clean, dated, non-trivial instance of practitioner-literature drift against primary text, and is directly usable as an illustration in teaching or in a paper's motivation section.

5. **India framed as a regional outlier on automated-decision rights** (feeds S3, P4). The entry states that AI-specific obligations under DPDP are limited and that consequential decision-making rights *"are not explicit, which makes India an outlier among the region's newer statutes."* It also notes the cross-border model as a blacklist inverting the GDPR's whitelist logic, and identifies the Significant Data Fiduciary designation as the mechanism by which large AI-driven processors acquire enhanced obligations. The outlier claim is a comparator assertion worth testing rather than adopting — it is offered without the regional comparison that would support it, and P4 is better placed to substantiate or refute it than the manual is.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The structured regulatory entry template (Finding 2) is immediately usable as a client-facing comparison format for multi-jurisdiction AI obligations, and the *Common failure pattern* callout is a good teaching device — it names the audit finding to design out before it appears, which lands better with practitioner audiences than an abstract control list. Finding 4 is a ready-made classroom illustration of why practitioner references must be checked against gazetted text.

**Consulting connections:** **AEGIS_OS** — the five-layer Stack's premise, that a regulator's expectation of human oversight is a deployment-gate problem long before it is a courtroom problem, is a well-phrased articulation of the runtime-enforcement thesis and is quotable in positioning material. **PrivacyWeave** — the DPDP entry's Layer 1 framing of multilingual consent infrastructure across up to 22 scheduled languages as "an engineering project as much as a legal one" is a useful third-party statement of the purpose-enforcement problem.

**Teaching connection:** Framework example (regulatory entry schema); cautionary case study (Finding 4).

---

## Assessment

Treat this as a **structural and comparative resource, not an authority on Indian law.** Its architecture and entry schema are genuinely good and worth borrowing. Its India content is one entry, is stale on the single most consequential development in the jurisdiction, and omits every sectoral regulator this vault tracks. Its value to PRIS is therefore mostly as (a) a design reference for knowledge-product structure and (b) evidence, in Findings 3 and 4, about the state of the practitioner literature on India.

The author's stated credentials and reach are self-supplied biography and are not independently verified (⚠#378).

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S6, S2, S3
**Concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] · [[05_Concepts/05_Concepts_Signature/Governance_Debt]] · [[05_Concepts/05_Concepts_Standard/Accountability]] · [[05_Concepts/05_Concepts_Standard/Human_Oversight]]
**Corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] · [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]]
**Related intake notes:** [[04_Knowledge_Products/Wiki_Intake/F121_Correa_Kluge_Worldwide_AI_Ethics_200_Guidelines_2023]] · [[04_Knowledge_Products/Wiki_Intake/IAPP_AIGP_Body_of_Knowledge_v21_2026]]
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] · [[04_Knowledge_Products/BFSI_AI_Governance_Handbook]] · [[04_Knowledge_Products/DPDP_Playbook]]
**Projects:** [[02_Projects/P1_SLR_RG]] · [[02_Projects/P4_Doctrinal_IJLIT]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## Claims Flagged for Verification

- **⚠ #377 (MEDIUM) — absence claim.** Finding 3's "zero occurrences" statement rests on a programmatic term sweep of a full-document `pdftotext` extraction: 128,544 words, all 300 pages yielding text except page 1, which is the image-only cover. The sweep is therefore genuinely full-document and not a partial-extraction inference. **Two residual risks before publishing the claim:** an institution could be named in a form the sweep did not test (for example "Indian central bank" rather than "RBI"), and Appendix J is an alphabetical index of every law and standard covered which has not been separately inspected. Confirm against Appendix J before making the claim in publication-track output. Note also that a bare `India` string count returns matches inside `Indiana`; the sweep used word-boundary matching, but any re-run must do the same.
- **⚠ #378 (LOW).** The author's biography — advising "over 60 organizations", a prior 2026 textbook "reaching more than 100,000 readers", presentation at a United Nations Global AI Dialogue stakeholder meeting, named media citations — is author-supplied and unverified. Do not repeat these figures as fact; if the author's standing matters to an argument, verify independently.

---

## Log

- 2026-08-23: Intake note created from `Desktop/AI Governance Practioner manual.pdf`. Desktop intake batch. Full-text extraction (128,544 words, 300pp). Principal contributions: the role-indexed architecture and structured regulatory entry schema as design references for PRIS knowledge products; and Findings 3–4, which together evidence that a current, self-consciously verification-heavy practitioner manual covers India in one data-protection entry, omits every Indian sectoral regulator in the vault, and is nine months stale on the DPDP Rules while marked "Verified: August 2026". Two flags (⚠#377–#378), none HIGH.
