---
type: Process Document
status: active
last_updated: 2026-08-02
tags:
  - type/process-document
  - status/active
  - engine/phd
---

# Thin-Node Analysis & Perplexity Sourcing Prompts — 2026-08-02

**Method:** Ranked every node in `03_Domains/`, `05_Concepts/`, `06_Frameworks/` on two axes — word count (depth of synthesis) and count of wikilinks to `07_Institutions/` (evidentiary grounding, per the PRIS hierarchy: Evidence → Concepts/Domains). A node with high word count but few institution-links is *argued but not anchored*; a node with low word count is under-developed regardless.

**Parent:** [[AI_Governance_Wiki]] | [[PRIS_Corpus_Intake_Prompts]]

---

## 1. Thin-Node Ranking

### Domains (9 total)

| Node | Words | Evidence links | Status | Read |
|---|---|---|---|---|
| Healthcare_Governance | 489 | 1 | `status/stub` | Already actioned — candidate sources logged 2026-07-31, not yet intaken |
| Privacy_DataProtection | 1,184 | 2 | active | **Thin** — core to your research, under-anchored |
| DPI_Governance | 1,177 | 3 | active | **Thin** |
| BFSI_Governance | 1,289 | 3 | active | **Thin** — feeds P3/JEIM directly |
| Cybersecurity_Governance | 1,544 | 4 | active | Moderate |
| AI_Governance | 1,616 | 5 | active | Moderate — but this is your flagship domain; 5 institution-links is low for its centrality |
| Judicial_Governance | 2,062 | 8 | active | Adequate |
| Systemic_Regulatory_Governance | 4,392 | 17 | active | Well-anchored |
| International_Comparators | 1,522 | 22 | active | Well-anchored (link-dense) |

### Concepts (13 total)

| Node | Words | Evidence links | Tier | Read |
|---|---|---|---|---|
| Legitimacy | 2,707 | 4 | Standard | **Thin** — lowest evidence density of any concept note |
| Deontic_Bifurcation | 1,084 | 5 | Signature | **Thin** — shortest signature construct; needs more empirical grounding before it can carry weight in fsQCA/IG2.0 work |
| Assurance_Reuse_Gap | 1,298 | 7 | Standard | Moderate |
| Records_Rules_Asymmetry | 4,488 | 8 | Signature | Adequate |
| Agentic_AI_Governance | 4,707 | 8 | Standard | Adequate given topic's fast-moving nature |
| Retention_Horizon_Divergence | 2,164 | 9 | Standard | Adequate |
| Transparency | 3,162 | 11 | Standard | Well-anchored |
| Evidentiary_Governance | 3,165 | 12 | Signature | Well-anchored |
| Accountability | 4,093 | 14 | Standard | Well-anchored |
| Governance_Capacity | 5,566 | 24 | Standard | Well-anchored |
| Institutional_Coherence | 5,699 | 33 | Signature | Well-anchored |
| Governance_Debt | 5,334 | 37 | Signature | Well-anchored |
| Regulatory_Parallelism | 6,063 | 51 | Signature | Best-anchored node in the vault |

### Frameworks (10 total)

| Node | Words | Evidence links | Read |
|---|---|---|---|
| OECD_AI_Principles | 1,059 | 0 | **Thin** — no primary-source anchoring at all (no institution links, no URLs) |
| UNESCO_Recommendations | 1,096 | 0 | **Thin** — same gap |
| NIST_AI_RMF | 1,125 | 0 | **Thin** — same gap |
| DPDP_Act_2023 | 1,763 | 1 | **Thin** — this is India's central data-protection statute and should be one of your best-anchored nodes, not one of the weakest |
| IndiaAI_Framework | 1,173 | 2 | Moderate |
| EU_AI_Act | 1,356 | 2 | Moderate |
| RBI_Free_AI | 1,279 | 3 | Moderate |
| SEBI_AI_Circular | 1,426 | 3 | Moderate |
| Manifestation_Evidence_Layer | 710 | 3 | Moderate (short but is a meta-framework, not primary-source dependent) |
| Cross_Regulator_Coordination_Pattern_Matrix | 2,251 | 14 | Well-anchored |

