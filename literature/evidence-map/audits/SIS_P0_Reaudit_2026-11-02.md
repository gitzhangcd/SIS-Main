# SIS P0 Claim-Level Re-Audit | 2026-11-02

**Authority:** SIS v0.3.1 Scientific Core FROZEN and existing claim semantics. **Coder:** first coder only. **Second coder / adjudication:** PENDING. **Primary evidence:** official ACL Anthology research abstracts and original arXiv abstract; appendix-level effect sizes, confidence intervals and exact randomization not independently rerun. **No whole-paper CL2/CL3 upgrade, no new T3/T4.** Read source version lineage before applying any claim ceiling.

## SIS-LIT-059 — Asclepius: An Adaptive Harness for Long-Horizon Clinical Agents
**StudyVersionRecord:** [Findings EMNLP 2026 authoritative; long-horizon Clinical Environment Simulator](https://aclanthology.org/2026.findings-emnlp.2094/). **Boundary variables:** 急诊班次拥堵程度、病例危重度、调度策略、专家评估可靠性、运行资源、是否有真实患者.

| ClaimRecord | Source anchor / reported observation | Primary / Cross / Framework | Estimand | Decision and provisional ceiling | I/T |
|---|---|---|---|---|---|
| 059-C1 | 临床长时程诊断正确但关键治疗遗漏/延迟，三个失败计数 | SDR/BGT;TD,MEAS,ID,BT | `CLINICAL_SHIFT_FAILURE_MODE_OBSERVATION` | CL1 descriptive; confirm, no causal bottleneck | I1/T0 |
| 059-C2 | 未见演化批次的 critical-action correctness +22% (p=0.024) vs strong baseline | SDR/CSCI,BGT;TD,DR,IA,MEAS,BT | `ADAPTIVE_CLINICAL_HARNESS_HELDOUT_CRITICAL_ACTION_EFFECT` | CL1 composite; local CL2 candidate contingent on matched resource/strata | I1/I2-candidate/T1 |
| 059-C3 | Operating manual rewrites + clinical library + three isolated subagents jointly reduce bottlenecks | SCF/CSCI,BGT;MI,IA,ID,MEAS | `CLINICAL_HARNESS_COMPONENT_INTERACTION_MEDIATION` | CL0 causal mediator hypothesis; demote paper-level interpretation; factorial absent | I0/I1/T0 |

**Decision:** Separate observed performance, local intervention and unverified causal explanation. Source-specific boundary, measured resource cost and independent Gold remain prerequisites for upgrading any controlled or mechanistic claim.

## SIS-LIT-077 — Chronicle: Cut-Point Replay for Regression Testing of LLM Agents
**StudyVersionRecord:** [REALM 2026 Workshop archival entry; same lineage arXiv:2609.20625 (2026-09-17)](https://aclanthology.org/2026.realm-1.71/). **Boundary variables:** 冻结边界数量、录制粒度、环境外部副作用、模拟模型输出、变更代码作用域.

| ClaimRecord | Source anchor / reported observation | Primary / Cross / Framework | Estimand | Decision and provisional ceiling | I/T |
|---|---|---|---|---|---|
| 077-C1 | 不可变边界封装让 20 次重放位级一致，零模型调用 | SDR/BGT;TD,EG,MEAS | `REPLAY_ENVELOPE_DETERMINISM_CONFORMANCE` | CL0 implementation property + CL1 controlled observation; confirm | I1/T0 |
| 077-C2 | 六次录制故障中 Cut-point 检测错误代码、允许修复与良性修改 | SDR/BGT;TD,ID,EG,MEAS | `CUT_POINT_VS_FULL_STUB_REGRESSION_DETECTION_EFFECT` | CL1, local CL2 candidate in six simulated episodes; scope restriction | I2-local/T0 |
| 077-C3 | 每次跨边界增加 23μs (0.008% of assumed 300ms model call) | ASR/BGT;DR,MEAS,BT | `REPLAY_RECORDING_OVERHEAD_CONDITIONAL_NET_VALUE` | CL1 conditional cost; no general deployment benefit; split | I1/T0 |

**Decision:** Separate observed performance, local intervention and unverified causal explanation. Source-specific boundary, measured resource cost and independent Gold remain prerequisites for upgrading any controlled or mechanistic claim.

## SIS-LIT-096 — MemCalib: Benchmarking and Optimizing Memory Use in LLM Agents
**StudyVersionRecord:** [arXiv:2609.24259, preprint, 2026-09-21](https://arxiv.org/abs/2609.24259). **Boundary variables:** 记忆原子分割、正确影响程度 Gold、基础模型、token 级归因、评价规则相关性与分布迁移.

| ClaimRecord | Source anchor / reported observation | Primary / Cross / Framework | Estimand | Decision and provisional ceiling | I/T |
|---|---|---|---|---|---|
| 096-C1 | 记忆误用有 over-use 与 under-use 的不对称性 | SCF/BGT;MEAS,EG,ID,BT | `MEMORY_INFLUENCE_CALIBRATION_DIRECTIONAL_ERROR` | CL1 descriptive negative; confirm, target rubric is constructed | I1/T1 |
| 096-C2 | GRPO/OPSD 等优化可能改善一端并恶化另一端 | ASR/BGT;DR,ID,MEAS | `MEMORY_CALIBRATION_SINGLE_CHANNEL_OPTIMIZATION_TRADEOFF` | CL1 conditional comparison; needs matched-seed/independent test | I1/T1 |
| 096-C3 | MemCalib-RL 使用双向反事实原子消融提高平衡分数 | ASR/CSCI,BGT;DR,ID,MI,MEAS | `BIDIRECTIONAL_MEMORY_CREDIT_ASSIGNMENT_POLICY_EFFECT` | CL1 composite; local CL2 candidate only if atom-ablation factorial and independent Gold verified | I1/I2-candidate/T2-perf-only |

**Decision:** Separate observed performance, local intervention and unverified causal explanation. Source-specific boundary, measured resource cost and independent Gold remain prerequisites for upgrading any controlled or mechanistic claim.


## Audit ledger
- **Confirmations:** 059 diagnostic vs critical-action execution gap; 077 deterministic replay observation; 096 directional memory-use calibration gap.
- **Splits:** 059 composite heldout effect vs component-mediator attribution; 077 replay conformance vs regression-detection and runtime cost; 096 over/under-use vs RL policy benefit.
- **Demotions/ceilings:** 059 all-three-components mediator remains CL0; Chronicle only six simulated failures and no causal transport; MemCalib atom-level ablation and downstream judgment dependence prevent unqualified mechanism claim.
- **Version lineage:** Chronicle's [REALM 2026 archival Workshop entry](https://aclanthology.org/2026.realm-1.71/) supersedes metadata-only arXiv preprint status but is the *same Study*.
- **Pending:** second-coder blinded assessment; audit of ablations, exact control budgets, judge independence and source passages; formal adjudication not authorized by this first-coder pass.
