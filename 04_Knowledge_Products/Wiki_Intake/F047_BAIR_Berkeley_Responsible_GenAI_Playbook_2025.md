---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - section/S1
  - tier/medium
  - project/p1
  - project/p3
  - project/fsqca
---

# BAIR / Berkeley Haas: Responsible Use of Generative AI — A Playbook for Product Managers and Business Leaders (2025)

**Node ID:** F047  
**Type:** Wiki Intake Note  
**Wiki Section:** S1 (Governance Fundamentals) / P3 (BFSI JEIM)  
**Status:** Active  
**Tier:** Medium  
**Last Updated:** 2026-06-19  

---

## Source

**Full Citation (APA):** Smith, G., Luka, N., Newman, J., Osborne, M., Nonnecke, B., Lattimore, B., & Mittelstadt, B. (2025). *Responsible use of generative AI: A playbook for product managers and business leaders*. BAIR Responsible AI Initiative, UC Berkeley; Berkeley Haas School of Business.  
**Document Type:** Practitioner playbook / research-based guidance (grey literature)  
**Issuing Institution:** BAIR Responsible AI Initiative (Berkeley Artificial Intelligence Research), UC Berkeley; Berkeley Haas School of Business  
**Additional Affiliations:** Brian Lattimore (Stanford); Brent Mittelstadt (University of Oxford Internet Institute)  
**Funder:** Google (⚠ VERIFY #173 — funder disclosed; potential conflict of interest in a responsible AI governance document)  
**Publication Date:** 2025 (exact month not stated; references events through early 2025; executive summary developed with NotebookLM)  
**URL / DOI:** BAIR blog / Berkeley Haas website (⚠ VERIFY for canonical URL)  

**Routing note:** UC Berkeley / Berkeley Haas / BAIR is a US academic-industry research consortium, not an Indian regulatory or government body. Format B (Wiki Intake Note) applies.

---

## Executive Summary

This playbook synthesises 25 practitioner interviews and 300 survey responses with academic literature to produce a practitioner-oriented responsible AI governance framework for organisational leaders deploying generative AI. The core contribution is a 10-play framework — five Organisational Leadership (OL) plays and five Product Manager (PM) plays — operationalising responsible AI governance from strategic commitment through to day-to-day product decisions. The playbook identifies five key responsibility risks (Data Privacy, Transparency, Hallucinations/Inaccuracy, Bias, Safety and Security) and three additional concerns (Future of Work, Environmental Issues, Copyright and IP). A statistically significant finding is that only 9% of organisations have achieved "Optimized" responsible AI maturity (Reuel et al. 2024, ⚠ VERIFY #175), with 0.8% achieving operational maturity — indicating that responsible AI governance exists primarily as aspiration and policy, not operational practice. The Google funding relationship should be noted but does not invalidate the academic authorship team's methodological independence.

---

## Key Frameworks and Findings

### Five Key Responsibility Risks

| Risk Category | Description | Illustrative Example Cited |
|---|---|---|
| **Data Privacy** | Training data, inference inputs, and outputs may expose personal or confidential data | Air Canada chatbot — *Moffatt v. Air Canada* (BC Civil Resolution Tribunal, 2024); Mata v. Avianca (GPT hallucinations in legal filings, US federal court, 2023) |
| **Transparency** | Users may not understand AI's role in decisions or the basis for AI outputs | Automated credit decisions without explanation; AI-generated content without disclosure |
| **Hallucinations/Inaccuracy** | GenAI systems confidently produce false outputs at statistically significant rates | 3–27% hallucination rate depending on model (general); 69–88% hallucination rate in legal domain (Stanford researchers); 47% fabricated medical references |
| **Bias** | AI systems may perpetuate or amplify demographic biases from training data | Obermeyer et al. healthcare algorithm racial bias study (Black patients systematically under-referred); hiring algorithm bias |
| **Safety and Security** | AI systems can be exploited to produce harmful outputs, bypass safety measures, or compromise organisational security | Prompt injection; jailbreaking; data exfiltration via AI assistant |

### Three Additional Concerns

| Concern | Description |
|---|---|
| **Future of Work** | AI displacement of roles and skills; reskilling obligations; workforce transition |
| **Environmental Issues** | Energy consumption of GenAI model training and inference; carbon footprint |
| **Copyright and IP** | Training data copyright; AI-generated content ownership; derivative works claims |

### 10-Play Framework

**Organisational Leadership (OL) Plays:**

| Play | Title | Core Action |
|---|---|---|
| OL-1 | Demonstrate Leadership Commitment | Executives publicly articulate responsible AI commitment; establish dedicated RAI leadership role |
| OL-2 | Develop Policies and Standards | Create organisation-wide GenAI use policies covering the five key risks; update regularly as capabilities evolve |
| OL-3 | Build RAI Governance Framework | Establish cross-functional RAI governance body (cf. Microsoft AETHER committee, Salesforce OEHU, Mastercard two-tier review) |
| OL-4 | Create Aligned Incentives | Performance management, procurement criteria, and business case frameworks that reward responsible AI practice |
| OL-5 | Provide Tailored Training | Role-specific AI literacy and responsible use training; not generic one-size-fits-all modules |

**Product Manager (PM) Plays:**

| Play | Title | Core Action |
|---|---|---|
| PM-1 | Apply a Gut Check | Pre-deployment informal assessment: is this use case appropriate? Would I be comfortable if this decision appeared in the press? |
| PM-2 | Choose Models Thoughtfully | Assess model transparency (model card, training data disclosure), accuracy for the specific task, and provider governance (cf. Anthropic RSO) |
| PM-3 | Conduct Risk Assessments and Audits | Formal risk assessment against the five key risks; third-party audit for high-risk applications (cf. Google EARR; Adobe Firefly review process) |
| PM-4 | Test Adversarially | Red-teaming; prompt injection testing; bias evaluation; output accuracy sampling |
| PM-5 | Embed Responsibility in Micro-Moments | Day-to-day product decisions (feature scoping, output disclosure, user feedback) are the actual site of responsible AI; Brookings ETAG framework cited |

### Decoupling / Recoupling Framework

The playbook's theoretical anchor (drawing from Institutional Theory and neo-institutional sociology) is the concept of **decoupling** — the gap between formal organisational policies and actual practice. Key finding from empirical literature:
- Organisations adopt responsible AI policies to achieve legitimacy (Institutional Theory)
- Actual AI product decisions diverge from stated policies (decoupling)
- The playbook's intervention is **recoupling**: designing structures (micro-moments, incentive alignment, cross-functional governance) that close the policy-practice gap

This framing is directly relevant to India's AI governance context: India's NITI Aayog RAISE 2020 principles, SEBI AI guidelines, and RBI CSCRF create formal responsible AI commitments (legitimacy-seeking behaviour) that are decoupled from operational BFSI AI product decisions.

### RAI Maturity Data

| Statistic | Source | ⚠ VERIFY |
|---|---|---|
| 39.4% of US adults use GenAI tools | Bick et al. (2024) | #173 LOW |
| 65% of organisations regularly use GenAI | McKinsey (2024) | #174 LOW |
| Near doubling of genAI organisational use in past year | McKinsey (2024) | #174 LOW |
| ChatGPT 200M weekly active users (August 2024) | OpenAI disclosed | LOW |
| BCG/GPT-4: 12.2% more tasks; 25.1% faster | BCG (2023) | LOW |
| Hallucination rates: 3–27% general; 69–88% legal | Multiple sources | LOW |
| 47% fabricated medical references | Multiple sources | LOW |
| 9% "Optimized" RAI maturity | Reuel et al. (2024) | #175 MEDIUM |
| 0.8% operational maturity | Reuel et al. (2024) | #175 MEDIUM |

The Reuel et al. (2024) RAI maturity study covered 1,000 organisations, 20 industries, and 19 regions — making it the most generalisable RAI maturity baseline in the corpus. The 9%/0.8% figures are the most significant empirical findings in this document.

### Illustrative Case Studies

| Case | Issue | Outcome |
|---|---|---|
| *Moffatt v. Air Canada* (BC Civil Resolution Tribunal, 2024) | Air Canada chatbot provided incorrect bereavement policy information; customer relied on it | Airline held liable; tribunal rejected argument that AI chatbot was separate legal entity — deployer accountability affirmed |
| *Mata v. Avianca* (US federal court, 2023) | Lawyer submitted ChatGPT-fabricated case citations | Sanctions imposed on lawyers; highlights legal professional accountability for AI outputs |
| Microsoft AETHER Committee | Cross-functional governance body for responsible AI; provides OL-3 model | Active governance framework — PM plays reference AETHER as exemplar |
| Anthropic RSO governance model | Model safety governance with internal Responsible Scaling Officer | Cited as organisational governance benchmark |
| Mastercard two-tier review | High-risk AI applications subject to two independent reviews before deployment | Operationalises PM-3 risk assessment for high-stakes BFSI context |

---

## India Relevance and Governance Gap Analysis

The playbook's India relevance is primarily indirect — no Indian case studies, no India-specific data — but its framework directly applies to the BFSI AI governance maturity gap.

**Key India-BFSI governance applications:**

1. **Decoupling as India's primary governance problem:** NITI Aayog RAISE 2020 (principles), RBI CSCRF 2024 (cybersecurity focus, not AI-specific), and SEBI AI guidelines 2025 (aspirational) are precisely the type of legitimacy-seeking formal commitments that institutional theory predicts will be decoupled from operational practice. India BFSI's responsible AI maturity is likely below the global 9%/0.8% benchmark given the recency of formal governance instruments.

2. ***Air Canada* deployer accountability principle:** The BC Civil Resolution Tribunal's ruling that Air Canada cannot disclaim liability for its chatbot's outputs is directly relevant to Indian banking and insurance entities deploying customer-facing GenAI. India's consumer protection framework (Consumer Protection Act 2019) and banking ombudsman scheme may provide analogous accountability paths, but no India case law yet establishes this principle.

3. **Hallucination rates in regulated BFSI applications:** 69–88% hallucination rates in legal domain (from Stanford research) and 47% fabricated medical references indicate that GenAI deployment in credit decision explanations, insurance claim assessments, and financial advisory requires adversarial testing (PM-4) as a condition of responsible deployment. RBI/SEBI have not yet mandated adversarial testing of AI outputs.

4. **Organisational governance models (OL-3):** Microsoft AETHER, Salesforce OEHU, and Mastercard two-tier review provide benchmarks that India's major BFSI entities (SBI, HDFC Bank, ICICI Bank, BSE, NSE) could adopt. No Indian BFSI entity has publicly disclosed a cross-functional RAI governance committee at AETHER/OEHU equivalent standard.

5. **Copyright and IP (Additional Concern 3):** India's Copyright Act 1957 does not address AI-generated content ownership or AI training data copyright. The UK's December 2024 consultation and the US *Bartz v. Anthropic* / *Kadrey v. Meta* litigation are the live reference points; India has analogous but unresolved questions.

---

## Research Programme Applications

| Project | Application |
|---|---|
| P1 (SLR RG) | Decoupling/recoupling framework is a theoretical contribution to governance SLR; 9%/0.8% RAI maturity figures establish empirical baseline; hallucination rate data provides risk calibration; responsible AI implementation literature anchor |
| P3 (BFSI JEIM) | **Primary** — 10-play framework is a direct implementation model for BFSI responsible AI governance; Air Canada liability principle; Mastercard two-tier review as BFSI benchmark; decoupling identifies the India BFSI governance problem as structural (legitimacy-seeking → operational decoupling) |
| P4 (Doctrinal IJLIT) | Air Canada chatbot deployer accountability; Mata v. Avianca professional liability; copyright and IP section complements F046 Law Commission analysis |
| fsQCA | OC condition — decoupling framework provides theoretical basis for calibrating Organisational Commitment as formal-vs-operational distinction; 9%/0.8% maturity data anchors OC calibration |

---

## Concept Links

- [[Accountability]] — Air Canada deployer accountability principle; Mata v. Avianca lawyer accountability; OL-3 cross-functional governance body as an accountability mechanism; PM-3 third-party audit as an accountability infrastructure component
- [[Transparency]] — PM-2 model selection criteria include transparency (model cards, training data disclosure); Transparency risk is one of the five key responsibility risks; BAIR distinguishes output transparency (disclosure to users) from model transparency (explainability)
- [[Governance_Capacity]] — 9%/0.8% RAI maturity finding is the most direct empirical measure of organisational governance capacity deficit in the corpus; the 10-play framework is a capacity-building instrument
- [[Governance_Debt]] — Decoupling framing provides theoretical mechanism for governance debt: organisations adopt formal AI policies (accruing legitimacy) without building operational capacity (accumulating governance debt); "recoupling" is the debt-reduction programme
- [[Legitimacy]] — Institutional Theory framing is explicit: organisations adopt responsible AI frameworks to achieve legitimacy with stakeholders; the document's theoretical contribution is identifying when legitimacy-seeking produces decoupling rather than genuine governance improvement; India's NITI RAISE 2020 principles are a textbook legitimacy-seeking instrument
- [[Agentic_AI_Governance]] — PM-4 adversarial testing and prompt injection testing directly address agentic AI attack surfaces; the playbook's focus on GenAI output governance foreshadows agentic AI governance as GenAI capabilities expand into autonomous action

---

## ⚠ VERIFY BEFORE PUBLISHING

- **V-B14-10 / #173 — GenAI usage statistics (Bick et al. 2024; McKinsey 2024) — LOW.** 39.4% US adults (Bick et al. 2024, cited) and 65% organisations regularly using GenAI (McKinsey 2024, cited) are sourced from named academic and industry studies. Verify: confirm survey periods and methodologies from cited studies before using as current-state statistics; note that the 39.4% and 65% figures are 2024 baselines that may have changed materially.
- **V-B14-11 / #174 — Google funding — LOW.** Google funded this research; the playbook acknowledges this. Not a factual verification issue, but note potential funding bias in conclusions. The academic authorship team's multi-institutional composition (UC Berkeley, Stanford, Oxford) mitigates this concern. Recommend noting funding source in any P3 citation.
- **V-B14-12 / #175 — 9%/0.8% RAI maturity (Reuel et al. 2024) — MEDIUM.** This is the document's most significant empirical finding. Reuel et al. (2024) is cited as a study of 1,000 organisations, 20 industries, 19 regions. Verify: locate Reuel et al. 2024 primary paper; confirm sample, methodology, and the specific definition of "Optimized" maturity level before using in P3 or SLR. The figures are plausible but the survey instrument definitions of maturity levels are critical to interpreting the 9%/0.8% finding correctly.

---

## Cross-Links to Corpus

- [[F046_UK_LawCommission_AI_and_Law_DiscussionPaper_2025]] — F046's automation bias analysis (Theme 6) complements F047's operational governance plays; the Air Canada liability principle in F047 is consistent with F046's supply chain deployer accountability doctrine
- [[F043_MIT_AI_Risk_Mitigation_Taxonomy_2025]] — BAIR's 10 plays largely operationalise MIT taxonomy's Governance & Oversight (30%) and Operational Process (36%) categories; PM-4 adversarial testing populates the Technical & Security category (12%); the decoupling finding explains why operational process mitigations predominate: they are the organisational response to legitimacy-seeking
- [[F048_FLI_AI_Safety_Index_Winter_2025]] — FLI's finding that no company scored above C+ in responsible AI governance is consistent with BAIR's 9%/0.8% organisational maturity; both documents confirm systemic responsible AI governance deficit at developer and deployer levels
- [[F042_IBM_Cost_Data_Breach_Report_2025]] — IBM's 63% lacking AI governance policies complements BAIR's 9%/0.8% operational maturity finding; together they triangulate a pervasive AI governance deficit at policy and implementation levels
- [[F035_Microsoft_Administering_Governing_Agents]] — Microsoft AETHER governance committee (cited in F047) is documented in F035; cross-corpus coherence confirmed
