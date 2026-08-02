---
type: Process Document
status: active
last_updated: 2026-08-02
tags:
  - type/process-document
  - status/active
  - engine/phd
---

# Missing-Node & Tier Audit — Perplexity Sourcing Prompts (2026-08-02, third pass)

**Parent:** [[Thin_Node_Perplexity_Prompts_2026-08-02]] (pass 1 — Domains/Concepts/Frameworks) | [[Sector_Gap_Audit_Perplexity_Prompts_2026-08-02]] (pass 2 — five sectors)

**Why a third pass:** passes 1 and 2 both closed out fully today. Between them they audited `03_Domains`, `05_Concepts`, `06_Frameworks`, and five sectoral verticals — and every prompt they generated has been run and intaken. What neither pass examined is (a) the tiers below and beside those — `07_Institutions` parent notes, `08_Methods`, `04_Knowledge_Products` proper, `09_Teaching`; and (b) the harder question of **nodes that should exist and don't**. A thin node announces itself. A missing node does not.

**Method:** Three measurements across all 429 non-archive notes.

1. **Depth** — word count per note.
2. **Wiring** — resolved wikilinks out, and inbound links from other notes. A note with high inbound is load-bearing; a note with zero inbound is inert regardless of length.
3. **Missing-node detection** — term-frequency sweep across the whole vault for constructs, statutes, standards and institutions that recur often in prose but have **no dedicated note of their own**. High mention count with zero node is the signature of a concept the vault relies on but has never formalised.

---

## 1. Headline finding — two real failures (a third was retracted)

> ### ⚠ RETRACTION — "Finding A: evidence orphaning" (issued and withdrawn 2026-08-02)
>
> The first version of this audit reported that **195 of 246 evidence-layer nodes had zero inbound links**, called it the most serious finding in the vault, and recommended a dedicated wiring session before any further ingest.
>
> **That was a measurement artifact, not a vault condition.** The profiling script matched wikilink targets against note *stems* only. This vault predominantly writes links in full-path form — `[[04_Knowledge_Products/Wiki_Intake/F085_Sudjianto_Zhang_Model_Validation_Practice_Banking_2024]]` rather than the bare-stem form `F085_Sudjianto_Zhang_…` — and every path-style link was silently discarded before the inbound count was taken. Since path-style is the house convention for evidence citations specifically, the discard fell almost entirely on the evidence layer, manufacturing exactly the pattern reported.
>
> **Corrected figures, stem-normalised:** **10 of 247** evidence-layer nodes had zero inbound links before today's work; **8 of 247** after. The evidence layer is not orphaned. It is close to fully wired, and the wiring discipline of the two earlier passes today held.
>
> The eight remaining are listed in §2 and are a fifteen-minute job, not a structural problem.
>
> **What else the bug touched:** all inbound counts in the first version were understated, most visibly for institution parent notes — `International` was reported at 0 inbound and is actually 20; `MEITY` 66, `CERT_IN` 50, `RBI` 47, `SEBI` 58. Those notes are short but load-bearing, which is a different diagnosis from short and inert. Corrected table in §2. **Unaffected:** the missing-node detection (§2, grep-based), all word counts, and the empty-folder / misfiled-file / empty-tier findings — those were verified directly against the filesystem. Findings B and C stand as issued.

| # | Failure | Scale | Right remedy |
|---|---|---|---|
| ~~A~~ | ~~Evidence orphaning~~ | **Retracted — see above. Actual: 8 of 247** | Fifteen minutes of wiring |
| **B** | **Missing nodes** — high-frequency constructs and instruments with no note | 4 frameworks, ~6 concepts, 4 institutions (detail below) | **Sourcing.** Prompts in §3 |
| **C** | **Thin tiers** — whole ontology layers under-built | `08_Methods` (4 notes, 2,645 words); `09_Teaching` (empty); Knowledge Products are outlines | Mixed — §3 covers the sourceable part |

**Methodological note for future audits of this vault:** normalise wikilink targets to their final path segment before computing inbound degree. Mixed link conventions (stem-style in concept notes, path-style in evidence citations) will otherwise produce a false orphan signal concentrated in whichever tier uses paths. Also exclude `\|` (escaped-pipe) links before flagging broken targets — the house style escapes pipes inside table cells, and a naive regex reads the trailing backslash as part of the target.

### The real link-integrity finding (2026-08-02, replaces the retracted one)

A corrected vault-wide scan found **156 apparently broken wikilinks**. Of these, ~87 were false positives from escaped pipes in tables. **68 were genuine broken paths, and were fixed.** They fell into a small number of systematic classes, all caused by writing a plausible-but-wrong folder path:

| Wrong path | Correct path | Count |
|---|---|---|
| `01_Strategy/fsQCA` | `08_Methods/fsQCA` | 14 |
| `05_Concepts/<Concept>` | `05_Concepts/05_Concepts_Signature/` or `.../05_Concepts_Standard/` | 41 |
| `07_Institutions/Corpus/International/<node>` | `04_Knowledge_Products/Wiki_Intake/<node>` (misfiled sector nodes) | 6 |
| Assorted one-offs (`07_Institutions/Corpus/CERT_IN`, `MeitY_IndiaAI_Mission`, `OECD_AI_Principles_2024`, `SEBI_15_TEMPLATE_original`) | — | 7 |

**This is the finding the orphan bug was masking.** The evidence layer was well cited; a meaningful share of those citations simply did not resolve, because the two-tier concept folder structure (`05_Concepts_Signature` / `05_Concepts_Standard`) and the `08_Methods` location are easy to mis-key, and Obsidian fails such links silently rather than warning. The `05_Concepts/<Concept>` class alone accounted for 41 dead links pointing at the five most load-bearing concept notes in the vault.

**Recommendation:** prefer bare-stem links (`[[Regulatory_Parallelism]]`) over path-style links for concepts, methods and frameworks — stems are unique across this vault and cannot be mis-keyed. Reserve path-style for corpus nodes, where the folder is part of the identifier.

**Nine genuine broken links remain, all deliberate or already-tracked:** `06_Frameworks/GDPR` (forward reference — Prompt 5 will build it); `UIDAI_Circular_Face_Auth_2022` and `MeitY_PM_KISAN_Guidelines_2024` (the two non-existent nodes already recorded in [[_Concepts_MOC]] as the reason [[Records_Rules_Asymmetry]] was downgraded to candidate); and two references to `contribution-framing`, which is a skill, not a note.

---

## 2. Missing-node detection — mentions vs. node existence

Term-frequency sweep. "Files" = number of notes mentioning the term at least once.

### Frameworks / instruments with no `06_Frameworks` node

| Instrument | Files mentioning | Node? | Read |
|---|---|---|---|
| **DEPA** (Data Empowerment & Protection Architecture) | **72** | None | Most-mentioned un-noded instrument in the vault. Central to consent architecture, DPI, and Ch.4 of the DPDP Playbook. Chronic |
| **MAS FEAT / Veritas** (Singapore) | 51 / 9 | None | Named as a primary comparator in `Doctrinal_Analysis` and P4's redesign proposal — carrying analytic weight with no node behind it |
| **GDPR** | 41 | None | Already self-flagged in pass 1's own log ("the still-unbuilt GDPR framework node") and still unbuilt |
| **ISO/IEC 42001** (+ 23894, 27001) | 32 / 7 / 11 | None | The AI management-system certification standard. Directly load-bearing for [[Assurance_Reuse_Gap]] and [[Evidentiary_Governance]] |
| Telecommunications Act 2023 | 4 | None | New `Telecom_AI_Governance` domain built today has no statutory anchor |

### Constructs with no `05_Concepts` node

| Construct | Files mentioning | Read |
|---|---|---|
| **Fairness / non-discrimination** | **70** | No note |
| **Model risk** | **69** | No note — despite SR 11-7, Sudjianto, Rao & Scepanovic, Tammenga all sitting in `Wiki_Intake` unwired |
| **Explainability** | **65** | No note |
| **Bias** | 60 | No note |
| **Human oversight / human-in-the-loop** | 39 / 17 | No note |
| Risk-tiering | 32 | No note |
| Redress / contestability | 23 / 10 | No note |
| Auditability | 18 | No note |
| Proportionality | 16 | No note |
| Conformity assessment | 15 | No note |
| Polycentricity | 13 | No note |

**This is the sharpest finding in the audit.** Your fsQCA outcome is operationalised as "combined **EA-principle** calibration (pending TAC decision D4)" per [[fsQCA]]. The EA principle set — fairness, explainability, human oversight, contestability — is the single most-referenced cluster of constructs in the entire vault, and **not one of its members has a concept note**. `Transparency`, `Accountability` and `Legitimacy` were built; their siblings were not. Until D4 is decided, the outcome variable of your empirical chapter rests on constructs the vault has never defined, calibrated, or literature-anchored. That is a thesis-path dependency, not a tidiness issue.

