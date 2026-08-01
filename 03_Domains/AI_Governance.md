---
type: Domain
tags:
  - type/domain
  - status/active
  - paper/p1
  - paper/p2
  - paper/p3-primary
  - paper/p4-primary
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/linkedin
  - engine/consulting
  - engine/knowledge-product
  - content/carousel-ready
  - content/wiki-entry
  - content/thought-leadership
---

# **AI Governance**

**Type:** Domain**Status:** Active**Last Updated:** 2026-06-11

---

## **Core Synthesis**

AI governance is understood in this research as the set of institutional arrangements, regulatory instruments, organisational processes, accountability structures, and oversight mechanisms through which AI systems are designed, deployed, monitored, and governed throughout their lifecycle. It is distinct from ethics statements, fairness aspirations, or model safety practices because governance requires documented decision authority, ownership assignment, operational controls, and auditable accountability. The domain is examined through an India-centric lens in which governance is emerging through a layered regulatory ecosystem rather than a dedicated AI regulator. The central research tension concerns the gap between governance as an institutional and regulatory arrangement and governance as a normative aspiration. The multi-regulator environment created by DPDP, RBI, SEBI, IRDAI, CERT-In, and other institutions generates coordination challenges that underpin the research agenda across this vault.

---

## **Scope and Boundary**

This domain includes regulatory frameworks, governance architectures, accountability mechanisms, risk-tiering models, enforcement structures, institutional coordination arrangements, and organisational governance processes for AI systems. The focus is on how authority is allocated, exercised, monitored, and enforced across jurisdictions and sectors. The domain excludes AI safety as a technical discipline concerned with model robustness and excludes AI ethics as a standalone normative field. The research boundary is therefore centred on governance instruments, institutional arrangements, and regulatory implementation rather than technical model behaviour.

---

## **Key Debates**

### **Governance vs Ethics**

The domain distinguishes governance from ethics by treating governance as an operational and institutional capability rather than a normative aspiration. Ethics principles may articulate desired outcomes, but governance determines who holds authority, how decisions are made, what controls are implemented, and how accountability is demonstrated. The India AI Governance Framework operationalises governance through design principles that translate into lifecycle controls, while the AIGP framework emphasises decision-making authority and oversight mechanisms. This distinction is central to the treatment of [[Accountability]], [[Institutional_Coherence]], and the governance artefacts examined across P2, P3, P4, and the fsQCA chapter.

### **Regulatory Fragmentation vs Coordination**

India operates a layered regulatory model combining horizontal and sector-specific regulation. DPDP provides the horizontal privacy foundation, while RBI, SEBI, IRDAI, and TRAI exercise sectoral authority through existing mandates. The absence of a dedicated AI regulator produces coordination challenges because obligations emerge through multiple regulatory pathways rather than a unified governance architecture. This creates compliance complexity and generates the institutional conditions examined through [[Regulatory_Parallelism]] and [[Governance_Debt]]. The resulting governance environment is characterised by overlapping mandates, differing enforcement mechanisms, and limited cross-regulatory coordination.

### **Sectoral vs Horizontal Regulation**

A recurring tension concerns the relationship between horizontal governance obligations and sector-specific regulatory requirements. DPDP establishes baseline privacy and accountability obligations applicable across sectors, while regulators such as RBI and SEBI impose additional requirements linked to specific regulated activities. When multiple obligations apply simultaneously, organisations must often comply with the strictest applicable requirement. This tension is particularly important in BFSI environments where AI systems may simultaneously trigger privacy, outsourcing, cyber resilience, and sectoral governance obligations. The issue provides a core analytical foundation for P3 and P4.

### **Agentic AI Governance Gap**

Agentic systems challenge existing governance assumptions because they act autonomously rather than merely assisting human decision-makers. Existing governance frameworks were largely designed for static systems, deterministic workflows, and human-mediated decision processes. Agentic architectures introduce new governance concerns related to autonomous decision execution, cascading failures, audit trail reconstruction, and accountability assignment. The governance implications extend beyond model governance to questions of identity, authority, and operational control. Emerging expectations around agent registers, decision logs, and accountability mapping indicate that governance frameworks are evolving but remain unsettled.

