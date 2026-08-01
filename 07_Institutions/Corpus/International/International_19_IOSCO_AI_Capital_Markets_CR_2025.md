---
type: Corpus Node
tags:
  - type/corpus-node
  - status/active
  - engine/phd
  - jurisdiction/global
  - institution/international
  - theme/capital-markets
  - theme/bfsi
---

# International_19 — IOSCO: Artificial Intelligence in Capital Markets — Use Cases, Risks, and Challenges (CR/01/2025)

**Type:** Corpus Node
**Vault path:** `07_Institutions/Corpus/International/International_19_IOSCO_AI_Capital_Markets_CR_2025.md`
**Institution:** [[07_Institutions/International]]
**Issuing body:** International Organization of Securities Commissions (IOSCO) — Fintech Task Force (FTF)
**Document date:** March 2025 (Consultation Report); comment period closed April 11, 2025
**Pages:** ~100 pp (confirmed) — source file 1.7MB; vault file confirmed as IOSCO IOSCOPD788 CR/01/2025 (verified 2026-06-19)
**Domain:** [[03_Domains/AI_Governance]] | [[03_Domains/BFSI_Governance]]

---

## Instrument Identity

**Full title:** *Artificial Intelligence in Capital Markets: Use Cases, Risks, and Challenges* (Consultation Report CR/01/2025, IOSCOPD788)
**Type:** Consultation Report (Phase 1 of 2-phase IOSCO approach to AI in securities markets; not yet binding regulatory standard)
**Target entities:** IOSCO member securities regulators (130+ jurisdictions); securities market participants; AI vendors serving capital markets
**Legal basis:** IOSCO mandate under its founding statutes (protect investors, ensure fair/efficient markets, reduce systemic risk); FTF mandate
**Companion documents:** IOSCO AI Report 2021 (predecessor); IOSCO Supervisory Toolkit for AI Use in Capital Markets (FR/02/2026, IOSCOPD823, May 2026 — Phase 2 finalised); ESMA AI guidance 2024 (MiFID II); CFA Institute comment letter (April 2025)

**SOURCE CONFIRMED (2026-06-19):** Vault file `/Users/vivek/Documents/LinkedIn/Policy Dump Future/AI_on_capital_markets_1764279852.pdf` positively identified as IOSCO CR/01/2025 (IOSCOPD788) via direct Read tool access to the full PDF. Title page confirms: *"Artificial Intelligence in Capital Markets: Use Cases, Risks, and Challenges — CONSULTATION REPORT — The Board of the International Organization of Securities Commissions — CR/01/2025 — March 2025 — Board/2025/017."* SEBI explicitly named as AIWG member (footnote 1, page 5). Eight governance principles confirmed on page 49. NOT the Azzutti (2025) SSRN paper 5213493. **⚠ VERIFY flag #152 is RESOLVED.**

---

## Analytical Classification

**Wiki section:** S3/S6/S2
**Jurisdiction:** Global (IOSCO — 130+ member securities regulators)
**Confidence:** High — source file confirmed IOSCOPD788 (2026-06-19)
**AI explicit:** Yes
**Tier classification:** Tier A — IOSCO consultation report is the global securities regulatory standard-setting process for AI; sets international baseline for securities market AI governance
**AI Governance Wiki relevance:** HIGH — first IOSCO-level systematic treatment of AI governance in capital markets since 2021; directly relevant to SEBI (IOSCO member) and India's P3 BFSI comparative analysis

---

## Substantive Content

### IOSCO AMCC Survey Findings (184 market participants)

Key empirical data from the AMCC survey embedded in the Consultation Report:

| Metric | Finding |
|--------|---------|
| AI adoption | 49% of respondents have adopted AI |
| AI investment | 50% have invested in AI |
| AI in production | 41% of use cases already in production |
| AI in pilot | 8% remaining in pilot phase |
| Most common application | Communications with clients — 66.7% of IOSCO member respondents |

**Most common AI use cases (by frequency):**
1. Internal productivity support — 30.4%
2. Market analysis — 27.7%
3. Code generation — 25.0%
4. Client-facing communications (chatbots, personalised investment communications, NLP) — 66.7% at regulator-survey level

**For P3 context:** IOSCO members' survey of securities market participants shows AI adoption is already operational (not pilot) in 41% of use cases — this is the empirical baseline against which SEBI's AI/ML reporting circulars (SEBI_9, SEBI_10, SEBI_12, SEBI_17) should be assessed. The gap between IOSCO's 2025 empirical baseline and SEBI's 2019 reporting framework is a measurable [[Governance_Debt]] item.

### Risk Framework

The Consultation Report identifies three macro risk categories for AI in capital markets:

**1. Investor Protection Risks**
- Algorithmic bias in robo-advice and credit scoring
- Lack of explainability for AI-driven investment recommendations
- Market manipulation enabled by AI (spoofing, layering at ML speed)
- Agentic AI autonomy risks — reinforcement learning systems acting without human oversight

**2. Market Integrity Risks**
- Algorithmic collusion (de facto price coordination via similar ML systems — without explicit coordination)
- Flash events/cascades from correlated AI trading strategies
- Model herding — multiple AI systems converging on same positions, amplifying volatility

**3. Financial Stability Risks**
- AI vendor concentration (few dominant AI infrastructure providers for capital markets — cloud + model level)
- Third-party risk arising from lack of explainability of vendor AI systems
- Cross-border regulatory arbitrage where AI-enabled trading exploits jurisdictional gaps

### Regulatory Approaches Observed by IOSCO

