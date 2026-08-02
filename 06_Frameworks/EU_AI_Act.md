---
type: Framework
tags:
  - type/framework
  - status/active
  - paper/p1
  - paper/p4-primary
  - paper/fsqca
  - gate/open
  - engine/phd
  - engine/linkedin
  - content/carousel-ready
  - content/wiki-entry
---

# EU AI Act

**Type:** Framework **Status:** Active **Last Updated:** 2026-06-12

---

## Core Synthesis

Regulation (EU) 2024/1689 is the world's first comprehensive binding AI regulation — the only binding instrument among the seven PRIS framework cases — and its defining analytical property within PRIS is precisely that binding character combined with a risk-tiered Regulatory Logic. The Act organises AI governance not around sector or technology type but around risk level, establishing a structural hierarchy of obligations that scales from outright prohibition to unregulated deployment. Within the fsQCA model, the EU AI Act functions as the canonical RL benchmark: it is the comparative reference against which advisory, principles-based, and sectoral instruments in India and elsewhere are diagnosed as lacking calibrated binding force. In P4, it is the international transplant-model against which Indian regulatory fragmentation is measured.

## Framework Identity

- **Issuing body:** European Parliament and the Council of the European Union
- **Instrument type:** Binding Regulation (directly applicable in all EU member states)
- **Jurisdiction:** European Union; extraterritorial reach applies to any provider or deployer placing AI systems on the EU market or whose AI system output is used within the EU
- **Binding status:** Binding — legally enforceable with administrative penalty regime
- **Key dates:**
    - 2024: Regulation adopted and published in Official Journal
    - February 2025: Prohibitions and AI literacy obligations enter force
    - August 2025: General-Purpose AI (GPAI) obligations apply; notified-body designation infrastructure (Ch. IV) opens
    - **2 December 2027** (amended — see 2026-07-15 update below): High-risk Annex III obligations, including conformity assessment (Arts. 43–49)
    - **2 August 2028** (amended): High-risk Annex I (product-embedded AI) obligations

**⚠ 2026-07-15 update — Digital Omnibus on AI deferral:** The "2026–2027 phase-in" dating above is superseded. The Digital Omnibus on AI (COM(2025) 836, Council final approval 29 June 2026) deferred Annex III high-risk obligations (originally 2 Aug 2026) to **2 December 2027**, and Annex I product-embedded obligations (originally 2 Aug 2027) to **2 August 2028**. Art. 50(2) watermarking is deferred to 2 Dec 2026 for systems already on market. See [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] for full detail on the conformity-assessment/notified-body mechanism and the amended timeline table. This affects the "prior" fsQCA calibration note below (RL/EA scoring should account for the deferred binding date, not the original 2026 date) — revisit before Q3 2026 NVivo coding.

**⚠ 2026-08-02 update — no conformity-assessment standards exist yet.** Article 40 grants presumption of conformity only to harmonised standards published and cited in the Official Journal. As of June 2026, **zero AI-specific harmonised standards have been cited** — presumption of conformity under this Act currently attaches to nothing. The CEN-CENELEC JTC 21 pipeline is entirely in draft/enquiry/approval stages, with prEN 18286 (QMS, Art. 17) most advanced at Formal Vote and targeted for Q4 2026; the Commission mandate deadline is amended to 28 February 2027. See [[07_Institutions/Corpus/International/International_33_CEN_CENELEC_JTC21_Harmonised_Standards_2026]]. This plausibly supplies the mechanical reason for the Digital Omnibus deferral recorded above — the standards the high-risk obligations depend on were not going to exist in time — though that is an inference, not a documented causal claim. **ISO/IEC 42001 is not part of the EU harmonisation process**; the European AI Office signalled in May 2024 that it is not fully aligned with the final Act text. See [[06_Frameworks/ISO_IEC_42001]].

## Structural Overview

The Act organises AI systems into four risk tiers. At the apex, a small category of AI applications is outright **prohibited** on grounds of incompatibility with fundamental rights — social scoring by public authorities, real-time biometric surveillance in public spaces (with narrow exceptions), and systems exploiting vulnerabilities. Below prohibition sits the **high-risk** tier, which carries the primary compliance burden: conformity assessment against harmonised standards, CE marking, mandatory risk-management systems, data-governance requirements, technical documentation, logging and audit-trail obligations, human-oversight mechanisms, and post-market monitoring. A **limited-risk** tier applies primarily transparency obligations — users must know when they are interacting with AI. The **minimal-risk** tier is largely unregulated, with voluntary codes of conduct encouraged.

Layered over this risk pyramid is a separate horizontal track for **General-Purpose AI (GPAI) models**, including systemic-risk GPAI with enhanced obligations. This layer reflects the architectural reality that foundation models do not fit neatly into the product-risk taxonomy and require distinct governance logic.

The structural logic — risk-tiering as the organising principle rather than sector, function, or nationality — is what gives the Act its comparative significance. It creates an obligation architecture whose proportionality can be evaluated empirically, and it operationalises Regulatory Logic (RL) as a condition in the fsQCA model more precisely than any principles-based instrument.

## Regulatory Position & Comparative Significance

