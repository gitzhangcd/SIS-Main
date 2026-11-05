# SIS P0 Claim-Level Re-Audit | 2026-11-05

Scientific authority: SIS v0.3.1 FROZEN. Three higher-priority candidates never previously re-audited as first coder. The current decision is a provenance-bound **first-coder screening**, not second-coder consensus. Source bases: primary arXiv abstract for all 3 and available paper text for Ecdysis. Full table/appendix independent verification and blind adjudication PENDING. No paper-level CL2/CL3 promotion.

## SIS-LIT-001 — WHALE: A Simple Recipe for Joint Harness-Weight Optimization

StudyVersionRecord: https://arxiv.org/abs/2609.00196 (v1, 2026-08-31). Boundary: Qwen 2B/4B, SearchQA/math/chess, switching rule, training rollouts, mean@8 metric.

| Claim | Primary observation | Routing; estimand | First coder scientific decision | Identification/transport |
|---|---|---|---|---|
| 001-C1 | Alternating weight/harness training has 4.15–24.38 percentage points better best mean@8 than studied weight-only, harness-only and Fast-Slow controls | SCF/CSCI; JOINT_WEIGHT_HARNESS_COMPOSITE_EFFECT; MI/IA/MEAS/ID/BT | CL1 combination; confirmation, **not** independent mechanism/mediator | I1/T1 |
| 001-C2 | Harness updating quickly benefits SearchQA; math gains only after a model-weight update; interleaving beats stagewise in tested setups | SCF/CSCI; MODEL_BY_HARNESS_UPDATE_ORDER_INTERACTION; MI/ID/MEAS/BT | CL1 conditional boundary; local CL2 candidate only with independent matched-budget and randomized order audit | I1/I2-local/T1 |
| 001-C3 | Fixed/adaptive phase-switch patience changes training rollout consumption | ASR/BGT; PHASE_SWITCH_COST_ADJUSTED_VALUE; DR/MEAS/BT | CL1 resource outcome; total computation and heldout performance not separated | I1/T0 |

Decision: split paper-level joint optimization claim into composite performance, model-harness conditional interaction, and switching resource value. No whole-study CL3 mechanism. Need 2x2 frozen factorial weight x harness, equal training + inference budget, held-out validation.

## SIS-LIT-020 — Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Models Catch Up Where Imitation Fails

StudyVersionRecord: https://arxiv.org/abs/2609.09134 (v1, 2026-09-08). Boundary: enterprise task distribution, weak/strong model, scaffold tailored to weak model, source of supervision and correction budget.

| Claim | Primary observation | Routing; estimand | First coder scientific decision | Identification/transport |
|---|---|---|---|---|
| 020-C1 | Expert often performs better using harness evolved for weaker model | SCF/CSCI; MODEL_HARNESS_COMPATIBILITY_CROSS_EXECUTOR_GAP; MI/IA/MEAS/BT | CL1 conditional interaction; not invariance | I1/T2 performance only |
| 020-C2 | Full expert-trajectory imitation under evolved harness regresses 4–30 points on 7 enterprise tasks for specified weak models, although it can help with unevolved harness | SDR/CSCI+BGT; FULL_IMITATION_EVOLVED_HARNESS_REGRESSION; TD/ID/MEAS/BT | CL1 important negative; local comparison potentially CL2 candidate but not universal failure | I1/I2-local/T1 |
| 020-C3 | Local turn-level on-policy expert correction recovers useful performance compared with complete teacher imitation | ASR/CSCI+BGT; ON_POLICY_LOCAL_CORRECTION_EFFECT; DR/MI/ID/MEAS/BT | CL1 joint intervention; local CL2 candidate conditional on teacher, budget and rollout matching | I1/I2-local/T2 performance only |

Decision: confirm negative model-harness incompatibility in studied tasks, but preserving native planning style is a **hypothesis** until independently intervened upon. T2 performance transfer does not establish T3 causal transport.

## SIS-LIT-032 — Ecdysis: Efficient and Effective Training of Runtime Harnesses for LLM Agents

StudyVersionRecord: https://arxiv.org/abs/2609.11677 (v1, 2026-09-10; not a new study). Boundary: number/diversity of failures, model task, iteration costs, cross-model transfer and stability of failure patterns.

| Claim | Primary observation | Routing; estimand | First coder scientific decision | Identification/transport |
|---|---|---|---|---|
| 032-C1 | Batch failure aggregation plus Failure-Driven Collaborative Refinement improves evolved-harness accuracy, reported +18.56% relative vs studied controls | ASR/CSCI+BGT; CROSS_INSTANCE_AGGREGATION_UPDATE_VALUE; DR/ID/MEAS/BT | CL1 composite confirmed; local CL2 candidate pending independent 2x2 aggregation x FDCR comparison | I1/I2-local/T1 |
| 032-C2 | Harness training up to 1.84x faster, quarter-data condition sometimes comparable to full-data | ASR/BGT; HARNESS_EVOLUTION_FULL_COST_DATA_EFFICIENCY; DR/MEAS/BT | CL1 cost and sampling only; must include coding/critic/evaluation workload | I1/T0 |
| 032-C3 | Repeat failures motivate bias toward systematic harness deficiencies; accommodation ratio and cross-LLM performance are reported | SCF/CSCI+BGT; HARNESS_DEFECT_VS_MODEL_ACCOMMODATION_IDENTIFICATION; IA/MI/ID/MEAS/BT | CL1 diagnostic boundary; **explicitly not causal proof** (authors call recurrence an inductive bias) | I1/T2 performance only |

Decision: restrict original whole-study CL1-to-CL2 candidate to local contrasts. Recurrent symptom does not identify a shared causal failure root. Candidate CL2 is not a final promotion.

## Audit governance

- First coder: 3 studies -> 9 distinct claims; source-linked confirmations, claim splitting, demotions of overbroad mechanistic interpretations.
- Second coder must inspect original experiment tables, sample sizes, confidence intervals, seed variability, resource budgets and exact model/task versions, test for training/test leakage and non-regression.
- Next kill tests: factorial harness x model update; local versus full imitation with equal training budgets; batch recurrence x collaborator diagnosis with independently injected harness versus model faults.
- FinalClaimLevel=PENDING_CLAIM_LEVEL_AUDIT. No confirmed new CL3, T3 or T4. Preserve any previously adjudicated claims elsewhere without silent overwrite.