Applying the PRIS ontology rule (concept notes only for high-value recurring constructs), the defensible additions are **Explainability, Fairness, Human Oversight, Contestability/Redress, Model Risk** — and arguably **Proportionality** as the calibration logic linking risk-tiering to obligation intensity. Bias folds into Fairness. Auditability folds into [[Evidentiary_Governance]]. Polycentricity folds into [[Institutional_Coherence]].

### Institutions with no `07_Institutions` note

| Institution | Files | Read |
|---|---|---|
| **Data Protection Board of India** | 17 | Statutory body under DPDP with no institution note. Pass 1 logged "no DPB orders yet" — but the institution shell should exist to receive them |
| **Department of Telecommunications (DoT)** | 4 | `Telecom_AI_Governance` domain built today; the rule-making ministry has no node (TRAI, the regulator, does) |
| **Ministry of Power / Grid-India** | 5 / 2 | `Power_Grid_Critical_Infrastructure_Governance` built today with CEA and NCIIPC nodes; the ministry and system operator are absent |
| **NPCI** | 3 | UPI/AA operator. `DPI_Governance` has UIDAI but not NPCI |
| Bureau of Indian Standards (LITD 30) | 0 | India's own AI standardisation body — total absence, and directly connected to the ISO 42001 gap above |

### Evidence-layer orphans — the actual list (8 of 247, corrected)

All eight are recent Wiki_Intake additions never cited from a concept or domain note. None is a structural failure; all are ingest-ahead-of-wiring at the margin.

| Node | Likely home |
|---|---|
| `F120_Bassey_Mulligan_Ojo_Digital_Tax_Administration_Framework_2022` | [[Systemic_Regulatory_Governance]] or a tax-administration use case |
| `F128_Seetharaman_Mathew_De_Does_Location_Matter_IS_Research_2024` | Methods / IS-research positioning — arguably belongs with [[SLR_Protocol]] |
| `F131_Juelich_Boko_Haram_Frontier_AI_2026` | No natural home in the current ontology — candidate for deletion or archive |
| `F133_Trout_et_al_AI_Insurance_Stack_2026` | [[Insurance_AI_Governance]] — built today, this should have been wired into it |
| `F134_Crichton_Reddy_Ji_Operationalizing_AI_Guidance_2026` | [[Governance_Debt]] / [[Assurance_Reuse_Gap]] |
| `F136_HTI_Directors_Guide_AI_Governance_2026` | [[Board_AI_Risk_Oversight_Checklist]] and [[Accountability]] |
| `F137_LeoneDeCastris_Jiang_Wang_AI_Governance_China_2026` | [[International_Comparators]] |
| `F138_GoogleDeepMind_AI_Control_Roadmap_2026` | [[Agentic_AI_Governance]] / [[Human_Oversight]] |

Separately, **21 of 22 notes in `10_Consulting/VV_Advisory_Outreach_Templates/` have zero inbound links** — they are not reachable from [[Consulting_Deliverable_Templates_Index]]. That is a genuine (if low-stakes) wiring gap, and the only one the corrected analysis supports.

### Structural / filing integrity

- `07_Institutions/Corpus/Judiciary/` and `/MoHFW/` — **both empty directories**. `SCI_1_White_Paper_AI_and_Judiciary_2025` and `MoHFW_1_SAHI_Healthcare_AI_Strategy_2026` are sitting in `04_Knowledge_Products/Wiki_Intake/` instead. Misfiled, and both have zero inbound links as a result.
- `09_Teaching/` — **completely empty**, 0 files. Given the stated Professor-of-Practice / adjunct track, this is a blank tier, not a thin one.
- `2026-07-15.md` at vault root — 16 words, isolated. Stray daily note.
- Duplicate pair: `Deepthi_Gupta_Rai_Arora_AI_Dynamics_Indian_Banking_2022` and `..._AI_Indian_Banking_Dynamics_2022`.

### Thin tiers

| Tier | Size | Read |
|---|---|---|
| `08_Methods` | 4 notes, 2,645 words total | **Thinnest tier relative to structural weight in the vault.** `fsQCA` 611w, `Institutional_Grammar_IG2` 605w, `Doctrinal_Analysis` 566w, `SLR_Protocol` 866w. These four methods carry the entire thesis. Missing entirely: **comparative regulatory analysis** (used throughout P4 and the fsQCA comparator logic, no note), **NVivo coding protocol / inter-coder reliability**, **calibration & case selection protocol** |
| `04_Knowledge_Products` (the four strategic assets) | `AI_Governance_Wiki` 709w, `Regulatory_Complexity_Handbook` 647w, `BFSI_AI_Governance_Handbook` 640w, `DPDP_Playbook` 619w | These are **outlines with chapter headings, not products**. Not a sourcing gap so much as an unwritten-content gap — except DPDP_Playbook Ch.4 (DEPA) and Ch.7 (cross-border), which are blocked on the missing DEPA node |
| `07_Institutions` parent notes | **Corrected inbound counts:** `International` 198w / 20 in; `Parliament` 206w / 3 in; `NCIIPC` 361w / 4 in; `NITI_Aayog` 371w / 10 in; `CEA` 522w / 5 in; `DPIIT` 550w / 6 in; and at the other end `MEITY` 513w / **66 in**, `SEBI` 512w / **58 in**, `CERT_IN` 481w / **50 in**, `RBI` 518w / **47 in** | Revised diagnosis. These are short *and heavily depended upon* — the four busiest are each ~500 words fronting 8–11 corpus nodes and absorbing 47–66 inbound links. That is thin-at-a-load-bearing-point, which is worse than thin-and-inert but a smaller job to fix: each needs a synthesis paragraph, not new sourcing. `International` at 198 words fronting 32 corpus nodes remains the single worst ratio in the vault |

---

## 3. Perplexity Deep Research Prompts

Same house pattern as passes 1 and 2: confirmed, dated, linked primary sources only; no synthesis; output pasteable straight into a node's Candidate Sources section, then run through [[PRIS_Corpus_Intake_Prompts]].

---

### PROMPT 1 — EA-principle concept cluster (highest priority; thesis-path dependency)

```
I am building Concept-level nodes for five constructs that recur constantly across my AI-governance research corpus but that I have never formalised: Explainability, Fairness/Non-discrimination, Human Oversight, Contestability/Redress, and Proportionality. These will serve as the constituent principles of a calibrated outcome variable in a fuzzy-set QCA study of AI governance regimes, so I need sources that OPERATIONALISE and MEASURE these constructs, not sources that merely advocate for them.

For each of the five constructs, find and list, with exact title, author/issuing body, date, and direct link (DOI where available):

1. The canonical operational definition used in Information Systems, public administration, or regulatory governance literature — prioritise ABDC A/A* journals (MISQ, ISR, JMIS, JSIS, Government Information Quarterly, Regulation & Governance, Public Administration Review)
2. Any published measurement instrument, index, scale, or coding scheme that renders the construct empirically assessable across cases — this is the critical requirement, since these constructs must be calibrated to fuzzy-set membership scores
3. Any study that has used the construct as a dependent, independent, or moderating variable in a configurational, comparative, or QCA-based design
4. The authoritative regulatory-instrument definition of each construct as it appears in the EU AI Act, OECD AI Principles (2019/2024), UNESCO Recommendation (2021), and NIST AI RMF (2023) — I need the exact operative text and article/section reference, not a paraphrase
5. Any critique arguing the construct is not meaningfully measurable or is contested in definition — I need to know where the operationalisation is unsafe before I calibrate on it

For each item confirm exact date, author/venue, and working link. Flag which of the five constructs has the weakest measurement literature. Do not summarize findings — I will read and code these myself.
```

---

### PROMPT 2 — DEPA / Account Aggregator / NPCI (most-mentioned un-noded instrument, 72 files)

```
I am building a Framework-level research node on India's Data Empowerment and Protection Architecture (DEPA) and the Account Aggregator ecosystem it underpins. This is referenced across 72 notes in my corpus but has no primary-source anchoring of its own. I need primary sources only — no consultancy explainers.

Find and list, with exact title, issuing body, date, and direct link:
1. The original DEPA framework document (NITI Aayog, 2020) and any subsequent official revisions or successor documents
2. RBI's Account Aggregator regulatory instruments — the NBFC-AA Master Directions (2016) and every subsequent amendment, circular, or clarification, with current consolidated version identified
3. ReBIT (Reserve Bank Information Technology Pvt Ltd) published AA technical standards and specifications, and any governance or audit requirements attached to them
4. Sahamati (the AA industry alliance) published governance frameworks, participation criteria, or grievance/redress mechanisms — flag clearly that these are self-regulatory, not statutory
5. NPCI governance documents for UPI — circulars, participation rules, or any published policy on algorithmic/AI systems in payments (fraud detection, risk scoring, transaction monitoring)
6. Any official document connecting DEPA's consent-manager architecture to DPDP Act 2023 Consent Manager obligations, including MeitY's DPDP Rules 2025 provisions on Consent Managers and any registration framework issued
7. Any government or RBI document extending DEPA's consent architecture beyond finance (health via ABDM, telecom, or the proposed cross-sectoral consent layer)

For each item confirm exact date, issuing body, current-vs-superseded status, and a working link. Where an instrument is self-regulatory rather than statutory, say so explicitly. Do not summarize — I will read and code these myself.
```