**Bottom line:** the international soft-law frameworks (OECD, UNESCO, NIST) and DPDP — arguably your single most important statute — carry zero to one primary-source anchor each. That's the highest-value gap to close. Among Domains, Privacy_DataProtection, DPI_Governance, and BFSI_Governance are thin relative to their strategic weight. Among Concepts, Legitimacy and Deontic_Bifurcation are thinnest.

---

## 2. Perplexity Deep Research Prompts

Each prompt below follows the pattern already used for `Healthcare_Governance` (2026-07-31): request confirmed, dated, linked primary sources only — no synthesis, no fabrication. Output format matches what can be pasted straight into the node's "Candidate Sources" section, then run through [[PRIS_Corpus_Intake_Prompts]] (Prompt 1/2/3) for actual vault intake.

---

### PROMPT — DPDP Act 2023 (Framework, highest priority)

```
I am building a research corpus on India's Digital Personal Data Protection Act 2023 and its implementing rules. I need primary-source documents only — no commentary, no law-firm summaries unless they are the only available secondary gloss on an unpublished draft rule.

Find and list, with exact title, issuing body, date, and direct link:
1. The DPDP Act 2023 itself (official Gazette text) and any subsequent amendments
2. The DPDP Rules (draft and/or final, whichever is current as of your search date) issued by MeitY
3. Any Data Protection Board of India (DPB) procedural notifications, orders, or guidance issued to date
4. MeitY FAQs, explanatory memoranda, or official clarifications on the Act
5. Any sectoral regulator circulars (RBI, SEBI, IRDAI) that explicitly cross-reference DPDP compliance obligations
6. Comparative regulatory impact assessments or parliamentary standing committee reports on the Act, if publicly available

For each item confirm: exact publication date, issuing authority, and a working link. Flag anything superseded or draft-only. Do not summarize content — I will read and code these myself.
```

---

### PROMPT — OECD AI Principles (Framework)

```
I am building a research corpus on the OECD AI Principles (2019, updated 2024) and need primary and near-primary sources to anchor a vault node that currently has none.

Find and list, with exact title, issuing body, date, and direct link:
1. The original OECD AI Principles (2019) full text and the 2024 revision/update
2. OECD.AI Policy Observatory implementation reports or country reviews that specifically assess adoption of these Principles
3. Any G20 AI Principles documents (which formally adopted the OECD Principles) and their official text
4. OECD working papers or secretariat reports analyzing implementation gaps across member states
5. Any India-specific OECD engagement documents (India is not an OECD member but participates in OECD.AI) — flag if none exist

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — UNESCO Recommendation on the Ethics of AI (Framework)

```
I am building a research corpus on the UNESCO Recommendation on the Ethics of Artificial Intelligence (2021) and need primary and implementation-tracking sources to anchor a vault node that currently has none.

Find and list, with exact title, issuing body, date, and direct link:
1. The full official Recommendation text (2021) adopted by the General Conference
2. UNESCO's Readiness Assessment Methodology (RAM) and Ethical Impact Assessment (EIA) tools published to operationalize the Recommendation
3. Any UNESCO country-level implementation or readiness assessment reports, particularly for India or comparable jurisdictions (Brazil, South Africa, Indonesia)
4. UNESCO progress reports or reviews on global adoption of the Recommendation since 2021
5. Any formal critiques or academic assessments of the Recommendation's enforceability, published in policy or IS journals

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — NIST AI Risk Management Framework (Framework)

```
I am building a research corpus on the NIST AI Risk Management Framework (AI RMF 1.0, 2023) and its companion materials, and need primary sources to anchor a vault node that currently has none.

Find and list, with exact title, issuing body, date, and direct link:
1. NIST AI RMF 1.0 (January 2023) full text
2. The NIST Generative AI Profile (companion to the RMF, 2024)
3. NIST's AI RMF Playbook and any updates to it
4. Any NIST crosswalks mapping the AI RMF to other frameworks (ISO/IEC 42001, EU AI Act) — these are especially valuable for comparative/fsQCA work
5. GAO or other US federal oversight reports assessing agency adoption of the AI RMF
6. Any published comparative analyses of NIST AI RMF vs India's IndiaAI/RBI FREE-AI approach

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — Privacy & Data Protection Domain

```
I am building out a Domain-level research node on Privacy and Data Protection governance (India-centric, with comparative angle) that is currently thin on primary evidentiary sources (only 2 institution-level anchors against 1,184 words of synthesis).

