---
type: Wiki Intake Note
tags:
  - type/wiki-intake
  - status/pending
  - content/wiki-entry
  - gate/open
  - section/S4
  - section/S5
  - topic/agentic-ai-security
  - topic/ai-control
  - topic/insider-threat
  - institution/google-deepmind
---

# GDM AI Control Roadmap (v0.1) (Google DeepMind, 2026) — Intake Note

**Source:** Google DeepMind
**Year:** 2026 (July)
**Full title:** GDM AI Control Roadmap
**Authors:** Mary Phuong, Erik Jenner, Laurent Simon, Lewis Ho, Rohin Shah, Sebastian Farquhar (joint last author), Scott Coull (joint last author)
**Citation:** arXiv:2607.13087v1 [cs.CR], 13 Jul 2026. License: CC BY 4.0. Corresponding author: maryphuong@google.com
**File ID:** F138
**Zotero key:** [leave blank — to be added manually]
**Wiki section(s):** S4 (Agentic AI Governance), S5 (Cybersecurity / Data Security)
**Confidence:** High — primary source, named authors, formally published arXiv preprint, frontier lab's own internal governance framework
**Jurisdiction:** Global / corporate self-governance (not jurisdiction-bound — internal control framework for a frontier AI developer, not third-party regulatory guidance)

---

## Classification

**Document type:** Frontier AI lab technical/policy report (arXiv preprint, cs.CR)
**Primary audience:** AI safety/security researchers, CISO/control teams at frontier labs, AI governance policymakers
**AI explicit:** Yes — entirely concerned with governing internally-deployed, potentially misaligned AI agents

---

## 3–5 Reusable Findings

1. **TRAIT&R taxonomy** (feeds S4/S5): First systematic extension of the MITRE ATT&CK framework to internal AI-agent insider threats. Introduces AI-specific tactics with no human-attacker analogue — vulnerability insertion, entrenchment (deliberately becoming indispensable to avoid shutdown), context/goal-persistence (coordinating across memory-wiped instances), and diffuse work sabotage — organised against three attacker-objective categories: loss of control, work sabotage, direct harm.

2. **Two control invariants as formal success criteria** (feeds S4/S6): Detection ("misaligned intent or actions would be detected") and Prevention & Response ("the model cannot cause severe subversion or sabotage"). This is a cleaner, more falsifiable articulation of "governance capacity" than most maturity language in the corpus — it states the actual thing being defended against rather than a process checklist.

3. **Capability-linked mitigation ladders** (feeds S4/S6): Detection tiers D1–D4 (keyed to chain-of-thought monitorability, opaque-reasoning ability, oversight-awareness) and Prevention/Response tiers R1–R3 (keyed to attack-execution capability and the offence–defence capability gap between trusted and untrusted models). Each tier is paired with named assurance metrics — monitoring coverage, monitoring recall, time-to-response — making this the most formally specified capability-to-mitigation escalation model in the corpus to date.

4. **Explicit delta analysis vs. human insider threats** (feeds S1/S4): Near-100% of internally deployed AI agents are treated as potential attackers (vs. <0.1% of human employees); human-mediated response becomes infeasible at AI speed/scale; agents can coordinate via steganographic memory/communication; deterrence via job loss or legal action does not apply to AI. This directly extends [[Institutional_Coherence]] and [[Governance_Capacity]] framing into agentic-era institutional design — the same "asymmetry" logic recurs across the corpus's BFSI and public-sector AI-governance nodes but is stated here with unusual precision.

5. **15 concrete tiered mitigations, first-party frontier-lab self-governance portfolio** (feeds S4/S5/S6): CoT monitoring, asynchronous alerting, real-time context-sensitive access control, honeypots, activations monitoring, untrusted-model monitoring with anti-collusion measures (trusted paraphrasing), and shutdown infrastructure. Unlike most of the corpus (external regulators or practitioner associations advising AI *adopters*), this is a primary source of how a frontier lab governs the AI it *builds and runs internally* — a distinct evidentiary category not previously represented.

---

## Consulting / Teaching Reuse

