---
type: Institution
status: active
tags:
  - type/institution
  - status/active
  - paper/p1
  - paper/p3
  - gate/open
  - engine/phd
  - engine/consulting
---

# Grid-India — Grid Controller of India Limited

**Type:** Institution **Status:** Active **Created:** 2026-08-02 (missing-institutions sourcing pass)

---

## Institutional Identity

| | |
|---|---|
| **Incorporated** | March 2009 as Power System Operation Corporation Limited (**POSOCO**), then a PGCIL subsidiary |
| **Independence** | Wholly-owned Government of India company from **3 January 2017** |
| **Renamed** | **Grid Controller of India Limited**, effective 9 November 2022 (PIB announcement 13 Nov 2022) |
| **Statutory basis** | Central Government notification **27 September 2010** under Electricity Act 2003 **ss. 26(3) and 27(2)**, entrusting operation of the National Load Despatch Centre and five Regional Load Despatch Centres from 1 October 2010 |
| **Classification** | Schedule 'A' / Miniratna CPSE under the administrative control of [[Ministry_of_Power]] |
| **Capital** | Authorised ₹200 crore; paid-up ₹40.85 crore (31 Mar 2025); 100% GoI; 631 regular employees |
| **Primary regulator** | ⚠ **CERC — Central Electricity Regulatory Commission — not CEA.** Revenue and operational standards governed by CERC regulations under the Electricity Act 2003 |

**Institutional-map correction.** The [[Power_Grid_Critical_Infrastructure_Governance]] domain was built with [[CEA]] and [[NCIIPC]] as its institutional anchors. CEA issues sector-wide technical and cybersecurity guidelines that apply across the power sector including Grid-India's control centres, but **Grid-India's primary standard-setting regulator is CERC**, which has no node in this vault. Recorded as an open gap below.

## The Central Finding — production AI, zero governance instrument

Grid-India runs substantial machine learning in live national grid operations. Confirmed in specific technical detail:

**Demand forecasting (NLDC).** Day-ahead electricity demand forecasting using artificial neural networks (Levenberg–Marquardt algorithm) and gradient-boosting models (**XGBoost**), achieving Mean Absolute Percentage Error of **2–5%**. LSTM recurrent networks under refinement.

**Renewable data cleaning.** Collaboration with **IIT Kanpur** developing an AI/ML engine to clean real-time renewable-energy data, piloted at a **250 MW solar plant** in the southern region using approximately 200 features.

**Security operations.** A 24×7 Security Operations Centre integrating AI-powered SIEM, **UEBA** (User and Entity Behaviour Analytics), Network Behaviour Anomaly Detection, and **SOAR** for IT/OT cybersecurity.

Independently corroborated at ministerial level: [[Ministry_of_Power]] confirmed in a **Rajya Sabha written reply of 18 December 2023** that "Artificial Intelligence (AI) / Machine Learning (ML) tools are being used for maintenance of transmission lines" and that all grid substations use sensors for predictive maintenance.

**Against this: no Grid-India AI governance instrument exists.** No model governance policy, no validation or assurance requirement, no incident-reporting obligation specific to AI, no published documentation of these systems on grid-india.in. The applicable instruments — the CEA Cyber Security in Power Sector Guidelines and CERC's operational regulations — are cybersecurity and power-system regulations that predate and do not address machine learning.

## Analytical Significance

**Second infrastructure-layer [[Governance_Debt]] instance, and it is the stronger one.** [[NPCI]] runs federated AI fraud detection with no published governance instrument. Grid-India runs demand forecasting, renewable-data cleaning and AI-driven security analytics on **national grid operations** with none either. Both are systemically significant operators rather than regulators; neither is reached by any AI-specific obligation. The pattern is now confirmed across two unrelated critical sectors, which makes it a structural feature of Indian AI governance rather than a payments-sector anomaly: **India regulates AI at the regulator layer and not at the infrastructure-operator layer.**

**⚠ This qualifies the Power Grid domain's central claim.** [[Power_Grid_Critical_Infrastructure_Governance]] records that this is "the only domain in the vault where India tracks global peers rather than lagging — a genuine, unsolved regulatory frontier, not a capacity gap." That reading needs adjusting. It is true that no jurisdiction has AI-specific grid regulation. But India's grid operator is running production ML at national scale *now*, with parliamentary confirmation. This is not a frontier where nobody has arrived; it is **deployment running ahead of governance in a designated Critical Information Infrastructure sector**. The finding is stronger for the domain, not weaker — but it is a different finding, and the domain note should carry the correction rather than the original framing.

**Methodological consequence for [[fsQCA_Thesis_Chapter]].** The domain note logs an explicit caution against folding this sector into the fsQCA model on grounds of "near-zero cross-case variance on any AI-specific-regulation condition." That caution stands and is arguably reinforced — but the *reason* changes. Variance is near-zero on the regulation condition while AI **deployment intensity** varies substantially across jurisdictions. If deployment intensity were a condition rather than regulation presence, the sector would carry information. Worth raising with the TAC as a design question rather than treating the sector as simply excluded.

## Corpus Nodes

- [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]]

## Open Questions

- **OQ-GRID-01:** **CERC has no node in this vault** despite being Grid-India's primary regulator. Has CERC issued anything touching automated or AI-assisted system operation? Not searched. This is the most consequential gap left by the Power Grid domain build.
- **OQ-GRID-02:** Does Grid-India publish any internal model-governance, validation or assurance policy? Nothing located on grid-india.in.
- **OQ-GRID-03:** Do the CEA Cyber Security in Power Sector Guidelines reach AI/ML systems, or only conventional IT/OT? The Guidelines are referenced in the Rajya Sabha reply but the primary text was not retrieved in this pass.
- **OQ-GRID-04:** Is there any contestability or accountability route where an AI-driven forecasting or despatch decision contributes to an adverse outcome? None identified.

## Related Institutions

[[Ministry_of_Power]] — administrative control

[[CEA]] — sector-wide technical and cybersecurity guidelines

[[NCIIPC]] · [[CERT_IN]] — CII protection and CSIRT-Power coordination

[[NPCI]] — the structural parallel: systemically significant operator, production AI, no governance instrument

## Linked Frameworks

[[ISO_IEC_42001]] — the assurance standard that would apply if anything required assurance here

## Linked Concepts

[[Governance_Debt]] · [[Governance_Capacity]] · [[Accountability]] · [[Transparency]] · [[Human_Oversight]] · [[Contestability_Redress]] · [[Evidentiary_Governance]]

## Linked Domains

[[Power_Grid_Critical_Infrastructure_Governance]] · [[Cybersecurity_Governance]] · [[AI_Governance]]

---

_Back to [[_Institutions_MOC]]_