---

### PROMPT 3 — ISO/IEC 42001, 23894 and India's own AI standardisation

```
I am building a Framework-level node on AI management-system standards and certification. My corpus references ISO/IEC 42001 across 32 notes with no dedicated node, and has zero coverage of India's own AI standardisation activity. My analytic interest is whether certification to a management-system standard can substitute for, or be reused as evidence of, regulatory compliance.

Find and list, with exact title, issuing body, date, and direct link:
1. ISO/IEC 42001:2023 (AI management system) — official ISO catalogue entry, publication date, current amendment status, and any published corrigenda
2. ISO/IEC 23894:2023 (AI risk management guidance) and ISO/IEC 22989 (AI terminology) — same details
3. Any published crosswalk or mapping between ISO/IEC 42001 and the EU AI Act, NIST AI RMF, or ISO/IEC 27001 — issued by ISO, national standards bodies, accreditation bodies, or certification bodies
4. Accreditation-body guidance on how ISO/IEC 42001 certification is audited (IAF, UKAS, ANAB, or NABCB in India) — including any mandatory-document or auditor-competence requirements
5. Bureau of Indian Standards (BIS) work on AI standards — specifically the LITD 30 sectional committee (Artificial Intelligence), any published Indian Standards on AI, adoption of ISO/IEC 42001 as an IS, or draft standards under public comment
6. Any regulatory instrument, in any jurisdiction, that formally recognises ISO/IEC 42001 certification as evidence of compliance or as a presumption of conformity — this is the key question; if no such recognition exists anywhere, confirm the absence explicitly rather than offering near-misses
7. Any EU harmonised standards under the AI Act (CEN-CENELEC JTC 21) published or in draft, and their relationship to ISO/IEC 42001

For each item confirm exact date, issuing body, and working link. Distinguish published standards from drafts and work-items. Do not summarize — I will read and code these myself.
```

---

### PROMPT 4 — Singapore MAS FEAT / Veritas / IMDA Model AI Governance Framework

```
I am building a Framework-level node on Singapore's AI governance architecture. It is cited as a primary comparator across 51 notes in my corpus — including in the redesign proposal of a law-journal paper — but has no node and no primary-source anchoring. I need primary documents.

Find and list, with exact title, issuing body, date, and direct link:
1. MAS FEAT Principles (Fairness, Ethics, Accountability, Transparency) — original 2018 document and any revisions
2. The Veritas Initiative outputs — all published phases, including the FEAT assessment methodologies, the open-source toolkit, and any whitepapers on fairness/ethics/accountability/transparency assessment methodology
3. MAS Information Paper on AI Model Risk Management in the financial sector (2024) and any subsequent MAS guidelines, circulars, or consultation papers on AI
4. IMDA/PDPC Model AI Governance Framework — the 2019 and 2020 editions, plus the Model AI Governance Framework for Generative AI (2024), and AI Verify (the testing framework and toolkit) with its governing foundation's published documents
5. Any Singapore statutory instrument (as distinct from guidance) that imposes binding AI obligations — if none exists, confirm that explicitly, since the binding-vs-advisory distinction is analytically central for me
6. Any published comparative analysis of Singapore's approach against India's RBI FREE-AI, the EU AI Act, or the UK's regulator-led model — particularly anything in peer-reviewed IS, law, or regulatory-governance journals

For each item confirm exact date, issuing body, binding vs. advisory status, and a working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT 5 — GDPR as a framework node (comparative anchor)

```
I am building a Framework-level node on the EU General Data Protection Regulation, scoped specifically to its automated-decision-making and AI-relevant provisions. GDPR is referenced across 41 notes in my corpus with no node. I do not need general GDPR explainers — I need the AI/ADM-specific primary layer, for comparison against India's DPDP Act 2023.

Find and list, with exact title, issuing body, date, and direct link:
1. GDPR Articles 22, 13(2)(f), 14(2)(g), 15(1)(h) and Recital 71 — official consolidated EUR-Lex text reference
2. EDPB (and predecessor WP29) guidelines specifically on automated individual decision-making and profiling, including current adopted versions and any superseded editions
3. CJEU judgments interpreting Article 22 — specifically SCHUFA (C-634/21) and any subsequent rulings on automated decision-making, credit scoring, or algorithmic profiling
4. National DPA enforcement decisions and fines issued specifically against AI, algorithmic, or automated-processing practices (2020 onward) — the largest and most doctrinally significant, with authority and date for each
5. Any official EDPB or Commission document addressing the interaction between GDPR and the EU AI Act, including allocation of supervisory competence
6. Any published comparative legal analysis of GDPR Article 22 against India's DPDP Act 2023 — noting that DPDP has no ADM provision at all, so I am specifically looking for scholarship that treats that absence analytically

For each item confirm exact date, issuing body/court, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT 6 — Missing institutions: DPB, DoT, Ministry of Power, NPCI, BIS

```
I need primary-source material to create institution-level nodes for five Indian bodies that appear throughout my AI-governance corpus but have no dedicated node. For each, I need the constitutive instrument, the current leadership/composition, and any published output.

Find and list, with exact title, issuing body, date, and direct link:

1. DATA PROTECTION BOARD OF INDIA — the establishment notification under DPDP Act 2023; appointment notifications for Chairperson and Members; the Board's procedural rules (whether under DPDP Rules 2025 or separately notified); any orders, directions, or public statements issued to date; and its official web presence if one now exists
2. DEPARTMENT OF TELECOMMUNICATIONS — all rules notified under the Telecommunications Act 2023 to date (with a complete list, since I need to establish which subject areas have been covered and which have not); any DoT notification, advisory, or consultation referencing AI, automated systems, or algorithmic decision-making; and the current status of the Act's phased commencement
3. MINISTRY OF POWER — any notification, advisory, or scheme document on grid cybersecurity, smart-grid automation, or AI in power-system operation; the constitutive relationship between MoP, CEA and Grid Controller of India (Grid-India); and any National Electricity Policy or Plan provision addressing digital/AI systems
4. GRID CONTROLLER OF INDIA (Grid-India, formerly POSOCO) — corporate constitution, regulatory reporting obligations, and any published document on automated or AI-assisted grid operation, load forecasting, or system security
5. BUREAU OF INDIAN STANDARDS — the LITD 30 sectional committee on Artificial Intelligence: its constitution, scope, membership, published Indian Standards, drafts under public comment, and its formal relationship to ISO/IEC JTC 1/SC 42

For each item confirm exact date, issuing body, and working link. Where a body has published nothing in the relevant area, state that explicitly rather than substituting adjacent material. Do not summarize — I will read and code these myself.
```

---

### PROMPT 7 — Methods tier: comparative regulatory analysis, coding reliability, fsQCA calibration

```
I am strengthening the methodology layer of a doctoral thesis that combines fuzzy-set QCA, Institutional Grammar 2.0 (ADICO) coding, doctrinal legal analysis, and systematic literature review. Three method areas are currently under-anchored and one has no methodological source base at all. I need authoritative methodological references, not applications.

Find and list, with exact title, author, venue, date, and direct link (DOI where available):

1. COMPARATIVE REGULATORY ANALYSIS as a method — I have no methodological anchor for this at all despite using it throughout. I need: canonical texts on comparative regulatory/legal method; the functional-equivalence debate in comparative law and its applicability to regulatory instruments rather than statutes; and any methodological work on comparing regulatory regimes across jurisdictions where the instruments differ in binding force
2. QUALITATIVE CODING RELIABILITY for institutional/regulatory text — methodological literature on inter-coder reliability for rule-level coding specifically (not general content analysis); the current methodological debate on Cohen's kappa vs Krippendorff's alpha for this kind of data; reporting standards for IG/ADICO coding reliability; and any published IG 2.0 study that reports its reliability procedure in enough detail to serve as a template
3. fsQCA CALIBRATION for institutional and governance data — methodological guidance on calibrating qualitative institutional conditions into fuzzy-set membership; the debate on direct vs indirect calibration and on theoretical vs data-driven anchor selection; robustness-testing standards post-2020 (Oana & Schneider, Skaaning); and guidance on limited diversity and counterfactual analysis in mid-N designs
4. MIXED IG-QCA DESIGNS — any published study that uses Institutional Grammar coding to generate the conditions for a QCA analysis. If no such study exists, confirm that explicitly, since it would be methodologically significant for my contribution claim

For each item confirm exact date, author/venue, and working link. Prioritise ABDC A/A* and equivalent methodological venues. Do not summarize findings — I will read and code these myself.
```

---

### PROMPT 8 — Model Risk as a concept node (69 files, unwired evidence already present)

