# SIS P0 Claim-Level Re-Audit｜2026-11-23

**Authority:** SIS v0.3.1 Scientific Master; Evidence Map P0; ClaimRecord schema; Registry and Audit Queue main as fetched this run. **Status:** FIRST_CODER_ONLY; SECOND_CODER_PENDING; ADJUDICATION_PENDING. This note documents evidence ceilings and claim splits, **not formal CL promotions**.

## SIS-LIT-076｜SoL-Pi
**Primary source:** https://arxiv.org/abs/2609.20519. **Inspected:** arXiv原始全文的Method 2.1/2.2、Table 1–3、3.2跨Benchmark；NVIDIA研究页面版本身份核对. **Qualification:** `PRIMARY_HTML_METHOD_TABLES_VERIFIED_2026-11-23`. Source identity is verified; no independent execution replication.

| Claim | Primary estimand / SIS Program / Framework | Evidence role, measured contrast and first-coder ceiling | Independent Kill Test |
|---|---|---|---|
| 076-C1 | `FOUR_MECHANISM_HARNESS_SCORE_TOKEN_COST_PARETO`; SCF+BGT; MI/MEAS/ID/BT | EdgeBench GPT-5.6 Sol：Pi得分44.833/成本$1339；完整SoL-Pi效率配置42.003/$894。分数降低2.83但价格降低33.2%，不能描述成无代价的能力提升。 **Ceiling:** CL1/I1/T1. | 事先约定非劣效容忍度×等端到端预算×盲测试多次重复 |
| 076-C2 | `INDIVIDUAL_MECHANISM_CONDITIONAL_COST_PERFORMANCE`; SCF+CSCI+BGT; MI/IA/MEAS/ID/BT | GPT-5.6 Sol下单独ObservationPack得47.208、$1271；完整栈42.003/$894。组件收益非加性；消融不是4机制的全因子正交识别。 **Ceiling:** CL1/I1; local CL2 candidate conditional. | 四机制析因×固定模型×缓存策略×等Token×中介证据 |
| 076-C3 | `FROZEN_HARNESS_ACROSS_BACKBONE_PERFORMANCE_TRANSFER`; SCF+CSCI/BGT; MI/IA/BT/MEAS/ID | 同一效率栈迁移到未参与搜索的Opus 5：Pi得44.756/$1741，对应SoL-Pi 42.224/$1158；显示条件性成本优势但非T3/T4因果机制可迁移。 **Ceiling:** CL1/I1/T2-performance. | 跨主干与任务域×完全冻结配置×统一基础Harness×净收益与不变性检验 |

**Audit decision:** split performance, mechanistic explanations and transport/stopping. No CL2/CL3 promotion or T3/T4 certification until independent second coder and adjudication. 

## SIS-LIT-078｜FORGE
**Primary source:** https://arxiv.org/abs/2609.15209. **Inspected:** arXiv原始全文Introduction/Experiments/Table 2累积消融及Transfer部分. **Qualification:** `PRIMARY_ARXIV_FULLTEXT_TABLE_VERIFIED_2026-11-23`. Source identity is verified; no independent execution replication.

| Claim | Primary estimand / SIS Program / Framework | Evidence role, measured contrast and first-coder ceiling | Independent Kill Test |
|---|---|---|---|
| 078-C1 | `CO_EVOLVED_PROMPT_TRAINING_DATA_TOTAL_OPTIMIZATION_VALUE`; ASR+BGT; DR/EG/MEAS/ID/BT | 八基准平均：原始55.66，FORGE 72.18（+16.52点）。多模块联合方案，不能因训练数据增长推断科学原因。 **Ceiling:** CL1/I1/T1. | 同预算静态数据×相同提示搜索×独立测试×种子与总成本 |
| 078-C2 | `FAILURE_MEMORY_MUTATION_GUIDANCE_CONDITIONAL_INCREMENT`; ASR+SCF/BGT; DR/MI/EG/ID/MEAS | Table 2：仅提示优化64.17，加入随机合成降至62.38，再加失败记忆68.24、再加定向变异72.18。作者明确说明这些是累积条件贡献，不是独立主效应。 **Ceiling:** CL1/I1; conditional local CL2 candidate. | 随机合成/失败抽象/变异策略2×2×2正交×数据真实性与独立验证 |
| 078-C3 | `SYNTHETIC_FAILURE_DATA_CROSS_OPTIMIZER_TRANSFER_VALUE`; SCF+CSCI/BGT; MI/IA/EG/MEAS/BT | 匹配训练预算下作者报告9项APO比较和3项GRPO比较均有提升；是跨优化流程表现迁移，不是已鉴定数据生成中介或T3。 **Ceiling:** CL1/I1/T2 performance. | 任务生成器与训练模型交叉×匹配数据样本×独立验证集×假失败模式负控制 |

