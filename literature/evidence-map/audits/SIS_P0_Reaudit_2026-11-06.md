# SIS P0 Claim-Level First-Coder Re-Audit | 2026-11-06

Authority: SIS v0.3.1 FROZEN; ClaimRecord v0.1. **Source-limited screening, not final re-adjudication.** The primary arXiv metadata/abstract and accessible original descriptions were inspected. Full paper tables, appendices, seed-level trajectories and blind second-coder checks remain PENDING. Therefore none of these candidate labels is a formal CL2/CL3 promotion.

## SIS-LIT-005 — LLM-as-a-Judge Is Not an Oracle

StudyVersionRecord: https://arxiv.org/abs/2609.02246; source anchor: arXiv v1 2026-09-02, original abstract and reported production case narratives; tables/appendices not independently checked. Boundary variables: contract, compliance and code tasks; production-derived examples, unknown independent labels and denominator.

| ClaimRecord ID | Primary observation / provenance | Program, estimand and Framework | First-coder scientific decision | Identification / transport |
|---|---|---|---|---|
| 005-C1 | Eleven evaluation failures grouped into judge bias, metric/harness, ground-truth and reward-hack issues; cached-key perfect metric conceals 68% true capability | SDR/BGT; `EVALUATOR_FAILURE_SURFACE_OBSERVED_MISALIGNMENT`; `TD/EG/MEAS/ID/BT` | CL1 case evidence, confirmation of measurement failure not population rate | I1/T0 |
| 005-C2 | PROCTOR gates LLM teacher with hermetic sandbox, disjoint privileges, deterministic checks, frozen holdouts and canaries | ASR/BGT; `DETERMINISTIC_UPDATE_GATE_ADMISSION_VIABILITY`; `DR/EG/ID/MEAS/BT` | CL0 architecture and CL1 examples; no isolated factorial gate effect | I0-I1/T0 |
| 005-C3 | Rubric edits plateau but structural output-order constraint helps in case observations | ASR/BGT; `RUBRIC_REWRITE_VS_STRUCTURAL_CONSTRAINT_EFFECT`; `DR/MI/ID/MEAS/BT` | CL1 descriptive conditional; not controlled general causal effect | I1/T0 |

Claim decisions: **split** the paper-level summary into exactly three evidential claims. Confirm descriptive/comparative evidence within contract, compliance and code tasks; production-derived examples, unknown independent labels and denominator; explicitly demote any implied universal mechanism or T3/T4 extrapolation without a matched intervention. All final claim levels remain `PENDING_CLAIM_LEVEL_AUDIT`. The next adjudicator must inspect the exact experiment tables and trace/control provenance.

## SIS-LIT-025 — ARISE-RL: Agentic Rubric-Grounded Iterative Self-Evolution

StudyVersionRecord: https://arxiv.org/abs/2609.01058; source anchor: arXiv v1 2026-09-01 original abstract; full numeric tables and ablations not independently fetched. Boundary variables: open-ended deep research / travel planning; solver capability boundary, model feedback, verifier privilege and reward density.

| ClaimRecord ID | Primary observation / provenance | Program, estimand and Framework | First-coder scientific decision | Identification / transport |
|---|---|---|---|---|
| 025-C1 | Joint task/rubric generator and solver co-evolution reports aggregate performance gains | ASR/BGT; `JOINT_RUBRIC_TASK_GENERATION_SOLVER_COMPOSITE_GAIN`; `DR/EG/MEAS/ID/BT` | CL1 joint system performance; no isolated task-generation causal effect | I1/T1 |
| 025-C2 | Reward-Gated Self-Evolution Distillation uses memory-conditioned performance gating | ASR/CSCI+BGT; `REWARD_GATED_MEMORY_DISTILLATION_INCREMENTAL_EFFECT`; `DR/MI/ID/MEAS/BT` | CL0 architecture and CL1 combined evidence; local CL2 requires equal-budget ablations | I1/T0 |
| 025-C3 | ECR-Bench expert calibrated rubrics support evaluation of open-ended tool outcomes | ROUTING_ABSTAIN/BGT; `EXPERT_RUBRIC_GOLD_CONSTRUCT_VALIDITY`; `MEAS/EG/ID/BT` | CL1 measurement instrument pending inter-rater and independent-Gold validation | I1/T0 |

