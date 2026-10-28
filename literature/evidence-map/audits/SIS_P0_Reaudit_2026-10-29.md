# SIS P0 Claim-Level Re-Audit | 2026-10-29

**Authority:** SIS v0.3.1, SIS-LEM-P0 v0.1, ClaimRecord v0.1. **Scope:** three high-priority unaudited studies, nine separate claims. First coder only; no final promotion. Source-linked full papers (arXiv HTML), not abstract-only triage. Source dates and version identity provided below. **Second coder = PENDING; Adjudication = PENDING.**

## SIS-LIT-103 — CausalLoss-Fin

**StudyVersionRecord:** [primary v1 preprint](https://arxiv.org/abs/2609.25960); source classification PREPRINT. Canonical ID remains SIS-LIT-103, with no duplicate new study.

| Claim ID | Verified author-source anchor / contrast | Program and Framework | Primary estimand | First-coder ceiling / decision | I/T |
|---|---|---|---|---|---|
| 103-C1 | §V-C exact three-way loss decomposition; 3852/3852 deterministic checks | ROUTING_ABSTAIN; ID/EG/MEAS/BT | `SIGNED_LOSS_ACCOUNTING_IDENTITY` | CL0 formal identity conditional on specified policy/reference/world; no empirical mechanism level | I0/T0 |
| 103-C2 | §VII–VIII planted single/conjunctive/overdetermined faults; 545 episodes/3 deterministic policies; repair intervention | SDR; TD/MI/ID/MEAS/BT | `JOINT_INFRASTRUCTURE_POLICY_FAULT_REPAIR_EFFECT` | Local CL2 candidate for exact deterministic planted-world interventions; do not extend to stochastic LLM agents | I2-local/T0 |
| 103-C3 | §VIII interaction cases; 27.8% [23.3,32.3] infrastructure-loss episodes nonadditive, 5.6% overdetermined subset | SDR; TD/IA/ID/MEAS/BT | `INTERACTING_MESSAGE_FAULT_NONADDITIVITY_RATE` | CL1 conditional prevalence over planted generator, with local intervention examples; no universal population prevalence | I2-local/T0 |

**Evidence, confounding and mechanism ceiling:** The article explicitly states NO language-model agent was evaluated. Baseline is an agent-step intervention-scope abstraction, not an exact reimplementation of published CAR/CausalFlow/REFLECT. Signed Shapley allocation is not automatically causal mediation. Existing registry whole-paper CL2→CL3 candidate is split; full CL3 claim is unsupported. Competing direct infrastructure effects not represented.

**Provenance:** Coder=first independent SIS audit on 2026-10-29; original author claim and audited inference kept separate; source URL above, section anchors in row. Second coder PENDING, adjudication PENDING.


## SIS-LIT-003 — AutoSaddler

**StudyVersionRecord:** [primary v1 preprint](https://arxiv.org/abs/2608.23041); source classification PREPRINT. Canonical ID remains SIS-LIT-003, with no duplicate new study.

| Claim ID | Verified author-source anchor / contrast | Program and Framework | Primary estimand | First-coder ceiling / decision | I/T |
|---|---|---|---|---|---|
| 003-C1 | Abstract, §5.2: test improvements +9.0/+9.6/+10.0 pp GAIA2/SWE-bench Pro/Terminal-Bench 2.0 over base harnesses | SCF; MI/MEAS/BT | `COMPOSITE_HARNESS_OPTIMIZATION_PERFORMANCE_EFFECT` | CL1 bundled performance; no individual mechanism attribution | I1/T1 |
| 003-C2 | §5.3, Appendix F Table 10: dev filtering removed 60.7→50.0; removing Reflection+EvoDAG further 44.9 | ASR; DR/EG/ID/MEAS/BT | `DEVELOPMENT_SET_FILTERING_UPDATE_ADMISSION_EFFECT` | Local CL2 candidate for tested filtering contrast; optimize/replay variance and fixed-task selection require further audit | I2-local/T0 |
| 003-C3 | §5.3: deep diagnosis vs shallow LLM-only 62.0→57.8 GAIA2, deep variant +6.2 tool calls and +5.8 file accesses per step | ASR; DR/ID/MEAS/BT | `DIAGNOSTIC_DEPTH_COST_ADJUSTED_OPTIMIZATION_GAIN` | CL1/I1, not isolated causal mechanism: more information/compute accompanies diagnosis | I1/T0 |

**Evidence, confounding and mechanism ceiling:** Generalization-aware selection bundles dev filtering and reflection in major ablation; finer-grain comparison only one universe and three repeats. Different developer/test domains help T1 performance replication, not T3. Reflection path and dev-gating are not fully controlled mediators.

**Provenance:** Coder=first independent SIS audit on 2026-10-29; original author claim and audited inference kept separate; source URL above, section anchors in row. Second coder PENDING, adjudication PENDING.


## SIS-LIT-004 — DCFA

**StudyVersionRecord:** [primary v1 preprint](https://arxiv.org/abs/2609.04749); source classification PREPRINT. Canonical ID remains SIS-LIT-004, with no duplicate new study.

| Claim ID | Verified author-source anchor / contrast | Program and Framework | Primary estimand | First-coder ceiling / decision | I/T |
|---|---|---|---|---|---|
| 004-C1 | Abstract/§5.4: Who&When six LLMs; reported up-to +8.27% step-level attribution accuracy | SDR; TD/ID/IA/MEAS/BT | `TRACE_DIAGNOSTIC_STEP_LABEL_ACCURACY_GAIN` | CL1 prediction/label agreement; not causal failure localization | I1/T1 |
| 004-C2 | §5.4.2 Table 2: LCE module adds mean +3.45% hand-crafted and +1.93% algorithm-generated step accuracy over GCA-only | SCF; MI/ID/MEAS/BT | `LOCAL_CONTEXT_EXPLORATION_DIAGNOSTIC_ACCURACY_INCREMENT` | CL1/I1 localized ablation; procedure/information conditions change; no executed recovery manipulation | I1/T1 |
| 004-C3 | §3–5: graph construction + counterfactual-inspired LLM search called decisive-error attribution | SDR; TD/ID/EG/BT | `TRUE_DECISIVE_ERROR_OUTCOME_FLIP_MEDIATION` | CL0 unverified mechanism: no exhaustive environment rerun with corrected error and independently verified outcome flip; do not inherit CL2 from title | I0/T0 |

**Evidence, confounding and mechanism ceiling:** Causal-inspired reasoning and dependency graphs are not do-interventions on executable system states. Ground truth Who&When labels measure diagnostic agreement, not true recovery causality. Longer-trace conditions change task complexity; model-level comparisons only T1.

**Provenance:** Coder=first independent SIS audit on 2026-10-29; original author claim and audited inference kept separate; source URL above, section anchors in row. Second coder PENDING, adjudication PENDING.

## Governance ledger

- **Confirmations:** 103 exact signed accounting and controlled planted-fault contrast; 003 tested held-out performance improvements and narrower selection contribution; 004 step-label diagnostic improvements.
- **Splits:** nine independent scientific questions, no inherited paper-wide maturity/Primary. 103 algorithmic identity is not CL3 causal mediation; 003 bundle gains vs component validity; 004 predicted step error vs true counterfactual repair.
- **Demotions and non-inflation:** 103 whole-paper CL2→CL3 candidate reduced to CL0 identity / local CL2 candidate / conditional CL1; 004 causal-inspired mechanism does not support CL2; 003 deep-diagnosis causal claim remains CL1 under extra-tool-call confounding.
- **Final adjudication:** no new final CL2/CL3, T3 or T4. Maintain source/claim lineage and independent coder gate.
