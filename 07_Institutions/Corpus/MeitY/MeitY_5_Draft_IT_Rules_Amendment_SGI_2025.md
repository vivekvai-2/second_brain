---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/india
  - institution/meity
---

# MeitY_5 — Draft Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Amendment Rules, 2025 (Synthetically Generated Information / Deepfake Labelling)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/MeitY/MeitY_5_Draft_IT_Rules_Amendment_SGI_2025.md`
**Institution:** [[07_Institutions/MEITY]]
**Issuing body:** Ministry of Electronics and Information Technology, Government of India
**Document date:** Draft — base instrument is the Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Rules, 2021 (G.S.R. 139(E), dated 25.2.2021), consolidated/marked-up version "[updated as on __.__.2025]" showing proposed amendments with placeholder citations "Ins. by G.S.R. ___(E), dated ___.___.2025". ⚠ VERIFY BEFORE PUBLISHING — this is a **draft/consolidated working text**, not a gazetted amendment; the placeholder G.S.R. numbers and blank dates confirm the synthetically-generated-information (SGI) provisions are **not yet notified** as of 2026-06-15.
**Pages:** 31 (consolidated IT Rules 2021 text with all amendments through 2023 shown as tracked changes, plus draft 2025 SGI/deepfake amendments in highlighted text)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/DPI_Governance]]

**⚠ 2026-07-15 backlink:** [[07_Institutions/Corpus/MeitY/MeitY_7_IT_Intermediary_Guidelines_Digital_Media_Ethics_Code_Rules_2021]] is now the vault's dedicated primary-source node for the base 2021 Rules this consolidated/marked-up text builds on — reference it for Part II/Part III baseline obligations rather than re-deriving them from this draft-amendment node.

---

## Instrument Identity

**Full title:** The Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Rules, 2021 [updated as on __.__.2025] — consolidated text incorporating draft Information Technology (Intermediary Guidelines and Digital Media Ethics Code) Amendment Rules, 2025
**Type:** Subordinate legislation (Rules) under Section 87(1), clauses (z) and (zg) of Section 87(2), Information Technology Act, 2000 — base 2021 Rules already in force; **2025 SGI provisions are draft/proposed**
**Target entities:** All intermediaries (Part II); significant social media intermediaries (Rule 4) specifically for the new synthetic-media labelling obligations; publishers of news/online curated content (Part III, unchanged by the 2025 draft)
**Legal basis:** Section 87(1) and 87(2)(z)/(zg), IT Act 2000; supersedes IT (Intermediaries Guidelines) Rules, 2011
**Companion documents:** Base 2021 Rules already amended twice — G.S.R. 794(E) dated 28.10.2022 (Grievance Appellate Committee, periodic compliance reports) and G.S.R. 275(E) dated 6.4.2023 (online gaming framework: Rules 4A–4C, online real money game definitions). The draft 2025 amendments add: definition of "synthetically generated information" (Rule 2(1)(wa)), Rule 2(1A) (extending "information" in unlawful-act provisions to include SGI), new Rule 3(3) (intermediary due diligence for SGI labelling), and new Rule 4(1A) (significant social media intermediary obligations for SGI declaration/verification/labelling).

---

## Analytical Classification

