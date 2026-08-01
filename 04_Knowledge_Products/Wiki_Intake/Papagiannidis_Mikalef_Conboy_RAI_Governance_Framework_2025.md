---
file_id: F050
title: "Responsible Artificial Intelligence Governance: A Review and Research Framework"
authors: Papagiannidis, E., Mikalef, P., & Conboy, K.
year: 2025
outlet: "Journal of Strategic Information Systems"
outlet_rank: "A* (confirmed against full ABDC 2022 Journal Quality List text via Perplexity Deep Research, 2026-07-31 — #181 resolved)"
doi: "10.1016/j.jsis.2024.101885"
document_type: Systematic Literature Review (Scoping)
format: B
wiki_sections: [S1, S2]
tags: [responsible-AI, RAI-governance, structural-practices, procedural-practices, relational-practices, principles-to-practice-gap, AI-lifecycle, scoping-review, trustworthy-AI, AI-literacy]
corpus_cluster: Cluster_1
priority: A
project_relevance: [P1, P3, fsQCA]
date_added: 2026-06-24
batch: B15
batch_marker: ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
---

# F050 — Papagiannidis, Mikalef & Conboy (2025): Responsible AI Governance Framework
*Scoping Review — Structural, Procedural & Relational Practices*

> **Wiki Intake Note — Format B**
> Papagiannidis, E., Mikalef, P., & Conboy, K. (2025). Responsible artificial intelligence governance: A review and research framework. *Journal of Strategic Information Systems, 34*, 101885. https://doi.org/10.1016/j.jsis.2024.101885

---

## 1. Core Argument

Responsible AI (RAI) governance has remained at the level of high-level principles (fairness, accountability, transparency, etc.) without adequate operationalisation into firm-level governance practices. A significant *principles-to-practice gap* persists: adherence to responsible AI principles is systematically deprioritised during actual AI project implementation. This scoping review synthesises 48 peer-reviewed papers (from 1,080 identified) to propose a conceptual framework that defines responsible AI governance through three types of **organisational practices** — structural, procedural, and relational — and locates these within a broader causal model of antecedents and effects.

**Definition adopted**: "A set of practices for developing, deploying, and monitoring AI applications in a safe, trustworthy, and ethical manner that ensures appropriate functionality of AI over the entire lifecycle."

---

## 2. The Seven RAI Principles Synthesised

| Principle | Sub-dimensions |
|-----------|---------------|
| Accountability | Auditability; Responsibility allocation |
| Diversity, non-discrimination & fairness | Accessibility; No unfair bias |
| Human agency & oversight | Human review; Human well-being |
| Privacy & data governance | Data quality; Data privacy; Data access |
| Technical robustness & safety | Accuracy; Reliability; General safety; Resilience |
| Transparency | Explainability; Communication; Traceability |
| Social & environmental well-being | Social well-being; Environmental well-being |

The paper traces these principles primarily to the EU AI HLEG Ethics Guidelines for Trustworthy AI (European Commission, 2019) and the Singapore Model AI Governance Framework (2020). This EU/Singapore orientation is acknowledged as a limitation: the corpus is predominantly European/US-centric.

---

## 3. The Responsible AI Governance Framework

The framework organises around three causal blocks: **Antecedents → Responsible AI Governance (Practices) → Effects**, with a feedback loop ("Reshape") from effects back to antecedents.

### 3.1 Antecedents
1. **Societal norms and regulations** — Formal directives (EU AI Act) and informal norms shape which RAI principles are prioritised
2. **Organisational values** — Internal culture, path dependencies, and power structures filter which external signals are acted upon
3. **Responsible AI principles** — The operationalised set of principles the firm decides to govern toward

### 3.2 Governance Practices (Three-Type Framework)

| Practice Type | Core Activities | Key Research Gaps |
|--------------|-----------------|-------------------|
| **Structural** | AI governance committees; role/responsibility assignment; decision-making protocols; rights frameworks | How to structure vertical + horizontal governance; inter-organisational AI governance structures |
| **Procedural** | Data/model lifecycle management; compliance monitoring; incident response; strategic planning | How to translate strategic RAI intent to operational processes; harmonising competitiveness with responsibility |
| **Relational** | Cross-functional collaboration; stakeholder involvement; responsible AI literacy; external partner governance | How to develop AI literacy across levels; managing competing stakeholder interests; sourcing/contracting for RAI |

