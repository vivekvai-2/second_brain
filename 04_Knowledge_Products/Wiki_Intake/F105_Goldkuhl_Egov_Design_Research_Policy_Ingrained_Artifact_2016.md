---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - section/S6
  - section/S7
  - project/p2
---

# Goldkuhl: E-Government Design Research — Towards the Policy-Ingrained IT Artifact (2016) — Intake Note

**Source:** Göran Goldkuhl, Linköping University
**Year:** 2016 (available online 14 June 2016; received 1 July 2015; accepted 22 May 2016)
**Full title:** E-government design research: Towards the policy-ingrained IT artifact
**File ID:** F105
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S6 (Implementation & Governance Artifacts) / S7 (Research Methods)
**Confidence:** High
**Jurisdiction:** Method-general (Swedish social-welfare case illustration)

---

## Classification

**Document type:** Academic paper — design-research methodology (Elsevier, *Government Information Quarterly*)
**Primary audience:** Researcher
**AI explicit:** No — zero AI-governance content. Admitted under the same scope exception already established for [[04_Knowledge_Products/Wiki_Intake/Frantz_Siddiki_Institutional_Grammar_2_2021|F056]]/F087/F095/F096/F097/F099 (pure-methods/theory papers with no AI content, captured when they materially serve an active PRIS need — here, P2's DPI governance-design methodology).

---

## Scope Note — Why This Node Exists

No AI-governance subject matter. Added opportunistically because its core construct — the **policy-ingrained artifact** — is directly transferable analytical vocabulary for P2 (DPI Governance): an IT artifact that has legal/regulatory policy built into its structure and operation, illustrated by a Swedish social-welfare multi-query application whose security mechanisms mechanically enforce a policy rule (users may only query households with *open* welfare cases). This is a pre-AI, e-government-era articulation of exactly the "policy embedded in system design" phenomenon PRIS's AI-governance work (and the AEGIS_OS consulting inbound's runtime-enforcement thesis) addresses for AI systems specifically — worth noting as a light conceptual precedent, not a forced link.

---

## Key Findings and Framework

### The policy-ingrained artifact — core construct

An IT artifact is "policy-ingrained" when public policy (defined broadly — "laws, regulations, policy/strategy declarations, workpractice goals and other value-statements") is directly built into its design and operation, not merely referenced by it. The worked example: a multi-query application built for Swedish municipalities' social welfare administration contains security mechanisms that mechanically prevent users from querying data on households whose welfare case is not currently open — the eligibility *policy* is enforced by the *system*, not just documented alongside it.

**Direct P2 relevance:** this is a citable, named construct for describing DPI systems (Aadhaar, UPI, Account Aggregator) that encode eligibility, consent, or purpose-limitation rules directly into their technical architecture rather than leaving them to downstream administrative discretion.

### Three EgovDR design principles

1. **The policy principle** — design must be explicitly grounded in an analysis of the relevant policies (legal acts, regulations, policy declarations, institutional values) to produce a policy-ingrained artifact.
2. **The co-design principle** — the workpractice and the IT artifact must be analysed, designed, and evaluated together, not sequentially or independently.
3. **The theorizing principle** — design research must produce explicit theoretical results in parallel with the design process; "Design research must include theorizing otherwise it cannot be distinguished from plain design."

### Institutional dimensions of e-government (Table, drawing on Scott 2014 / Gronow 2008)

Five inter-related aspects of institutions relevant to e-government design: **regulative** (which rules to follow), **normative** (which values to aim at), **cognitive-linguistic** (how to conceive of and talk about things), **performative** (how to conduct work), **relational** (what roles exist). A directly reusable five-dimension taxonomy for coding institutional content in DPI governance documents — complementary to, though independently derived from, PRIS's own Institutional Grammar 2.0 (ADICO) coding approach.

### Assessment finding — most e-government "design research" isn't

Of 553 sampled e-government papers, only 53 showed any design-research orientation, and only **4** fully met Hevner et al.'s (2004) design-research criteria. Of those four, only two (Robertson 2008; Saleem et al. 2008) fully met the paper's own Policy and Co-design principles, and none fully met the Theorizing principle. A citable methodological-rigor baseline: even in a field explicitly about designing government IT systems, design research meeting recognised DR criteria — let alone principles adequate for capturing the policy dimension — is rare.

### DSRM vs. EgovDR comparison (Table 1)

Maps Peffers et al.'s (2008) six-stage Design Science Research Methodology onto Goldkuhl's four-part EgovDR model: problem identification → workpractice analysis + theorizing; define objectives → policy analysis; design/development → workpractice+IT co-design; demonstration/evaluation → workpractice+IT co-evaluation; communication → theorizing. Directly useful if P2's own methods section needs to position itself against standard DSRM.

---

## Relevance to PRIS Research

### For [[P2_DPI_JSIS]] (primary)

The policy-ingrained artifact construct and the three EgovDR principles (policy/co-design/theorizing) supply named, citable vocabulary for analysing how DPI systems (Aadhaar, UPI, Account Aggregator) encode — or fail to encode — regulatory policy directly into their technical design, rather than leaving policy compliance to downstream administrative processes. The five institutional dimensions (regulative/normative/cognitive-linguistic/performative/relational) offer a complementary coding lens to Institutional Grammar 2.0 for P2's DPI governance-document analysis.

### Light conceptual parallel (non-evidentiary)

The welfare multi-query application's built-in eligibility-enforcement mechanism is a pre-AI, 2016-era instance of the same "runtime enforcement of policy at the system level" logic the AEGIS_OS consulting inbound applies to AI systems specifically — noted as a conceptual precedent only, not a corpus evidentiary instance of any signature concept.

---

## Connections

**Related concepts:** None forced — no signature/standard PRIS concept "Instances in Corpus" entry added; the paper's contribution is methodological/theoretical, not an empirical instance of Regulatory_Parallelism, Institutional_Coherence, or Governance_Debt.

**Related corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F095_Drahos_Regulatory_Theory_Foundations_Applications_2017]] (both supply general regulatory/institutional-theory vocabulary rather than AI-specific evidence).

**Related methods:** None currently — candidate addition to a future P2-specific methods note if one is created.

**Related projects:** [[P2_DPI_JSIS]]

---

## VERIFY Flags

**#265 — RESOLVED (2026-07-31, editorial convention).** Standard academic practice cites the printed volume/issue year, not intermediate submission/revision/acceptance milestones. All source dates (received 2015, accepted May 2016, online June 2016) converge on **2016** as the volume year, which this node's own Year line already correctly uses. No change needed — flag closed as already-compliant.

---

## Log

- 2026-07-16: Node created. NotebookLM Ingestion Pipeline (PROMPT 0b relay), per [[Session_Handoff_NotebookLM_Ingestion_20260715]]. Duplicate check against [[Corpus_Index_MOC]], `04_Knowledge_Products/Wiki_Intake/`, and `_Institutions_MOC.md` (searched "Goldkuhl," "policy-ingrained," "EgovDR") found no existing vault match — confirmed genuinely new. Classified Format B, routed to `04_Knowledge_Products/Wiki_Intake/`, admitted under the standing pure-methods/no-AI-content scope exception given direct P2 relevance. One new VERIFY flag (#265). New institution row (Linköping University) added to `_Institutions_MOC.md`. No concept-file "Instances in Corpus" edits.
