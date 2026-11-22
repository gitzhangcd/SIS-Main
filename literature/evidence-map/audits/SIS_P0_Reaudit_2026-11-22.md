# SIS P0 Claim-Level Re-Audit｜2026-11-22

**Authority:** SIS v0.3.1 Master / current Registry / P0 Audit Queue. **Status:** FIRST_CODER_ONLY; SECOND_CODER_PENDING; ADJUDICATION_PENDING. All scientific claim levels are conservative ceilings, not formal promotions. Exact source scope noted below.

## SIS-LIT-113｜HIPO
**Primary source:** https://aclanthology.org/2026.findings-acl.996/ ; **Findings ACL 2026, July**. Official conference metadata and abstract verified. The full PDF tables were not independently checked in this run.

| Claim | Primary estimand / routing / Framework | First-coder scientific evidence and ceiling | Kill test |
|---|---|---|---|
| 113-C1 | `SAMPLE_DIFFICULTY_CONDITIONAL_PROMPT_TIER_PACKAGE_VALUE`; ASR+BGT / DR,MEAS,ID,BT | Router predicts sample difficulty and selects from five prompt tiers, evaluated on 27 tasks. Combined routing+two refinement stages outperform reported baselines; CL1, I1, T1. | Freeze prompt pool + route samples randomly vs learned difficulty, equal token and API costs, independent test set |
| 113-C2 | `PREDICTED_DIFFICULTY_TIER_INTERACTION_WITH_TASK_QUALITY_COST`; ASR+CSCI+BGT / DR,IA,MI,MEAS,ID,BT | Claimed task-aware effects conditional on classifier quality and task difficulty; no independently reproduced interaction estimand. CL0 mechanistic hypothesis + CL1 package result, I1, T0. | Matched actual difficulty × predicted difficulty × tier assignment factorial with outcome and complete cost |
| 113-C3 | `ATTRIBUTION_REFINEMENT_VS_DESCRIPTION_REFINEMENT_INDEPENDENT_GAIN`; SCF+BGT / MI,EG,MEAS,ID,BT | Two-stage refinement bundled with sample routing. No verified mediator evidence and no final CL2/CL3. CL1 author-level package, I1. | Freeze router and candidates; 2×2 attribution/description refinement; hidden task robustness and calibrated judge |

**Decision:** confirm peer-reviewed source class, not causal maturity; previous queue source qualification upgraded to Anthology verified. No CL2/CL3 promotion.

## SIS-LIT-119｜Jev-Mem
**Primary source:** https://arxiv.org/html/2609.23986v1 ; source methods/Table 1/Table 2 checked. LoCoMo answer score based on LLM-as-a-Judge, not independent action-grounded Gold.

| Claim | Primary estimand / routing / Framework | First-coder scientific evidence and ceiling | Kill test |
|---|---|---|---|
| 119-C1 | `LIGHTWEIGHT_MEMORY_CONTROL_PACKAGE_QUALITY_LATENCY_FRONTIER`; SCF+CSCI+BGT / MI,IA,MEAS,ID,BT | Overall Judge score 0.777 vs strongest baseline 0.700; query latency 0.93s vs 1.47s fastest memory baseline; 158s build vs 1044s. CL1/I1/T1; comparison is multi-component package. | Hold memory corpus, model backbone, inference budgets and hardware fixed; randomize control plane and assess independent task gold |
| 119-C2 | `RETRIEVAL_POLICY_ROUTING_BUDGET_STOPPING_MARGINAL_VALUE`; ASR+BGT / DR,MI,ID,MEAS,BT | Typed controller performs routing, scoring, budget and stopping; reported package results cannot uniquely identify routing vs graph vs stopping; CL0 mechanism+CL1 implementation, I1. | 2×2 controller/routing plus stopping ablations with fixed candidate traces and total query budgets |
| 119-C3 | `EVIDENCE_ACQUISITION_TO_ACTUAL_DECISION_GROUNDEDNESS`; SCF+BGT / MI,EG,MEAS,ID,BT | Answer correctness judged by model; evidence retrieved and used as claimed is not independently intervened; CL1 QA endpoint only, no CL3. | Evidence-swap/suppress randomized within fixed retrieved candidates; blind human/executable gold and decision consequences |

**Decision:** split observed quality/cost from endogenous regulation and causal evidence use; no promotion. Table 1 descriptive paragraphs contain minor category-specific number differences; table is preferred over prose where contradictory.

## SIS-LIT-120｜Trajectory-Based Early Outcome Calibration Transfer Audit
**Primary source:** https://arxiv.org/abs/2609.25647 ; arXiv abstract and frozen protocol claims verified; source PDF tables were **not** independently re-analysed.

| Claim | Primary estimand / routing / Framework | First-coder scientific evidence and ceiling | Kill test |
|---|---|---|---|
| 120-C1 | `TARGET_HEAD_SPECIFIC_EARLY_OUTCOME_CALIBRATION_TRANSFER_GAP`; ROUTING_ABSTAIN+BGT / MEAS,ID,BT | Two target-head combinations show persistent corrected gaps 0.1377 and 0.1107 in SWE-bench Verified; CL1/I1/T1, conditional source-only observation. | Re-run frozen head+threshold with raw trajectories, independent scorer and bootstrap |
| 120-C2 | `PAIRED_AGENT_HETEROGENEITY_CALIBRATION_NULL_CONTRAST`; ROUTING_ABSTAIN+BGT / MEAS,ID,BT | Pre-registered broad heterogeneity criterion not met; pairwise medians 0.0180 SUCCESS/0.0385 FAILURE. Null on criterion is not proof of invariance or equivalence; CL1/I1. | Equivalence bound preregistration, adequate power and independent agent pairs |
| 120-C3 | `CROSS_BENCHMARK_EARLY_STOP_CALIBRATION_TRANSPORT_ELIGIBILITY`; ASR+BGT / DR,MEAS,ID,BT | TerminalBench success head had zero decisions (INDETERMINATE), failure head failed persistence criterion. T3/T4 NOT established; this study does not demonstrate safe stopping, CL1/T1. | Positive decision coverage across new benchmark×calibration×random STOP/CONTINUE×downstream harm |

**Decision:** confirm boundary/negative evidence and source qualification; preserve normative `ROUTING_ABSTAIN` for the measurement-focused Study. No cross-benchmark transport claim.

## Governance
- **Nine claim splits** across three Study identities. Formal CL2/CL3 promotions **0**; confirmed T3/T4 **0**.
- Second coder and adjudicator remain pending. Historical study-level candidate maturity must never be inherited by these Claim IDs.
- Formal SIS impact of today's literature: `MEASUREMENT_IDENTIFICATION_DELTA` secondary `BENCHMARK_DELTA`; Core pressure `WATCH`; `ScientificCoreDelta=0`.
