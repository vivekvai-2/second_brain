---
type: Corpus Node
status: active
last_updated: 2026-08-02
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/parliament
---

# BSA_1 — Bharatiya Sakshya Adhiniyam, 2023, Section 63 and Schedule (Admissibility of Electronic Records)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/Parliament/BSA_1_Section_63_Admissibility_2023.md`
**Institution:** [[07_Institutions/Parliament]]
**Issuing body:** Parliament of India (Act No. 47 of 2023); Gazette hosted by the Ministry of Home Affairs
**Document date:** Act No. 47 of 2023; in force 1 July 2024 (repealed the Indian Evidence Act, 1872)
**Pages:** Not independently paginated in this extraction (Section 63 plus Schedule only)
**Domain:** [[03_Domains/Judicial_Governance]]

---

## Instrument Identity

**Full title:** The Bharatiya Sakshya Adhiniyam, 2023 — Section 63 (Admissibility of Electronic Records) and the Schedule [see Section 63(4)(c)]
**Type:** Binding primary statute (evidence law)
**Target entities:** All courts and tribunals in India applying the law of evidence; any party seeking to admit a computer/device-generated record
**Legal basis:** Enacted by Parliament, replacing the Indian Evidence Act, 1872 (whose s.65B is the direct predecessor of this s.63)
**Companion documents:** None yet coded — this is the corpus's first dedicated evidence-law instrument

**Primary source link:** https://www.mha.gov.in/sites/default/files/2024-04/250882_english_01042024_0.pdf (official MHA-hosted Gazette PDF, full Act text)
**Schedule (certificate format):** https://upload.indiacode.nic.in/schedulefile?aid=AC_CEN_5_23_00049_2023-47_1719292804654&rid=1163 (official India Code portal)
**Cross-reference mirror:** https://indiankanoon.org/doc/125020475/

---

## Analytical Classification

**Wiki section:** New — Judicial Governance / Evidentiary Standards (no existing wiki section covers evidence law; recommend a subsection under S2 or a new dedicated section)
**Jurisdiction:** India
**Confidence:** High — primary Gazette text (MHA) cross-confirmed against the official India Code Schedule PDF and Indian Kanoon mirror
**AI explicit:** No — general electronic-records admissibility provision, not AI-specific; its relevance is that it is the standard against which AI-system-generated records (logs, audit trails, inference outputs) must be tested for evidentiary admissibility
**Tier classification:** Tier A — this is the foundational admissibility standard for every logging/audit-trail obligation coded elsewhere in this corpus (RBI, SEBI, CERT-In, MeitY, DPDP)
**AI Governance Wiki relevance:** HIGH — closes the single most significant structural gap previously identified in [[03_Domains/Judicial_Governance]]

---

## Substantive Content

### Section 63(1) — deeming provision
Computer/device-generated "computer output" is deemed a document and admissible without production of the original, **provided the conditions in s.63(2) are satisfied.**

### Section 63(2) — four conditions
(a) regular use of the device for the relevant activity; (b) regular feeding of information into the device in the ordinary course of that activity; (c) proper operation of the device throughout the material period (or, if not properly operating, that the improper operation did not affect the accuracy of the output); (d) the output reproduces or is derived from information fed into the device in the ordinary course of the activity.

### Section 63(4) — mandatory certification requirement
A certificate must be submitted **with the record at each instance of its production**, which must: identify the electronic record and describe the manner of its production; describe the device involved; deal with the s.63(2) conditions; and be signed by a person occupying a responsible official position in relation to the operation of the device or the management of the relevant activity — with an expert additionally able to attest. Matters may be stated to the best of the signatory's knowledge and belief (i.e., certification does not require the signatory's personal, first-hand technical verification of every element).

