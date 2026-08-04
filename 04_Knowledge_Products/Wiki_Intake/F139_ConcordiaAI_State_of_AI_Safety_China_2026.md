---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - source/grey-literature
  - source/longitudinal-series
  - content/wiki-entry
  - gate/open
  - section/S3
  - topic/china
  - topic/comparative-regulation
  - topic/agentic-ai
  - paper/p1
  - paper/p4
  - paper/fsqca
---

# State of AI Safety in China (Concordia AI, 2026) — Intake Note

**Source:** Concordia AI (安远 AI), a social enterprise working on AI safety in China
**Authors:** Gabriel Wagner, Erik Lindblad, Kwan Yee Ng, Brian Tse
**Year:** July 2026 (fourth edition; series began 2023)
**Coverage period:** July 2025 – June 2026
**File ID:** F139
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S3 (International Regulatory Context)
**Confidence:** Medium-High — well-sourced to primary Chinese-language instruments with full citation apparatus; grey literature with a prominently disclosed conflict of interest
**Jurisdiction:** China
**Companion site:** aisafetychina.com (interactive policy-risk matrix, research database, key research groups)

---

## Why This Node Exists Alongside F137 and International_21

Three China nodes now sit in the vault and they do different work. Do not treat them as substitutes.

| Node | Type | Function |
|---|---|---|
| [[07_Institutions/Corpus/International/International_21_China_CAC_GenAI_Interim_Measures_2023]] | Corpus node, primary instrument | The 2023 GenAI Interim Measures themselves — ADICO-codeable primary text |
| [[04_Knowledge_Products/Wiki_Intake/F137_LeoneDeCastris_Jiang_Wang_AI_Governance_China_2026]] | Country profile, single snapshot | Turing Institute structural overview of China's regulatory architecture |
| **F139 (this note)** | **Longitudinal annual series, 4th edition** | **Year-on-year change across five domains: domestic governance, international governance, technical research, expert views, industry governance** |

F139 is the only node in the vault that tracks *any* jurisdiction over time. That is its distinct value: it supports claims about regulatory trajectory and velocity, not just regulatory state. It also **corrects** a claim in F137 — see below.

---

## Classification

**Document type:** Annual research report / longitudinal jurisdiction tracker (grey literature)
**Primary audience:** Researchers, policymakers, international coordination practitioners
**AI explicit:** Yes
**PRIS role:** Primary evidence for [[China_AI_Governance]]; correction source for [[04_Knowledge_Products/Wiki_Intake/F137_LeoneDeCastris_Jiang_Wang_AI_Governance_China_2026]]; second-jurisdiction instance for [[Assurance_Reuse_Gap]]; convergence evidence for [[Agentic_AI_Governance]]
**IG 2.0 status:** Secondary source. Not codeable. Its value is as a **map to primary instruments** — the footnote apparatus cites original Chinese-language sources with URLs, making it an efficient sourcing route to codeable texts.

---

## Reusable Findings

### 1. Content control → action control (the headline finding)

China's governance framework pivoted from regulating **what AI says** to regulating **what AI does**. The trigger was concrete and datable: the open-source agent **OpenClaw** proliferated through China's developer community in February 2026, prompting warnings from the National Vulnerability Database, CNCERT, and the Ministry of State Security; NIFA advised financial institutions not to deploy it on business terminals; the MSS guidance passed a million views on RedNote. In May 2026 the CAC and two other agencies issued dedicated agentic-AI guidance devoting a full chapter to safety and proposing risk-based governance with filing-and-testing for high-risk domains.

**This converges independently with [[SAIL_Secure_AI_Lifecycle]].** See *Convergence* section below — this is the most analytically valuable item in the document.

### 2. Two mandatory national AI standards — a finer-grained RL signal

China's AI standards are overwhelmingly **recommended**, not mandatory. As of June 2026 there are exactly two mandatory national AI standards:

- AI-generated content labelling (2025)
- **General Security Requirements for AI Agent Applications** — announced April 2026, would be the second

