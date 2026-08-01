---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - section/S1
  - section/S3
  - section/S5
---

# Viljanen & Parviainen: AI Applications and Regulation — Mapping the Regulatory Strata (2022) — Intake Note

**Source:** Mika Viljanen & Henni Parviainen, Faculty of Law, University of Turku
**Year:** 12 January 2022
**Full title:** AI Applications and Regulation: Mapping the Regulatory Strata
**Journal:** *Frontiers in Computer Science* (Frontiers Media S.A.)
**File ID:** F124
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S1 (Foundational Landscape), S3 (International Comparators), S5 (Data/Privacy Governance)
**Confidence:** High
**Jurisdiction:** Finland (EU member state) — GDPR/EU Charter-anchored, with two fully worked domestic case studies

---

## Classification

**Document type:** Academic paper (Original Research), peer-reviewed, *Frontiers in Computer Science*
**Primary audience:** Researcher / Regulator / Practitioner (legal advisors to AI developers/deployers)
**AI explicit:** Yes — the paper's entire subject is AI application regulation, mapped through two fully worked AI-deployment case studies.

---

## Scope Note — Why This Node Exists

The corpus's most granular single-jurisdiction doctrinal mapping of how AI applications intersect multiple independent bodies of law simultaneously. Where most of the PRIS corpus documents *cross-regulator* Regulatory_Parallelism (RBI vs. SEBI vs. MeitY), this paper documents **intra-jurisdictional regulatory layering** at a level of statutory granularity the corpus has not previously captured — a single hiring-AI deployment in Finland must simultaneously satisfy GDPR, national data-protection law, non-discrimination law, co-determination/works-council law, IP law, and criminal-liability law, each independently sourced and cited. Directly complementary to the same-batch [[04_Knowledge_Products/Wiki_Intake/F123_Sloane_Moss_Chowdhury_Hiring_Algorithms_Auditability_2021|F123]] (Sloane, Moss & Chowdhury) — both papers independently select hiring AI as their central worked example, one from an audit-practice angle, this one from a doctrinal-mapping angle.

---

## Key Findings and Framework

### The five-layer AI law stratigraphy — the paper's central, directly reusable framework

AI law is construed as five layers: (1) **data rules** (regulate data use generally — GDPR, national data-protection acts), (2) **application-specific AI rules** (target specific AI applications/domains — e.g., automated-decision-making constitutional rules), (3) **general AI rules** (apply broadly across AI applications — e.g., GDPR Art. 22 automated-decision-making provisions, EU AI Act), (4) **application-specific non-AI rules** (apply to the specific activity regardless of whether AI is used — e.g., employment law, criminal-background-check mandates), (5) **general non-AI rules** (apply generically across domains — e.g., general non-discrimination law). This is a directly reusable classification scheme for auditing India's own AI-governance instrument stack against the same five-layer structure — several of the PRIS corpus's documented "parallelism" and "coherence gap" findings can be re-read through this lens as **layer-conflation** (an instrument that should sit at layer 3 (general AI rules) instead behaves as if it were layer 2 (application-specific), or vice versa) rather than simple cross-regulator duplication. Complements [[04_Knowledge_Products/Wiki_Intake/Paladin_GI_AI_Tech_Stack_Primer|F052]]'s three-layer compute/model/application stack decomposition — a different axis of layering (technical stack vs. legal-rule stratigraphy) that could be cross-referenced in future PRIS synthesis work.

### Worked Case 1 — Recruiting people (hiring AI) in Finland

An exceptionally granular statutory mapping for a fictional 400-hire automotive-assembly recruitment scenario, citing by name and section: GDPR (lawful-basis and automated-decision-making requirements — "the employer and AI developer should ensure either that the AI recruitment system does not make automated decisions, or... the decision framework must comply with all the requirements set in the GDPR"), Finland's Data Protection Act (1050/2018), Act on Services for Electronic Communications (917/2014), Act on Protection of Privacy in Working Life (759/2004) — mandating that employers "may only collect data directly from the applicants," Security Clearance Act (726/2014), Act on Checking Criminal Background of Persons Working with Children (504/2002), Occupational Health Care Act (1383/2001), Communicable Diseases Act (1227/2016), Young Workers Act (998/1993), Aliens Act (301/2004), Act on Public Employment and Business Service (916/2012), Non-Discrimination Act (1325/2014), Act on Equality between Women and Men (609/1986), Employment Contracts Act (55/2001), Act on Co-operation within Undertakings (334/2007 — triggers mandatory co-operation negotiations for employers with 30+ staff before implementing or amending AI recruitment systems), IP statutes (Copyright/Patents/Utility Model/Trade Secrets Acts), the Finnish Criminal Code, and IEEE P7005 (Draft Standard for Employer Data Governance) as a voluntary technical standard sitting alongside the binding statutory stack. Thirteen-plus independently sourced instruments apply to a single hiring-AI deployment — the most granular single-application multi-instrument regulatory map in the PRIS corpus to date.

### Worked Case 2 — COVID-19 contact tracing (Koronavilkku)