### The Schedule — certificate format, two parts
**Part A** (completed by the producing party): identifies the source device across defined categories (Computer/Storage Media, DVR, Mobile, Flash Drive, CD/DVD, Server, Cloud, Other); attests lawful control of the device and regular use for the relevant activity; confirms that any device malfunction did not affect the accuracy of the output.
**Part B** (completed by a person with relevant technical expertise): addresses matters regarding the electronic record's production requiring specialist knowledge.

### Direct relevance to DHC_1 — the question the judgment never asked
[[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] determined LLM training-data behaviour **without any party invoking s.63 or submitting a s.63(4) certificate for any AI-system-generated artefact** — the court instead reconstructed behaviour from the vendor's own published training-cutoff dates. Section 63's four conditions (regular use, regular feeding, proper operation, faithful reproduction) map awkwardly onto generative AI systems whose outputs are non-deterministic by design — a large language model does not "operate" in the sense CEA's or RBI's technical infrastructure does, and whether an LLM's output "reproduces or derives from information fed into the device in the ordinary course of the activity" is a genuinely unresolved question this statute was not drafted to answer. This is not a defect in the statute; it is evidence that no party or court has yet worked out how s.63's conditions apply to generative-AI-system outputs at all.

---

## Analytical Significance for PRIS Research

### For Judicial_Governance and Evidentiary_Governance — closes the blocking gap
This node directly answers [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]]'s OQ-EG-01 and [[03_Domains/Judicial_Governance]]'s OQ-JG-01: **do artefacts generated under Indian regulatory logging mandates (RBI's audit trails, SEBI's AI/ML reporting records, CERT-In's incident logs, DPDP's breach-notification records) satisfy s.63(4)'s certification requirement?** The answer is now analytically tractable rather than blocked — each of those instruments' retention/logging provisions can be checked against s.63(2)'s four conditions and s.63(4)'s certificate-signatory requirement directly. Preliminary read: most regulatory logging obligations in this corpus specify *retention* but not *certification-readiness* — none of RBI_8, CERT_In_2/3, or SEBI's AI/ML reporting circulars appear (on current coding) to have been drafted with s.63(4)'s certificate format in mind. This is a genuine, checkable cross-instrument gap-analysis opportunity, not yet performed — flagged as the immediate next step below.

### Sharpens, rather than resolves, DHC_1's silence
DHC_1's failure to engage s.63 at all — across 21 hearings, six intervenors, and two Amici — is now confirmed as a genuine gap rather than an artefact of this corpus's prior lack of an s.63 primary source. With BSA_1 now coded, the silence is fully documentary: the primary evidentiary standard existed, was in force throughout the entire ANI v. OpenAI proceeding (in force since 1 July 2024, well before the case's 24 July 2026 disposal), and was never invoked.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/DHC/DHC_1_ANI_v_OpenAI_2026]] (the silence this node makes documentary), [[04_Knowledge_Products/Wiki_Intake/SCI_1_White_Paper_AI_and_Judiciary_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Evidentiary_Governance]] (this is the terminal evidentiary standard the construct concerns), [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (candidate — do regulatory logging mandates anticipate s.63 certification at all?)
**Related frameworks:** None directly — evidence law sits outside the 06_Frameworks AI-governance set
**Related projects:** [[02_Projects/P4_Doctrinal_IJLIT]] — primary
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** Not applicable (evidence statute, not a regulatory instrument)
- **Wiki intake status:** Pending — this closes a priority-1 blocking gap; High priority for cross-referencing against RBI/SEBI/CERT-In/DPDP logging provisions

---

## Log

- 2026-08-02: Corpus node created. Sourced via Perplexity Deep Research per [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] Judiciary verification prompt. **This closes the priority-1 blocking gap identified in [[03_Domains/Judicial_Governance]]'s 2026-08-02 log** — the domain's OQ-JG-01 can now be addressed. Immediate next step (not yet done): systematically check RBI_8, CERT_In_2/3, SEBI's AI/ML reporting circulars, and DPDP's breach-notification retention rules against s.63(2)'s four conditions and s.63(4)'s certificate-signatory requirement.
