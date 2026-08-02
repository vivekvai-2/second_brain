---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - section/S6
  - tier/high
  - project/p1
  - project/p3
  - project/p4
  - project/fsqca
  - engine/phd
---

# RAND / GovAI: Designing Incident Reporting Systems for AI (2025)

**Node ID:** F051
**Type:** Wiki Intake Note (Format B)
**Wiki Section:** S1 (Governance Fundamentals) / S6 (Model Risk / Implementation)
**Status:** Active
**Tier:** High
**Last Updated:** 2026-07-14 (Batch 15 continuation)

---

## Source

**Full Citation (APA):** Wei, N., Anderljung, M., Shevlane, T., & Siegmann, C. (2025). *Designing incident reporting systems for AI: Lessons from safety-critical industries.* arXiv:2511.05914v1. Accepted, AAAI 2026.
**Document Type:** Working paper / conference paper (AAAI 2026 accepted)
**Issuing Institutions:** RAND Corporation (Wei); Centre for the Governance of AI / GovAI (Anderljung, Shevlane, Siegmann)
**Publication vehicle:** arXiv preprint (November 2025); AAAI 2026 conference proceedings
**Batch:** 15 (continuation) | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump Future

---

## Summary

Wei et al. develop a seven-dimension institutional design framework for AI Incident Reporting Systems (AIIRS), derived from nine safety-critical industry analogues — nuclear, aviation, pharmaceuticals, medical devices, cybersecurity, food safety, occupational safety, rail, and financial services. The core argument is that incident reporting is necessary but insufficient for AI governance: effective AIIRS must resolve a structural tension between *learning* (requires confidentiality and blame-free culture) and *accountability* (requires transparency and liability clarity). Existing AI-specific reporting regimes — principally China's GPAI incident reporting mandate and EU AI Act mandatory notification obligations — are assessed as design-incomplete relative to mature safety industry analogues.

---

## Key Findings and Framework

### Seven-Dimension AIIRS Design Framework

| Dimension | Core Design Options | Cross-Industry Learning |
|-----------|--------------------|-----------------------|
| **1. Reporting mandate** | Voluntary / mandatory / tiered-mandatory | Aviation: mandatory + voluntary dual-track; financial services: mandatory for material events only |
| **2. Reporter scope** | Developer / deployer / user / third-party auditor | Nuclear: multi-actor primary obligation; pharma: manufacturer-primary with downstream voluntary |
| **3. Incident definition** | Harm-materialised / near-miss / anomaly / operational deviation | Aviation near-miss system (ASRS) generates highest learning value; pharma near-miss systematically underreported |
| **4. Confidentiality regime** | Full public disclosure / structured non-attribution / selective release | Nuclear full-disclosure enables cross-operator learning; aviation non-attributed ASRS enables candid near-miss reporting |
| **5. Legal liability insulation** | Full immunity / qualified immunity / none | Absence of liability protection suppresses voluntary near-miss reporting in every industry examined |
| **6. Governance body** | National regulator / independent safety board / international body | ICAO aviation framework cited as gold standard for cross-border incident management |
| **7. Learning infrastructure** | Database / causal analysis unit / corrective action tracking | FDA MAUDE database archetype; cybersecurity CVE/NVD as digital-native model |

### The Near-Miss Case

Near-miss reporting — events that *could have* caused harm but did not — is argued to provide higher marginal learning value than harm-realised reporting, for three reasons: (1) near-misses are more frequent and thus statistically tractable; (2) they reveal systemic failure modes before harm materialises; (3) they require confidentiality protections incompatible with mandatory public disclosure regimes. The US Aviation Safety Reporting System (ASRS) is cited as the canonical near-miss architecture: non-punitive, non-attributable, federally protected, generating ~100,000 annual reports with demonstrated safety outcomes.

### The Dual-Goal Tension and Two-Track Resolution

Accountability-oriented regimes (mandatory, public, attributed) suppress learning-oriented reporting. The paper proposes a two-track architecture:
- **Track A (mandatory/attributed):** Harm-materialised incidents above defined severity threshold → public database, regulatory review, potential enforcement
- **Track B (voluntary/non-attributed):** Near-misses and anomalies → confidential, immunity-protected, learning-focused system

This architecture requires institutional separation: Track A under the enforcement regulator; Track B under an independent safety analysis body.

---

## Implications for Indian Governance Context