Finland's decentralised DP-3T-design contact-tracing app, mapped against: GDPR Art. 5(1)(c) data-minimisation ("additional collection is not allowed without significant benefits"), EU Charter of Fundamental Rights proportionality requirements ("restrictions... should, in particular, be temporary... and do not continue to exist, without an adequate justification, after the crisis has passed" — European Commission 2020b), and Finland's constitutional requirement that "public authorities need a legislative basis for all administrative actions" — "Barring new laws, AI use must fit existing authorizations." A second, independently sourced worked example demonstrating the same multi-layer-stratigraphy logic applied to a public-health/public-authority AI deployment rather than a private-employer one.

### Constitutional rules on AI decision-making — the Finnish discretion-based ADM prohibition

A named 2018 incident: the Finnish Constitutional Law Committee ruled that a proposed Immigration Service automated-decision-making system was **not permitted** where "decision-making contained a discretionary element," as such automation was "incompatible with the Finnish Constitution." This is a directly citable, binding constitutional-law precedent for the general principle (already present elsewhere in the corpus in less doctrinally specific form) that ADM is permissible for rule-bound, non-discretionary determinations but constitutionally suspect where discretion is legally required — a sharper, court/committee-sourced version of the ADM-discretion distinction implicit in [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] and [[04_Knowledge_Products/Wiki_Intake/F116_Liu_Zhou_Liang_Digital_Inclusion_Vulnerable_Groups_2025|F116]]'s "automated systems... in lieu of a civil servant" definition.

### Explicit practitioner obligation — "wide-ranging surveys of legislation"

The paper's central practitioner-facing recommendation: "practitioners should conduct wide-ranging surveys of legislation when advising clients developing or using AI applications in domains unfamiliar to the practitioner," warning explicitly against analogising from a bordering domain ("relying on insights and experiences from a bordering domain could provide inadequate guidance") — a direct, citable methodological caution for PRIS's own comparative-regulatory-mapping work (P3, P4, fsQCA), reinforcing that cross-sectoral or cross-jurisdictional pattern-matching in AI governance carries a documented, named risk of superficial-analogy error.

---

## Relevance to PRIS Research

### Institutional_Coherence — layer-conflation as a refinement of the coherence-gap diagnosis

The five-layer stratigraphy offers a sharper diagnostic than the corpus's existing coherence-gap evidence: rather than simply asking whether instruments cross-reference each other, it asks whether each instrument operates at its *correct* layer. India's own AI-governance stack (MeitY's general AI guidelines, sectoral regulators' application-specific mandates, DPDP's data-layer rules, and general non-discrimination/constitutional law) can be re-coded against this five-layer scheme as a future refinement to fsQCA SR calibration.

### P4 doctrinal analysis — direct methodological template

The Case 1 (hiring) statutory-stack-mapping method is a directly transferable template for [[P4_Doctrinal_IJLIT]]'s own doctrinal analysis of India's BFSI AI-governance stack — demonstrating what a complete, granular, instrument-by-instrument regulatory map looks like for a single AI application domain.

---

## Connections

**Related concepts:** [[05_Concepts/05_Concepts_Signature/Institutional_Coherence]], [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F123_Sloane_Moss_Chowdhury_Hiring_Algorithms_Auditability_2021|F123]] (same-batch companion — shared hiring-AI worked domain, doctrinal vs. audit-practice angles), [[04_Knowledge_Products/Wiki_Intake/Paladin_GI_AI_Tech_Stack_Primer|F052]] (companion layering framework — technical stack vs. legal-rule stratigraphy), [[04_Knowledge_Products/Wiki_Intake/F032_Maas_Architectures_Global_AI_Governance_2025|F032]] (Maas's four governance-architecture archetypes — a complementary macro-level framework to this paper's micro-level five-layer stratigraphy), [[04_Knowledge_Products/Wiki_Intake/Sejwal_Gupta_ADM_Indian_Credit_Scoring_2026]] (ADM-discretion distinction, sharpened by the Finnish Constitutional Law Committee precedent)

**Related projects:** [[P4_Doctrinal_IJLIT]], [[fsQCA_Thesis_Chapter]]

---

## VERIFY Flags

**#286 — RESOLVED (2026-07-31, editorial convention).** Article-ID/DOI format in place of page numbers is standard practice for Frontiers journals, not missing pagination — no correction needed. Flag closed as already-compliant.

---

## Log

- 2026-07-16: Node created. NotebookLM Ingestion Pipeline (PROMPT 0b relay), per [[Session_Handoff_NotebookLM_Ingestion_20260715]]. Duplicate check against [[Corpus_Index_MOC]], `04_Knowledge_Products/Wiki_Intake/`, and `_Institutions_MOC.md` (searched "Viljanen," "Parviainen," "regulatory strata," "stratigraphy," "Koronavilkku") found no existing vault match — confirmed genuinely new. Classified Format B, full treatment given the paper's directly reusable five-layer stratigraphy framework and its status as the corpus's most granular single-jurisdiction multi-instrument regulatory map. One new VERIFY flag (#286). New institution row (University of Turku, Faculty of Law) added to `_Institutions_MOC.md`. "Instances in Corpus" addition to Institutional_Coherence (layer-conflation refinement).
