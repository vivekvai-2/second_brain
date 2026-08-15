---
type: Institution
status: active
tags:
  - type/institution
  - status/active
  - paper/p2
  - paper/p3
  - gate/open
  - engine/phd
---

# NPCI — National Payments Corporation of India

**Type:** Institution **Status:** Active **Created:** 2026-08-02 (DEPA sourcing pass)

---

## Institutional Identity

NPCI operates India's retail payments infrastructure, most significantly UPI. It is an umbrella organisation for retail payments constituted under RBI and IBA auspices, and functions as a systemically significant infrastructure operator rather than a regulator — its instruments are Operating Circulars binding on participant banks and PSPs by contract and network-membership condition rather than by statute.

Circular repository (live, continuously updated): https://www.npci.org.in/circulars/upi

## Primary Finding — confirmed governance absence

**NPCI has published no primary governance instrument of any kind on AI or algorithmic systems in UPI.** Confirmed by direct search of the Operating Circular index, 2026-08-02.

What exists instead:

- **Operational AI in production.** A federated AI fraud-detection pilot with partner banks generating comparative risk scores across institutions; NPCI's own public communications describe "advanced fraud detection" using "proven AI models" and "continuous monitoring."
- **Evidence base is secondary only.** Economic Times BFSI reporting (3 April 2025) and NPCI promotional/social-media material. No circular, policy paper, technical standard, or governance framework.
- **Adjacent circulars exist but are not AI-scoped.** OC No. 234 (FY 2026-27) "Safeguarding User Information in UPI"; OC 235 (FY 26-27) on turnaround time for fraud and wrong-credit chargebacks. Security- and fraud-adjacent, silent on algorithmic systems.

## Analytical Significance

**India's highest-volume payment rail governs its AI by press release.** A federated cross-institutional risk-scoring system — which shares inferred risk signals about customers between banks — operates with no published governance instrument, no disclosed model governance, no stated contestability route for a customer adversely scored, and no audit or assurance requirement in the public record.

This is a [[Governance_Debt]] instance at the **infrastructure layer**, structurally distinct from the regulator-layer instances that dominate the corpus. The gap is not that a regulator has issued advisory rather than binding rules; it is that a systemically significant operator has issued nothing at all while deploying the technology at national scale.

**The contrast within DEPA sharpens it.** The Account Aggregator regime — same broad domain, same regulator, same architecture family — carries binding Master Directions, delegated technical specification with change control and 30-day adoption reporting, an RBI-recognised SRO, and a four-tier grievance chain. UPI's AI layer carries none of these. See [[DEPA]].

**Comparison case for [[Sahamati]]:** comparable systemic significance, no SRO, no published governance instrument.

## Corpus Nodes

None. **No NPCI document met the PRIS evidence threshold** — the confirmed absence is the finding, and is recorded here rather than fabricated into a node.

## Open Questions

- **OQ-NPCI-01:** Does the federated fraud-detection pilot have a governance document that is unpublished or circulated only to participants? Worth a targeted RTI or a direct approach — this is the kind of gap where a practitioner enquiry may succeed where search does not.
- **OQ-NPCI-02:** Does RBI's FREE-AI framework, once operationalised, reach NPCI as an infrastructure operator, or only Regulated Entities? The scope question determines whether this gap closes automatically or persists.
- **OQ-NPCI-03:** Is there any contestability route for a customer adversely affected by a federated risk score? None located.

## Related Institutions

[[RBI]] · [[Sahamati]] · [[UIDAI]]

## Linked Frameworks

[[DEPA]] · [[RBI_Free_AI]]

## Linked Concepts

[[Governance_Debt]] · [[Contestability_Redress]] · [[Transparency]] · [[Accountability]] · [[Fairness]]

## Linked Domains

[[DPI_Governance]] · [[BFSI_Governance]]

---

_Back to [[_Institutions_MOC]]_


## Corpus Nodes

- [[07_Institutions/Corpus/NPCI/NPCI_1_AI_ML_Payments_Operations_2025_2026]] — AI/ML in retail payments operations (2025–26): EFRM ecosystem-level fraud alerting, the NVIDIA sovereign-AI programme, the UPI Help Assistant pilot, and the regulatory perimeter finding — NPCI is inside `RBI/DPSS/2024-25/123`'s cyber-resilience perimeter and outside every AI-governance perimeter. Created 2026-08-15.
