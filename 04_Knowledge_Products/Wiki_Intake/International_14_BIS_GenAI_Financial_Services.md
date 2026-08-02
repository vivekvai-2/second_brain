---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/active
  - engine/phd
  - theme/genai-financial-services
  - theme/cyber-risk
  - theme/central-bank-ai
  - wiki-section/S3
  - batch/11
---

# BIS (2024/2025) — Generative AI in Financial Services (BIS Working Paper)

**Source:** Bank for International Settlements (BIS) — Working Paper Series  
**Year:** 2024/2025 (⚠V-I14-1: exact date unconfirmed)  
**Full title:** Generative AI in Financial Services (BIS Working Paper)  
**File ID:** K5 (md_cache)  
**Node designation:** International_14  
**Wiki section(s):** S3 — International Regulatory / S4 — Academic/Secondary  
**Jurisdiction:** Global  
**Authority:** High — BIS Working Papers carry significant weight in central bank and financial regulatory discourse; not a binding standard but authoritative in policy framing

> **Format note:** Format B (Wiki Intake Note) — BIS Working Paper is a research/analytical document, not a primary regulatory instrument. Upgrade to Format A only if direct obligation-creating content is identified.

---

## Classification

BIS Working Paper on the use of generative AI (GenAI) in financial services. The paper synthesises findings from central bank surveys (majority of surveyed central banks reported using or planning to use GenAI ⚠V-I14-2) and analyses the specific risk landscape that GenAI introduces beyond traditional AI/ML. For PRIS, International_14 is the corpus's primary node on GenAI-specific risks in financial sector context — distinct from general AI risk (RBI_FREE_AI_2025, SEBI_11) and from central bank internal AI governance (International_13). It documents four GenAI-specific cyber risk categories and argues for human oversight as a governance requirement rather than a design preference.

Companion to International_13 (BIS/IMF Governance of AI Adoption in Central Banks): where International_13 provides the governance framework, International_14 provides the risk evidence base for why GenAI-specific governance elements are needed beyond the standard AI risk toolkit.

---

## Reusable Findings

1. **Majority of central banks using or planning GenAI (feeds P1/S3):** BIS survey data confirms GenAI adoption is not emergent but current among central banks globally. The pace of adoption has outrun governance frameworks — a finding structurally parallel to the BFSI sector's F024 documentation-quality decline (17%→14%, earlier corpus). For fsQCA: the EME-AE governance capacity gap documented in International_7 applies specifically to GenAI: AE central banks are earlier adopters with more mature governance; EME central banks (including RBI) face higher risk exposure relative to governance readiness. (⚠V-I14-2: confirm survey percentage and methodology)

2. **Four GenAI-specific cyber risk categories (feeds P3/Governance_Capacity):** International_14 identifies four categories of GenAI-specific cyber risk distinct from traditional AI/ML risk:
   - *Social engineering amplification*: GenAI enables more sophisticated, contextualised phishing and deceptive communications targeted at financial institution employees and customers
   - *Zero-day vulnerability exploitation*: GenAI accelerates attacker capacity to identify and exploit previously unknown vulnerabilities in financial systems
   - *Malware and data leakage*: GenAI tools can inadvertently exfiltrate confidential financial institution data when used by employees without proper controls (particularly in cloud-hosted GenAI services)
   - *Direct AI system attacks*: adversarial inputs, prompt injection, and model manipulation attacks that exploit the specific architecture of GenAI systems
   
   These four categories are not addressed in any current RBI, SEBI, CERT-In, or MeitY governance instrument. The corpus's existing India cyber governance nodes (SEBI CSCRF, CERT-In notifications, RBI_1/RBI_2 IT governance) are pre-GenAI in framing. International_14 establishes the governance gap. ⚠V-I14-3: confirm whether International_15 (FSB FIRE) addresses GenAI-specific incident categorisation.

3. **Human oversight requirement for GenAI (feeds Accountability/P1):** International_14 argues that GenAI's stochastic and emergent output characteristics — including hallucination risk — require mandatory human oversight layers that are qualitatively different from those needed for deterministic ML models. This is a governance design argument: the oversight requirement is not simply a risk mitigation preference but a structural necessity given GenAI's non-determinism. Connects to International_13's Action A7 (monitoring and oversight) and RBI_FREE_AI_2025's "human oversight" Sutra — both of which acknowledge oversight without specifying the GenAI-specific design requirements that International_14 identifies.

4. **Human capital investment as governance prerequisite (feeds Governance_Capacity):** The paper identifies human capital — GenAI-literate risk officers, AI-aware compliance staff, technically competent board members — as a prerequisite for effective GenAI governance, not an implementation detail. This is the capacity-building argument: governance frameworks that assume human oversight will work without investing in the humans who provide oversight will fail. Parallels International_13's Action A8 (organisational readiness). For India: the RBI, SEBI, and MeitY governance frameworks do not address the human capital investment requirement; they assume oversight capacity exists.

5. **GenAI risk as categorically distinct (feeds P1/fsQCA):** International_14 argues GenAI is not a more powerful version of existing AI/ML — it introduces qualitatively different risk categories (particularly social engineering and direct system attack surfaces). This has fsQCA calibration implications: the SR (Systemic Regulatory) and EA (Enforcement Architecture) conditions designed around 2019-era AI/ML reporting (SEBI_9/10/17, Cluster C09) may not capture the governance requirements specific to GenAI. International_14 provides the theoretical basis for why the fsQCA conditions may need a GenAI-era recalibration.

---

## ⚠ VERIFY Flags

| Flag | Claim | Action |
|---|---|---|
| ⚠V-I14-1 | Exact BIS Working Paper date and number | bis.org → Research → Working Papers → search "generative AI financial services" |
| ⚠V-I14-2 | Survey finding: "majority of central banks using or planning GenAI" — confirm percentage, sample size, and survey methodology | Primary text; also cross-check International_7 (BIS/IFC Report No. 18, Apr 2025) for cross-reference |
| ⚠V-I14-3 | Does FSB FIRE (International_15/L3) include GenAI-specific incident categorisation, or is it technology-neutral? | International_15 primary text |

---

## Backlinks

← [[07_Institutions/Corpus/International/International_7]] (BIS/IFC Report No. 18 — empirical central bank AI survey; complementary survey evidence)  
← [[07_Institutions/Corpus/International/International_13]] (BIS/IMF Governance of AI Adoption in Central Banks — governance framework companion; International_14 provides risk evidence base for International_13's Action A5/A6)  
← [[07_Institutions/Corpus/International/International_15]] (FSB FIRE — incident reporting standard; relevant to GenAI-specific incident categorisation gap identified in International_14)  
← [[07_Institutions/Corpus/RBI/RBI_FREE_AI_2025]] (Seven Sutras — "human oversight" Sutra; International_14 provides GenAI-specific design requirements that RBI_FREE_AI_2025 does not specify)  
← [[05_Concepts/05_Concepts_Standard/Governance_Capacity]]  
← [[05_Concepts/05_Concepts_Standard/Accountability]]