Find and list, with exact title, issuing body, date, and direct link, primary sources not yet likely to be in a standard India AI-governance corpus:
1. Data Protection Board of India (DPB) — any published orders, procedural rules, or public statements to date
2. MeitY notifications specifically on data localisation, cross-border transfer rules, or Significant Data Fiduciary criteria under DPDP
3. RBI data localisation directions (2018 circular and any subsequent clarifications) as they interact with DPDP
4. Comparative privacy-regulator documents: EU GDPR enforcement decisions relevant to AI/automated processing, or Singapore PDPA/California CCPA-CPRA materials useful for comparative regulatory-configuration analysis
5. Academic or think-tank (CIS, IFF, Vidhi) publications specifically analyzing India's privacy-AI governance intersection, published 2023 onward

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — Digital Public Infrastructure (DPI) Governance Domain

```
I am building out a Domain-level research node on Digital Public Infrastructure (DPI) governance in India (Aadhaar, UPI, Account Aggregator, and emerging AI-DPI integration) that is currently thin on primary evidentiary sources (only 3 institution-level anchors against 1,177 words of synthesis).

Find and list, with exact title, issuing body, date, and direct link:
1. UIDAI circulars or policy documents on AI/automated decision-making use in Aadhaar authentication (2024 onward)
2. NPCI/RBI documents on AI governance in UPI or Account Aggregator ecosystem
3. MeitY's official DPI strategy or India Stack governance documents that explicitly address AI or algorithmic accountability (not just general data governance)
4. Any global DPI governance comparative material — World Bank, UNDP, or Modular Open Source Identity Platform (MOSIP) publications addressing AI governance within DPI stacks
5. Academic papers (2023 onward) analyzing DPI governance as an institutional/regulatory design problem, particularly any using comparative or fsQCA-style methods

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — BFSI (Banking, Financial Services, Insurance) AI Governance Domain

```
I am building out a Domain-level research node on AI governance in India's BFSI sector — this directly feeds a doctoral research stream (P3/BFSI-JEIM) — and it is currently thin on primary evidentiary sources (only 3 institution-level anchors against 1,289 words of synthesis).

Find and list, with exact title, issuing body, date, and direct link:
1. RBI's FREE-AI framework/report and any subsequent RBI circulars operationalizing it
2. IRDAI circulars or guidance specifically on AI/ML use in insurance underwriting, claims, or fraud detection
3. SEBI circulars on AI/ML in trading, advisory, or market surveillance beyond what may already be coded (SEBI AI/ML reporting circulars, AI Responsibility Board memo)
4. Any RBI/IRDAI/SEBI joint or coordinated statements on AI governance — useful for coordination-pattern analysis
5. Comparative BFSI AI-governance material: MAS (Singapore) FEAT principles, UK FCA/PRA AI guidance, or US banking-regulator (OCC/Fed) AI risk guidance — for comparative regulatory-configuration analysis
6. Big 4 or industry-body (IBA, IIB) reports specifically on AI governance maturity in Indian BFSI, published 2024 onward

For each item confirm exact date, issuing body, and working link. Do not summarize — I will read and code these myself.
```

---

### PROMPT — Legitimacy (Concept)

```
I am developing a Concept-level node on "Legitimacy" as it applies to AI/regulatory governance institutions — this is a recurring theoretical construct in my research but currently has the lowest evidentiary density of any concept note in my corpus (4 institution-anchors against 2,707 words).

Find and list, with exact title, author/issuing body, date, and direct link:
1. Foundational and recent (2020 onward) Information Systems / public-administration journal articles operationalizing "institutional legitimacy" or "regulatory legitimacy" in the context of algorithmic/AI governance
2. Any empirical studies measuring public or stakeholder legitimacy perceptions of AI regulators or AI regulatory instruments (survey-based or discourse-analytic)
3. Government Information Quarterly, Regulation & Governance, or comparable ABDC-A journal articles specifically using "legitimacy" as a dependent or moderating construct in regulatory-design studies
4. Any Indian-context studies (or with Indian AI/DPI regulators as case subjects) addressing perceived legitimacy of regulatory bodies