That binding-ness varies *at standard level within a single jurisdiction* is a more granular Regulatory Logic measure than the instrument-level binary currently used in [[fsQCA_Thesis_Chapter]]. The fact that the second-ever mandatory AI standard is an agent standard is itself a signal about where Beijing places the risk.

### 3. Ethics review with pre-R&D temporal scope

MIIT's March 2026 *Administrative Measures for the Ethical Review and Services of AI Science and Technology (Trial)* require universities, research institutes and companies to establish and **register** ethics review committees, reviewing against six dimensions. Three categories of high-risk project trigger mandatory second-round review by a government-assigned expert panel.

**The notable feature is temporal:** review is required *before R&D begins* — in principle before pre-training — rather than before deployment, as under the CAC algorithm registry. Institutions may outsource review to "AI ethics service centers," with CAICT, CESI and CEPREI positioning to provide them. Ten-province implementation pilot running June–November 2026.

### 4. Anthropomorphic AI regulation as registry extension

The *Interim Measures on Anthropomorphic AI Interaction Services* (effective 15 July 2026) impose obligations around suicide intervention, dependency monitoring, guardian contact in high-risk situations, and a mandatory stricter "minor mode." Governance-design point: these obligations **layer on top of** the existing algorithm registry rather than creating a parallel regime — the registry as extensible base layer. The official Chinese explanation cites EU and California legislation directly, which the report reads as room for mutual learning.

### 5. Frontier risk entering standards vocabulary

CBRN misuse appeared in a Chinese national standard for the first time (GB/T 46347-2025, Appendix B). TC260's Safety Governance Framework 2.0 adds "derivative risks" as a third risk class, introduces "catastrophic" terminology absent from V1.0, and proposes **"circuit breakers" and "safety stop switches"** for autonomous systems. Xi Jinping and Li Qiang have both publicly referenced "risks of technological loss of control." The report is careful that concrete requirements remain limited — the vocabulary is moving faster than the obligations.

### 6. Multilateral positioning as the US withdraws

China backed two new UN mechanisms (Independent International Scientific Panel on AI; Global Dialogue on AI Governance), had two experts appointed to the IISP-AI, and proposed a **World AI Cooperation Organization** with Shanghai floated as headquarters. The US voted against the Secretary-General's IISP-AI appointments. A China–US intergovernmental AI dialogue was announced in May 2026, ending a two-year freeze. Both appointed Chinese experts are oriented toward application and diffusion rather than safety — the report flags this as potentially shaping panel dynamics.

### 7. Industry disclosure lags Western peers

Only five of ten leading Chinese foundation-model developers reported safety evaluation results alongside *any* release in the year surveyed, and none did so consistently. DeepSeek-R1's Nature paper (10-page safety appendix, full risk-review prompt disclosed) and Moonshot's Kimi K2 card were the most detailed to date — yet DeepSeek-V4 and Kimi K2.5 shipped with **no safety evaluation results at all**. Given that Chinese open-weight models now lead Hugging Face downloads, this is a global governance question, not a domestic one.

---

## Convergence: Action Control Across Adversarial Jurisdictions

Two documents intaked into PRIS within four days, from actors with no relationship and opposite starting points, describe the same conceptual pivot:

| | [[SAIL_Secure_AI_Lifecycle]] | F139 (China) |
|---|---|---|
| **Actor** | Pillar Security — US commercial AI security vendor | CAC, TC260, MIIT — Chinese state regulators and standards bodies |
| **Baseline being left** | **Access** control — authorising sessions and identities | **Content** control — regulating what models say |
| **Destination** | Action control — authorising every discrete action | Action control — governing what agents do |
| **Trigger** | Enterprise agentic deployment | OpenClaw proliferation, Feb 2026 |
| **Date** | June 2026 | May–June 2026 |

Neither cites the other. The mechanisms proposed rhyme closely: TC260's eleven agent threats (Table 1.2) map substantially onto SAIL's risk catalogue — agent hijacking, identity spoofing and privilege escalation, tool abuse, memory manipulation, multi-agent cascading failure. Both propose agent IDs; both propose least-privilege tool scoping; both propose human confirmation for high-risk operations.