**Audit decision:** split performance, mechanistic explanations and transport/stopping. No CL2/CL3 promotion or T3/T4 certification until independent second coder and adjudication. 

## SIS-LIT-094｜SelfOp
**Primary source:** https://arxiv.org/abs/2609.22792. **Inspected:** arXiv原始全文Introduction/3.4 convergence/benchmark methods/ablation；未独立复现CyberGym执行. **Qualification:** `PRIMARY_ARXIV_FULLTEXT_METHOD_RESULTS_VERIFIED_2026-11-23`. Source identity is verified; no independent execution replication.

| Claim | Primary estimand / SIS Program / Framework | Evidence role, measured contrast and first-coder ceiling | Independent Kill Test |
|---|---|---|---|
| 094-C1 | `CROSS_INSTANCE_CONTEXT_OPTIMIZATION_SECURITY_SUCCESS_GAIN`; ASR+BGT; DR/MI/EG/ID/MEAS/BT | 作者报告少于200训练例，冻结模型/执行框架时，GPT-5.4-mini提升17点、GPT-5.4提升18.5点。成功率增益为整体文本优化方法，不是梯度可微的证明。 **Ceiling:** CL1/I1/T1. | 独立任务分割×随机反馈/一致性控制×等优化预算×真实执行评分器 |
| 094-C2 | `TEXTUAL_GRADIENT_CONSENSUS_COVERAGE_MECHANISM`; SCF+ASR/BGT; MI/DR/EG/ID/MEAS | 链式错误文本回传、跨实例主题聚类、hard/soft梯度注释一起改变；未测到可识别的中介路径，所谓‘chain rule’是设计隐喻，不是数值梯度。 **Ceiling:** CL0 mechanistic hypothesis plus CL1 implementation. | 分离逐阶段归因×一致性门控×梯度质量独立Gold×错误定位干预 |
| 094-C3 | `VALIDATION_FREE_TEXTUAL_SIGNAL_STOPPING_HELDOUT_NET_VALUE`; ASR+BGT; DR/TD/MEAS/ID/BT | Section 3.4：信号停止于第8步测试55%，验证选择第11步测试51%，测试集oracle第12步56.2%；相差1个/80任务的峰值效应不显著。噪声基线p0与窗口参数经验标定，不能宣布免验证永远更好。 **Ceiling:** CL1/I1/T0 (local stop candidate). | 预冻结停机规则×新任务分布×STOP/CONTINUE随机化×相同完整计算成本 |

**Audit decision:** split performance, mechanistic explanations and transport/stopping. No CL2/CL3 promotion or T3/T4 certification until independent second coder and adjudication. 

## Governance / Reconciliation
- 3 existing StudyVersionRecords, **9 independently identified scientific Claim units**. Final CL promotions **0**, confirmed causal transport T3/T4 **0**. Their prior registry paper-level `CL1→CL2 candidate` is triage metadata only.
- All three have upgraded primary-source verification based on first-coder original HTML/table review; update Queue status and leave normative final fields `PENDING_CLAIM_LEVEL_AUDIT`.
- To strengthen P0 validity, plan a second-coder test of exact authors' tables, resource equivalence, selection bias and evaluation independence before any formal maturity change.