### 3.3 Effects
- **Organisational level**: Legitimacy in broader ecosystems; customer trust; ESG reputation; competitive advantage
- **Individual level**: Reduced AI-induced anxiety; higher job satisfaction and organisational commitment
- **Societal level**: Dynamic social evaluation of AI offerings; feedback into regulatory/normative evolution

---

## 4. Methodological Profile

| Parameter | Detail |
|-----------|--------|
| Review type | Scoping review (Paré et al., 2015; Arksey & O'Malley, 2005) |
| Search period | Data collection Nov 2022; refined Dec 2023 |
| Initial records | 1,080 |
| Final corpus | 48 peer-reviewed papers |
| Databases | Scopus, BSC, Emerald, T&F, Springer, Web of Knowledge, ABI/Inform, IEEE Xplore, AIS, ScienceDirect, JSTOR, Google Scholar |
| Inclusion scope | AI in organisational context; 2017 onwards; English; peer-reviewed journals |
| Exclusion scope | Technical AI papers (architecture, benchmarking); book chapters; pre-prints |

---

## 5. Critical Assessment for PRIS

### Strengths
- Most comprehensive synthesis of firm-level RAI governance practices in IS literature as of 2025
- The structural-procedural-relational typology (derived from Van Grembergen et al., 2004; Tallon et al., 2013) provides a rigorous IS governance vocabulary
- 14 structured research questions provide a gap map for P1's research agenda
- JSIS venue provides strong publication-quality endorsement for the framework

### Limitations (acknowledged)
1. **Predominantly EU/US corpus**: Principles and frameworks are Western-normative; limited applicability to BFSI contexts in India or Asia-Pacific without contextualisation
2. **Firm-level scope**: The framework addresses *intra-organisational* governance only; does not address multi-regulator, inter-agency, or ecosystem-level AI governance — precisely the domain of P3 and the Regulatory Parallelism research
3. **Conceptual only**: "Our arguments and assumptions must be tested empirically" — no empirical validation presented
4. **Static principles set**: The seven principles are EU HLEG-derived; the framework does not address how organisations navigate *conflicting* regulatory mandates from different jurisdictions

---

## 6. PRIS Concept Connections

### [[Governance_Debt]]
F050 provides the **eighth documented Governance_Debt variant** in the Batch 15 corpus: **principles-adoption-without-operationalisation** as governance debt at the organisational level. The "principles-to-practice gap" — where RAI principles exist as policy artefacts but are systematically deprioritised during AI implementation — is structurally identical to the espoused-theory vs theory-in-use gap documented in →[[04_Knowledge_Products/Wiki_Intake/Butler_Brooks_Operational_Risk_Paradigm_Change_2024]] (Butler & Brooks). The distinction is level of analysis: Butler & Brooks locate GD at the risk management execution layer; Papagiannidis et al. locate it at the AI project governance layer. Together they constitute a multi-layer account of governance debt in BFSI AI deployment.

### [[Governance_Capacity]]
The relational practice of "responsible AI literacy" is the most direct treatment of [[Governance_Capacity]] in the corpus to date: it frames the competency-building challenge explicitly as a prerequisite for effective RAI governance. The paper identifies "what skills and competencies employees at different roles and levels need to be equipped with" as a critical open question — affirming that governance capacity deficits are not peripheral but structurally constitutive of the RAI implementation problem.

### [[Accountability]]
Accountability is treated as both a RAI principle (auditability + responsibility allocation) and a governance practice design challenge. The paper's identification of "who is accountable for a judgment made by an AI system" as multilayered and difficult to resolve is the IS research community's articulation of the accountability gap documented at the regulatory level in the EU AI Act (→[[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]]).

### [[Transparency]]
The paper provides the most granular operationalisation of transparency in the corpus: explainability (technical process intelligibility), communication (right to know when interacting with AI), and traceability (data/algorithm documentation chain). These three sub-dimensions provide a more actionable vocabulary than the generic "transparency" language in most regulatory instruments, including RBI FREE-AI (→International_6).

### [[Legitimacy]]
The effects dimension explicitly models legitimacy as an outcome of RAI governance: "organisations that apply responsible AI governance... are often perceived as more reliable and trustworthy business partners." This is an IS research-grounded confirmation of the legitimacy-as-governance-outcome logic that underpins the DiMaggio & Powell institutional framework (→[[04_Knowledge_Products/Wiki_Intake/RAND_GovAI_AI_Incident_Reporting_Institutional_Design]], to be processed).

### [[Regulatory_Parallelism]]
The firm-level scope of this framework is simultaneously its key gap for P3: the framework assumes a single regulatory environment and single organisational actor. Real BFSI AI governance in India involves multiple simultaneous regulatory mandates (RBI + SEBI + IRDAI + MeitY + DPDPA), each potentially specifying different structural/procedural/relational requirements. The framework provides no mechanism for navigating this multi-mandate complexity — establishing that the "multi-regulator operationalisation gap" is a genuine research contribution of P3.

---

## 7. Research Project Applications

### P1 — AI Governance SLR
- F050 is a *primary synthesis source* for the P1 literature review — the structural-procedural-relational typology should be foregrounded as a competing or complementary framework to any synthesis framework P1 produces. The 48-paper corpus (search: Nov 2022 / Dec 2023) can be treated as the pre-P1 baseline; any P1 synthesis must either build on or critically differentiate from this framework.
- The 14 research questions in Table 5 provide a ready gap-map for the P1 research agenda section.

### P3 — BFSI AI Governance Regulatory Parallelism (JEIM)
- The framework's firm-level limitation is P3's opening. P3's contribution: extending Papagiannidis et al.'s intra-organisational framework to the **inter-regulatory and ecosystem level**, specifically addressing how BFSI firms in India navigate structural/procedural/relational governance under simultaneous RBI + SEBI + IRDAI mandates.

### fsQCA (Thesis Chapter)
- The antecedents model (societal norms + org values + RAI principles → governance practices → legitimacy/ESG outcomes) provides a candidate causal pathway for fsQCA condition selection. Specifically: "societal regulatory pressure" (coercive isomorphism), "organisational AI capability" (governance capacity), and "structural practice maturity" could serve as fsQCA conditions calibrated against legitimacy or AI governance quality as the outcome.

---

## 8. Key Quotations

> "Adhering to responsible AI principles is generally deprioritized or considered an ancillary task during the actual implementation and management of AI projects." *(p. 2)*

> "A significant challenge exists in translating theoretical principles into practical implementation approaches." *(p. 2)*

> "Responsible AI governance relies on collaboration between firms and individuals who comprise the system and extends beyond a single company." *(p. 6)*

> "There is limited knowledge concerning how organizational path dependencies, culture, and other internal factors influence an organization's ability to be receptive and adaptive to such signals." *(p. 11)*

---

## 9. AI Governance Wiki Classification

| Field | Classification |
|-------|---------------|
| **Primary Wiki Section** | S1 — Governance Fundamentals (RAI governance framework, principle operationalisation) |
| **Secondary Wiki Section** | S2 — Regulatory Frameworks (EU AI HLEG synthesis; Singapore MAS framework cited) |
| **Instrument Type** | Systematic Literature Review — Conceptual Framework |
| **Jurisdiction** | Global (EU/Singapore-primary; Western-normative) |
| **AI Governance Maturity** | Framework synthesis + research agenda |

---

## 10. VERIFY Flags

- **#181 — RESOLVED (2026-07-31, Perplexity Deep Research against full ABDC 2022 Journal Quality List text).** *Journal of Strategic Information Systems* confirmed **A\*** — High confidence. Strengthens rather than weakens the "strong publication-quality endorsement" note in Section 5 above.

---

## 11. Citation

Papagiannidis, E., Mikalef, P., & Conboy, K. (2025). Responsible artificial intelligence governance: A review and research framework. *Journal of Strategic Information Systems, 34*, 101885. https://doi.org/10.1016/j.jsis.2024.101885

**Linked nodes**: [[04_Knowledge_Products/Wiki_Intake/F037_WEF_Capgemini_AI_Agents_Evaluation_Governance]] [[04_Knowledge_Products/Wiki_Intake/Butler_Brooks_Operational_Risk_Paradigm_Change_2024]] [[04_Knowledge_Products/Wiki_Intake/RAND_GovAI_AI_Incident_Reporting_Institutional_Design]] [[Governance_Debt]] [[Governance_Capacity]] [[Accountability]] [[Transparency]] [[Legitimacy]] [[Regulatory_Parallelism]] [[Institutional_Coherence]]

---
*Batch 15 — PRIS Corpus Intake | Processed: 2026-06-24*
