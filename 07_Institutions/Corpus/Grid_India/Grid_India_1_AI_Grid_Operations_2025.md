---
type: Corpus Node
status: active
tags:
  - type/corpus-node
  - status/active
  - institution/grid-india
  - paper/p1
  - paper/p3
  - gate/open
  - engine/phd
---

# Grid_India_1 — AI/ML in National Grid Operations (2023–2025)

**Institution:** [[Grid_India]] | **Added:** 2026-08-02 (missing-institutions sourcing pass)

Consolidated node — the operational AI record plus its ministerial corroboration.

---

## Document Identity

**(a) "AI in Grid Operations: Enhancing flexibility, security and reliability"**
Venue: *Powerline*, 31 August 2025
https://powerline.net.in/2025/09/01/ai-in-grid-operations-enhancing-flexibility-security-and-reliability/
⚠ **Trade publication, not a Grid-India-hosted document.** Content is a first-person institutional account of Grid-India's own initiatives, consistent with an authored/attributed piece rather than external commentary — but **no grid-india.in whitepaper or technical report was independently retrieved.** Verify against grid-india.in's publications section before citing in publication-track output.

**(b) Ministry of Power, Rajya Sabha written reply, 18 December 2023**
https://sansad.in/getFile/annex/262/AU1906.pdf?source=pqars
Verbatim: "Artificial Intelligence (AI) / Machine Learning (ML) tools are being used for maintenance of transmission lines. All grid substations use sensors for measuring various parameters of power system to carry out predictive maintenance." Also confirms CSIRT-Power notified for power-sector cybersecurity incidents, and that power-sector communication systems must comply with the CEA (Cyber Security in Power Sector) Guidelines.
**Status: parliamentary record — the strongest-provenance confirmation of Indian grid AI use in the corpus.**

**(c) Ministry of Power / PIB parliamentary reply, 8 August 2024**
https://www.pib.gov.in/PressReleasePage.aspx?PRID=2043154
As of March 2024, 30 of 35 State Load Despatch Centres — including Grid-India's six control centres (NLDC, NRLDC, SRLDC, WRLDC, ERLDC, NERLDC) — had conducted VAPT cybersecurity audits within the prior five years. No cybersecurity incident has affected Indian grid operations. NCIIPC, CERT-In and CSIRT-Power named as the agencies running cybersecurity awareness training.

## Substantive Content — the AI stack

| Application | Technique | Detail |
|---|---|---|
| Day-ahead demand forecasting (NLDC) | Artificial neural networks (**Levenberg–Marquardt**); gradient boosting (**XGBoost**) | **MAPE 2–5%**. LSTM recurrent networks under refinement |
| Renewable real-time data cleaning | AI/ML engine, **IIT Kanpur** collaboration | Piloted at a **250 MW solar plant**, southern region, ~200 features |
| IT/OT cybersecurity | **SIEM, UEBA, NBAD, SOAR** | 24×7 Security Operations Centre |
| Transmission-line maintenance | AI/ML + substation sensor arrays | Predictive maintenance; confirmed in Parliament |

## Analytical Significance

**Production AI at national infrastructure scale, governed by nothing AI-specific.** The applicable instruments — CEA Cyber Security in Power Sector Guidelines, CERC operational regulations — are cybersecurity and power-system regulations that predate machine learning and do not address it. No model governance policy, no validation or assurance requirement, no AI-specific incident-reporting obligation, no published documentation.

**Second confirmed instance of infrastructure-layer [[Governance_Debt]]**, after [[NPCI]]. Two unrelated critical sectors — payments and electricity — each with a systemically significant operator running production AI and no governance instrument reaching it. The pattern is structural: **India regulates AI at the regulator layer, not at the infrastructure-operator layer.** Neither NPCI nor Grid-India is a "Regulated Entity" in the sense RBI FREE-AI addresses, and no instrument in the corpus reaches either.

**⚠ Qualifies the Power Grid domain's central claim.** [[Power_Grid_Critical_Infrastructure_Governance]] records this as "the only domain where India tracks global peers rather than lagging — a genuine, unsolved regulatory frontier, not a capacity gap." That framing predates this evidence. It remains true that no jurisdiction has AI-specific grid regulation; it is now also true that India's grid operator runs production ML at national scale with parliamentary confirmation. **Not a frontier nobody has reached — deployment running ahead of governance inside a designated Critical Information Infrastructure sector.** Stronger for the domain, but a different claim.

**fsQCA note.** The domain's logged caution against inclusion (near-zero cross-case variance on AI-specific regulation) still holds, but the reason shifts: regulation presence has no variance while **AI deployment intensity** does. As a condition, deployment intensity would carry information where regulation presence does not. A design question for the TAC rather than grounds for exclusion.

## Coding Notes (IG 2.0)

Near-zero ADICO yield — a trade article and two parliamentary replies contain no institutional statements with deontic force. Value is evidentiary, not rule-level: this node establishes **the fact of deployment**, against which the absence of governing rules can be measured. That absence is the codeable finding.

## Related Nodes

- [[07_Institutions/Corpus/CEA/CEA_1_Cyber_Security_Guidelines_2021]] — the sole binding Indian anchor for this sector; ⚠ does it reach AI/ML? (OQ-GRID-03)
- [[07_Institutions/Corpus/CEA/CEA_2_Draft_Cyber_Security_Regulations_2025]] — folds in CSIRT-Power
- [[07_Institutions/Corpus/International/International_26_NERC_CIP_ENISA_IEC62443_AI_Gap_2026]] — the comparators, all confirming the same AI-specific gap
- [[NPCI]] — the structural parallel in payments

## Linked Concepts

[[Governance_Debt]] · [[Governance_Capacity]] · [[Accountability]] · [[Human_Oversight]] · [[Transparency]] · [[Evidentiary_Governance]] · [[Contestability_Redress]]

## Linked Domains

[[Power_Grid_Critical_Infrastructure_Governance]] · [[Cybersecurity_Governance]] · [[AI_Governance]]

---

_Back to [[Grid_India]] | [[Corpus_Index_MOC]]_