**Wiki section:** S2 (India Regulatory Framework) / S4 (Agentic AI Governance — synthetic media as an AI-output governance problem) / S5 (Data, Privacy & Security)
**Jurisdiction:** India
**Confidence:** Medium — base 2021 Rules and 2022/2023 amendments are confirmed in force; the 2025 SGI provisions are **draft only** (Confidence: Low for those specific provisions until gazetted)
**AI explicit:** YES — the draft 2025 amendments are the corpus's most explicit **AI-output (generative AI / deepfake) governance instrument** to date, defining and regulating "synthetically generated information" directly
**Tier classification:** Tier A (for the draft SGI provisions) — directly and explicitly regulates AI-generated content; Tier B (for the base 2021 Rules) — general intermediary/platform governance
**AI Governance Wiki relevance:** VERY HIGH — this is the first corpus node addressing **generative AI content labelling/watermarking** as a regulatory obligation, a central topic in global AI governance debates (cf. EU AI Act Article 50 transparency obligations, China's deep synthesis labelling rules, US state deepfake laws) — directly relevant to comparative analysis in P1 (AI Governance SLR) and P4 (BFSI doctrinal — synthetic media fraud risk)

---

## Substantive Content

### Definition: "Synthetically Generated Information" (Rule 2(1)(wa), draft)
"Information which is artificially or algorithmically created, generated, modified or altered using a computer resource, in a manner that such information reasonably appears to be authentic or true." This is a broad, technology-neutral definition covering text, image, audio, and video generative-AI outputs — **not limited to "deepfakes" in the narrow audiovisual sense**. ⚠ VERIFY BEFORE PUBLISHING — confirm final wording against the gazetted version once notified, as draft definitions are frequently narrowed (e.g., to add intent/deceptive-purpose qualifiers) between draft and final stages.

### Extension of "Information" in Unlawful-Act Provisions (Rule 2(1A), draft)
References to "information" in the context of committing an unlawful act — specifically under Rule 3(1)(b)/(d) (prohibited content categories) and Rule 4(2)/(4) (originator-tracing and proactive-monitoring obligations) — are deemed to include synthetically generated information "unless the context otherwise requires." This is the mechanism by which SGI is **brought within the existing content-takedown and traceability framework** without creating a wholly separate enforcement regime — an example of regulatory layering onto an existing instrument rather than a standalone AI law.

### General Intermediary Due Diligence for SGI (new Rule 3(3), draft)
Where an intermediary's computer resource enables creation/generation/modification/alteration of SGI, it must ensure every such output is:
- **Prominently labelled or embedded** with a "permanent unique metadata or identifier" (terminology deliberately broad — covers visible watermarks, embedded metadata, or other identifiers)
- **Visibility/audibility threshold**: the label must cover **at least 10% of the surface area of the visual display**, or for audio content, be present **during the initial 10% of its duration**
- The label/metadata/identifier **must be immediately usable to identify** the content as SGI generated via that intermediary's computer resource
- The intermediary **may not enable modification, suppression, or removal** of the label by users

⚠ VERIFY BEFORE PUBLISHING — the 10% surface-area/duration thresholds are precise numeric design parameters that are highly likely to be debated/revised before finalisation (comparable provisions in other jurisdictions — e.g., China's January 2025 deep synthesis labelling measures — use different visibility/placement standards); do not cite these figures as settled law. Also note the "Provided that the removal/disabling of access... shall not amount to a violation of Section 79(2)(a)/(b)" safe-harbour clause inserted alongside Rule 3(1)(b)(xi) — this is a significant safe-harbour clarification for SGI-related takedowns specifically.

### Significant Social Media Intermediary (SSMI) Obligations for SGI (new Rule 4(1A), draft)
An SSMI that displays/uploads/publishes information must, **prior to publication**:
1. **Require users to declare** whether information being uploaded is synthetically generated;
2. **Deploy reasonable and appropriate technical measures** (automated tools or other mechanisms) to **verify the accuracy of such declarations**, having regard to nature/format/source;
3. Where declaration or technical verification confirms SGI status, **ensure clear and prominent labelling/notice** indicating the content is synthetically generated.

**Deemed-failure clause**: if an SSMI becomes aware (or it is otherwise established) that it knowingly permitted, promoted, or failed to act on SGI in contravention of these rules, it is **deemed to have failed to exercise due diligence** — this is significant because failure of due diligence under Rule 3 is the trigger for loss of safe-harbour immunity under Section 79 of the IT Act. The Explanation reinforces that SSMI responsibility extends to "reasonable and proportionate technical measures" to verify user declarations — a standard of **proportionate verification**, not absolute/strict liability for every piece of SGI.

### Relationship to Existing Online-Gaming Framework (Rules 4–4C, in force since 2023)
The draft SGI provisions sit alongside (and are textually adjacent to) the 2023-inserted online gaming intermediary framework (Rules 4A–4C: online gaming self-regulatory bodies, permissible online real money game verification, KYC requirements per RBI standards, 72-hour/24-hour grievance and law-enforcement-cooperation timelines). No direct substantive overlap, but both represent the same regulatory technique: **layering category-specific due-diligence obligations onto the general intermediary framework via amendment** rather than separate primary legislation.

### Grievance Appellate Committee (Rules 3A, in force since Oct 2022)
Statutory appeal mechanism for users aggrieved by Grievance Officer decisions or unresolved complaints — GAC must resolve appeals within 30 calendar days via online dispute resolution. Relevant as the likely appellate venue for disputes arising from SGI-labelling/removal decisions once Rule 3(3)/4(1A) are notified.

### Part III (Digital Media Ethics Code) — Unaffected by 2025 Draft
The three-tier self-regulation structure (publisher self-regulation → industry self-regulatory bodies → Inter-Departmental Committee/Oversight Mechanism) for news and online curated content publishers remains unchanged by the draft SGI amendments — confirms the SGI labelling regime is being inserted as an **intermediary (Part II) obligation**, not a publisher/content-classification (Part III) obligation, even though synthetic media most often appears as published/curated content.

---

## Analytical Significance for PRIS Research

### For P1 (AI Governance SLR) and Comparative Regulatory Analysis
This draft is India's first sector-general (i.e., not BFSI/securities-specific) regulatory text directly defining and addressing generative-AI/synthetic-media outputs. Structurally, it follows the **same "amend an existing technology-neutral framework" pattern** seen in MeitY_4 (DPDP Rules — SDF algorithmic due diligence inserted into a general data-protection framework) and RBI_6/SEBI_9/SEBI_10 (AI/algorithmic provisions inserted into existing outsourcing/reporting frameworks). This reinforces the [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] finding: **India is governing AI/generative-AI outputs through incremental amendment of multiple pre-existing sectoral instruments rather than a horizontal AI law** — a pattern directly comparable (and contrastable) to the EU's horizontal AI Act approach, useful for P1's comparative regulatory-configuration analysis (fsQCA candidate variable: "amendment-based" vs. "horizontal-statute" AI governance design).

### For Institutional Grammar / ADICO Coding
The new Rule 3(3) and 4(1A) are unusually precise ADICO-structured provisions — explicit **Attributes** (intermediary, SSMI), **Deontics** ("shall ensure", "shall require", "shall not enable"), **Aims** (labelling, verification, non-removal), **Conditions** (prior to publication, where computer resource enables SGI creation), and a rare explicit **quantified threshold** (10% surface area/duration) — making this draft an excellent candidate for Institutional Grammar 2.0 coding exercises, particularly because the side-by-side draft/base-text format allows direct before/after ADICO comparison of the same legal provision.

### Draft Status as a Research Finding in Itself
The fact that this consolidated text exists with placeholder G.S.R. citations is itself evidence of **India's iterative, amendment-heavy regulatory style for digital/AI governance** (three rounds of amendment to the 2021 Rules already: Oct 2022, April 2023, and this pending 2025 draft) — relevant to any [[05_Concepts/05_Concepts_Signature/Governance_Debt]] discussion regarding the compliance burden of frequently-amended intermediary obligations on platforms operating in India.

### Coordination / Parallelism Pattern
**Existing nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (SDF algorithmic due diligence — both are MeitY instruments addressing algorithmic/AI accountability via amendment to existing frameworks, issued within months of each other in the same regulatory cycle).
**Pattern:** **Within-regulator parallelism** — MeitY is simultaneously developing (a) a general data-protection algorithmic-audit obligation (DPDP Rules, Rule 13(3)) and (b) a content-labelling obligation for AI-generated information (draft IT Rules SGI amendments), via two textually separate instruments rather than a unified AI-content-and-data framework. Both nonetheless converge on the same underlying policy concern — accountability for AI-system outputs — suggesting an emerging (but not yet consolidated) MeitY AI-governance agenda for 2025–2026.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] (within-regulator algorithmic-governance parallelism), [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_10]] (cross-regulator AI/algorithmic-output governance comparison), [[07_Institutions/Corpus/RBI/RBI_6_AIFI_Outsourcing_Directions_2025]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]] (amendment-based AI governance across MeitY/SEBI/RBI), [[05_Concepts/05_Concepts_Signature/Governance_Debt]] (cumulative amendment burden — three rounds since 2021), [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (generative-AI output labelling as a governance mechanism), [[05_Concepts/05_Concepts_Standard/Transparency]] (labelling/disclosure as transparency mechanism), [[05_Concepts/05_Concepts_Standard/Accountability]]
**Related frameworks:** None yet in `06_Frameworks` — candidate for a future "India Synthetic Media / Deepfake Governance" framework synthesis node once this and document 7 (Takedown Procedure for Intimate Photos/Videos/Deepfakes — next in this batch) are both processed
**Related projects:** [[02_Projects/P1_SLR_RG]] (AI Governance SLR — generative AI/deepfake regulation comparative element), [[08_Methods/Institutional_Grammar_IG2]] (ADICO coding candidate, draft/base text comparison)
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]] (S4 — generative AI governance)
**Related consulting:** Potentially relevant to any future engagement involving platform content-moderation compliance (synthetic-media labelling) — flag if AEGIS_OS scope expands to platform/intermediary clients.

---

## Coding Status

- **P3 NVivo:** Not primary BFSI evidence — but flag for P1 SLR screening corpus given direct generative-AI regulatory relevance
- **Wiki intake status:** Pending — HIGH priority for S4 (Agentic AI Governance) given this is the first explicit generative-AI-output regulatory text in the corpus

---

## Log

- 2026-06-15: Corpus node created. Batch 7. Cowork session. Document recorded as DRAFT pending gazette notification — re-verify status in future sessions before treating SGI labelling obligations as binding law.