```
I am building a Concept-level node on Model Risk and Model Risk Management as it applies to AI/ML systems in regulated financial institutions. The construct appears across 69 notes in my corpus but has never been formalised, and several primary documents on it are already in my collection unconnected to any concept. I need the authoritative regulatory and academic layer.

Find and list, with exact title, issuing body/author, date, and direct link:
1. The current authoritative supervisory statements on model risk management: US Fed/OCC SR 11-7 (2011) and any subsequent update or AI-specific supplement; UK PRA SS1/23 (model risk management principles for banks, 2023); ECB guide to internal models and any AI-related supervisory expectations
2. Any supervisory document that explicitly addresses whether AI/ML models fall inside existing model-risk frameworks or require a separate regime — this boundary question is my central interest
3. MAS Information Paper on AI Model Risk Management (2024) and any equivalent from other Asian regulators (HKMA, BoJ, BSP)
4. RBI's position on model risk — any circular, master direction, or FREE-AI provision addressing model validation, model inventory, or model governance for Indian regulated entities, including whether an SR 11-7 equivalent exists in India at all
5. Peer-reviewed literature (2020 onward) on the adequacy of traditional model-risk frameworks for machine-learning and generative systems, particularly anything arguing they are structurally insufficient
6. Any published work connecting model risk management to the three-lines-of-defence structure for AI specifically

For each item confirm exact date, issuing body, and working link. On item 4, if India has no model-risk-management instrument equivalent to SR 11-7 or SS1/23, state that clearly — the absence is analytically important to me. Do not summarize — I will read and code these myself.
```

---

## 4. Recommended sequence

1. **Prompt 1 (EA-principle cluster)** — run first. It is the only item on this list that sits on the thesis critical path: the fsQCA outcome variable cannot be calibrated on constructs the vault has not defined. TAC decision D4 is blocked behind it.
2. **Prompt 2 (DEPA/AA/NPCI)** — highest mention count of any un-noded instrument (72 files), and it unblocks DPDP Playbook Ch.4 and Ch.7.
3. **Prompt 3 (ISO 42001 + BIS)** — feeds [[Assurance_Reuse_Gap]] and [[Evidentiary_Governance]] directly, and item 6 (does any regulator recognise 42001 as presumption of conformity?) is a publishable finding either way it resolves.
4. **Prompt 7 (Methods)** — item 4 tests whether the IG→QCA design is genuinely novel. If no prior study exists, that is a contribution claim, and it is worth knowing before writing the methodology chapter rather than after.
5. **Prompts 4 and 5 (Singapore, GDPR)** — comparative anchors. Both are currently doing analytic work in P4 without a node behind them.
6. **Prompt 8 (Model Risk)** — moderate priority; much of the evidence is already in the vault and needs wiring more than sourcing.
7. **Prompt 6 (missing institutions)** — lowest urgency of the eight. These are mostly empty shells to be created; several will return confirmed absence, which is itself worth recording.

**~~Not addressed by any prompt above, and arguably more valuable than all of them: the 195 orphaned evidence nodes.~~** Retracted — see §1. The real number is 8, listed in §2 with suggested homes, plus the 21 unreachable outreach templates. Both are short jobs and neither should displace the sourcing sequence above.

**What replaces it as the highest-value non-sourcing work:** the four load-bearing institution parent notes (`MEITY`, `SEBI`, `CERT_IN`, `RBI`) are each ~500 words absorbing 47–66 inbound links. They are the vault's most-traversed synthesis points and currently function as indexes rather than as synthesis. A paragraph each on the institution's governance posture, instrument-issuing pattern, and coordination behaviour would compound across every path that runs through them — no sourcing required, the material is already in their own corpus folders.

**Also outstanding, no prompt written (housekeeping):** move `SCI_1_White_Paper_AI_and_Judiciary_2025` → `07_Institutions/Corpus/Judiciary/` and `MoHFW_1_SAHI_Healthcare_AI_Strategy_2026` → `07_Institutions/Corpus/MoHFW/` (both folders exist and are empty); merge the duplicated Deepthi/Gupta/Rai/Arora 2022 node; delete the stray root-level `2026-07-15.md`; and decide whether `09_Teaching` is a live tier or should be removed from the ontology.

---

## Log

- 2026-08-02: **Prompt 8 (Model Risk) run and intaken — all eight prompts now closed.** New concept node [[Model_Risk]]; new corpus node [[07_Institutions/Corpus/RBI/RBI_13_Draft_Model_Risk_Credit_2024]].

  **⚠ The corpus was carrying a superseded instrument. SR 11-7 was replaced on 17 April 2026 by SR 26-2** (Fed, jointly with OCC and FDIC; companions OCC Bulletin 2026-13, FDIC FIL-15-2026), which also supersedes SR 21-8 and rescinds four OCC/FDIC issuances and the Comptroller's Handbook MRM booklet. [[04_Knowledge_Products/Wiki_Intake/Fed_OCC_SR11-7_Model_Risk_Management_2011]] now carries a supersession banner; **five further notes reference SR 11-7 and need a currency check** before use. Successor changes: applicability narrowed to banks above $30bn; model definition tightened to three cumulative criteria (excludes arithmetic, deterministic rules, spreadsheets without embedded statistics); new third-party/vendor-model section; **explicitly non-enforceable**.

  **The finding that matters: four jurisdictions, four different answers to the AI/model boundary question.**
  - **US (SR 26-2):** exclusion by carve-out. Non-generative, non-agentic ML stays in scope; **generative and agentic AI are explicitly carved out** as "novel and rapidly evolving," pending a promised RFI. The boundary is *generative/agentic vs everything else*, not AI vs non-AI.
  - **UK (SS1/23):** inclusion by default — AI/ML as a sub-principle inside the unified framework.
  - **ECB (Guide to Internal Models, rev. 2025/26):** middle path — a first-ever dedicated ML section with supplementary expectations, ML risks integrated "**across the three lines of defence**," Internal Audit required to cover ML models at higher frequency. ⚠ Narrower scope (Pillar 1 internal models only).
  - **India:** bifurcated patchwork.

  **India's position, stated precisely.** No general-purpose binding instrument equivalent to SR 26-2 or SS1/23 exists. What exists is (a) the **RBI Draft Circular on Model Risks in Credit** (5 Aug 2024, DOR.STR.REC./21.04.048/2024-25) — **credit-scoped and still draft**, requiring Board-approved policy, Model Inventory, independent validation before deployment and annually, RMCB reporting, and review of "instances of bias or discrimination"; and (b) **FREE-AI** ¶4.4.68 (comprehensive AI system inventory with specified fields, semi-annual updates, supervisory inspection) and Recommendation 24 (AI Audit Framework — internal audit for all AI, third-party audit for high-risk, biennial framework review) — **non-binding**.

  **A rare positive for India, worth stating in P3.** FREE-AI's scope covers "increasingly autonomous AI systems" — **India includes where the US excludes.** On conceptual scope India aligns with the UK and is ahead of the US, which has carved out the fastest-moving category. India's deficit here is **bindingness, not scope**, which is a more precise and more defensible diagnosis than the corpus's usual framing.

  **Three further findings:**
  1. **The US carve-out is the strongest evidence in the corpus for [[Agentic_AI_Governance]]** as a categorically distinct governance object — a mature supervisory regime looked at agentic AI in 2026 and declined to govern it as model risk. A considered judgment, not an oversight, and arguably better evidence for structural insufficiency than any paper. Consequence: a system outside model validation is outside the independent-challenge structure validation provides ([[Human_Oversight]]).
  2. **The "names it without specifying a test" pattern now holds across two independent Indian instruments.** The draft circular requires review of bias/discrimination without stating a criterion — matching the [[Fairness]] finding exactly. Two instruments, same pattern: an observation becomes a pattern.
  3. **A candidate fifth [[Deontic_Bifurcation]] type: prospective deontic** — the draft circular is written throughout in mandatory language and binds nobody. Distinct from designed, emergent, delegated-across-documents and supervisory-expectation. Compare the DPDP commencement structure and the [[DPB]] shell. Also yields a clean **within-institution deontic gradient**: RBI_11 (complete ADICO, licence-condition Or-else) → RBI_13 (mandatory language, no Or-else, no force) → RBI_FREE_AI (recommendations, no Or-else).

  **⚠ Evidential honesty note carried into the concept.** The strongest **peer-reviewed** source (Maheshwari, *Journal of Risk Model Validation*, 16 Mar 2026) concludes existing frameworks **can** be extended to GenAI — the opposite of the structural-insufficiency thesis. The bluntest insufficiency statement ("plainly insufficient") is an industry white paper (CRISIL, Jun 2023). Any P3 claim of structural inadequacy must acknowledge that the best-quality literature currently cuts the other way; the US carve-out is the stronger argument.

  **Confirmed absences:** no HKMA, BoJ or BSP equivalent to the MAS AI MRM paper located — ⚠ stated as a search finding, not an exhaustive audit, since those regulators may use "AI governance" rather than "model risk" terminology. ⚠ The RBI draft was retrieved via an **FIDC-hosted copy**, not rbi.org.in, and its finalisation status is unconfirmed. ⚠ A "23 April 2026" date variant for SS1/23 appeared once and looks like an indexing artifact — verify before citing any 2026 amendment.

