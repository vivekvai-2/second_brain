---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S3
  - section/S5
  - tier/high-medium
  - project/p1
  - project/p3
  - project/p4
  - project/fsqca
  - engine/phd
---

# Paladin Global Institute: The AI Tech Stack — A Policy Primer (2025)

**Node ID:** F052
**Type:** Wiki Intake Note (Format B)
**Wiki Section:** S3 (International Regulatory Context) / S5 (Data, Privacy & Security)
**Status:** Active
**Tier:** High-Medium
**Last Updated:** 2026-07-14 (Batch 15 continuation)

---

## Source

**Full Citation (APA):** Walden, K., & Lynch, D. (2025). *The AI tech stack: A policy primer.* Paladin Global Institute. *(Author name corrected 2026-07-31 — co-author is **Devin Lynch**, not "Chris Lynch" as originally recorded; see VERIFY #183 resolution.)*
**Document Type:** Policy primer / practitioner brief
**Issuing Institution:** Paladin Global Institute
**Batch:** 15 (continuation) | **Batch marker:** ⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕⊕
**Source corpus:** Policy Dump Future

---

## Summary

Walden and Lynch provide a layered decomposition of the AI technology stack — from compute (semiconductors, data centres) through model development (training, fine-tuning, RLHF) to application and deployment layers — framed as a structured policy primer for national security and governance audiences unfamiliar with the technical substrate. The document's primary governance argument is that AI regulation must be *layer-aware*: interventions calibrated to the compute layer (export controls, chip restrictions) have fundamentally different governance implications than interventions at the model layer (safety evaluations, frontier model licensing) or application layer (sector-specific deployment standards). Conflation of layers in regulatory design produces both over-regulation at the application level and under-regulation at the compute/model levels.

**#183 — RESOLVED (2026-07-31, Perplexity Deep Research).** See full resolution in VERIFY Flags section below.

---

## Key Findings and Framework

### Three-Layer AI Stack Decomposition

**Layer 1 — Compute Infrastructure**
- Semiconductors (GPUs, TPUs, custom AI accelerators): US-designed, primarily Taiwan-fabricated (TSMC), with South Korea secondary
- Data centres: physical infrastructure, power requirements, cooling, geographic concentration
- Cloud compute: hyperscaler concentration (AWS, Azure, GCP) creates single-point-of-failure governance risks
- *Policy leverage points:* Export controls (BIS Entity List, CHIPS Act), data centre FDI screening, cloud provider security requirements

**Layer 2 — Model Development**
- Foundation model training: compute-intensive, data-intensive, increasingly concentrated among frontier labs
- Fine-tuning and adaptation: lower compute threshold; widely accessible; enables regulatory arbitrage
- RLHF and alignment techniques: post-training safety modifications; not externally verifiable without audit
- *Policy leverage points:* Frontier model licensing, compute thresholds for reporting requirements, mandatory safety evaluations pre-deployment, model registries

**Layer 3 — Application and Deployment**
- Application APIs: downstream developer access to foundation model capabilities
- End-user applications: consumer-facing products with direct harm potential
- Sector-specific deployments: healthcare, financial services, critical infrastructure, defence
- *Policy leverage points:* Sector-specific regulations, use-case restrictions, algorithmic impact assessments, liability frameworks

### Layer-Specific Regulatory Implications

| Layer | Primary Risk | Governance Mechanism | Jurisdictional Complexity |
|-------|-------------|---------------------|--------------------------|
| Compute | Strategic resource concentration; export to adversarial actors | Export controls; FDI screening | High — cross-border supply chains |
| Model | Dual-use capability proliferation; misalignment | Licensing; evaluations; incident reporting | Medium — frontier lab concentration in US/UK |
| Application | Discriminatory outcomes; operational failures; misuse | Sector regulations; liability; AIA | Low — jurisdiction-of-deployment primary |

### National Security Frame

The primer frames AI governance through a national security lens: compute and model layer controls are cast as strategic/foreign policy instruments (analogous to nuclear non-proliferation); application layer standards are domestic regulatory instruments. This layer-separation argument supports a governance architecture in which export controls (Commerce/USTR) operate independently from, but in coordination with, domestic AI safety regulation (NIST/AISI).

---

## Relevance to Indian Context

The Paladin primer is primarily US-centric, but the layer-decomposition framework is directly applicable to India's AI governance architecture:
- **Compute layer:** India's Chips to Startup (C2S) programme, IndiaAI Compute Initiative, and semiconductor policy (SemiconIndia Programme) address layer 1 but without explicit AI-governance integration
- **Model layer:** MeitY's AI governance framework (Advisory for Responsible Development and Deployment, March 2024) operates at Layer 3 (application/deployment); no Layer 2 equivalent (frontier model evaluation, model registry) exists
- **Gap:** India has no model-layer governance mechanism — the policy gaps identified by Paladin for the US context are more acute in India's case given compute dependency on foreign hyperscalers
- **fsQCA relevance:** SR condition (Structural Readiness) — layer-aware vs. layer-blind regulatory architecture is a structural readiness dimension

---

## Connections to Research

**[[P1_SLR_RG]]:** S3 (international frameworks) and S5 (technology and infrastructure) — provides technical vocabulary and layer-decomposition model that anchors literature on compute governance and export controls.

**[[fsQCA_Thesis_Chapter]]:** Relevant to **SR condition** (Structural Readiness) — layer-aware regulatory architecture is a structural readiness indicator; jurisdictions with only application-layer governance score lower on SR.

**[[P2_DPI_JSIS]]:** Indirect — IndiaAI's cloud compute acquisition for government AI deployments is a Layer 1 governance question that intersects DPI infrastructure.

**Concept links:**
- [[Governance_Capacity]] — layer-aware governance requires technical capacity to assess each layer's risks independently; capacity-poor regulators default to application-layer only
- [[Institutional_Coherence]] — layer-separated governance bodies (export controls regulator vs. AI safety regulator vs. sector regulator) require coordination mechanisms to avoid contradictory interventions
- [[Regulatory_Parallelism]] — compute/model/application layer governance involves different ministries and agencies; RP risk is high at layer boundaries

**Related nodes:**
- [[04_Knowledge_Products/Wiki_Intake/F041_AEF1_Minimum_Operating_Conditions_AI_Evaluations|F041]] (AEF-1) — complementary at model layer: evaluation standards operate at Layer 2
- [[07_Institutions/Corpus/CERT_In/CERT_In_2]] — CERT-In space cybersecurity framework operates at Layer 3 (application/deployment) in satellite domain
- [[07_Institutions/Corpus/International/International_20_Australia_DTA_AI_Impact_Assessment_Tool|International_20]] — Layer 3 government-as-deployer instrument

---

## VERIFY Flags

**#183 — RESOLVED (2026-07-31, Perplexity Deep Research).** **Name correction, High confidence:** the co-author is **Devin Lynch**, not "Chris Lynch" — the original tracker entry contained a name error, now corrected in the citation above. Devin Lynch is Senior Director of the Paladin Global Institute, and previously served as Director for Cyber Policy and Strategy Implementation at the Office of the National Cyber Director (ONCD) — consistent with Kemba Walden's own prior ONCD role (Acting US National Cyber Director, Biden administration), suggesting both co-authors moved from ONCD to Paladin. **Update confirmed, High confidence:** the Institute released a 2026 follow-up primer, **"The Governance Layer: A Primer for Tech and Cyber Policy"** (published 8 June 2026), which explicitly builds on this 2025 "AI Tech Stack" primer — a strong candidate for its own future F-series corpus node, cross-linked back to this one (F052).

---

*Node written: 2026-07-14 | Batch 15 continuation (rescued from staging; renumbered from staged F050 → F052) | PRIS v2.2*