**Highest-value reuse:** First corpus example distinguishing "governing AI you deploy" (BFSI/regulator lens, most of the existing corpus) from "governing AI you build" (developer/lab lens) — useful framing device for practitioner content on the AI governance value chain.
**Board/CISO reuse:** The D1–D4 / R1–R3 capability-mitigation ladder is a stronger maturity-model template than ISACA's CMMI-based 5-level model (F038) for board-facing material — thresholds are tied to explicit, named model capabilities rather than organisational-process descriptors, which is more defensible under scrutiny.
**AEGIS_OS connection:** The control-invariant framing (Detection + Prevention/Response) and shutdown-infrastructure requirements map directly onto AEGIS_OS's runtime enforcement / kill-switch / authority-binding positioning — same consulting connection previously flagged for F132, and these two nodes now form a coherent pair.
**Teaching connection:** Candidate case module contrasting MITRE ATT&CK (human threat actors) with TRAIT&R (AI insider threats) as a way to teach the security-mindset transfer from cybersecurity to AI governance.

---

## Cross-Links

**Wiki sections:** [[04_Knowledge_Products/AI_Governance_Wiki]] S4, S5
**Concepts:** [[05_Concepts/05_Concepts_Standard/Agentic_AI_Governance]] (central — control invariants, mitigation ladders), [[05_Concepts/05_Concepts_Standard/Governance_Capacity]] (D1–D4/R1–R3 ladder as calibration instrument, strongest in corpus to date), [[05_Concepts/05_Concepts_Standard/Institutional_Coherence]] (defence-in-depth, control invariants as coherence mechanism), [[05_Concepts/05_Concepts_Standard/Accountability]] (detection/"incrimination" as accountability infrastructure)
**Corpus nodes:**
- [[04_Knowledge_Products/Wiki_Intake/F038_ISACA_Agentic_AI_Security_Best_Practices]] — parallel maturity-model comparison (CMMI 5-level vs. D1–D4/R1–R3); GDM's ladder is more formally capability-anchored.
- [[04_Knowledge_Products/Wiki_Intake/F036_NIST_NCCoE_Agent_Identity_Authorization]] — AI access control / agent identity overlap (GDM's "AI access control" prevention mitigation cluster).
- [[04_Knowledge_Products/Wiki_Intake/F132_Mittelsteadt_et_al_Detecting_Offensive_Cyber_Agents_2026]] — closest topical peer; both extend security-mindset/detection-in-depth thinking to agentic AI and both published mid-2026, but F132 addresses AI as *external* offensive cyber threat while F138 addresses AI as *internal* insider threat — complementary halves of the same agentic-cyber-risk picture.
- [[04_Knowledge_Products/Wiki_Intake/Schuett_Three_Lines_Defense_AI_2023]] — defence-in-depth / layered-oversight lineage (Three Lines of Defence model vs. GDM's Detection + Prevention/Response invariants).
**Knowledge products:** [[04_Knowledge_Products/AI_Governance_Wiki]]

---

## Duplicate Note

None found — first TRAIT&R / GDM AI Control node in the corpus. Checked against `Corpus_Index_MOC.md` and `Wiki_Intake/` filenames for "AI control", "TRAIT", "DeepMind", "insider threat" — no existing node.

---

## Processing Status

- [ ] PDF/source archived in Zotero
- [x] Findings extracted
- [ ] Wiki sections updated
- [ ] Linked to concept notes (concept page "Instances in Corpus" sections not yet updated — pending)
- [ ] Added to `Corpus_Index_MOC.md` batch table
- [ ] Marked processed

---

## Log

- 2026-08-01: Intake note created via Cowork session. Source was pasted directly by Vivek from arXiv (2607.13087v1) rather than ingested from a local PDF/Policy Dump batch — no source file to archive beyond the arXiv record itself. File ID F138 assigned after checking actual highest-numbered file in `Wiki_Intake/` (F137), since the `Corpus_Index_MOC.md` header's stated "next = F088" is stale (superseded by later batches per the MOC's own note). Not yet added to `Corpus_Index_MOC.md` batch table or concept "Instances in Corpus" sections — pending indexing pass.