---

## Sequence Complete — all 8 prompts run and intaken (2026-08-02)

Third-pass audit closed. Cumulative additions across the eight prompts: **6 framework nodes** ([[DEPA]], [[ISO_IEC_42001]], [[Singapore_AI_Governance]], [[GDPR]] + existing), **8 institution nodes** ([[Sahamati]], [[NPCI]], [[BIS]], [[DPB]], [[DoT]], [[Ministry_of_Power]], [[Grid_India]]), **6 concept nodes** ([[Explainability]], [[Fairness]], [[Human_Oversight]], [[Contestability_Redress]], [[Proportionality]], [[Model_Risk]]), **2 method nodes** ([[Comparative_Regulatory_Analysis]], [[Coding_Reliability_Protocol]]), and 14 corpus nodes.

**Five corrections issued against pre-existing vault claims** — the audit's most valuable output, and the reason to keep running sequences like this:

1. **This document's own finding A** (evidence orphaning) — retracted; a script artifact. Real figure 10 of 247, not 195. Replaced by the genuine finding: 68 broken wikilink paths, since fixed.
2. **[[Assurance_Reuse_Gap]]** — "EU regulators accept ISO 42001-based evaluations as discharging AI Act obligations" was false. No jurisdiction anywhere recognises ISO/IEC 42001 as compliance evidence, for a structural reason (organisation-level certification vs system-level regulation).
3. **[[P4_Doctrinal_IJLIT]] benchmark framing** — "what India is missing" is wrong on Singapore, which has no binding AI instrument at all. India leads on binding force, lags on assessment methodology.
4. **[[fsQCA]] contribution claim** — IG-QCA is not novel; priority is Schlager et al. (2021), stated explicitly by Siddiki & Frantz. Second such correction after the Akbarighatar precedent.
5. **[[Power_Grid_Critical_Infrastructure_Governance]]** — "a frontier nobody has reached" is wrong; Grid-India runs production ML at national scale. Deployment ahead of governance, not absence of both.

**The cumulative thesis-level finding:** the India-lags framing collapsed on inspection three separate times (ISO 42001, Singapore, model-risk scope). **The defensible claim is not that India lags a mature international standard but that no mature international standard yet exists** — which repositions P4's redesign proposal as filling a void rather than transplanting a working model, and is corroborated by three confirmed literature white spaces (fsQCA-DPI; four-jurisdiction comparative; the missing ADM right in Indian data law).

**Outstanding, not addressed by any prompt:** CERC has no node (OQ-GRID-01, most consequential); five SR 11-7 references need currency checks; `09_Teaching` remains empty; two corpus folders still hold misfiled contents; the four Knowledge Products remain outlines rather than products.

- 2026-08-02: **Prompt 7 (methods) run and intaken. Item 4's premise was wrong, and it costs a contribution claim.** New method notes [[Comparative_Regulatory_Analysis]] and [[Coding_Reliability_Protocol]] — `08_Methods` goes from 4 notes to 6, and from the thinnest tier relative to structural weight to adequately anchored.

  **⚠ IG-QCA is not novel — priority belongs to Schlager et al. (2021).** The prompt asked whether any published study combines Institutional Grammar coding with QCA, on the assumption that none did. **One does:** Schlager, Bakkensen, Olivier & Hanlon, *Institutional Design for a Complex Commons*, **Public Administration**, 19 Jan 2021 (DOI 10.1111/padm.12715). And the field states the priority explicitly — Siddiki & Frantz's companion symposium introduction (*Public Administration* 2021, DOI 10.1111/padm.12753): **"Schlager et al.'s (2021) study is the first to use QCA to analyze institutional statements coded using the Institutional Grammar."** No subsequent IG-QCA study appears in the citation trail or on institutionalgrammar.org's published-research index.
  - **Cannot claim** first to combine IG and QCA. Cite and build on Schlager et al.; do not contest.
  - **Can claim** first application to AI governance / regulatory-institution comparison — Schlager et al. is domain-distinct (commons and public-goods governance).
  - The chapter's stated contribution (§6.4) is **substantive-configurational**, not methodological, so it survives intact. The correction bites only on framings that present IG-QCA as methodological innovation.
  - **Second contribution-claim correction of the day**, after the Akbarighatar precedent surfaced in Prompt 1 — both from the same cause: assuming novelty without searching for the incumbent. Worth treating as a standing rule: search for the incumbent before claiming a first.

  **Three corrections to the locked reliability design**, all recorded in [[Coding_Reliability_Protocol]] and flagged on [[Institutional_Grammar_IG2]]:
  1. **Terminology.** ADICO is a pre-established deductive schema, so the correct term is **Inter-Coder Agreement (ICA)**, not inter-rater reliability (Halpin 2024, AJQR). Free to fix; a methods reviewer will notice.
  2. **PRIS departs from IG field practice without saying so.** The IG 1.0 Codebook (Brady et al. 2018) specifies **simple percent agreement at ≥80%** (Basurto et al. 2010; Siddiki et al. 2011), not κ. The 20% subsample matches exactly; the κ choice does not. The departure is defensible — percent agreement doesn't correct for chance — but must be **stated and justified**, not left implicit.
  3. **κ is the wrong chance-corrected statistic for this corpus.** Cohen's κ is unstable under prevalence imbalance, and ADICO coding is exactly that — Or-else components are rare. PRIS's own P2 finding ("of 11 Rules, 0 govern citizen-facing fallback") is an extreme-skew result; κ will report poor reliability where coding is consistent. **Gwet's AC1** is the remedy, and **Schlager et al. (2021) engaged this exact kappa-vs-AC1 debate in its own reliability reporting** — following it is precedented, not idiosyncratic. Recommended: report **percent agreement + Gwet's AC1**, κ alongside only where distribution permits.

  **Calibration source located — the one this design actually needs.** **Basurto & Speer**, *Structuring the Calibration of Qualitative Data as Sets for QCA*: "Existing direct and indirect calibration techniques for quantitative data (Ragin 2008) cannot be applied to qualitative data as such data need to be coded and summarized before fuzzy-set values can be assigned." Six-step procedure built for qualitative/institutional data; settles the theoretical-vs-data-driven anchor question in favour of theory ("not on internal criteria such as the mean or the mode"). **The single most directly applicable calibration source for an IG-coded → fsQCA design.**

  **Robustness standard located.** Oana & Schneider, *A Robustness Test Protocol for Applied QCA*, **Sociological Methods & Research** 53(1) 2024 — sensitivity ranges, fit-oriented and case-oriented robustness; "test set" and "robust core"; **SetMethods** R package (an addition to the locked software list). Pair with Skaaning (2011, SMR) as foundational precedent.

  **⚠ Gap in the locked design: negation analysis.** Schneider & Wagemann's *Standards of Good Practice* (2010) requires that "the outcome and the negation of the outcome should always be analyzed in two separate analyses." The locked Design Decisions table covers all three solution types but not the negated outcome. Standard reviewer catch — add it. Also live while the 10-case list is open: Thomann (2020, SMR) on reducing limited diversity *a priori* through case selection rather than only correcting post hoc.

  **Confirmed methodological white space — and this one is load-bearing.** **No published method exists for comparing regulatory regimes where instruments differ in binding force.** The functional-equivalence literature (Michaels; Mahy; Zweigert & Kötz) addresses doctrinal difference between statutes and never treats binding-vs-advisory status as a methodological variable. Given that Prompts 3–5 established that two of P4's three benchmarks are far less binding than assumed, this is central rather than peripheral: **the warrant must be constructed, from Michaels' "similarity in difference," not cited.** Publishable in its own right. Also recorded: Michaels' own limit — functional comparison is "a weak tool for evaluating" — meaning **P4 §5's normative redesign proposal exceeds what the method licenses** and must rest on regulatory-governance theory instead. And the step-1 discipline: PRIS habitually frames the comparison legally ("how is AI governed in BFSI?") where the functional method requires a non-legal problem statement.

