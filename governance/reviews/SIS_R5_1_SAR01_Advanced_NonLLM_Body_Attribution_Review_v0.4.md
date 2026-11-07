# SAR-01 v0.4 — Advanced Non-LLM Procedural Body & Attribution Review

> SCIENTIFIC DISCUSSION ONLY. SAR-01 OPEN / NON-NORMATIVE. No R5.1 modification, no adoption, no experimental conformance PASS. User-selected scheme B: allow advanced workflows and domain rules inside a non-LLM body; stratify their cognitive contribution.

## Scientific boundary

SIS examines LLM/LMM-centered systems under task, risk, information and resource conditions. It asks when non-LLM execution tools, structured knowledge, generic workflows and precompiled domain procedures compensate for the limitations of a smaller core model; where the cognitive interface floor lies; and whether execution feedback changes cross-task system capability. Traditional ML can be a tool/comparator, not an independent main scientific program in this proposed scope.

**Existing R5.1 grounding:** Scientific Identity §§1–3; Capability Frontier §14; SCF/SDR/ASR §§22–33; CSCI and boundaries §§34–38. Part VII-A **PROPOSED** clauses §39B, §39I, §39J, §39L, §39M, §39P, §39Q, §39U inform possible localization and resource governance; they are not adopted here.

## Three-level non-LLM body typology

| Level | Body | Key distinction |
|---|---|---|
| B1 | Atomic execution: code, calculator, database/API | Core model maps task to actions and interprets results |
| B2 | General workflow: orchestration, state, generic verification, retry/fallback | Organization and some control are externalized |
| B3 | Domain procedures: expert SOP, decision trees, rules and domain pipelines | Task-specific reasoning may already be encoded outside model |

B3 is allowed and can demonstrate real system capability. But *system task success ≠ model intrinsic reasoning ≠ unique LLM contribution*. Preserve SOP authorship, expertise, development/amortized cost, scope, provenance and possible answer contamination.

## Four causal questions

1. What capability does the frozen model possess with minimal support?
2. What is the *total system effect* of body/manual augmentation, allowing cost and risk?
3. What is the *model × body/manual interaction* across independently measured model capability?
4. What amount of performance is achieved by precompiled procedures without the LLM?

A **no-LLM fixed-rule-router + identical B3** is indispensable as an attribution negative control. Comparable performance supports external automation, but cannot prove that the LLM contributed necessary reasoning. An **oracle router** (diagnostic upper bound, not deployable baseline) distinguishes routing deficiency from external execution ceiling.

## Cognitive floor

Measure goal understanding, tool binding, plan construction, result interpretation/verification and error recovery as a task-conditioned vector, not parameter size or universal IQ. For each task distribution, body/manual, resource and risk envelope, estimate an *observed viable set* of models meeting pre-registered success, catastrophic risk and cost gates. No universal scalar, no monotonicity assumption.

## Generalization tests

G0 held-out within-SOP instances; G1 parameter/paraphrase perturbations; G2 novel SOP and skill recombinations; G3 unseen tools, API changes and failure recovery; G4 shifted task families, domains, constraints and evidence. Hold out by task family and SOP author/source provenance. SOPs may contain useful domain knowledge but not eval-instance solutions or hidden grading instructions.

## Proposed study arms

Strong/core-only; weak/core-only; weak+B1; weak+B2; weak+B3; weak+B3+rich manual; rule-only+B3; oracle-router+B3; strong+B3. Separate body and knowledge treatment factors where claims require causal separation. Control model identity, initial information and resource capacity; measure realized calls/latency and SOP authoring cost, and prevent evaluator leakage. Evaluate repeated stochastic runs, critical safety failures, task stratification and long-horizon effects.

**Compensation** requires local pre-registered noninferiority of weak+B3+manual relative to strong+minimal system, **plus** separate reliability, risk and cost conditions. A non-significant difference is not an equivalence test.

**Feedback learning** distinguishes within-episode retry, external memory revision, persistent parameter/policy update and optimizer self-modification (RSI candidate). Compare feedback-trained weak model with *equal-budget generic training* under identical frozen body; separately measure tool-choice, monitoring, error repair and held-out tool/task generalization. No claims of transfer from training-task replay alone.

## Proposed kill tests (not run)

No-brain equivalence; oracle-routing gap; SOP answer precompilation; hidden stronger LLM; task-family leakage; risk-stratum collapse; unmatched compute; misleading non-significant equivalence; feedback-only memorization; reward/evaluator hacking; changed tool interfaces; contradictory evidence.

## Candidate first-principles definition (NOT ADOPTED)

SIS studies how task-, information-, resource-, time- and risk-conditional capabilities of LLM/LMM-centered intelligent systems are formed, compensated, maintained, regulated and evolved through non-LLM external execution, structured knowledge, procedural skills, organization, state and feedback. It examines the interaction and limits of model cognitive-interface competence with external capability and subsequent feedback-based improvement. Advanced workflows are legitimate system resources but their precompiled domain knowledge and development costs are part of the scientific contract. System capability, model capability and causal contribution must not be conflated.

## One open science-owner decision

**Q-SAR01-06:** When B3 succeeds as well with a fixed non-LLM controller, should SIS count that as a valid *external system-capability* finding but mark *necessary LLM contribution* unsupported or null? **Review recommendation: YES**, with separate claims. This is an open question; do not freeze.

## Relevant external research (context, not proof of SIS hypotheses)

- SOP-Bench (KDD 2026): https://www.amazon.science/blog/sop-bench-a-new-benchmark-for-evaluating-ai-agents-on-real-business-procedures
- GenTool (ACL Findings 2025): https://aclanthology.org/2025.findings-acl.61/
- AutoTool (ICML 2026): https://proceedings.mlr.press/v306/zou26p.html
- OpenAgent tool-use generalization (ICML 2026): https://proceedings.mlr.press/v306/wu26al.html
- ToolRL (NeurIPS 2025): https://papers.nips.cc/paper_files/paper/2025/hash/97c5b2707228e7e3fb67e4ecc2e0e607-Abstract-Conference.html

**Status: SAR-01 OPEN; conceptual stress tests drafted, no scientific/engineering tests executed.**
