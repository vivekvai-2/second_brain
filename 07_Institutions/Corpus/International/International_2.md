---
type: Corpus Node
status: active
last_updated: 2026-07-21
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/global
  - institution/international
---

# International_2 — BIS: Generative Artificial Intelligence and Cyber Security in Central Banking

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/International/International_2.md`
**Institution:** [[07_Institutions/International]] (Bank for International Settlements)
**Issuing body:** Bank for International Settlements, Monetary and Economic Department (BIS Papers No. 145)
**Document date:** May 2024
**Pages:** Not fully determinable
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/Cybersecurity_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** Generative artificial intelligence and cyber security in central banking (BIS Papers No. 145)
**Type:** Research Paper (survey-based, non-binding)
**Target entities:** Central banks (cyber security functions)
**Legal basis:** BIS research publication — views are authors' own, not official BIS positions
**Authors:** Iñaki Aldasoro, Sebastian Doerr, Leonardo Gambacorta, Sukhvir Notra, Tommaso Oliviero, David Whyte
**Companion documents:** [[07_Institutions/Corpus/International/International_1]] (OECD Gen AI risk taxonomy); [[07_Institutions/Corpus/CERT_In/CERT_2]] (GenAI Best Practices, India)

---

## Analytical Classification

**Wiki section:** S5 (Data, Privacy & Security) — feeds the "threat landscapes" gap identified for S5
**Jurisdiction:** Global (central banking community)
**Confidence:** Medium (survey-based research, not a binding standard)
**AI explicit:** Yes (Generative AI specifically)
**Tier classification:** Tier C — AI-adjacent governance (research evidence base for future policy)
**AI Governance Wiki relevance:** MEDIUM — provides empirical (survey) evidence of central-bank gen AI adoption intentions and risk perceptions, useful for benchmarking RBI's own survey findings in FREE-AI Committee Report.

---

## Substantive Content

### Survey-based findings
Based on a survey of cyber security experts at major central banks:
- Most central banks have **already adopted or plan to adopt** gen AI tools for cyber security, with perceived benefits outweighing risks.
- Experts foresee gen AI **improving cyber threat detection** and **reducing response time** to cyber attacks.
- Gen AI simultaneously **increases risks** of: (a) social engineering attacks (AI-enhanced phishing/deepfake-based attacks), and (b) unauthorised data disclosure (e.g., through gen AI tool usage leaking sensitive information).

### Human capital implications
To mitigate risks and capture benefits, central banks anticipate needing **substantial investment in human capital** — specifically staff with combined expertise in cyber security AND AI/programming (a dual-skill profile). Respondents expect gen AI to automate routine tasks while also **supporting human experts in oversight roles** — i.e., gen AI augments rather than replaces human oversight of AI models, a "human-in-the-loop for AI oversight of AI" framing.

---

## ⚠ 2026-07-15 Enrichment — Granular Detail from Second Independent Extraction Pass

*One-time exception to the session's flag-only-on-duplicate rule, per explicit user instruction. The following adds the granular figures, taxonomies, and quotes the original Batch 3 (2026-06-14) intake did not capture.*

### Survey Methodology and Institutional Context
- Survey conducted **January 2024** among members of the **Global Cyber Resilience Group (GCRG)**; **32 respondents**.
- GCRG sits within the **Cyber Resilience Coordination Centre (CRCC)**, established **2019**, comprising experts from **58 BIS member central banks** — a global cyber-resilience collaboration platform with over 300 active security professionals.
- Contemporaneous context: a **March 2024 US Department of the Treasury report** independently flagged generative AI as an emerging critical aspect of financial-sector cyber security — an external corroboration of this paper's central finding, arriving two months after the GCRG survey closed.
- Four survey design pillars: (1) current adoption status, (2) benefit/challenge evaluation, (3) preparedness for the "AI revolution", (4) key strategic/ethical/regulatory concerns.

### Adoption Figures (Section 3)
- **71%** of respondents already using gen AI; **26%** plan to incorporate it within 1–2 years.
- Formal integration strategy: only **19%** have one; **23%** do not; **55%** report it "in development."
- Net benefit-vs-risk assessment: **19%** completely agree gen AI provides more benefit than risk, **56%** partially agree, **19%** neutral, **6%** partially/completely disagree.
- Perceived benefit dimensions: cyber threat detection (**57%**), summarising documents/meeting notes (**43%**), drafting emails/documents (**36%**).

### Effectiveness and Risk Ratings (Section 4)
- Effectiveness for cyber defence: **44%** rate gen AI "very effective" or "effective"; **41%** "moderately effective"; only **3%** "not very effective" (13% abstained).
- Impact rating (1–10 scale): ~25% rate 5–6; **>45%** rate 7–8; **11%** rate 9–10; 7% rate ≤2 — a strongly right-skewed distribution toward positive impact.
- **Risk rating is the paper's sharpest figure: 96% of respondents rated implementation risk 5 or higher on a 1(low)–10(high) scale** — i.e., near-universal acknowledgment of material risk *despite* the majority-positive effectiveness ratings above. This benefit/risk co-existence (high perceived value AND high perceived risk, simultaneously) is the paper's core empirical tension.
- Risk/challenge taxonomy (Graph 3.A — vulnerabilities AI systems introduce): model theft, dependence on data, adversarial attacks, data poisoning, automated propagation, black-box algorithms, privacy issues, unauthorised data disclosure, social engineering.
- Challenge taxonomy (Graph 3.B — challenges for existing cyber security systems): high initial costs, compatibility issues, data quality/availability, ethical/privacy concerns, understanding AI decisions, security of AI systems, skill gap.

### IT Investment and Human Capital (Section 5)
- Cloud-based gen AI access: only **3%** of central banks allow unrestricted staff access; **13%** plan to implement soon; **9%** have no plans to enable it.
- Staff-preparedness concern: **40%** report high/extreme concern; **35%** moderate; **15%** slight; effectively none unconcerned.
- Named tools referenced: ChatGPT, Claude, Bard, Copilot, Midjourney (general-purpose); Siri, Alexa (assistant baseline); **FraudGPT, WormGPT** (named malicious/offensive gen AI tools — direct evidence base for the offensive-use taxonomy below).

### Definitions and Taxonomies (Section 2)
- **Machine learning:** "a set of techniques designed to extract information from data, with a view to making predictions."
- **Training:** "the process of fitting a machine learning model to data."
- **Neural networks:** built from artificial neurons "which take multiple input values and transform them in a non-linear way to output a single number"; **depth** = number of layers; **parameters** = weights/biases determining connection strength.
- **Transformers** (unveiled 2017): models that "attempt to capture the relationship between the different components of a text sequence, even if they are far apart in the paragraph or document" — the architecture underlying ChatGPT-class tools.
- **Offensive-use taxonomy (cyber threat actors' uses of gen AI):** (i) social engineering techniques, (ii) malware/code generation, (iii) disinformation.
- **AI-system-targeted risk taxonomy:** (i) data/model poisoning, (ii) data leakage during inference, (iii) vulnerability discovery.
- **Cyber resilience** (Section 6 definition): "the capacity of central banks to foresee, adapt to and swiftly recover from cyber incidents while continuing their essential operations."
- **Ethical/regulatory concerns taxonomy (Graph 5.A):** intellectual property rights, bias and discrimination, compliance with international laws, consent and transparency, accountability for AI actions, data protection and privacy, autonomous decision-making.
- **Crucial human roles taxonomy (Graph 5.B):** AI ethicists, compliance officers, AI developers/engineers, AI security analysts, AI supervisors, data scientists — a named role taxonomy directly relevant to any AI-governance organisational-design/RACI work (cf. [[04_Knowledge_Products/Wiki_Intake/F079_AgilityAtScale_RACI_Matrix_AI_Accountability_2026]]).

### Key Quotes
- "There is a strong consensus on the adoption of common rules for the use of AI for cyber security, and a recognition that new forms of cooperation at the central bank level are needed."
- "Such collaborative efforts should address the establishment of new data protection standards to ensure the responsible implementation of gen AI and, crucially, tackle the issue of the 'Skill gap' among human personnel."
- "Cooperation and information-sharing are key to collectively reducing cyber risk and preventing and containing major cyber incidents."
- "An implication is that introducing internal practices and common regulatory policies might be necessary for a safe and widespread adoption of gen AI tools in central banks."

### 2020 ESG/ISSA Corroborating Statistic (background, cited by the paper)
A 2020 Enterprise Strategy Group/Information Systems Security Association report found **70%** of cyber security professionals reported a skills shortage and **>60%** reported security positions vacant ≥3 months — cited by the paper as the pre-existing skills-shortage baseline the gen AI skill-gap finding compounds, not a new finding of this paper itself.

---

## Analytical Significance for PRIS Research

### For P3/fsQCA and Governance Capacity concept
This paper provides a direct **comparator data point** to RBI FREE-AI's domestic survey (20.8% AI adoption across 612 REs, low adoption among smaller institutions). The BIS survey of central banks (a more sophisticated institutional population than commercial REs) shows near-universal gen AI adoption intent specifically for cyber security — suggesting a **capability gradient**: central banks (regulators) may be adopting gen AI for their own operations faster than the regulated entities they supervise are adopting AI generally. This is relevant to the [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] construct — regulators' own AI capacity may outpace their regulatory frameworks for supervising AI in regulated entities.

### Coordination / Parallelism Pattern
Existing node: [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]]. Pattern: **Unpaired** — no evidence RBI's FREE-AI survey addressed RBI's own (central bank) internal gen AI/cybersecurity adoption in the way this BIS paper surveys central banks generally; a potential blind spot in the Indian framework (regulator's own AI governance vs. regulated entities' AI governance).

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/International/International_1]], [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]], [[07_Institutions/Corpus/CERT_In/CERT_2]]
**Related concepts:** [[05_Concepts/05_Concepts_Standard/Governance_Capacity]], [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]]
**Related frameworks:** —
**Related projects:** [[02_Projects/P3_BFSI_JEIM]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]
**Related consulting:** AEGIS_OS (gen AI for cyber threat detection/response is directly relevant to runtime governance/enforcement use cases)

---

## Coding Status

- **P3 NVivo:** Screening corpus (candidate — useful as comparator/benchmark rather than core BFSI-AI-governance instrument)
- **Wiki intake status:** Pending

---

## Log

- 2026-06-14: Corpus node created. Batch 3. Cowork session. Source: BIS Generative AI.pdf.
- 2026-07-15: Enriched from a second, independent NotebookLM extraction pass — one-time exception to the session's flag-only-on-duplicate rule, per explicit user instruction. Added: survey methodology/institutional context (CRCC est. 2019, 58 member central banks, 32 GCRG respondents, Jan 2024 survey window, contemporaneous March 2024 US Treasury report); full adoption/effectiveness/risk figure set (71% current adoption, 96% risk-rating ≥5/10 as the paper's sharpest tension point, benefit-dimension percentages); IT-investment/human-capital figures (3% unrestricted cloud access, 40% high/extreme staff-preparedness concern); named tools (FraudGPT, WormGPT as offensive examples; ChatGPT/Claude/Bard/Copilot/Midjourney as general-purpose); full definitions/taxonomies (ML/neural-network/transformer definitions, offensive-use taxonomy, AI-system risk taxonomy, ethical/regulatory concerns taxonomy, crucial-human-roles taxonomy); four Key Quotes. No new VERIFY flags required (publication-date and pagination uncertainty already captured in the original intake).
