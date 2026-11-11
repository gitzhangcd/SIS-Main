# SIS P0 Claim-Level Re-Audit｜2026-11-11
Authority: SIS v0.3.1 Master / Registry v1.3 / P0 Audit Queue / ClaimRecord schema. First-coder only. A paper-level prior CL2/CL3 label is triage, NEVER automatically promoted; no second-coder adjudication conducted.

## SIS-LIT-002｜JIT-Agent — v2, 2026-09-03
Primary source: https://arxiv.org/html/2608.25593v2 ; https://arxiv.org/abs/2608.25593
Verification: FULLTEXT_HTML_METHOD_AND_TABLES_REAUDITED; Section 5.1–5.5 and Tables 2–3 inspected. The fixed-backbone Table 2 comparison covers 18 backbone×task cells. Separate fixed-backbone comparison across six harnesses gives performance, token and API cost, but no independently validated causal mediation.

| Claim ID | Precise estimand | Routing / identification / evidence | First-coder decision |
|---|---|---|---|
| 002-C1 | FIXED_BACKBONE_JIT_HARNESS_TOTAL_PERFORMANCE_EFFECT | SCF/BGT; MI/MEAS/ID/BT; I1/I2-local, T1; SUPPORT | CL1 CONFIRM; local CL2 candidate ONLY for full harness package. Across nine tasks the same base model improves on 18 paired configurations; harness changes multiple modules, no unique pathway. |
| 002-C2 | BACKBONE_CAPABILITY_MODERATES_JIT_HARNESS_GAIN | SCF/CSCI/BGT; MI/IA/ID/BT; I1, T2 performance only; LIMIT | CL1 boundary; variation in gains across GLM/DeepSeek/Qwen/Mimo suggests capability interaction, but model architectures, training and evaluation are not a matched causal transport test. |
| 002-C3 | ONLINE_HARNESS_REPAIR_POLICY_INCREMENTAL_VALUE | ASR/BGT; DR/TD/EG/ID/BT; I0/I1, T0; IMPLEMENTATION | CL0 isolated mechanism / CL1 combined program. Training stages, candidate search, repair and online policy selection are bundled; not evidence of a uniquely identified continual adaptation benefit. |

Key boundaries: same model, tasks, prompts, tool visibility, candidate proposal count, parallel calls, wall-clock and token/cost; possible training task overlap. Kill Test: 2×2 fixed backbone × static/generated harness and independent JIT-repair on/off, equal token/call budgets, unseen task families. No CL2/CL3 promotion. **Action: split three claims; paper-level causal explanation demoted to pending.**

## SIS-LIT-007｜Adaptive Influence Graphs for Failure Attribution in Multi-Agent Systems
Primary source: https://arxiv.org/abs/2608.24361 (arXiv abstract); additional discovery context only, NOT primary mechanism evidence. Qualification PRIMARY_ABSTRACT_REAUDITED_2026-11-11_FULLTEXT_PENDING. Original experimental tables not independently inspected.

| Claim ID | Precise estimand | Routing / identification / evidence | First-coder decision |
|---|---|---|---|
| 007-C1 | TRACE_REPRESENTATION_CONDITIONAL_ERROR_STEP_LABEL_ACCURACY | SDR/BGT; TD/MI/MEAS/ID/BT; I1, T0; SUPPORT | CL1 descriptive/associational: graph-structured access improves Who&When step-level label accuracy within the tested benchmark. |
| 007-C2 | ADAPTIVE_GRAPH_BUILD_AND_READER_TRAVERSAL_INCREMENT | SDR/BGT; TD/DR/MI/ID/MEAS/BT; I1, T0; IMPLEMENTATION | CL1 for bundled graph-builder/reader; local CL2 candidate only after fixed diagnostic model, equal context size/inspection budget and ablation. |
| 007-C3 | CRITICAL_LABEL_EQUALS_EXECUTED_CAUSAL_FAILURE_SOURCE | SDR/BGT; TD/ID/EG/BT; I0, T0; LIMIT | CL0 unvalidated mechanism interpretation. Agreement with error-step labels is not a do(step)-based repair or mediator test. |

Key boundaries: synthetic versus hand-built Who&When traces, late failure position, graph abstraction losses, context length and judge Gold quality. Kill Test: independently seeded injected faults, graph/no-graph fixed-budget contrast, intervention at predicted locus, paired replay placebo, restored state certification. **Action: split diagnostic accuracy from causal attribution; full-text verification pending.**

## SIS-LIT-015｜TruthInsightBench
Primary source: https://arxiv.org/abs/2609.05079 (arXiv HTML full text, Sections 3–4 and score specification). Qualification PRIMARY_HTML_METHOD_REAUDITED_2026-11-11_JUDGE_VALIDATION_PENDING.

| Claim ID | Precise estimand | Routing / identification / evidence | First-coder decision |
|---|---|---|---|
| 015-C1 | BLIND_DISCOVERY_TASK_EVIDENCE_MATURITY_PROFILE | ROUTING_ABSTAIN/BGT; MEAS/EG/ID/BT; I1, T0; INSTRUMENT | CL1: forty blind tasks from ten scientific domains and 29 artifact-oriented items identify measurement gaps; does not directly demonstrate causal capability formation. |
| 015-C2 | FIXED_BACKBONE_SCIENTIFIC_HARNESS_SCORE_DIFFERENCE | SCF/BGT; MI/MEAS/ID/BT; I1, T1; NULL/BOUNDARY | CL1: four different execution scaffolds under same base model form a 58.4–60.3/100 score plateau with no reliable pairwise separation; one run per system–task, no repeated seeds. |
| 015-C3 | AUTOMATED_JUDGE_SCORE_INDEPENDENT_SCIENTIFIC_TRUTH | ROUTING_ABSTAIN/BGT; MEAS/EG/ID/BT; I0/I1, T0; LIMIT | CL0 independent validity claim; fixed W4A8 thinking-off GLM Judge is not an independently calibrated human expert Gold, even though numeric score aggregation is deterministic. |

Key boundaries: task selection from 40 papers, leaked domain priors, output artifacts, judge-induced scoring, per-instance absence of human review; author freeze holds model fixed but run artifacts/prompt details not fully redistributed. Kill Test: blind multi-expert item-level Gold on a stratified sample, paired alternative judge versions, repeated stochastic runs, contamination controls. **Action: confirm measurement value, demote implied 'scientific discovery competence objectively measured' claim pending independent judge validation.**

## Governance / adjudication handoff
- 3 studies, 9 first-coder claim records; promotions 0, confirmed T3/T4 0.
- Qualified: 002 HTML method/tables; 007 abstract only; 015 HTML method/results, judge Gold validation outstanding.
- All final_claim_level = PENDING_CLAIM_LEVEL_AUDIT; second_coder = PENDING; adjudication = PENDING.
- Prior paper-level candidate labels remain non-normative. This is evidence-map maintenance, not SIS Scientific Core change.