### **Risk-Tiered vs Principles-Based Approaches**

Jurisdictions differ significantly in how governance obligations are structured and enforced. The European Union adopts a risk-tiered model in which regulatory obligations increase according to system risk classification. India has favoured a principles-based approach emphasising accountability, transparency, privacy, inclusivity, and continuous assurance. The United States relies primarily on voluntary frameworks and distributed enforcement authorities. These alternative models create different enforcement characteristics, compliance burdens, and institutional incentives, making them important comparative cases for the research programme.

---

## **Indian Regulatory Landscape**

The DPDP Act 2023 and Rules 2025 provide the foundational horizontal governance layer for AI systems processing personal data. The framework requires DPIAs for AI systems processing personal data, mandates Data Protection Officer responsibility, establishes board-level accountability expectations, and creates enforceable obligations around consent, auditability, and governance controls. AI governance enters organisations primarily through privacy and accountability obligations rather than through dedicated AI legislation.

RBI’s Material Outsourcing Directions represent the most significant sectoral governance intervention affecting BFSI AI deployments. RBI treats AI systems performing regulated functions as outsourced functions regardless of whether they are developed internally or procured externally. Governance obligations therefore arise from the regulated function rather than the technological label. Requirements include board oversight, continuous monitoring, audit rights, incident management, and six-hour notification requirements for material failures.

SEBI’s updated Regulatory Sandbox incorporates explicit governance expectations for AI systems making autonomous decisions. The framework emphasises auditability, transparency, and explainability, particularly in algorithmic trading and market surveillance environments. Autonomous decision systems require pre-approval and must maintain evidence demonstrating how decisions were reached.

IRDAI’s data governance framework extends governance expectations into insurance environments through data localisation, lineage documentation, validation requirements, and breach notification obligations. Governance expectations increasingly focus on demonstrable control over data and decision processes.

CERT-In and the IT Rules operate as cross-cutting governance mechanisms. They provide operational cyber governance controls that apply regardless of sector and increasingly serve as enforcement pathways when AI systems create operational or security risks.

The overarching insight is that India’s governance model does not depend on a dedicated AI regulator. Governance is emerging through existing institutional authorities that extend established regulatory mandates into AI-enabled environments.

|**Instrument**|**Issuing Body**|**Type**|**Key AI Governance Hook**|
|---|---|---|---|
|DPDP Act 2023 & Rules 2025|Data Protection Board / Government of India|Horizontal privacy law|DPIA requirements; DPO accountability; governance obligations|
|RBI Material Outsourcing Directions|RBI|Sectoral regulation|AI agents treated as outsourced functions; six-hour incident notification|
|SEBI Regulatory Sandbox|SEBI|Sectoral regulatory framework|Pre-approval and audit trail requirements for autonomous systems|
|IRDAI Data Governance Mandate|IRDAI|Sectoral regulation|Data localisation, lineage, validation, and breach reporting|
|CERT-In / IT Rules|CERT-In / MeitY|Cross-cutting operational controls|Cyber governance, incident reporting, operational resilience|
|IndiaAI Framework|Government of India|Advisory framework|Principles-based governance architecture|

---

## **International Regulatory Context**

The EU AI Act represents the most comprehensive risk-tiered governance framework currently in force. It classifies systems into prohibited, high-risk, limited-risk, and low-risk categories, with high-risk systems subject to conformity assessment, documentation requirements, monitoring obligations, and human oversight controls. Its enforcement mechanisms and penalty structure establish a global benchmark for regulatory intervention.

The NIST AI Risk Management Framework provides a voluntary governance vocabulary and risk management structure that has become widely adopted across public and private sectors. Unlike the EU model, it relies on organisational adoption rather than legal compulsion. Its influence derives from standardisation rather than enforcement.