**Corrected 2026-07-31 (see VERIFY #182 resolution) — India has no *dedicated, AI-specific* AIIRS, but does have a binding, general-cyber regime that explicitly names AI/ML as reportable.** The original framing below ("India has no AIIRS framework") overstated the gap; CERT-In's April 2022 Direction 70B, Annexure I, explicitly lists AI/ML-related incidents as a mandatory-reportable category — a binding obligation in force since 2022. What India genuinely lacks is a **dedicated AI-specific AIIRS with near-miss/learning-track infrastructure** (Track B in this paper's framework), not a binding reporting obligation covering AI incidents at all. Existing reporting regimes remain exclusively Track A (harm-materialised) and do not provide near-miss infrastructure:
- **DPDP Act 2023 S.8(6):** Data breach reporting — harm-materialised only
- **RBI IT/Cyber Risk Master Directions:** Mandatory cyber incident reporting for regulated entities — punitive, attributed, no near-miss provision
- **CERT-In Direction 2022 (70B):** 6-hour reporting window for listed incident categories, **explicitly including AI/ML-related incidents (Annexure I)** — enforcement-oriented, antithetical to voluntary near-miss culture, but genuinely AI-inclusive, not merely AI-adjacent
- **Gap significance for PRIS, sharpened:** India's gap is specifically the **absence of a dedicated AI-specific AIIRS with near-miss/learning-track (Track B) infrastructure** — not a binary presence/absence of AI incident reporting altogether. This is a more precise, more defensible **Governance Capacity** gap and **Evaluative Authority** deficit claim for the fsQCA framework than the original "no AIIRS" framing, and it strengthens rather than weakens the underlying [[Regulatory_Parallelism]] argument: CERT-In's general-cyber mandate covering AI incidentally, alongside RBI/SEBI's separate reporting requirements, is itself a parallelism pattern (multiple regulators each partially covering AI incident reporting without a dedicated, coordinated AIIRS).

---

## Connections to Research

**[[P1_SLR_RG]]:** Core institutional design literature for AI safety reporting; covers both S1 (governance frameworks) and S6 (implementation and operationalisation). One of the strongest methodological papers in Batch 15.

**[[fsQCA_Thesis_Chapter]]:** Directly relevant to **EA condition** (Evaluative Authority). AIIRS is a core EA mechanism; cross-jurisdictional variation in AIIRS design — dual-track vs. single-track, mandatory vs. voluntary, immunity provision present/absent — generates configurational variation relevant to outcome analysis.

**[[P3_BFSI_JEIM]]:** Absence of AIIRS in India is a concrete governance gap finding.

**Concept links:**
- [[Governance_Capacity]] — AIIRS requires institutional capacity (technical causal analysis, database infrastructure, multi-actor coordination) that low-capacity regulators cannot implement at full seven-dimension specification
- [[Accountability]] — the learning/accountability dual-goal tension is a direct application; non-attribution vs. transparency trade-off is a live design problem
- [[Transparency]] — Track A vs. Track B maps onto deliberative vs. procedural transparency distinctions
- [[Regulatory_Parallelism]] — multi-actor reporting scope (developer/deployer/user) across overlapping regulators creates RP-compounding risk; single-window AIIRS architecture is a partial RP mitigation
- [[Institutional_Coherence]] — cross-border AI incidents require interoperable national AIIRS; IC condition failure mode where national systems are non-interoperable

**Related nodes:**
- [[07_Institutions/Corpus/CERT_In/CERT_In_2]] — contrast: CERT-In mandatory/punitive space-sector reporting vs. AIIRS voluntary near-miss architecture
- [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations|F041]] (AEF-1) — complementary: pre-deployment evaluation vs. post-deployment incident reporting as sequential governance layers
- [[07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool|International_20]] (DTA AIIA) — pre-deployment governance instrument; together with F051 defines pre/post-deployment governance lifecycle

---

## VERIFY Flags

**#182 — RESOLVED WITH CORRECTION (2026-07-31, Perplexity Deep Research), Medium-High confidence.** The paper's (and this node's) "only two binding regimes" framing needs revision:

- **EU AI Act (Art. 73):** confirmed still on track. Serious-incident reporting for GPAI providers already applies from August 2025; full Article 73 obligations for Annex III standalone high-risk systems are now deferred to **December 2027** (pushed from the original August 2026 date via the Digital Omnibus — see [[07_Institutions/Corpus/International/International_22_EU_AI_Act_Conformity_Assessment_Notified_Bodies]] VERIFY #226), with Annex I-embedded systems deferred further to August 2028. The European Commission opened a draft-guidance/reporting-template consultation (26 Sept–7 Nov 2025) to operationalise Art. 73.
- **India — CERT-In (the biggest correction):** India already has a binding, mandatory cyber-incident reporting regime that **explicitly names AI/ML systems** as a reportable category. CERT-In's April 2022 directive (70B) requires mandatory reporting of cyber incidents within 6 hours, and its incident taxonomy (Annexure I) explicitly lists "Attacks or malicious/suspicious activities affecting systems/servers/software/applications related to Artificial Intelligence and Machine Learning" as reportable. **India has had a binding, AI-inclusive incident-reporting obligation in force since 2022** — well before this paper's two-regime premise — though framed as a general cybersecurity directive rather than an AI-specific statute.
- **UK DSIT:** as of a late-2024 policy analysis, the UK still lacks a dedicated AI incident reporting framework — explicitly flagged as "a gap that DSIT should urgently address." The UK instead co-published the International AI Safety Report 2026 (3 Feb 2026) as a scientific/advisory document, not a binding regime. No binding UK AIIRS as of this query date.
- **Singapore MAS:** no dedicated binding AI-incident-reporting mandate found; MAS's MindForge Handbook (see [[04_Knowledge_Products/Wiki_Intake/MindForge_MAS_AI_Risk_Management_Executive_Handbook|F054]]) is risk-management guidance, not an incident-reporting law.

**Corrected picture:** China (GPAI incident reporting) and the EU AI Act (Art. 73, partially phased in since Aug 2025, full high-risk obligations deferred to Dec 2027/Aug 2028) remain the most comprehensive **dedicated, AI-specific** regimes. But India's CERT-In directive already constitutes a binding, AI-inclusive incident-reporting mandate since 2022 via its general cybersecurity framework, the UK has no binding regime, and Singapore's MAS framework is guidance only. **Recommended framing going forward: distinguish "AI-specific dedicated" regimes (EU, China) from "general cyber regimes that explicitly cover AI" (India/CERT-In)** — this is a real, useful distinction for P3's Regulatory_Parallelism argument, not a reason to treat India as having "no AIIRS" (see correction to Implications section below).

---

*Node written: 2026-07-14 | Batch 15 continuation (rescued from staging; renumbered from staged F049 → F051) | PRIS v2.2*
