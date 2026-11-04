# SIS P0 Claim-Level Re-Audit | 2026-11-04

Authority: SIS v0.3.1 frozen. First coder source-level audit; independent second coder and full-table/appendix statistical verification PENDING. No whole-study CL2/CL3 promotions, no T3/T4.

## SIS-LIT-115 — RRSI: Regularized Recursive Self-Improvement of Agent Harnesses

StudyVersionRecord: https://arxiv.org/abs/2609.24972 (v3 2026-10-04). Boundary: 演化任务重叠、模型、预算、跨域和计算成本.

| Claim | Source fact / observation | Scientific routing | Estimand | Preliminary decision / ceiling | ID/Transport |
|---|---|---|---|---|---|
| 115-C1 | 训练收益与 OOD 收益不一致 | ASR/BGT; DR/ID/MEAS/BT | UNREGULARIZED_RSI_ID_OOD_GAP | CL1 conditional negative; confirmed | I1/T1 |
| 115-C2 | 编辑约束、Critic、Pruner 组合在五个 OOD 基准最多提高 4.3 点 | ASR/CSCI,BGT; DR/MI/EG/ID/MEAS/BT | REGULARIZED_RSI_HELDOUT_POLICY_EFFECT | CL1 package; local CL2 candidate, mechanism not split | I1/I2-local/T2-performance-only |
| 115-C3 | 运行策略 token 消耗约减少 30%，非完整搜索总成本 | ASR/BGT; DR/MEAS/BT | POLICY_TOKEN_VS_FULL_RSI_COST | CL1 conditional cost; no CL3 | I1/T0 |

Decision: 将整篇因果候选拆为负结果、组合效果、成本测量；Proposer/Critic/Pruner 独立贡献未识别。

## SIS-LIT-118 — CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents

StudyVersionRecord: https://arxiv.org/abs/2609.26779 (v1 2026-09-22). Boundary: 上下文长度、模型、压缩条件、并行尝试数、成本范围.

| Claim | Source fact / observation | Scientific routing | Estimand | Preliminary decision / ceiling | ID/Transport |
|---|---|---|---|---|---|
| 118-C1 | 原始内容裁剪/删除压缩在 Terminal-Bench 等单次运行最多省 50% 成本 | SCF/BGT; MI/MEAS/BT | ORIGINAL_ONLY_COMPACTION_PER_RUN_COST | CL1; local CL2 candidate if matched budget verified | I1/I2-local/T1 |
| 118-C2 | 省下预算允许更多尝试，整体性能前沿变化 | ASR/CSCI,BGT; DR/ID/MEAS/BT | COMPACTION_ENABLED_SCALING_FRONTIER | CL1 composite; no unique mediator | I1/T2-performance-only |
| 118-C3 | KernelBench 200/400 步分别报告 2.23x/3.58x 加速 | SCF/BGT; MI/TD/MEAS/BT | LONG_SESSION_CONTEXT_RETENTION_EFFECT | CL1 empirical; no invariant mechanism | I1/T1 |

Decision: 按单次成本、额外搜索、长时程表现拆开；模型调用费用不等于总净成本。

## SIS-LIT-127 — A Wrong Turn Does Not Ruin the Journey: Deviation-Guided Skill Self-Evolution for LLM Agents

StudyVersionRecord: https://arxiv.org/abs/2609.29154 (v1 2026-09-24). Boundary: 偏离点精度、教师能力、共享前缀、技能状态、对比预算.

| Claim | Source fact / observation | Scientific routing | Estimand | Preliminary decision / ceiling | ID/Transport |
|---|---|---|---|---|---|
| 127-C1 | 执行有效性和目标进展识别正确前缀和错误后缀 | SDR/BGT; TD/ID/MEAS | DEVIATION_POINT_DETECTION_VALIDITY | CL1 diagnosis only; no causal mediator | I1/T1 |
| 127-C2 | 同前缀强教师续跑，比较失败后缀构造局部修复 | ASR/BGT; DR/MI/TD/ID/MEAS | SAME_PREFIX_LOCAL_SKILL_REPAIR_EFFECT | CL1 package; local CL2 candidate pending teacher/budget control | I1/I2-local/T1 |
| 127-C3 | ToolQA、LogicBench、WildClawBench 跨任务表现 | SCF/CSCI,BGT; MI/DR/MEAS/BT | SKILL_UPDATE_CROSS_EXECUTOR_TRANSFER | CL1 performance only; T2 not T3 | I1/T2-performance-only |

Decision: 教师强度与修复方案混杂；性能转移≠因果迁移，位置定位不能自动晋升。

## Audit governance

Confirmations: three studies have source-linked evidence. Splits: 115 into OOD gap, selection composite, cost; 118 into compaction, scaling and long-run retention; 127 into diagnosis, local repair and transfer. Demotions: original paper-level causal-candidate scope is not a CL3 mechanism; local CL2 candidates not finalized. Next blinded reviewer must check exact budget, independent Gold, randomization/variance and cross-version lineage. FinalClaimLevel=PENDING_CLAIM_LEVEL_AUDIT; second-coder=Pending.