The United States maintains a fragmented governance landscape characterised by federal agencies, state-level initiatives, NIST standards, and FTC enforcement authority. Governance obligations emerge through multiple institutions rather than a unified regulatory framework. Compared with both the EU and the US, India remains closer to a principles-based governance model implemented through existing sectoral institutions rather than dedicated AI legislation.

---

## **Dominant Theoretical Frames**

**Institutional Grammar 2.0 (IG 2.0)** — Developed from the Institutional Grammar tradition associated with Elinor Ostrom and colleagues, IG 2.0 provides the ADICO coding structure used to analyse governance instruments in the fsQCA chapter, P3, and P4.

**Institutional Theory** — Associated with DiMaggio, Powell, Scott, and subsequent institutional scholars, this perspective explains divergent regulatory logics and coordination failures across institutions such as RBI and SEBI.

**Regulatory Governance Theory** — Drawing on regulatory governance scholarship, this lens examines jurisdictional allocation, institutional authority, and governance design across regulatory ecosystems.

**IS Digital Infrastructure Theory** — Originating in information systems research on digital infrastructures, this perspective explains how governance architectures become embedded within infrastructural arrangements and participant relationships.

**Regime Complexity Theory** — Developed within international governance and regulatory scholarship, this perspective explains overlapping regulatory regimes and provides the theoretical foundation for [[Regulatory_Parallelism]].

---

## **Open Research Questions**

**OQ-AG-01:** Does Regulatory Parallelism exist beyond BFSI and emerge in healthcare AI governance, defence AI governance, and DPI governance environments?

**OQ-AG-02:** What is the measurable magnitude of Governance Debt generated by dual-regulated BFSI entities?

**OQ-AG-03:** What configurations of governance conditions are sufficient for legitimate AI governance outcomes across jurisdictions?

**OQ-AG-04:** Can Institutional Coherence be operationalised as a diagnostic instrument for governance architectures outside AI?

**OQ-AG-05:** How does India’s principles-based governance model compare configurationally with the EU’s risk-tiered model in producing legitimate governance outcomes?

---

## **Linked Projects**

[[P1_SLR_RG]]

[[P2_DPI_JSIS]]

[[P3_BFSI_JEIM]]

[[P4_Doctrinal_IJLIT]]

[[fsQCA_Thesis_Chapter]]

## **Linked Knowledge Products**

[[AI_Governance_Wiki]]

[[Regulatory_Complexity_Handbook]]

[[BFSI_AI_Governance_Handbook]]

[[DPDP_Playbook]]

## **Linked Signature Concepts**

[[Regulatory_Parallelism]]

[[Governance_Debt]]

[[Institutional_Coherence]]

## **Linked Standard Concepts**

[[Accountability]]

[[Legitimacy]]

[[Transparency]]

[[Governance_Capacity]]

## **Linked Frameworks**

[[OECD_AI_Principles]]

[[UNESCO_Recommendations]]

[[NIST_AI_RMF]]

[[EU_AI_Act]]

[[IndiaAI_Framework]]

[[RBI_Free_AI]]

[[SEBI_AI_Circular]]

## **Linked Institutions**

[[RBI_Free_AI]]

[[SEBI]]

[[MEITY]]

[[CERT_IN]]

[[TRAI]]

[[UIDAI]]

## **Linked Methods**

[[Institutional_Grammar_IG2]]

[[fsQCA]]

[[SLR_Protocol]]

## **Future Reuse Opportunities**

- Extend P3 findings into comparative studies examining Regulatory Parallelism across healthcare, defence, and digital public infrastructure governance environments.
- Develop executive teaching cases comparing India’s principles-based governance architecture with the EU AI Act’s risk-tiered approach for Information Systems and Public Policy programmes.
- Support development of the [[Regulatory_Complexity_Handbook]] through operationalisation of Regulatory Parallelism and Governance Debt as advisory frameworks.
- Generate practitioner-focused LinkedIn series examining sectoral AI governance through RBI, SEBI, DPDP, and CERT-In enforcement pathways.
- Develop consulting diagnostics assessing Institutional Coherence, governance maturity, and multi-regulator accountability structures across BFSI organisations.

---

_Back to [[Domains_MOC]]_