- 2026-08-02: **Prompt 6 (missing institutions) run and intaken.** New institution nodes [[DPB]], [[DoT]], [[Ministry_of_Power]], [[Grid_India]]; new corpus nodes [[07_Institutions/Corpus/DPB/DPB_1_Establishment_and_Vacancy_2025_2026]] and [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]]. [[BIS]] updated with the fuller LITD 30 scope. **Institution tier now 24 notes, up from 17 at the start of this audit.**

  **Two new [[Governance_Debt]] sub-patterns registered, and one domain claim corrected:**

  1. **The institutional shell — India's data-protection enforcer has no enforcers.** The Data Protection Board is constituted in law (DPDP Act s.18; Rules 17–21 in force 13 Nov 2025), its digital-first office software is built, applications were invited 6 May 2026 — and as of **31 July 2026 there is no Chairperson and no Members, and zero orders have issued**. LiveLaw: "It exists, in the strict sense, only as a statutory possibility." **The dependency nobody had flagged: Rule 4 Consent Manager registration commences 13 November 2026 and registration is with the Board.** An unstaffed Board cannot register anyone, and every substantive DPDP obligation commencing 13 May 2027 is Board-enforced. This is the **inverse of the corpus's four "institution before regulation" instances** (CSIRT-Power, the AA Directions, Sahamati, BIS) — those produced capacity ahead of authority; this produces authority with no capacity. Also a two-layer contestability gap: [[Contestability_Redress]] records DPDP creates no ADM right; this adds that the rights it *does* create have no forum.
  2. **Infrastructure-layer governance debt, now confirmed across two unrelated sectors.** [[Grid_India]] runs production ML on the national grid — day-ahead demand forecasting via ANN (Levenberg–Marquardt) and XGBoost at **2–5% MAPE**, LSTM under refinement, an IIT Kanpur AI/ML engine cleaning renewable data at a 250 MW solar plant, and a 24×7 SOC running AI-powered SIEM/UEBA/NBAD/SOAR — with no AI governance instrument reaching it. [[Ministry_of_Power]] confirmed AI/ML use in transmission maintenance in a **Rajya Sabha written reply of 18 December 2023** (parliamentary record — strongest provenance in that domain). Paired with [[NPCI]]: **India regulates AI at the regulator layer and not at the infrastructure-operator layer.** Neither operator is a "Regulated Entity" in the sense RBI FREE-AI addresses.

  **⚠ Power Grid domain claim corrected.** [[Power_Grid_Critical_Infrastructure_Governance]] recorded this as "the only domain where India tracks global peers rather than lagging — a genuine, unsolved regulatory frontier, not a capacity gap." Still true that no jurisdiction has AI-specific grid regulation; now also true that India's grid operator runs production ML at national scale. **Revised: not a frontier nobody has reached, but deployment running ahead of governance inside a designated Critical Information Infrastructure sector.** Stronger for the domain, different claim. fsQCA consequence: the logged exclusion caution stands, but because variance is near-zero on *regulation presence* while **AI deployment intensity** varies substantially — as a condition the latter would carry information. TAC design question, not grounds for exclusion.

  **⚠ Institutional-map gap surfaced: CERC.** The Power Grid domain was built with [[CEA]] and [[NCIIPC]] as anchors. **CERC — Central Electricity Regulatory Commission — is Grid-India's primary standard-setting regulator and has no node in this vault.** Unsearched. The most consequential omission left by that domain build (OQ-GRID-01).

  **Third independent telecom confirmation.** [[DoT]] — the rule-maker under the Telecommunications Act 2023, previously absent from the vault — has issued **no notification, advisory or consultation paper referencing AI, automated systems or algorithmic decision-making**. With TRAI's unenacted 2023 Recommendations and DEPA's unrealised 2020 telecom extension, that is three unrealised telecom AI announcements from three directions across six years.

  **Provenance flags:** the DPB vacancy rests on a **LiveLaw analysis of 31 July 2026**, not a government statement — re-verify before any submission, since an appointment would date the claim immediately. The Grid-India AI detail comes from a **trade publication** (*Powerline*, 31 Aug 2025) written as a first-person institutional account; **no grid-india.in whitepaper was retrieved**. A complete itemised inventory of Rules notified under the Telecommunications Act **was not compiled** — DoT's index returned no consolidated list, so the "no AI" finding is a search result rather than an exhaustive audit (OQ-DOT-01). The CEA Cyber Security in Power Sector Guidelines are referenced in the Rajya Sabha reply but **the primary text was not retrieved** — whether they reach AI/ML at all is open (OQ-GRID-03). No LITD 30 membership roster and no open draft-comment window located.

- 2026-08-02: **Prompt 5 (GDPR) run and intaken. Closes the vault's longest-standing forward reference** — `06_Frameworks/GDPR` had been a deliberate broken link since before this audit. New framework node [[GDPR]] (scoped to the ADM/AI layer, not GDPR generally); new corpus nodes [[07_Institutions/Corpus/International/International_36_CJEU_SCHUFA_C634_21]] and [[07_Institutions/Corpus/International/International_37_EDPB_AI_Opinions_and_Competence_2024_2026]].

  **Five findings:**
  1. **The India gap is a missing sub-architecture, not a missing clause.** GDPR delivers the ADM right through **four provisions** — the Art. 22(1) prohibition plus three transparency hooks (Arts. 13(2)(f), 14(2)(g), 15(1)(h)) each requiring "meaningful information about the logic involved" — plus Recital 71 and WP251 guidance. DPDP delivers none of the four. Stating it as a four-provision architecture is materially more precise than "DPDP has no Article 22," and it is now tabled in both [[GDPR]] and [[DPDP_Act_2023]].
  2. **Art. 22(1) is a prohibition, not a right — the corpus had this wrong.** Per WP251 (EDPB-endorsed 25 May 2018, never superseded) Art. 22 establishes a general prohibition on solely-automated significant decisions rather than a right requiring active invocation. [[Contestability_Redress]] previously treated it as a right; corrected in place. The prohibition reading is the stronger one for P4.
  3. **SCHUFA gives the Indian gap a concrete sectoral location.** CJEU C-634/21 (7 Dec 2023) holds a credit agency's **probability value** is itself Art. 22 decision-making where a third party draws strongly on it — the regulated moment moves upstream from lender to scorer. This lands exactly on the seam [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] identified independently: the AA regime governs the movement of data and nothing governs the inference drawn from it. **"India has no Article 22" becomes a specific claim about India's credit infrastructure.** First CJEU judgment in the corpus; second judgment overall after DHC_1, and the first that is final rather than interim.
  4. **The competence-allocation comparison is the one benchmark that survived this week.** Prompt 3 weakened the EU AI Act (zero cited harmonised standards); Prompt 4 weakened Singapore (no binding instrument at all). This one holds: the EU has a statutory allocation of supervisory competence between data-protection and AI regulators (AI Act Arts. 2(7), 74(9), 75), a joint EDPB–EDPS opinion interpreting it, and joint EDPB–Commission guidelines in preparation. India has four financial regulators plus MeitY with **zero cross-references** and no competence-allocation instrument. The EU's own allocation is imperfect — the EDPS's exclusive competence sits in recitals, not operative text — and **noting that makes the comparison credible rather than triumphalist**. Lean on this in P4 precisely because the other two had to be softened.
  5. **Third confirmed white space of the audit sequence.** No law-journal article treats the DPDP ADM absence as its primary analytical focus; the strongest sources are an IJSSHR comparative paper (Feb 2026, low-tier) and a Latham & Watkins note (12 Nov 2025) recording it as a "No-action gap." Combined with (3), **"the missing ADM right in Indian data law" is the most concrete P4 spin-off identified anywhere in this audit.**

  **Also recorded:** enforcement table — LinkedIn €310m (behavioural profiling, most significant for ADM doctrine), Clearview €30.5m (biometric), OpenAI €15m (GenAI training transparency — a distinct doctrinal category), Hamburg €492k (**explicitly algorithmic decision-making at a financial services provider — smallest fine, highest P3 relevance**). Meta €1.2bn flagged as international-transfers, **not** ADM — do not cite as ADM precedent. WP251's "solely automated excludes *meaningful* human involvement" is the only operative legal content the corpus holds for the nominal-vs-effective distinction in [[Human_Oversight]]. A new ADICO category noted: **competence-allocating rules**, entirely absent from the Indian corpus.

  **Provenance flags:** EDPB Statement 3/2024 and Guidelines 4/2019 referenced in an EDPB presentation but **no direct EDPB-hosted URL isolated** — retrieve before citing. Opinion 28/2024 dating varies across EDPB's own release (18 Dec), PDF timestamp (16 Dec) and adoption (17–18 Dec). The forthcoming joint EDPB–Commission AI Act/GDPR guidelines rest on a **LinkedIn commentary source** — the DMA–GDPR precedent is verifiable, the timeline is not; do not assert a date. No second CJEU Art. 22 judgment exists despite one source implying a line of cases. Still uncoded: the UK Data (Use and Access) Act 2025 replacement of Art. 22 (Arts. 22A–22D, in force 5 Feb 2026, SI 2026/82) — obvious next addition, noted on [[Privacy_DataProtection]].