For each item confirm exact date, author/venue, and working link (DOI where available). Do not summarize findings — I will read and code these myself.
```

---

### PROMPT — Deontic Bifurcation (Signature Concept)

```
I am developing a signature theoretical construct — "Deontic Bifurcation" — describing the split between mandatory ("must/shall") and advisory ("should/may") obligations within a single regulatory instrument, and its governance consequences. This is currently my shortest signature-concept node (1,084 words, 5 institution-anchors) and needs more empirical grounding before it can carry weight in Institutional Grammar 2.0 / fsQCA work.

Find and list, with exact title, author/issuing body, date, and direct link:
1. Institutional Grammar / Institutional Grammar 2.0 (Crawford & Ostrom; Frantz & Siddiki; Ostrom) papers that explicitly theorize the deontic component (Aim, Deontic, Object) of ADICO syntax — especially any that address mixed-deontic instruments
2. Regulatory-design literature (Regulation & Governance, Law & Policy) analyzing "hybrid" or "differentiated" regulatory instruments that combine binding rules with soft guidance in the same document
3. Empirical studies coding deontic modality (must/shall vs should/may) in regulatory text — any NLP/computational-linguistics papers doing this at scale would be especially useful as a methods reference
4. Any Indian regulatory instruments (RBI, SEBI, MeitY) that have been academically analyzed specifically for their internal deontic-mixing (mandatory core + advisory annexures)

