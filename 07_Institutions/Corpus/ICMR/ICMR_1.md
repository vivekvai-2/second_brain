---
type: corpus-node
node-id: ICMR_1
institution: ICMR
date: 2023
wiki-section: S2
tier: A
ai-explicit: true
tags:
  - type/corpus-node
  - institution/ICMR
  - wiki-section/S2
  - tier/A
  - batch/10
  - concept/Regulatory_Parallelism
  - concept/Governance_Debt
  - concept/Accountability
  - concept/Transparency
  - concept/Institutional_Coherence
  - project/P1
  - project/P3
---

# ICMR_1 — ICMR Ethical Guidelines for Application of Artificial Intelligence in Biomedical Research and Healthcare (2023)

**Node ID:** ICMR_1  
**Institution:** Indian Council of Medical Research (ICMR)  
**Document type:** Ethical Guidelines — primary government framework for healthcare AI governance in India  
**Date:** 2023  
**Jurisdiction:** India  
**Wiki Section:** S2 — India Regulatory (Healthcare sector — primary ICMR AI governance framework; new sector track)  
**Tier:** A (ICMR primary guidelines; 2023; ICMR is the apex Indian government body for biomedical research — these guidelines are the primary regulatory reference for AI in Indian healthcare; fills entire healthcare AI governance gap in PRIS corpus)  
**Source PDF:** Ethical_Guidelines_AI_Healthcare_2023.pdf  
**Institution Note:** New ICMR corpus track — ICMR_1 is the founding node for this institution series

---

## S1. Document Identity

| Field | Detail |
|---|---|
| Full Title | Ethical Guidelines for Application of Artificial Intelligence in Biomedical Research and Healthcare |
| Publisher | Indian Council of Medical Research (ICMR) |
| Date | 2023 |
| Jurisdiction | India |
| Target scope | Biomedical research + clinical care + hospital management + epidemiology |
| Addressees | Researchers, developers, ethics committees, institutions, funding agencies |
| Authority type | Government guidelines — primary ethical framework from India's apex medical research body |
| Corpus gap filled | First ICMR node; entire healthcare AI governance sector was absent from PRIS corpus prior to Batch 10 |

---

## S2. Governance Context

ICMR_1 is the primary Indian government framework for AI governance in healthcare and biomedical research. Its significance extends beyond its sector-specific scope because healthcare AI governance intersects with several PRIS research themes: the guidelines use an eight-principle ethical framework that parallels both OECD AI Principles and the EU AI Act's fundamental rights framework, and ICMR's governance architecture (ethics committees, institutional oversight, principle-based compliance) offers a comparative model for how sector-specific AI ethics frameworks are operationalised without sector-specific AI legislation.

For [[Regulatory_Parallelism]] analysis: ICMR_1 was issued by a health research body (under MoHFW) independently of MeitY's AI guidelines (MeitY_2), NITI Aayog's Responsible AI frameworks (NITI_3, NITI_6, NITI_7), and RBI's BFSI-focused FREE-AI — no cross-references evident. Healthcare AI, BFSI AI, and cross-sectoral AI governance in India are proceeding on separate institutional tracks, even where the underlying ethical principles are near-identical.

---

## S3. Eight-Principle Ethical Framework

ICMR_1 establishes eight core ethical principles for healthcare AI:

| # | Principle | Application in Healthcare AI |
|---|---|---|
| 1 | Autonomy | Patient informed consent for AI-assisted diagnosis/treatment; right to opt out |
| 2 | Safety | Clinical validation before deployment; ongoing post-market surveillance |
| 3 | Trustworthiness | Model reliability, calibration, and performance transparency for clinical users |
| 4 | Beneficence | AI must demonstrably improve clinical outcomes; benefit-to-risk assessment required |
| 5 | Non-maleficence | Harm avoidance: bias in training data leading to disparate diagnostic accuracy across demographic groups |
| 6 | Equity | Fair access; avoid AI exacerbating existing health disparities (urban/rural, gender, socioeconomic) |
| 7 | Accountability | Defined responsible party for AI-assisted clinical decisions; cannot delegate liability to AI |
| 8 | Privacy | Data minimisation; purpose limitation; security of sensitive health data used in AI training |

### Key Provisions (verbatim)

> "Ethical principles for AI in healthcare include: Autonomy, Safety, Trustworthiness, Beneficence, Non-maleficence, Equity, Accountability, and Privacy." — ICMR Ethical Framework

> "AI applications in biomedical research and healthcare span: Diagnostics, Therapeutics, Clinical Care, Epidemiology, Behavioral Health, and Hospital Management." — Scope of Application

> "These guidelines apply to: Researchers, Developers, Ethics Committees, Institutions, and Funding Agencies." — Regulatory Coverage

---

## S4. Governance Architecture

