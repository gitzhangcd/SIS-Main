# SIS P0 Claim-Level Re-Audit | 2026-10-30

**Governing sources:** SIS v0.3.1, SIS-LEM-P0 v0.1, ClaimRecord v0.1. **Scope:** 3 previously un-audited high-priority papers, nine ClaimRecords. Source identities, contrasts and limitations below. **Coder:** first only; second coder=PENDING, adjudication=PENDING, final_claim_level=PENDING. No paper-wide CL2/CL3 label inherited.

## SIS-LIT-023 — Does Your Agent's Memory Survive a Model Upgrade?

**StudyVersionRecord:** [original author source](https://arxiv.org/html/2609.05339v1). **Qualification:** 48合成历史，每个160个随机编码问题，两种小模型；签名分析锁中的4个>5pp预设检验，仅H2和H7a成立；H1/H4a不成立，不得平均掩盖方向差异。

| Claim ID | Source anchor / contrast | Program and Framework | Primary estimand | First coder ceiling & decision | I/T |
|---|---|---|---|---|---|
| 023-C1 | §4.1 Table 2 H1/H4a 未支持；§4.2 NOTES迁移方向 +9.91/-13.28pp、KG变化小 | SCF; CSCI/BGT; MI/EG/MEAS/ID/BT | `WRITER_READER_DIRECTIONAL_MEMORY_COMPATIBILITY` | CL1条件性差异；整体KG普遍更优不可声称 | I2-local/T2-performance |
| 023-C2 | §4.1 Table 2 H2: 完整重嵌入胜过50/50混合索引+6.95pp，Holm p=1.3e-6 | SDR; BGT; TD/MI/MEAS/ID/BT | `MIXED_INDEX_VS_FULL_REEMBED_ACCURACY` | 局部CL2候选；仅已测试嵌入对比 | I2-local/T0 |
| 023-C3 | §4.1 Table 2 H7a: 保存原始历史修复比仅修复NOTES +8.90pp，Holm p=3.9e-7 | ASR; BGT; DR/EG/MEAS/ID/BT | `RAW_SOURCE_RETENTION_REPAIR_EFFECT` | 局部CL2候选；原文源数据与预算必须受控 | I2-local/T0 |

**ClaimRecord controls:** source-versus-claim, model/resource regime, original author outcome versus audited causal interpretation, measurement independence and untested mediators retained; second coder required.

## SIS-LIT-031 — Artic: Natural-Language Workflows Are Not Software Yet

**StudyVersionRecord:** [original author source](https://arxiv.org/abs/2608.21341). **Qualification:** 本轮复核原始arXiv摘要及公开元数据，未重新核对全部实验表格；编译器、约束与执行控制组合改变，不允许自动晋升CL2。

| Claim ID | Source anchor / contrast | Program and Framework | Primary estimand | First coder ceiling & decision | I/T |
|---|---|---|---|---|---|
| 031-C1 | 摘要：11类工作流488实例，编译流程解决率高28百分点 | SCF; BGT; MI/TD/MEAS/BT | `COMPOSITE_ARTIFACT_COMPILATION_SUCCESS` | CL1组合收益 | I1/T1 |
| 031-C2 | 摘要：跨执行器一致性高32百分点，重复执行一致性高56百分点 | SCF; CSCI/BGT; MI/MEAS/BT | `CROSS_EXECUTOR_COMPILED_WORKFLOW_CONSISTENCY` | CL1性能迁移，不是T3因果可迁移性 | I1/T2-performance |
| 031-C3 | 方法：局部义务检查和情景dry-runs尝试确保原文流程忠实 | ROUTING_ABSTAIN; BGT; MI/EG/ID/MEAS | `COMPILED_WORKFLOW_SEMANTIC_COMPLETENESS` | CL0尚待验证的普遍完整性，未覆盖隐性要求 | I0/T0 |

**ClaimRecord controls:** source-versus-claim, model/resource regime, original author outcome versus audited causal interpretation, measurement independence and untested mediators retained; second coder required.

## SIS-LIT-045 — Prompt Optimization Is a Coin Flip

**StudyVersionRecord:** [original author source](https://arxiv.org/abs/2604.14585). **Qualification:** arXiv:2604.14585，2026-04-16；网格评价与优化重复单位不可混用；统计不显著不能证明相互作用为零。

| Claim ID | Source anchor / contrast | Program and Framework | Primary estimand | First coder ceiling & decision | I/T |
|---|---|---|---|---|---|
| 045-C1 | §4 6种方法×4任务×3重复=72 Haiku运行，49%低于zero-shot | ASR; BGT; DR/MEAS/BT | `PROMPT_OPTIMIZER_FAILURE_VS_BASELINE` | CL1负结果与特定任务边界 | I1/T1 |
| 045-C2 | §3 ANOVA 六个模型-任务条件均p>0.52、F<1；18,000次网格评价 | SCF; CSCI/BGT; IA/ID/MEAS/BT | `PROMPT_PAIR_INTERACTION_VARIANCE` | CL1条件性零结果，不等于因果独立或等效 | I2-local/T1 |
| 045-C3 | §6 ANOVA预检约80美元，headroom阈值2pt针对原测试校准 | ASR; BGT; DR/ID/MEAS/BT | `HEADROOM_PRETEST_OPTIMIZER_ADMISSION_VALUE` | CL1探索性，欠缺前瞻外部验证 | I1/T0 |

**ClaimRecord controls:** source-versus-claim, model/resource regime, original author outcome versus audited causal interpretation, measurement independence and untested mediators retained; second coder required.

## First-coder audit ledger

**Confirmation:** 023 H2/H7a planned local contrasts; 031 bundled accuracy/consistency performance; 045 mixed optimization value in selected tasks.
**Splits:** 023 directional migration vs symmetric null; 031 compiled artifact performance vs semantic conformance; 045 negative/ANOVA-null/pretest admission.
**Non-promotion:** 023 preregistered H1 and H4a NOT supported; 031 full semantic preservation unverified; 045 p>0.52 does not prove no component coupling. No verified complete mediator intervention. **Final maturity pending; T3/T4 not established.**
