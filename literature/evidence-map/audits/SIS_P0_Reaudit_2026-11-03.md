# SIS P0 Claim-Level Re-Audit | 2026-11-03

Authority: SIS v0.3.1 scientific semantics frozen. First coder only; second blinded coder/adjudication PENDING. Primary source abstracts and official ACL records verified. No automatic paper-level CL2/CL3, no confirmed T3/T4. Exact appendix-level ablations, CIs, randomization and independent gold remain second-coder tasks.

## SIS-LIT-089 — ARCHITECT: Uncertainty-Aware Dynamic Tool Learning via Causal Intervention for Open-World Agents

StudyVersionRecord: https://aclanthology.org/2026.acl-long.1707/; ACL 2026 Long, official archival publication; same study as any preprint.
Boundary variables: 规范质量、沙盒修改、代码、运行环境、模型、修复次数.

| Claim | Source observation / provenance | Primary/Cross; Framework | Estimand | First-coder claim decision / ceiling | ID / Transport |
|---|---|---|---|---|---|
| 089-C1 | 所研究动态生成工具首用失败率为 32.4% | SDR/BGT;TD,ID,MEAS,BT | DYNAMIC_TOOL_FIRST_FAILURE_BASE_RATE | CL1 descriptive; source-specific confirmed | I1/T0 |
| 089-C2 | 规范、代码和环境沙盒干预；ρ=0.90 置信排序，78% 归因准确率 | SDR/BGT;MI,ID,MEAS,EG | SANDBOX_FACTOR_INTERVENTION_ATTRIBUTION_VALIDITY | CL1 diagnostic accuracy; local CL2 candidate only for manipulated causal factors | I2-local/T1 |
| 089-C3 | 目标修复比错误类别判断提高约 9.6% 成功率；整体四个 Benchmark 改善 | SDR/CSCI,BGT;DR,MI,ID,MEAS | DIAGNOSIS_ROUTED_TOOL_REPAIR_NET_VALUE | CL1 composite; local CL2 candidate, inherited CL2→CL3 whole-study mediator DEMOTED | I1/I2-local/T1 |

Decision: 保留沙盒受控干预的局部因果候选，但 SCM 和预测归因准确率不构成完整 do(M)→Z→Y 中介。需独立审计随机化、干预路径与真实修复的相同状态对照。

## SIS-LIT-068 — Dream-RSI: Recursive Self-Improvement through Evolving Worlds

StudyVersionRecord: https://arxiv.org/abs/2609.14858; September 2026 arXiv preprint; no independently confirmed archival successor.
Boundary variables: 历史分支覆盖、基础模型、离线回放有效性、评价器固定、预算、未见空间.

| Claim | Source observation / provenance | Primary/Cross; Framework | Estimand | First-coder claim decision / ceiling | ID / Transport |
|---|---|---|---|---|---|
| 068-C1 | 发现树复用既有实际探索分支、保存结果供策略重排使用 | ASR/BGT;TD,DR,EG,MEAS | REALIZED_DISCOVERY_TREE_REPLAY_SUPPORT | CL0 conditional implementation + CL1 empirical; no unseen-world claim | I0/I1/T0 |
| 068-C2 | 历史回放更新探索策略，和固定探索策略在部分匹配预算实验比较 | ASR/BGT;DR,ID,MEAS,BT | MATCHED_BUDGET_REPLAY_POLICY_EFFECT | CL1; local CL2 candidate after full budget/seed verification | I1/I2-local/T1 |
| 068-C3 | 算法、数学优化和 GPU kernel 多类任务中表现及费用比较 | ASR/CSCI,BGT;DR,MEAS,BT | REPLAY_POLICY_CROSS_DOMAIN_QUALITY_COST_TRANSFER | CL1 performance only; T2 not T3 causal transport | I1/T2-performance-only |

Decision: 历史记录只覆盖真实出现过的候选，不是未知动作的可识别反事实。要把历史选择偏差与系统搜索净成本纳入第二编码者审核；跨领域得分不得晋升机制不变性。

## SIS-LIT-088 — What Prompts Don’t Say: Understanding and Managing Underspecification in LLM Prompts

StudyVersionRecord: https://aclanthology.org/2026.findings-acl.441/; Findings ACL 2026 official archival record, arXiv:2505.13360 same version lineage.
Boundary variables: 需求遗漏、默认推断、互斥需求、模型版本、Prompt 编辑、任务 Gold.

| Claim | Source observation / provenance | Primary/Cross; Framework | Estimand | First-coder claim decision / ceiling | ID / Transport |
|---|---|---|---|---|---|
| 088-C1 | 未声明需求被默认推断约 41.1%；欠规范 Prompt 在升级或变更后回归风险约两倍 | SCF/BGT;MI,ID,MEAS,BT | UNDERSPECIFIED_REQUIREMENT_REGRESSION_RISK | CL1 negative/conditional; CONFIRM | I1/T1 |
| 088-C2 | 把遗漏的全部要求直接写进 Prompt 并不能稳定改善表现 | SCF/BGT;MI,ID,MEAS | EXPLICIT_REQUIREMENT_ADDITION_CONDITIONAL_EFFECT | CL1 conditional; potential local CL2 pending exact matched contrast | I1/I2-local/T1 |
| 088-C3 | 需求感知 Prompt 优化比简单加入所有要求平均提高约 4.8% | ASR/BGT;DR,MI,ID,MEAS | REQUIREMENTS_AWARE_OPTIMIZATION_HELDOUT_VALUE | CL1 composite; no mechanistic CL3 | I1/T1 |

Decision: 拆分隐含需求推断、显式加需求的条件性负结果和多模块优化器收益；禁止将 4.8% 整体增益归因于单个机制。

## Audit ledger

- Confirmations: dynamic tool failure and attribution observations (089); observed-branch replay support and conditional optimization gain (068); underspecification and regression boundary (088).
- Splits: 089 descriptor/intervention/repair; 068 historical simulator/optimizer/transport; 088 inferred requirements/explicit requirements/optimized results.
- Demotions: 089 prior whole-paper CL2→CL3 candidate unsupported as a complete mediated causal effect; 068 prior generic CL2 label scoped to matched replay only; 088 optimizer effect remains CL1 without unique mechanism.
- Lineage: ARCHITECT and What Prompts Don't Say are archival ACL 2026 publications; Dream-RSI remains a preprint. No extra Study ID created.
- Finality: independent second-coder study-version, statistics and evidence path verification pending. final_claim_level remains PENDING_CLAIM_LEVEL_AUDIT.
