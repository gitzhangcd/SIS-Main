# SAR-01-A｜Four-System Boundary & Expressivity Stress Test

**Review date:** 2026-10-28  
**Status:** `SAR-01-A CONCEPTUAL_REVIEW_COMPLETE` / `SAR-01 IN_REVIEW / OPEN` / **NOT NORMATIVE**.  
**Source:** `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`; 14,825 lines.  
**Scope:** Latest R5.1 considered on its own merits; **not** a comparison with prior releases. Part VII-A is marked `PROPOSED NORMATIVE PATCH`; no proposed clause was adopted by this review.

## 1. Standardized four-system review

Each case has an identified scientific question and estimand, system/component boundaries, procedural knowledge source, state/observation/control roles, permitted information at decision time, matched controls, falsification conditions, tentative routing/claim ceiling and explicit generalization boundary.

| Case | Primary scientific status | R5.1 conceptual expressivity | Strongest counterexample | Outstanding gap |
|---|---|---|---|---|
| **A. Fixed rules + advanced SOP; no learned cognitive model** | Valid system-capability observation or comparator; **conditionally** a core research case when mechanism, information-dependent policy or trajectory is the actual estimand | **EXPRESSIBLE_WITH_SCOPE_AMBIGUITY** | A fixed symbolic solver can generalize to unseen skill combinations; conversely an SOP may simply contain benchmark solutions. Fixed does not imply non-intelligent, and successful automation does not itself identify a mechanism | **GAP-01 HIGH:** boundary between ordinary automation and SIS explanatory science |
| **B. Jev-like bounded learned decision module + B3 SOP + knowledge; no generative LLM** | **PRIMARY_IN_SCOPE** given system-level scientific question | **EXPRESSIBLE_CONDITIONAL_ON_OPTION_PROVENANCE** | Human/programmatic candidate-option generation may already solve the problem; typed choices do not guarantee validity or safety | **GAP-03 MEDIUM:** provenance of option generation vs learned selection, state freshness, authority |
| **C. Weak LLM + strong non-LLM body + manual vs strong LLM + minimal body** | **PRIMARY_IN_SCOPE** | **EXPRESSIBLE_WITH_CAUSAL_IDENTIFICATION_GATES** | Strong body may contain pre-encoded answers/hidden strong LLM; adding body and changing model simultaneously identifies no unique body mechanism | **GAP-04 MEDIUM:** operational noninferiority vs causally identified compensation; information and resource confounding |
| **D. Feedback-trained / optimizer-modifying system** | **PRIMARY_IN_SCOPE**, but strong RSI claim not approved | **ABSTRACT_EXPRESSIBLE_EXACT_RSI_CONTRACT_OPEN** | A fixed optimizer repeatedly improving task scores is not recursive self-modification; modified evaluator/reward invalidates capability growth claim | **GAP-02 HIGH:** explicit meta-improver identity, modification target, revision & independent future evaluation |

### Proposed claim-level routing (13 distinct hypotheses, not 13 scientific results)

- **A:** descriptive task completion → `DESCRIPTIVE_ONLY`; controlled verification mechanism → `SCF`; information-conditioned retry/abstention policy value → `ASR`. A temporal error-recovery estimand, if added as a separate claim, would require `SDR`.
- **B:** learned selection module's causal system effect → `SCF`; history-conditioned selector/abstention policy → `ASR`; cross-task transfer only → `DESCRIPTIVE_ONLY`/unresolved unless a primary scientific estimand is supplied, with `X2` as cross-cutting.
- **C:** weak/strong system package noninferiority → operational performance claim first, not automatic causal mechanism; controlled scaffold effect → `SCF + CSCI`; conditional tool/verification/escalation selection policy → `ASR`.
- **D:** controlled feedback-training mechanism → `SCF`; time-dependent failure/propagation/recovery → `SDR`; conditional choice of update target → `ASR`; changing the **improver itself** to improve future improvement capacity → **RSI question**, whose exact estimand and contract remain open. Do not create a fourth Primary Program merely from the name RSI.

**Universal constraint:** `FrameworkName/LLM/Jev/SOP/RSI` does not determine program. `OneClaim → OnePrimaryProgram` when identified; otherwise explicitly abstain.

## 2. Eighteen adversarial reasoning checks