- 2026-08-02: **Prompt 4 (Singapore MAS FEAT / Veritas / IMDA AI Verify) run and intaken.** New framework node [[Singapore_AI_Governance]]; new corpus nodes [[07_Institutions/Corpus/International/International_34_MAS_FEAT_Veritas_AI_MRM]] and [[07_Institutions/Corpus/International/International_35_IMDA_Model_Framework_AI_Verify]].

  **⚠ P4's benchmark framing corrected, and the correction compounds with Prompt 3.** [[P4_Doctrinal_IJLIT]] frames all three international benchmarks as comparators "for what India is missing" (§140, §252). On Singapore that is wrong in one direction. **Singapore has no binding AI instrument of any kind** — no statute, no AI-specific Notice or Directive, no designated AI regulator, no statutory AI definition (confirmed across three independent legal trackers, current Feb–Mar 2026). MAS issues Information Papers; RBI issues binding Master Directions. **On binding force India is ahead of Singapore.** What India lacks is Singapore's *assessment methodology*. [[Doctrinal_Analysis]] already framed this correctly as "operationalisation" — that framing is preserved and made explicit; P4's looser phrasing is the problem and has been annotated in place.

  **The cumulative finding across Prompts 3 and 4 is the important one.** Two of P4's three benchmarks are materially weaker than the corpus assumed: the EU AI Act has **zero cited harmonised standards**, so Art. 40 presumption of conformity attaches to nothing; Singapore has **no binding instrument at all**. The India-lags framing keeps collapsing on inspection. **The defensible thesis is not that India lags a mature international standard but that no mature international standard yet exists** — a stronger, more original claim that repositions P4 §5's redesign proposal as filling a void rather than transplanting a working model. Corroborated by a confirmed literature gap: no peer-reviewed study compares Singapore + India FREE-AI + EU + UK as co-equal comparators.

  **Five further findings:**
  1. **Veritas is the missing instrument class for D4.** Documents 3A (Fairness), 3B (Ethics & Accountability), 3C (Transparency) are published assessment methodologies with open-source toolkits (v1.0 2022, v2.0 2023) and seven-institution pilots. They assess the *deploying institution's process* — the level this thesis calibrates at — where SCS, XAI Trust Scale and CAS are all subject-perception scales. Added as a third D4 option in [[fsQCA]]. Caveat: Veritas closed at Phase 3 (Jun 2023) and covers neither generative nor agentic systems.
  2. **Independent corroboration of the Human Oversight weakness.** AI Verify operationalises eleven principles but runs **technical tests on only three — Fairness, Explainability, Robustness** — assessing the other eight, including Human Agency and Oversight, by process check. A testing framework built with IBM, Microsoft and Google reaches from the engineering side the conclusion [[Human_Oversight]] reached from the academic literature. Two independent routes; state as convergent evidence rather than an argument from absence.
  3. **A fourth [[Deontic_Bifurcation]] type: supervisory-expectation bindingness.** Singapore's entire regime operates on supervisory relationship rather than deontic text — MAS's FEAT and AI MRM carry de facto compulsion for regulated FIs with no de jure obligation; PDPC's guidelines carry PDPA s.49 interpretive weight while being "not legally binding." Distinct from mandatory-core-plus-advisory-annexure, designed-vs-emergent, and delegated-across-documents.
  4. **A second RL-low / SR-high fsQCA case.** Singapore (no binding instrument, highly developed assessment infrastructure) joins [[DEPA]] (never-enacted draft, operative licensed regime). Cases where RL and SR diverge carry the configurational information; both flagged for TAC.
  5. **New agentic instrument.** IMDA's Model AI Governance Framework for Agentic AI (~Jan 2026) — four pillars, pillar 2 "make humans **meaningfully** accountable" is the corpus's clearest regulatory statement of the nominal-vs-effective oversight distinction. Wired into [[Agentic_AI_Governance]]. Singapore's cross-sectoral pattern is **coherence by accretion**: traditional (2020) → generative (2024) → agentic (2026), four live voluntary frameworks, none replacing the last.

  **Also useful:** the Government of India's own **PIB comparative annex** to the India AI Governance Guidelines (4 Nov 2025) performs exactly the Singapore/EU/UK triangulation P4 needs, in the document that anchors India's own approach — citing it makes the comparison set the government's, not the researcher's construction.

  **Provenance flags:** Veritas Doc 3 retrieved via Scribd, not MAS-hosted. AI MRM date differs between MAS's page ("04 Dec 2024") and law-firm sources (5 Dec 2024). The Agentic AI framework date is not pinned (law-firm summary says Jan 2026; file timestamp 19 May 2026). An unverified LinkedIn claim that the AI MRM paper is "now fueling 2025 formal guidelines" is **not corroborated** — no MAS Notice or binding circular located; do not repeat. The FREE-AI comparator in this return came via a KPMG-hosted summary; prefer the confirmed direct RBI link already on [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]].

- 2026-08-02: **Prompt 3 (ISO/IEC 42001 + BIS) run and intaken. Item 6 resolved as a confirmed global absence, and it falsified a claim already held in the vault.** New framework node [[ISO_IEC_42001]]; new institution [[BIS]] with corpus node [[07_Institutions/Corpus/BIS/BIS_1_LITD30_and_IS_ISO_IEC_42001_Adoption]]; new corpus node [[07_Institutions/Corpus/International/International_33_CEN_CENELEC_JTC21_Harmonised_Standards_2026]].

  **⚠ Correction issued against [[Assurance_Reuse_Gap]].** That note recorded (Batch 12, from F034_Buscemi) that "EU regulators accept ISO 42001-based technical evaluations as discharging AI Act audit obligations" and that India's lack of an equivalent mapping was the gap. **This is wrong.** The European AI Office signalled in May 2024 that ISO/IEC 42001 is not aligned with the final AI Act text and is not part of the harmonisation process; the Commission's own standardisation page names CEN-CENELEC JTC 21 deliverables, not 42001, as the route to legal certainty; and AI Act Art. 40 grants presumption of conformity only to harmonised standards cited in the Official Journal, of which **zero AI-specific ones exist**. What F034 documents is a researcher-constructed verification mapping, not a recognised regulatory pathway. The claim has been struck through in place with the correction recorded beneath it rather than deleted.

  **Five findings:**
  1. **No jurisdiction anywhere recognises ISO/IEC 42001 as compliance evidence** — EU, US, UK and India all at zero. Confirmed, not merely unconfirmed by omission.
  2. **The reason is structural, not temporal: a unit-of-certification mismatch.** ISO/IEC 42001 certifies that an *organisation* runs an AI management system; the EU AI Act regulates *individual systems as products* at market placement. No crosswalk reconciles different objects of assessment. This is a stronger and more publishable finding than the India-lags claim it replaces, and it generalises beyond AI to any management-system standard meeting product regulation.
  3. **The India-lags framing must be rewritten in P4** — but a defensible comparison survives at the **accreditation** layer, where variance is real: ANAB and UKAS operate ISO 42001 accreditation schemes; **NABCB has none located**.
  4. **New sub-layer of the gap: assurance artefacts are not yet comparable to each other.** ISO/IEC 42006 — the auditor-competence standard for AIMS certification — **is not published** (UKAS confirms it is in development). Certification bodies audit under generic ISO/IEC 17021-1 with no AI-specific competence standard and no located IAF mandatory document. A certificate market is running ahead of the standard that would make its certificates comparable. Feeds [[Evidentiary_Governance]].
  5. **BIS closes a systematic blind spot.** The vault referenced ISO/IEC 42001 in 32 notes and had **zero mentions of the Bureau of Indian Standards**. PRIS is regulator-dense and standards-body-blank, while India holds a **P-membership vote in ISO/IEC JTC 1/SC 42** — a stream of revealed Indian positions on AI standards the research programme has never observed (OQ-BIS-03). India's build is *standard adopted ✅ → auditors trained ✅ → accreditation scheme ❌ → recognition ❌*: a fourth instance of the "institution before regulation" sequencing pattern, here as *capability before scheme*.

  **fsQCA consequence:** the SR calibration proposed in [[Assurance_Reuse_Gap]] ("ISO/IEC 42001 mapped to sectoral audit requirements") is **not viable** — zero variance across all cases carries no configurational information. Recalibrate SR on national accreditation-scheme existence, which does vary. Recorded on both notes.

  **Provenance flags carried into the notes:** the IS/ISO/IEC 42001 adoption is confirmed only from a BIS-hosted training brochure, not a gazette or Manakonline entry — the fact is well supported, **the date is not**. The NABCB gap is confirmed by search, not by direct site verification. The AI Office's May 2024 signal is reported via a Cloud Security Alliance note, not retrieved as a primary statement. The JTC 21 per-deliverable stages come from a third-party tracker cross-read against the Commission page. The ISO catalogue link supplied for 42001 was a generic Russian-language OBP root, not a record URL. One source in the return was a LinkedIn post; corroborated by the CSA note but not cited on its own.

  **Live window:** BIS LITD 30's **46th Sectional Committee Meeting is 5 August 2026** — three days out.

