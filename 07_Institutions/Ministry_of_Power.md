---
type: Institution
status: active
tags:
  - type/institution
  - status/active
  - paper/p1
  - gate/open
  - engine/phd
---

# Ministry of Power

**Type:** Institution **Status:** Active **Created:** 2026-08-02 (missing-institutions sourcing pass)

---

## Institutional Identity

Ministry of Power, Government of India. Administrative control over [[Grid_India]] (Grid Controller of India Limited, a Schedule 'A'/Miniratna CPSE) and policy authority over the power sector under the Electricity Act 2003.

**Institutional map — three bodies, three roles, and one missing node:**

| Body | Role |
|---|---|
| **Ministry of Power** | Policy, administrative control of Grid-India, schemes |
| **[[CEA]]** | Sector-wide technical and cybersecurity guidelines (incl. the Cyber Security in Power Sector Guidelines) |
| **CERC** (Central Electricity Regulatory Commission) | ⚠ **Grid-India's primary standard-setting and tariff regulator** under the Electricity Act 2003 — **no node exists in this vault** |
| **[[Grid_India]]** | System operator: NLDC + five RLDCs |

The [[Power_Grid_Critical_Infrastructure_Governance]] domain was built with CEA and [[NCIIPC]] as anchors. **CERC is the significant omission** — see OQ-GRID-01.

## Documented AI Position

**Rajya Sabha written reply, 18 December 2023** — https://sansad.in/getFile/annex/262/AU1906.pdf?source=pqars
Verbatim: "Artificial Intelligence (AI) / Machine Learning (ML) tools are being used for maintenance of transmission lines. All grid substations use sensors for measuring various parameters of power system to carry out predictive maintenance." Confirms CSIRT-Power notified for power-sector cyber incidents and that communication systems must comply with the CEA (Cyber Security in Power Sector) Guidelines.

**PIB parliamentary reply, 8 August 2024** — https://www.pib.gov.in/PressReleasePage.aspx?PRID=2043154
As of March 2024, 30 of 35 State Load Despatch Centres including Grid-India's six control centres had conducted VAPT audits within five years; no cybersecurity incident has affected Indian grid operations.

**National Smart Grid Mission** (2015) — 12 Smart Grid pilot projects supported in State utilities. The closest confirmed MoP scheme-level document bearing on grid digitalisation.

## Analytical Significance

**MoP has confirmed AI use in Parliament and issued no AI governance instrument.** The ministry acknowledges machine learning in transmission maintenance and predictive substation monitoring; it has published no model governance, validation, assurance or AI-specific incident-reporting requirement. Its confirmations are *parliamentary answers*, not regulatory instruments — a distinction worth preserving in coding, since an answer to a question is not an obligation on anyone.

This is the ministerial half of the finding recorded at [[Grid_India]] and [[07_Institutions/Corpus/Grid_India/Grid_India_1_AI_Grid_Operations_2025]]: production AI in national grid operations, governed by cybersecurity and power-system instruments that predate and do not address it.

## Open Questions

- **OQ-MOP-01:** **CERC has no node.** Has it issued anything touching automated or AI-assisted system operation, despatch or forecasting? Unsearched, and the most consequential remaining gap in this domain.
- **OQ-MOP-02:** Does the current National Electricity Plan (published by CEA) contain a clause-level digital/AI provision? **No specific NEP or National Electricity Policy AI clause was isolated** in this pass; the Smart Grid Mission is the closest confirmed instrument.
- **OQ-MOP-03:** The CEA Cyber Security in Power Sector Guidelines are referenced in the Rajya Sabha reply but the **primary text was not retrieved** — direct retrieval from cea.nic.in required to determine whether they reach AI/ML at all (see also OQ-GRID-03).

## Related Institutions

[[Grid_India]] · [[CEA]] · [[NCIIPC]] · [[CERT_IN]]

## Linked Concepts

[[Governance_Debt]] · [[Governance_Capacity]] · [[Accountability]] · [[Institutional_Coherence]]

## Linked Domains

[[Power_Grid_Critical_Infrastructure_Governance]] · [[Cybersecurity_Governance]] · [[AI_Governance]]

---

_Back to [[_Institutions_MOC]]_