**A-KT01–04**: score-only as mechanism; fixed algorithm with novel composition; conditional rule policy valid for ASR; SOP pre-encodes answers.  
**B-KT01–04**: missing correct option; option generator did cognitive work; stale-state/ordering errors; no-LLM rule-controller equivalence.  
**C-KT01–05**: no-LLM body control; hidden stronger LLM; unmatched knowledge/compute; `p>0.05` misread as equivalence; cross-task collapse.  
**D-KT01–05**: within-episode retry≠persistent learning; memory update≠parameter update; repeated gain≠meta-improver revision; evaluator gaming; future-task/data/resource leakage.

All 18 are **reasoned conceptual adversarial cases**. No live-system, physical-schema or empirical experiment was executed, and there are **zero observed effect estimates**.

## 3. Minimal candidate amendments — not applied

1. **Scientific Scope Gate** in §1–3, not a new primitive: `SystemBoundary → TargetSystemProperty → ScientificQuestion/Estimand → CompetingExplanation → RequiredEvidence`. Preserve descriptive evidence without inflated mechanism/causal claims.
2. **Cognitive and procedural-role distinction**, preferably an optional annotation, not an ontology change: learned selector vs option generator vs fixed rule vs SOP author vs execution vs knowledge vs authority vs independent evaluator.
3. **Capability / intelligence / attribution separation**: a fixed SOP can establish system capability; generalization requires task variation; system task success does not prove a generative LLM or learned decider is necessary.
4. **RSI minimum lineage to SAR-04**: separate F0 within-episode reaction, F1 external memory/SOP update, F2 persistent model/policy update and F3 modification of the improvement machinery. Strong RSI claim requires explicit cross-generation independent evaluation.
5. **Do not assume external support is positive or compensatory**: allow null/negative effects, saturation, thresholds, resource costs, safety losses and task boundaries.

## 4. Evidence and review gates

| Gate | Evidence status |
|---|---|
| Four stylized cases analyzed | **4/4 CONCEPTUAL REVIEW COMPLETE** |
| Distinct claim routes reasoned | **13/13 REVIEWED** |
| Adversarial thought-test dispositions | **18/18 REASONED, 0 LIVE EXECUTED** |
| Scientific semantics `G-S` | **CONDITIONAL — GAP-01 and GAP-02 remain OPEN** |
| Operational conformance `G-O` | **NOT EXECUTED** |
| Empirical validation `G-E` | **NOT EXECUTED** |
| SAR-01 scientific identity | **OPEN** |
| R5.1 normative master | **UNCHANGED / NOT ADOPTED** |

## 5. Verifiable local audit artifacts

The full 19,664-byte Chinese scientific report and the three structured CSV registries were generated in the active conversation as an auditable package. Hashes:

- Report: `59a386f1747816e8f9d3e08428797dbb9f1e0b80a16067a1aa9d05963a2955e5`
- 4-case / 22-column matrix: `af503186b35e7087d7f44b36c1b37487fed0765411144309f52d2a44c18b2154`
- 13-claim registry: `35d65771b83f14b65b9a80684f3a8fb66c58327b21c337ea22533f2c5d55ecd8`
- 18-test registry: `4af5a4b0865d25b250a31468107e2533dbae7e156dc2a60486e48aeeba18b9d1`

This GitHub record contains the main scientific disposition and traceable checks. **Do not treat the local-package filenames/hashes as though the raw CSV files were uploaded to GitHub.**

## 6. Source anchors and independent external context

- SIS R5.1: §§1–3 L160–299; §§5–10 L536–722; §§11–21 L728–1016; §§22–38 L1051–1682; §39A–39AF **PROPOSED** L1684–4082; §§40–50 L4087–5168; §§65–68 L5662–5789; §§71–73 L6172–6255; §§74–85 L6474–6867.
- TypeSafe official Jev state / typed decision interface: https://typesafe.ai/blog/introducing-system-one-models-and-jev
- JEVal independent evidence that strong local decision scores can fail to produce long-horizon system reliability: https://arxiv.org/abs/2610.03935
- JevAgentHarness: https://arxiv.org/abs/2610.21412

These papers provide **external stress context**, not proof of any SIS law or empirical result from these four hypothetical systems.

## 7. Next step and progress

- **SAR-01-A** conceptual deliverable: **COMPLETE**.
- **SAR-01-B**: Scientific Scope Gate & Automation Boundary Kill Tests — **NEXT**, with focus on GAP-01.
- **SAR-01-C**: concise Identity v0.8 candidate and minimal rule set — PENDING.
- **SAR-01-D**: one science-owner decision card, best rebuttal, conditional wording approval — PENDING.
- **SAR-01 overall** remains `IN_REVIEW / OPEN`, **0/10 full SAR topics accepted**, all remaining topics not started.

**No edit to the normative Master, no merge, no scientific truth claim.**