| Element | ICMR_1 Provision |
|---|---|
| Institutional oversight | Ethics committees (IECs) required to include AI expertise for review of AI-based research |
| Developer obligations | Safety assurance, validation testing, ongoing monitoring before clinical deployment |
| Researcher obligations | Data provenance documentation, bias assessment, transparent reporting of model limitations |
| Funder obligations | Require ethical compliance as grant condition; institutional audit rights |
| Hospital management AI | Equity assessment mandatory — resource allocation algorithms must not perpetuate disparities |
| Post-deployment monitoring | Ongoing performance surveillance for clinical AI; no one-time validation-and-forget |

### Comparison with Parallel AI Governance Frameworks

| Framework | Sector | Principle overlap | Cross-reference in ICMR_1 |
|---|---|---|---|
| NITI Aayog Responsible AI (NITI_3) | Cross-sector | High (7/8 principles common) | None cited |
| MeitY IndiaAI Guidelines (MeitY_2) | Cross-sector | High | None cited |
| RBI FREE-AI (RBI_FREE_AI_2025) | BFSI | Medium (accountability, transparency, safety) | None cited |
| EU AI Act | Global | High (autonomy, accountability, safety as high-risk) | None cited |

The null cross-referencing is evidence of [[Regulatory_Parallelism]] at the ethics-principle level: India now has healthcare, BFSI, telecom, and cross-sectoral AI ethics frameworks that share near-identical core principles but were drafted independently by separate institutions with no documented coordination.

---

## S5. Concept Linkages

| Concept | Evidence from ICMR_1 |
|---|---|
| [[Regulatory_Parallelism]] | ICMR, MeitY, NITI Aayog, RBI all independently articulate similar AI ethics principles without coordination — healthcare AI governance proceeds on its own institutional track |
| [[Governance_Debt]] | Ethics committee AI expertise requirement (IEC) is an aspirational standard — most Indian IECs do not currently have AI-qualified members; structural gap between guideline and implementation capacity |
| [[Accountability]] | Principle 7 (Accountability) explicitly states that liability for AI-assisted clinical decisions cannot be delegated to the AI system — defines responsible party requirement; most advanced accountability statement in Indian sector-specific AI guidance |
| [[Transparency]] | Principle 3 (Trustworthiness) operationalised through clinical performance transparency — directly applicable to explainability requirements in high-stakes AI decisions (analogous to EU AI Act Article 13) |
| [[Institutional_Coherence]] | ICMR_1's eight principles are substantively coherent with OECD, EU, and NITI Aayog frameworks — evidence of normative convergence; absence of formal cross-referencing is an institutional (not substantive) incoherence |

---

## S6. Project Relevance

| Project | Relevance |
|---|---|
| P1 (SLR — RG/GIQ) | ICMR_1 is important comparative evidence for the SLR's treatment of sector-specific vs. cross-sectoral AI governance design: India demonstrates parallel sector-specific frameworks (ICMR for healthcare, RBI for BFSI, TRAI for telecom) without a unified superordinate framework — a governance design choice with theoretical implications |
| P3 (BFSI — JEIM) | Healthcare-BFSI AI governance intersection: health data is increasingly used in insurance underwriting (IRDAI) and credit scoring (RBI) — ICMR's Principle 8 (Privacy) and Principle 6 (Equity) have direct BFSI implications when health data is an AI training input |
| fsQCA_Thesis_Chapter | ICMR provides India's healthcare sector configurational data — "sector-specific ethics guidelines without binding enforcement mechanism" — for comparison with BFSI (principles + reporting obligations) and telecom (mandatory deployment direction) |

---

## S7. ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-ICMR1 | Confirm exact year of publication (stated 2023) — is this the first edition or a revision? | Verify via icmr.gov.in |
| ⚠V-ICMR2 | Confirm whether ICMR_1 has been revised post-2023, particularly in light of DPDP Act 2023 and DPDP Rules 2025 | Web search: "ICMR AI guidelines update 2024 2025" |
| ⚠V-ICMR3 | Are IECs (Institutional Ethics Committees) currently required to include AI expertise? Or is this an aspirational/recommended provision in the guidelines? | Legal analysis of IEC constitution regulations under ICMR/DBT framework |

---

## Backlinks

← [[07_Institutions/Corpus/MeitY/MeitY_2]] (IndiaAI Guidelines — parallel cross-sector framework, no cross-reference)  
← [[07_Institutions/Corpus/NITI_Aayog/NITI_3]] (Responsible AI for All — parallel principles framework)  
← [[07_Institutions/Corpus/IRDAI/IRDAI_1_Maintenance_and_Sharing_of_Information_Regulations_2025]] (health data intersects IRDAI)  
← [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]  
← [[05_Concepts/05_Concepts_Standard/Accountability]]  
← [[05_Concepts/05_Concepts_Standard/Transparency]]