**Why this is analytically strong.** Convergence between a market actor and a state regulator, across a geopolitical divide, from different baselines, in the same quarter, is much harder to explain away as diffusion or copying than convergence between allied jurisdictions. It suggests the pivot is driven by the technology's properties rather than by policy transfer.

**India is absent from both.** Neither document references Indian instruments, and no Indian regulator has issued agent-specific guidance. Recorded in [[Agentic_AI_Governance]]; see that note for the framing.

⚠ Before building on this: verify the CAC May 2026 guidance and the TC260 March 2026 research report as primary sources. Both are cited with URLs in this report's notes (refs 16 and 54). A convergence claim resting on two secondary characterisations is weaker than one resting on the instruments themselves.

---

## Corrections to Existing Vault Claims

**[[04_Knowledge_Products/Wiki_Intake/F137_LeoneDeCastris_Jiang_Wang_AI_Governance_China_2026]] — "single-coordinator" framing is overstated.** F137's cross-link describes "China's single-coordinator departmental-rule model" contrasting with "India's multi-regulator parallelism pattern." F139 documents **three standards bodies drafting overlapping agent-security standards simultaneously** — TC260/WG9, MIIT/TC1/WG8, and TC28/SC42 — and states directly: *"There is some uncertainty about how TC260 will coordinate these efforts with other standard-setting bodies. For example, MIIT/TC1 is also working on multiple related standards."* That is [[Regulatory_Parallelism]] inside a centralised system. The India/China contrast survives in weakened form — different *degree*, not different *kind*.

**[[Assurance_Reuse_Gap]] — first non-Indian instance.** The unresolved relationship between MIIT's ethics-review regime and the CAC algorithm registry is your construct in a second jurisdiction: two authorities imposing review obligations on the same capability, with cross-recognition uncertain. Article 26 hints at second-round exemption for algorithm-registered systems, but implementation is unclear pending the pilot. This matters because the construct's evidence base is currently India-only, which limits its generalisability claim.

**[[Institutional_Coherence]] — coherence and parallelism in the same document.** TC260's WG9 deliberately seats CNCERT, CAICT, the MPS Third Research Institute and CNITSEC under a Shanghai AI Lab chair — coherence by institutional design, structurally similar to IRDAI's WG-AI composition. Yet the same body's work duplicates MIIT/TC1's. Coordination at the committee level does not produce coordination at the output level.

---

## Citation Hygiene

| Flag | Issue | Handling |
|---|---|---|
| **Conflict of interest** | Concordia AI advises Chinese AI developers, hosts forums, and has received consulting fees from companies discussed in the report | Fully and prominently disclosed by the authors, including a statement that no government or government-affiliated organisation provided input. Cite with the disclosure noted |
| **Self-referential sourcing** | Concordia co-authored several sources it cites — the Shanghai AI Lab *Frontier AI Risk Management Framework*, the Tianjin University AI×life-sciences report — and CEO Brian Tse is a signatory to statements the report covers | Disclosed in footnotes. Where the report is the *only* source for its own outputs, treat as self-report |
| **LLM-based classification** | Chapter 3 and 5 quantitative claims rest on LLM classification (Claude Sonnet) of paper titles/abstracts, with ~20% manual spot-checking. Full prompts are published in the footnotes | Methodologically transparent — unusually so. But the percentages are model-assigned, not human-coded. Cite the *direction*, not the decimal |
| **Year-over-year non-comparability** | The "key research groups" threshold was tightened between editions (3 papers → 5 papers per anchor author). The authors state explicitly the counts are **not directly comparable** to the 2025 report | Do not construct a growth series from group counts across editions. The paper-volume series is comparable; the group counts are not |
| **Selection is avowedly partial** | The authors state they cover frontier risks in greater depth than other risks, that this "reflects our own vantage point rather than their relative priority within the Chinese ecosystem," and that topic selection is not exhaustive | Unusually honest scoping. Do not read the report's emphasis as China's emphasis |