For each item confirm exact date, author/venue, and working link (DOI where available). Do not summarize findings — I will read and code these myself.
```

---

## 3. Recommended Sequence

1. Run the **DPDP Act 2023** prompt first — highest strategic priority, lowest excuse for being thin.
2. Run the three international-framework prompts (OECD / UNESCO / NIST) as a batch — same shape of gap, same fix.
3. Run **BFSI Governance** next — it feeds active doctoral output (P3/JEIM) directly.
4. Run **Privacy_DataProtection** and **DPI_Governance** together — both India-centric domains with similar gap profile.
5. Run **Legitimacy** and **Deontic_Bifurcation** last — concept-level, lower urgency, but Deontic_Bifurcation matters if you're using it in the IG2.0/fsQCA chapter this cycle.

Paste each Perplexity response back into this conversation (or a fresh Cowork session) with the vault MCP active, and I'll classify + write candidate-source tables into the corresponding node under a "Candidate Sources — Confirmed but Not Yet Intake" heading, matching the Healthcare_Governance precedent — then queue for actual intake via [[PRIS_Corpus_Intake_Prompts]].

---

## Log

- 2026-08-02: Thin-node analysis run across Domains/Concepts/Frameworks; 9 Perplexity sourcing prompts generated.
- 2026-08-02: DPDP Act prompt run and intaken. Results closed the framework's evidence gap: new corpus nodes [[07_Institutions/Corpus/MeitY/MeitY_8_DPDP_Act_2023]] (Act + commencement + DPB-establishment notifications) and [[07_Institutions/Corpus/Parliament/Parliament_1_Standing_Committee_48th_Report_2023]] (new Parliament institution folder). [[06_Frameworks/DPDP_Act_2023]] now has 2 corpus-node anchors instead of 1. Skipped low-reuse items (DPBI recruitment notice, unverified Explanatory Note link, superseded draft Rules) per PRIS evidence-threshold rule. Remaining prompts (Privacy_DataProtection/DPI_Governance/BFSI_Governance/Legitimacy/Deontic_Bifurcation) still queued.
- 2026-08-02: Privacy_DataProtection and DPI_Governance prompts run and intaken together. New corpus nodes: [[07_Institutions/Corpus/RBI/RBI_10_Storage_Payment_System_Data_2018]] (2018 payment-data localisation — intra-India blanket-vs-conditional contrast against DPDP Rule 15), [[07_Institutions/Corpus/UIDAI/UIDAI_1_Circular_8_2025_Data_Vaults_HSM]] (new UIDAI corpus folder, secondary-sourced, flagged for verification), [[07_Institutions/Corpus/International/International_25_World_Bank_DPI_Development_2025]] (consolidates 5 comparative DPI sources under one node per evidence-reuse threshold). Both domain notes went from 0 to 3+ linked corpus nodes. Confirmed gaps logged: no DPB orders yet, no SDF criteria notified, no cross-border restriction list issued, no fsQCA-DPI paper exists (genuine white space), no MOSIP self-published AI-governance doc. GDPR enforcement fines and UK DUA Act noted as reuse material for the still-unbuilt GDPR framework node.
- 2026-08-02: Legitimacy and Deontic_Bifurcation prompts run and intaken. Unlike the Domain/Framework batches, these are academic-literature citations (Suchman, Grimmelikhuijsen, Martin & Waldman, Crawford & Ostrom, Frantz & Siddiki, the Rangoni/Levi-Faur/Verhoest fsQCA-trust precedent, etc.) rather than institutional primary sources — added as "Literature Anchors" sections directly in the concept notes rather than as Corpus Nodes, consistent with Zotero being the authoritative reference store (per PRIS custom instructions) rather than duplicating a bibliography inside Obsidian. Confirmed three genuine original-contribution gaps: (1) no legitimacy-perception study exists for any Indian AI/DPI regulator specifically; (2) no NLP deontic-modality study has been applied to regulatory instruments (only contracts) — directly actionable using PRIS's own 18-instrument/450-RU ADICO corpus; (3) no peer-reviewed paper analyzes any Indian regulator's deontic-mixing architecture — SEBI's own Master-vs-Advisory Circular taxonomy is strong primary evidence of *designed* (not just emergent) bifurcation and was added as a new "Instances in Corpus" entry, distinguishing designed from emergent bifurcation for the first time in this concept note.
- **All 9 originally queued prompts now run and intaken (DPDP, OECD, UNESCO, NIST, Privacy_DataProtection, DPI_Governance, BFSI_Governance, Legitimacy, Deontic_Bifurcation). Sourcing pass complete.**
- 2026-08-02: BFSI_Governance prompt run and intaken. New corpus nodes: [[07_Institutions/Corpus/SEBI/SEBI_19_AI_ML_Consultation_Paper_2025]] (SEBI's shift toward risk-tiered AI governance) and [[07_Institutions/Corpus/IRDAI/IRDAI_3_Fraud_Monitoring_Framework_2025]] (both secondary-sourced, flagged for verification). Updated [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] with confirmed direct RBI link, the 7-instrument operationalizing-recommendations list (none yet implemented), and the confirmed RBI/SEBI/IRDAI non-coordination finding. Domain note went from 0 to 3 linked corpus nodes. This domain already had strong existing synthesis (Regulatory_Parallelism/Governance_Debt empirical base) — new material corroborates rather than restructures it. International comparator finding: UK/US moving toward technology-neutral/exclusionary AI postures while Singapore MAS and (eventually) RBI FREE-AI trend more prescriptive — useful for P3/fsQCA regulator-stance comparison.
- 2026-08-02: OECD/UNESCO/NIST prompts run and intaken together. New corpus nodes [[07_Institutions/Corpus/International/International_23_OECD_AI_Principles_2019_2024]] and [[07_Institutions/Corpus/International/International_24_NIST_AI_RMF_2023]]. Discovered that [[07_Institutions/Corpus/International/International_18_UNESCO_Recommendation_Ethics_AI_2021]] already existed but was never linked from its own parent framework note — fixed, no new node needed there. All three framework notes (OECD_AI_Principles, UNESCO_Recommendations, NIST_AI_RMF) went from 0 linked corpus nodes to 1 each. Flagged: India's UNESCO RAM status conflict ("In Process" tracker vs. "launched" 2026 press coverage); confirmed open research gap on NIST-vs-IndiaAI/FREE-AI comparative study; GAO-25-107933 and a Dec-2023 GAO report need direct GAO.gov verification before citing. Also added confirmed primary links to RBI_FREE_AI_2025 and MeitY_2 (both previously unlinked/unverified) as incidental finds from the NIST prompt's India-comparator search. Remaining queued: Privacy_DataProtection, DPI_Governance, BFSI_Governance, Legitimacy, Deontic_Bifurcation.