Claim decisions: **split** the paper-level summary into exactly three evidential claims. Confirm descriptive/comparative evidence within open-ended deep research / travel planning; solver capability boundary, model feedback, verifier privilege and reward density; explicitly demote any implied universal mechanism or T3/T4 extrapolation without a matched intervention. All final claim levels remain `PENDING_CLAIM_LEVEL_AUDIT`. The next adjudicator must inspect the exact experiment tables and trace/control provenance.

## SIS-LIT-029 — How Fast Do Agents Rot? An Empirical Study of Long-Horizon Degradation

StudyVersionRecord: https://arxiv.org/abs/2609.01660; source anchor: arXiv v1 2026-08-31 primary abstract (10,664 trajectories) and described model/task/horizon design. Boundary variables: 9 models, 4 constructed task families, 5 horizon levels, 3 context regimes; simulator versus production.

| ClaimRecord ID | Primary observation / provenance | Program, estimand and Framework | First-coder scientific decision | Identification / transport |
|---|---|---|---|---|
| 029-C1 | Success decays strongly with number of dependent steps, compatible with geometric curves in tested cells | SDR/BGT; `HORIZON_CONDITIONAL_SUCCESS_DECAY_SHAPE`; `TD/MEAS/ID/BT` | CL1 descriptive model fit, not universal system law | I1/T1 |
| 029-C2 | Compressed context steepens decay relative to natural history: fitted logit slope −0.69 versus −0.44 (p=3×10^-6) | SDR/BGT; `CONTEXT_REGIME_CONDITIONAL_HORIZON_DECAY_EFFECT`; `TD/MI/ID/MEAS/BT` | CL1; local CL2 candidate only for well-matched context manipulations; compression also changes memory content | I1-I2-local/T1 |
| 029-C3 | Long-horizon production reliability can be projected from fitted per-step reliability | ROUTING_ABSTAIN/BGT; `SHORT_TO_LONG_HORIZON_EXTRAPOLATION_CALIBRATION`; `MEAS/ID/BT` | CL0 model projection, not empirically verified production transport; no T3/T4 | I0/T0 |

Claim decisions: **split** the paper-level summary into exactly three evidential claims. Confirm descriptive/comparative evidence within 9 models, 4 constructed task families, 5 horizon levels, 3 context regimes; simulator versus production; explicitly demote any implied universal mechanism or T3/T4 extrapolation without a matched intervention. All final claim levels remain `PENDING_CLAIM_LEVEL_AUDIT`. The next adjudicator must inspect the exact experiment tables and trace/control provenance.

## Audit governance / handoff

- First-coder output: 3 studies, 9 ClaimRecords, each with source, scientific routing, estimand, evidence role/ceiling, identification limit and boundary; no silently inherited CL2/CL3.
- Auditing metadata: coder=AUTOMATED_FIRST_CODER_2026-11-06; second_coder=PENDING; adjudication_status=PENDING; final_level=PENDING_CLAIM_LEVEL_AUDIT.
- Missing to complete: independently check full-text tables, baseline/seed CI, budget parity, source labels, multi-model transport and matched mediator interventions; preserve original task/metric version.
- Proposed kill tests: (005) frozen holdout and manipulated oracle-failure canaries x guardrail ablation; (025) Generator/Rubric/Reward-Gate 2×2×2 with same samples and compute; (029) step horizon x context visibility x recovery policy under fixed task semantics.
- All three original source records retain their existing permanent SIS-LIT identity, without creating duplicates. Historical unmerged Oct 9–23 candidates still require independent global reconciliation.
