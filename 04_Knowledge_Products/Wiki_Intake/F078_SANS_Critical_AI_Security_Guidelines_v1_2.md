---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - topic/ai-security
  - topic/agentic-ai-governance
  - institution/sans-institute
---

# Draft: Critical AI Security Guidelines, v1.2 — Intake Note

**Source:** SANS Institute (multi-vendor/practitioner consortium — Fortinet, SAP, Palo Alto Networks, HiddenLayer, Binary Defense, OWASP AI, BSI, and 24 named contributors)
**Year:** Late 2024/early 2025 (exact date not stated; references DeepSeek and Stargate as occurring "during our editing period")
**Full title:** Draft: Critical AI Security Guidelines, v1.2
**File ID:** F078
**Zotero key:** [blank]
**Wiki section(s):** S5 (Data, Privacy & Security — primary), S4 (Agentic AI Governance — secondary)
**Confidence:** Medium-High (named 24-author practitioner/vendor consortium with strong industry credentials; explicitly labelled **Draft**, v1.2 — not a finalised standard)
**Jurisdiction:** Global (practitioner guidance; cites 8 jurisdictions' regulatory frameworks for context)

---

## Classification

**Document type:** Industry Report / Practitioner Guidelines (Draft)
**Primary audience:** CISO / Security Engineer / Practitioner
**AI explicit:** Yes

---

## 3–5 Reusable Findings

1. **Empirical encoding-bypass red-team finding** (feeds S5): Testing GPT-4o mini, Gemini Flash 1.5, Claude 3.5 Haiku, Llama 3.1, and DeepSeek v2.5, the authors found all five models would process Base64, Hex, or Morse-encoded inputs to bypass safety guardrails — without ever being explicitly asked to decode the input. A concrete, reproducible jailbreak vector distinct from conventional natural-language prompt injection.

2. **Six-domain AI security control taxonomy** (feeds S5/S6): Access Controls, Data Protection, Deployment Strategies, Inference Security, Monitoring, and Governance/Risk/Compliance (GRC) — a comprehensive practitioner control framework, comparable in function to F070's (Databricks DASF) 51-control catalogue and F038's (ISACA) four foundational principles, but organised around six operational domains rather than a maturity ladder.

3. **RAG-with-ACLs as an architectural alternative to model-internal guardrails** (feeds S4/S5): The guidance recommends implementing access control lists at the vector-retrieval layer of a RAG pipeline rather than relying on LLM-internal guardrails — "this eliminates the need to attempt to implement these guardrails in the LLM" — an architectural recommendation to move access enforcement outside the model itself, directly aligned with the AEGIS_OS pre-execution runtime-enforcement thesis.

4. **Least privilege extended explicitly to agents, not just users** (feeds S4): "Organizations must enforce focused functionality and apply the principle of least privilege not only to users, but to the agents themselves," operationalised via a four-part taxonomy (defined function scope, execution isolation, API/functional-call controls, feedback loops/escalation). This is the corpus's fifth independent-source-genre corroboration of the AEGIS_OS runtime-enforcement/authority-binding thesis, joining F036 (NIST), F038 (ISACA), F071 (AWS), and F073 (Google Cloud/Mandiant) — now spanning standards bodies, professional associations, Big Tech vendors, threat intelligence, and a multi-vendor cybersecurity-training consortium.

5. **Cross-jurisdictional regulatory-framework inventory (Table 1)** (feeds S3): Names 8 AI security/regulatory instruments across the EU, US federal, three US states (Tennessee, California, Utah), China, Israel, and the Council of Europe — an independent practitioner-consortium cross-jurisdictional snapshot (not a regulator or Big Tech source), reinforcing existing corpus evidence of parallel, uncoordinated AI regulatory development.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** The RAG-with-ACLs and agent-level-least-privilege recommendations are directly reusable in AEGIS_OS-relevant scoping conversations — both independently corroborate the runtime pre-execution enforcement thesis from a fifth source genre.
**Consulting connections:** AEGIS_OS (direct — runtime enforcement, least privilege for agents, execution isolation).
**Teaching connection:** The Base64/Hex/Morse encoding-bypass finding is a strong, concrete classroom example of a non-obvious LLM jailbreak vector.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S5, S4
**Concepts:** [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]], [[05_Concepts/05_Concepts_Signature/Regulatory_Parallelism]]
**Corpus nodes:** [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]], [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices]], [[04_Knowledge_Products/Wiki_Intake/F071_AWS_AI_for_Security_and_Security_for_AI_2025]], [[04_Knowledge_Products/Wiki_Intake/F073_Google_Cloud_Mandiant_Cybersecurity_Forecast_2026]] (AEGIS_OS corroboration cluster), [[04_Knowledge_Products/Wiki_Intake/F070_Databricks_AI_Security_Framework_DASF]] (control-catalogue comparator)
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Processing Status

- [ ] PDF in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes
- [ ] Marked processed

---

## ⚠ VERIFY BEFORE PUBLISHING

| # | Flag | Priority |
|---|---|---|
| #219 | Document is explicitly labelled "Draft: Critical AI Security Guidelines, v1.2" — not a finalised standard. Confirm whether a finalised/non-draft version has since been published before citing control recommendations as settled SANS guidance | MEDIUM |
| #220 | Exact publication date not stated in source — only inferable as late 2024/early 2025 from contextual references (DeepSeek, Stargate) — verify via SANS Institute's website before citing a precise date | LOW |

---

## Log

- 2026-07-15: Wiki intake note created. NotebookLM extraction relay, PROMPT 0b. Ad hoc pre-Batch 19 session. Duplicate check run against "Critical AI Security Guidelines," "Sounil Yu," "Ken Huang," "SANS Institute" — only prior match was Brandon Evans as a co-author on the unrelated F071 (AWS) whitepaper; confirmed new node.