- 2026-08-02: **Prompt 2 (DEPA / Account Aggregator / NPCI) run and intaken — closes the vault's largest missing-node gap (72 referencing notes, no node).** New framework node [[DEPA]]; new corpus nodes [[07_Institutions/Corpus/RBI/RBI_11_NBFC_Account_Aggregator_Master_Directions_2016]] and [[07_Institutions/Corpus/RBI/RBI_12_ReBIT_AA_API_Specifications_2023]]; new institution [[Sahamati]] with corpus node [[07_Institutions/Corpus/Sahamati/Sahamati_1_SRO_Recognition_and_Grievance_Architecture_2026]]; new institution [[NPCI]] recording a confirmed governance absence rather than a document. [[07_Institutions/Corpus/MeitY/MeitY_4_DPDP_Rules_2025]] updated with DEPA lineage rather than duplicated.

  **Five findings:**
  1. **New pattern — "operationalisation without enactment."** DEPA was published as a *Draft for Discussion* (NITI Aayog, Aug 2020), never finalised or superseded, and never enacted — yet became operative in finance and health and was subsequently written into statute as DPDP Rules 2025 Rule 4. The RBI Master Directions implementing it **predate the document by four years**. Paired with DPDP's "enacted but not operative," this gives P4 a two-sided typology of instrument-status/reality divergence. Strongest new theoretical material from this pass.
  2. **Coherence counter-case that bounds [[Regulatory_Parallelism]].** RBI, SEBI, IRDAI and PFRDA co-authored DEPA and their four ombudsman schemes jointly form one redress chain across four regulatory perimeters without a coordinating statute. The same four regulators produce non-cross-referencing AI instruments. Same institutions, same period — this isolates the parallelism variable to subject matter, defeats the "they lack capacity" rebuttal, and simultaneously **bounds the claim**: parallelism is a property of Indian regulation *of AI*, not of Indian financial regulation generally. Written into that note as a boundary condition; an unscoped parallelism claim is now falsifiable by a reviewer who knows India Stack.
  3. **The decisive comparison for [[Contestability_Redress]].** The AA ecosystem runs a four-tier grievance architecture (automated ascertainment with compensation → participant GRO/Internal Ombudsman → **statutory** regulator ombudsman → Sahamati ODR with arbitration fallback). India has built layered, multi-forum, partly-statutory redress — for consent disputes. It has built none for automated decisions, and DPDP still has no ADM provision. The capability rebuttal is now closed off.
  4. **NPCI: confirmed absence, not a thin node.** UPI runs a federated AI fraud-detection pilot generating cross-institutional customer risk scores with **no published governance instrument of any kind** — evidence is Economic Times reporting and NPCI promotional material. No model governance, no assurance requirement, no contestability route. Governance_Debt at the infrastructure layer rather than the regulator layer, which is structurally new for the corpus.
  5. **Telecom extension confirmed absent**, independently corroborating [[Telecom_AI_Governance]]'s "vision exceeding reach" finding from the DPI side — two unrealised telecom announcements, six years apart, from two different bodies. Also: the **N.U.D.G.E. gap has been half-closed in the wrong direction** — Vidhi proposed a *user-driven* governance entity for the AA ecosystem in 2023; RBI recognised an *industry* SRO in 2026. [[Records_Rules_Asymmetry]] survives and is arguably strengthened.

  **Provenance flags carried into the notes, not resolved silently:** RBI's SRO recognition of Sahamati is sourced only from Sahamati's own announcement — no RBI-hosted notification located, so the 5 June 2026 date is secondary. The Participation Terms came via a Scribd copy and the ReBIT v2.0.0 spec via a Sahamati-hosted mirror; both flagged for canonical verification. DEPA's public-comment closing date conflicts between two near-primary sources (1 Oct vs 30 Nov 2020) and is recorded as unresolved. The RBI Master Direction is a dynamically updated page with no separate consolidated version — a citation-hazard warning is recorded on the node requiring date-stamped retrieval.

  **Unblocked:** [[DPDP_Playbook]] Ch. 4 (Consent Architecture and DEPA Alignment) — source-blocked status cleared.

- 2026-08-02: **Prompt 1 (EA-principle cluster) run and intaken — the thesis-critical-path item is now closed.** Five new Standard Concept notes created: [[Explainability]], [[Fairness]], [[Human_Oversight]], [[Contestability_Redress]], [[Proportionality]]. Following the precedent set by the Legitimacy/Deontic_Bifurcation intake in pass 1, academic references were added as **Literature Anchors** sections inside the concept notes rather than as new Corpus Nodes, since Zotero is the authoritative reference store. Regulatory operative text was recorded in-note with article-level citation, anchored to existing corpus nodes (International_18/23/24, EU_AI_Act, NCAIC_1, RBI_FREE_AI_2025, MeitY_2) rather than duplicated as new nodes.

  **Six substantive findings, each affecting a live decision:**
  1. **D4 is now resolvable.** Recommended resolution recorded in [[fsQCA]]: calibrate the EA constituents on *specification* (does the instrument name the principle, specify a test, attach a consequence) rather than on *satisfaction*. This sidesteps the fairness impossibility problem, fits an institutional-design thesis, applies uniformly across all four EA constituents, and pre-empts the "rules or reality?" reviewer question.
  2. **Fairness cannot be a scalar.** Kleinberg's impossibility theorem proves independence, separation and sufficiency criteria are mutually incompatible outside degenerate cases. Any composite EA score silently averaging over fairness embeds an undisclosed normative choice. Bell et al. (2023) show the constraint binds loosely in practice — both sides recorded.
  3. **Proportionality removed from EA and reassigned to RL.** It is a regime-level property governing how the other principles are allocated, not a system-level property. Folding it into EA would mix levels of analysis. This also formalises the risk-proportionality property that [[Transparency]] had already attributed to RL without a measurement basis.
  4. **Human Oversight is the construct-validity exposure.** No validated psychometric instrument exists — a negative finding, confirmed rather than assumed. Bespoke five-item scheme built from EU AI Act Art. 14(4); disclosed as constructed, not adopted. Direction of bias (instrument text over-estimates practice) recorded explicitly.
  5. **Akbarighatar et al. (2026), *Information Systems Frontiers* 28(1) is both the key precedent and a positioning risk.** It is the only confirmed fsQCA study applied to an RAI principle set, which removes "first configurational analysis of AI governance principles" as an available contribution framing. No fsQCA study uses any of the five constituents individually as a calibrated condition — that space remains open. Must be read before the contribution statement is finalised.
  6. **Three India-side gaps of different kinds, now separable.** Fairness = criterion gap (every instrument names it, none specifies a test; NCAIC alone names demographic parity, non-bindingly). Human Oversight = specification-density gap (EU AI Act Art. 14 has four paragraphs and five sub-conditions; India has one noun phrase). Contestability = **statutory absence** — DPDP 2023 contains no ADM provision, so there is no Indian equivalent of GDPR Art. 22(3). The third is the strongest [[Governance_Debt]] instance in the cluster and the most quotable P4 finding.

  **Source-quality corrections made during intake, not carried through silently:** the four-fifths rule was attributed by the search return to Romei et al. (2013); it originates in the EEOC *Uniform Guidelines on Employee Selection Procedures* (1978), 29 CFR §1607.4(D) — corrected in [[Fairness]]. The Barocas/Hardt/Narayanan taxonomy was returned via a LinkedIn explainer and Speicher et al. (2018) via a personal blog; both flagged for primary verification. Truncated URLs on Rangone (EJRR 2025), the Stanford policy paper, and the UNESCO ¶35(f) source flagged for verification before citation.

  **Incidental wiring:** ~35 corpus nodes were pulled into the five new notes as Instances in Corpus, several of them previously uncited from any concept — F076 (CeRAI, the corpus's only Indian-authored empirical fairness work), F079, F135, MeitY_7, International_14. Net effect on the evidence layer: 10 orphans → 8.

- 2026-08-02: **⚠ RETRACTION issued against this document's own finding A.** The reported figure of 195 orphaned evidence nodes was a script artifact — wikilink targets were matched on stem only, discarding this vault's path-style evidence citations wholesale. Corrected: 10 of 247 before today's work, 8 after. Retraction notice, corrected orphan list, corrected institution inbound counts, and a methodological note for future audits are recorded in §1 and §2. Findings B (missing nodes) and C (thin tiers) were derived by grep and filesystem inspection, were unaffected by the bug, and stand as issued. The eight Perplexity prompts are unaffected — none of them was premised on the orphan finding.

- 2026-08-02: Third-pass audit run across the tiers not covered by the two earlier passes (`07_Institutions` parents, `08_Methods`, `04_Knowledge_Products`, `09_Teaching`) plus a vault-wide missing-node detection sweep. Principal findings: (1) 195 of 246 evidence-layer nodes have zero inbound links — a wiring failure, not a sourcing one; (2) the EA-principle construct cluster (fairness/explainability/human oversight/contestability) is the most-referenced material in the vault and has no concept notes, blocking fsQCA outcome calibration; (3) DEPA (72 files), MAS FEAT (51), GDPR (41) and ISO/IEC 42001 (32) all lack framework nodes; (4) `08_Methods` is the thinnest tier relative to structural weight, with comparative regulatory analysis entirely unanchored; (5) `09_Teaching` empty, two corpus folders empty with their contents misfiled in `Wiki_Intake`. Eight Perplexity sourcing prompts generated. None run yet.