Among the seven PRIS frameworks, the EU AI Act occupies a structurally singular position: it is the only instrument that combines binding legal status, cross-sectoral applicability, and tiered obligation architecture. The OECD Principles and UNESCO Recommendation are authoritative but non-binding. The NIST AI RMF is voluntary and jurisdiction-specific. IndiaAI operates as advisory guidance. RBI FREE-AI and the SEBI AI Circular are sectoral and binding within their domains but lack the cross-sectoral risk-tier architecture. The Act therefore anchors the high-RL end of the comparative spectrum and makes visible, by contrast, what the Indian multi-regulator landscape lacks: a framework for calibrating obligation intensity to risk level independently of which regulator is issuing the instrument.

## IG 2.0 Coding Summary

Full ADICO-level coding of the EU AI Act is in NVivo — this note does not replicate that output. At the construct level, the Act is expected to generate strong **Aim** and **Deontic** densities: its provisions are heavily prescriptive, obligations are clearly attributed to identified **Attribute** holders (providers, deployers, notified bodies), and **Or-else** components are explicit by virtue of the penalty regime. **Condition** specification is operationalised through the risk-classification criteria and the Annex III high-risk list. The GPAI track is likely to show a distinctive ADICO profile with more principle-level Deontic content and emergent Condition specification — a contrast worth examining during Q3 2026 coding.

## fsQCA Calibration

This framework is a candidate case in the 10-case fsQCA model. Case-level calibration is pending NVivo IG 2.0 coding (Q3 2026). Anchors: 0.00 / 0.33 / 0.67 / 1.00.

|Condition|Score|Status|
|---|---|---|
|EA — Ethical Alignment|⏳|Pending Q3 2026|
|SR — Stakeholder Role Clarity|⏳|Pending Q3 2026|
|RL — Regulatory Logic|⏳|Pending Q3 2026|
|SI — Stakeholder Inclusion|⏳|Pending Q3 2026|

_Prior (to be confirmed against coded data, not a result):_ The Act is expected to score high on RL given explicit risk-tiering and binding enforcement, and reasonably high on SR given the provider/deployer/notified-body attribution structure. EA and SI priors are less determinate — EA depends on how ethical principles are operationalised in the Annex criteria; SI depends on what the Act counts as stakeholder consultation vs. notification.*

## Coordination Pair Classification

Not applicable. The EU AI Act sits outside the P3 Indian BFSI corpus (RBI / SEBI / CERT-In). It enters PRIS as an international comparator in P1, P4, and the fsQCA model, not as a participant in the Indian regulatory coordination-pair analysis.

## Key Tensions & Gaps

The Act's risk-classification machinery depends on the Annex III high-risk list, which is subject to delegated acts — creating a structural gap between the stability of the legal text and the volatility of what actually counts as high-risk at any given time. The GPAI systemic-risk threshold (defined partly by compute thresholds that are already contested) creates an obligation boundary that may ossify at technically arbitrary parameters. Extraterritorial reach is clear in text but enforcement capacity against non-EU entities remains genuinely uncertain, which matters for how the Act functions as a transplant reference for Indian regulators. For jurisdictions treating the Act as a design model — as India's draft governance literature increasingly does — these structural ambiguities are exported alongside the architecture.

## Linked Projects

- [[P1_SLR_RG]]
- [[P4_Doctrinal_IJLIT]]
- [[fsQCA_Thesis_Chapter]]

## Linked Domains

- [[AI_Governance]]

## Linked Concepts

- [[Accountability]]
- [[Transparency]]
- [[Legitimacy]]
- [[Institutional_Coherence]]

## Linked Frameworks

- [[ISO_IEC_42001]] — assessed by the AI Office and found not aligned; not a conformity route

- [[OECD_AI_Principles]]
- [[NIST_AI_RMF]]
- [[IndiaAI_Framework]]
- [[UNESCO_Recommendations]]

## Linked Methods

- [[Institutional_Grammar_IG2]]
- [[fsQCA]]

## Linked Institutions

- [[MEITY]]

## Linked Corpus Nodes

- [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] — detailed conformity-assessment/notified-body mechanism (Arts. 28–34, 43–49; Annexes V–VII) and Digital Omnibus timeline deferral, added 2026-07-15 (Gap #4 closure)
- [[04_Knowledge_Products/Wiki_Intake/FRA_EU_Assessing_High_Risk_AI_Fundamental_Rights|F053]] — FRIA/Art. 27 companion

## Future Research / Reuse Opportunities

The RL benchmark function of this note feeds directly into the fsQCA truth table (Q3–Q4 2026): the Act's calibration score on RL and SR will anchor the high end of the condition spectrum against which India's RBI FREE-AI and SEBI Circular are positioned. In P4, it is the primary international comparator for the Three-Level Governance Alignment Model — specifically, the EU's provider/deployer attribution architecture is the counter-model to India's single-regulator-domain fragmentation. For the AI Governance Wiki, the Act underpins Section 3.1 and will require updating as delegated acts clarify the Annex III list. The Regulatory Complexity Handbook can use the Act as the canonical example of complexity imposed by design (risk-tiering as deliberate regulatory architecture) versus complexity arising from institutional fragmentation (as in India).

---

_Back to [[_Frameworks_MOC]]_