IOSCO mapped the regulatory landscape across member jurisdictions and found:
- **Majority do not have AI-specific capital markets regulation** (consistent with International_9's OECD 2024 finding: most jurisdictions extending existing regulation rather than creating AI-specific rules)
- Most common approach: **extending existing securities regulation** (suitability, best execution, AML/KYC) to AI-enabled functions
- Notable exceptions: ESMA MiFID II AI guidance (EU, 2024); CSA Canada AI guidance (Dec 2024); Qatar Central Bank AI Guideline (Sept 2024, previously identified at International_9)

### India-Specific Relevance (SEBI / RBI)

IOSCO's framing of "sole responsibility" for AI outputs (market intermediaries remain solely responsible for AI-generated outputs regardless of vendor) directly maps to SEBI_14's Regulation 16C ("sole responsibility" clause) and RBI_7's LSP accountability framework. This convergence without cross-reference is strong [[Regulatory_Parallelism]] evidence at the global level — SEBI and RBI arrived at the same "non-delegable responsibility" conclusion independently of the IOSCO consultation process (both predating the March 2025 IOSCO CR).

### Phase 2: IOSCO Supervisory Toolkit (May 2026, IOSCOPD823)

IOSCO published the final Supervisory Toolkit for AI Use in Capital Markets (FR/02/2026) in May 2026, converting the CR/01/2025 consultation into operational supervisory guidance for securities regulators. ⚠ VERIFY BEFORE PUBLISHING — whether SEBI has issued any circular implementing or referencing IOSCO's Supervisory Toolkit as of June 2026.

---

## Analytical Significance for PRIS Research

### For P3 (BFSI AI Governance — JEIM)
IOSCO CR/01/2025 provides the global securities regulatory baseline against which SEBI's AI governance instruments (SEBI_9/10/12/17/14) can be benchmarked. Three specific comparative findings: (a) SEBI's 2019 reporting circulars predate IOSCO's formal AI taxonomy by 6 years; (b) SEBI_14's "sole responsibility" clause (Feb 2025) converges with IOSCO's accountability framing without citation; (c) India lacks the AI-in-capital-markets assessment equivalent to IOSCO's AMCC survey — [[Governance_Capacity]] gap.

### For P4 (Doctrinal Analysis)
IOSCO's non-delegable responsibility principle (AI vendor outputs do not transfer liability from the regulated entity) is the global doctrinal consensus in securities law. Comparing this to RBI_7's LSP chain, SEBI_14's Regulation 16C, and the absence of a similar clause in IRDAI_1 reveals [[Regulatory_Parallelism]] within India's BFSI regulatory stack (SEBI/RBI convergence, IRDAI gap).

### Coordination / Parallelism Pattern
**Convergence with SEBI_14 + RBI_7:** All three independently converge on "regulated entity retains sole/non-delegable accountability for AI outputs" in 2025. This is the strongest three-way [[Institutional_Coherence]] finding in the Batch 12 corpus — global standard (IOSCO) + Indian capital markets regulator (SEBI) + Indian banking regulator (RBI) reaching identical accountability design without citation chain.

---

## Connections

**Related corpus nodes:** [[07_Institutions/Corpus/SEBI/SEBI_14]], [[07_Institutions/Corpus/SEBI/SEBI_9]], [[07_Institutions/Corpus/SEBI/SEBI_17]], [[07_Institutions/Corpus/RBI/RBI_7]], [[07_Institutions/Corpus/International/International_9]], [[07_Institutions/Corpus/International/International_10]], [[07_Institutions/Corpus/International/International_11]]
**Related concepts:** [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]], [[05_Concepts/05_Concepts_Signature/Governance_Debt]], [[05_Concepts/05_Concepts_Standard/Accountability]], [[05_Concepts/05_Concepts_Standard/Transparency]], [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]
**Related frameworks:** [[06_Frameworks/EU_AI_Act]]
**Related projects:** [[02_Projects/P3_BFSI_JEIM]], [[02_Projects/P4_Doctrinal_IJLIT]], [[02_Projects/P1_SLR_RG]]
**Related knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Coding Status

- **P3 NVivo:** In canonical corpus — primary international BFSI AI governance instrument; strong RU candidates on sole responsibility, algorithmic collusion, AI vendor concentration
- **Wiki intake status:** Pending — primary feed for S3 (International Regulatory Context — IOSCO), S6 (Model Risk / Implementation — algorithmic collusion, AI vendor risk), S2 (India Regulatory Framework — SEBI comparator)

---

## Log

- 2026-06-18: Corpus node created. Batch 12. Cowork session. Source: `/Users/vivek/Documents/LinkedIn/Policy Dump Future/AI_on_capital_markets_1764279852.pdf`. ⚠ CRITICAL NOTE (archived): Source file unreadable via bash (mount deadlock); node written from IOSCO.org source (IOSCOPD788 full text at iosco.org/library/pubdocs/pdf/IOSCOPD788.pdf) and IOSCO press release IOSCONEWS761. Vault source file identity unconfirmed at session close — flagged CRITICAL for verification before quotation-level use.
- 2026-06-19: Source file identity CONFIRMED. Read tool used directly on `/Users/vivek/Documents/LinkedIn/Policy Dump Future/AI_on_capital_markets_1764279852.pdf` (bypassing bash mount deadlock). Title page confirms IOSCO CR/01/2025 (IOSCOPD788), Board/2025/017, March 2025. SEBI confirmed as AIWG member (footnote 1, p. 5). Eight governance principles confirmed (p. 49). ⚠ VERIFY flag #152 RESOLVED. Confidence upgraded to High. Node is now cleared for quotation-level citation.