Note the report's own frame: it takes its risk taxonomy from the *International AI Safety Report* (Bengio et al., 2026), which is the more citable upstream source for taxonomy purposes.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S3
**Frameworks:** [[China_AI_Governance]] (created from this document) | [[EU_AI_Act]] | [[NIST_AI_RMF]] | [[ISO_IEC_42001]] | [[SAIL_Secure_AI_Lifecycle]] | [[IndiaAI_Framework]]
**Concepts:** [[Agentic_AI_Governance]] | [[Assurance_Reuse_Gap]] | [[Institutional_Coherence]] | [[Regulatory_Parallelism]] | [[Human_Oversight]] | [[Governance_Capacity]]
**Corpus nodes:** [[07_Institutions/Corpus/International/International_21_China_CAC_GenAI_Interim_Measures_2023]]
**Adjacent intake:** [[04_Knowledge_Products/Wiki_Intake/F137_LeoneDeCastris_Jiang_Wang_AI_Governance_China_2026]] (corrected by this note) | [[04_Knowledge_Products/Wiki_Intake/F133_Trout_et_al_AI_Insurance_Stack_2026]]
**Domains:** [[03_Domains/International_Comparators]] | [[03_Domains/AI_Governance]] | [[03_Domains/Cybersecurity_Governance]]
**Projects:** [[P1_SLR_RG]] | [[P4_Doctrinal_IJLIT]] | [[fsQCA_Thesis_Chapter]]

---

## Sourcing Leads (primary instruments worth ingesting)

The footnote apparatus is the most useful part of this document for corpus-building. High-value primary targets:

- CAC et al., *Implementation Opinions on the Standardised Application and Innovative Development of AI Agents* (May 2026) — ref 16
- TC260, *Cybersecurity Standardization Research Report — Agent Safety Standardization* (Mar 2026), the eleven-threat taxonomy — ref 54
- CAC et al., *Interim Measures on Anthropomorphic AI Interaction Services* (Apr 2026, effective 15 Jul 2026) — ref 23
- MIIT et al., *Measures for Ethical Review and Services of AI S&T (Trial)* (Mar 2026) — ref 25
- TC260, *AI Safety Governance Framework 2.0* (Sep 2025) — ref 99
- GB/T 46347-2025, *AI Risk Management Capability Assessment* (first CBRN mention in a Chinese national standard) — ref 51

---

## Monitoring

This is an annual series with a stable structure — it is a **standing watch item**, not a one-off. Next edition expected ~July 2027.

Near-term dated items from the report:

- Global Dialogue on AI Governance, Geneva, 6–7 July 2026 (IISP-AI first annual report released same event)
- MIIT ethics-review pilot concludes November 2026; ≥5 implementation standards expected
- APEC Leaders' Meeting, Shenzhen, November 2026 — China-hosted, AI on agenda
- G20 Miami, December 2026 — US-hosted, AI a focus
- Mandatory *General Security Requirements for AI Agent Applications* — trajectory to watch

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [x] Linked to concept notes
- [x] Corrections pushed downstream
- [ ] Wiki sections updated
- [ ] Marked processed

---

## Log

- 2026-08-04: Intake note created from full-text pass. Pre-flight duplicate check against `Corpus_Index_MOC.md` and `04_Knowledge_Products/Wiki_Intake/` (searched "China", "Concordia", "TC260", "CAC", "State of AI Safety") found two adjacent nodes — F137 (Turing country profile) and International_21 (CAC 2023 Measures) — neither a duplicate; distinct roles documented above. **File ID note:** F138 was already taken (`F138_GoogleDeepMind_AI_Control_Roadmap_2026`); assigned F139. Three corrections pushed downstream. Action-control convergence with [[SAIL_Secure_AI_Lifecycle]] recorded in [[Agentic_AI_Governance]]. [[China_AI_Governance]] framework node created, closing the comparator gap where `International_21` was tagged `project/fsqca` with no framework node behind it. Not yet added to `Corpus_Index_MOC.md` batch table — pending batch numbering confirmation.
