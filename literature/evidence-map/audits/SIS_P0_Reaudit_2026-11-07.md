# SIS P0 First-Coder Re-Audit｜2026-11-07

基准：SIS v0.3.1 / ClaimRecord v0.1。所有结论基于明确原始来源，**不等于第二编码者裁决或正式晋升**。018 与 054 已审核 arXiv HTML 方法/表格，108 只核对官方 ACL Anthology 摘要，完整表格仍 PENDING。

## SIS-LIT-018｜AgentGrad

StudyVersionRecord：https://arxiv.org/html/2609.08572v2。来源锚点：Sec 4, Algorithm 1, Tables 3/4/6。按 Claim 拆分：

| ClaimRecord | 原始实验/结果及边界 | Program / estimand / Framework | I/T | 初审决定 |
|---|---|---|---|---|
| 018-C1 | 序贯提示干预选择可使失败转为成功的组件，但可能有多个充分修复位置 | ASR/CSCI+BGT; `SUFFICIENT_LOCAL_HINT_REPAIR_LOCUS`; `DR/MI/ID/BT` | I2local/T0 | 局部CL2候选；撤回整篇CL2确认的自动继承 |
| 018-C2 | 表3：TI使HotpotQA 67.89→69.33、PUPA 85.74→89.58；AS/STGA又带来增量，但非完整交叉设计 | ASR/BGT; `TEXTUAL_GRADIENT_COMPONENT_INCREMENT`; `DR/MI/MEAS/ID/BT` | I1-I2local/T1 | CL1组合消融，局部候选，不能宣称完整中介 |
| 018-C3 | 表6同领域未见基准迁移，例如2WikiMultiHopQA 51.22与GEPA 44.89；另报告优化时间及成本改进 | ASR/BGT; `PROMPT_CROSS_BENCHMARK_VALUE_COST`; `DR/MEAS/BT` | I1/T2-performance | CL1性能，禁止T3推断 |

独立裁决条件：资源/信息等价对照、真实干预、独立 Gold、统计不确定性、跨模型条件及相应中介试验；若不满足，最高保持有界 CL1 / CL2 candidate，拒绝 CL3 与 T3/T4 自动外推。

## SIS-LIT-054｜TrajDebug

StudyVersionRecord：https://arxiv.org/html/2608.06346v1。来源锚点：Sec 3–6, Tables 1–3。按 Claim 拆分：

| ClaimRecord | 原始实验/结果及边界 | Program / estimand / Framework | I/T | 初审决定 |
|---|---|---|---|---|
| 054-C1 | 486条人工标注失败轨迹，关键步AVG 34.11 vs Qwen直接诊断25.69；表2消融表明历史压缩影响较大 | SDR/BGT; `CRITICAL_STEP_LABEL_AGREEMENT`; `TD/MEAS/ID/EG/BT` | I1/T1 | CL1预测准确率，不是因果根因 |
| 054-C2 | 四种错误生命周期状态及终点足迹分类；最终责任仍由LLM从候选中选出 | SDR/BGT; `ERROR_STATE_TERMINAL_FOOTPRINT`; `TD/ID/EG/BT` | I0-I1/T0 | CL0定义、CL1诊断，缺真实do(error) |
| 054-C3 | 表3：理想错误已知场景平均成功率78.07→88.87；失败记忆在保留集上有改善 | ASR/BGT; `DIAGNOSTIC_FEEDBACK_RERUN_VALUE`; `DR/TD/ID/MEAS/BT` | I1-I2local/T1 | CL1组合恢复；与对照的因果贡献需独立续跑 |

独立裁决条件：资源/信息等价对照、真实干预、独立 Gold、统计不确定性、跨模型条件及相应中介试验；若不满足，最高保持有界 CL1 / CL2 candidate，拒绝 CL3 与 T3/T4 自动外推。

## SIS-LIT-108｜Reasoning as Gradient

StudyVersionRecord：https://aclanthology.org/2026.findings-acl.438/。来源锚点：Findings ACL 2026 official abstract; tables and PDF not fully checked。按 Claim 拆分：

| ClaimRecord | 原始实验/结果及边界 | Program / estimand / Framework | I/T | 初审决定 |
|---|---|---|---|---|
| 108-C1 | Gome组合诊断方向、成功记忆和多轨迹搜索，在12h V100限制下报告MLE-Bench 35.1% any-medal | ASR/BGT; `DIRECTED_MLE_OPTIMIZATION_COMPOSITE_VALUE`; `DR/MI/MEAS/ID/BT` | I1/T1 | CL1组合表现，不可归于单一梯度机制 |
| 108-C2 | 十种模型中弱模型倾向树搜索，强模型倾向定向优化，能力分界可能存在 | SCF/CSCI+BGT; `MODEL_CAPABILITY_BY_OPERATOR_CROSSOVER`; `IA/DR/MEAS/ID/BT` | I1/T1 | CL1能力交互，后续需等算力因子实验 |
| 108-C3 | 将诊断比作梯度、成功记忆比作动量是算法解释，尚未证明连续数学梯度或机制中介 | ROUTING_ABSTAIN/BGT; `DIAGNOSTIC_GRADIENT_ANALOGY_VALIDITY`; `MI/ID/MEAS/BT` | I0/T0 | CL0解释，任何CL3倾向降级 |

独立裁决条件：资源/信息等价对照、真实干预、独立 Gold、统计不确定性、跨模型条件及相应中介试验；若不满足，最高保持有界 CL1 / CL2 candidate，拒绝 CL3 与 T3/T4 自动外推。

## 治理与交接

- 3 Studies / 9 claim-level records：split 9；确认有界 CL1；没有正式 CL2+ promotion。
- **Demotion:** 018 原 2026-09-24 paper-level `CL2_CONFIRMED` 重开，变更为 `PENDING_CLAIM_LEVEL_AUDIT`（已有局部控制不能解释整篇机制）。054「causal attribution」仅有专家标签与 LLM 推断，须 do(step) 续跑；108「gradient」属于类比，不是已识别中介。
- Second coder: PENDING; adjudication: PENDING; audit_version SIS-LEM-P0-v0.1; coder AUTOMATED_FIRST_CODER_2026-11-07。
- Kill Tests：018 TI×AS×STGA 等预算全因子；054 错误步骤替换 vs Placebo、冻结实际状态后续跑；108 模型能力×算子（树搜索/定向诊断）×预算三因子。
