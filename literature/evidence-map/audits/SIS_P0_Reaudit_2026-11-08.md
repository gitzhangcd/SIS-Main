# SIS P0 First-Coder Claim Re-Audit｜2026-11-08

Authority: SIS v0.3.1 / SIS Evidence Map P0 / ClaimRecord v0.1. 本文对历史 paper-level 候选拆分为独立 Claim，不继承任何原来的 CL2/CL3 整篇标签。9项均为第一编码者初审；**Second coder / adjudication / formal promotion: PENDING**。075/082 已核对原始摘要和来源标识，但原论文全表格、附录未独立复查；114 核查原始 arXiv HTML 方法、结果和 Tables 2–3。所有 I*/T* 是 Registry 内部编码而非 SIS normative maturity。

## SIS-LIT-075｜Knowledge-Based Zero-Replay Debugging of Multi-Agent LLM Traces

StudyVersionRecord: https://arxiv.org/abs/2606.14805 ; earliest 2026-06-11, source PREPRINT; source qualification PRIMARY_ABSTRACT_VERIFIED_2026-11-08_FULLTEXT_PENDING. 作者描述利用重放 Oracle 产生干预标签，再训练不运行新重放的预测器；在37个保留轨迹家族中，Branch Recall@5 为 0.73→0.93。**预测 Oracle 的标签不是实际对失败分支进行 do(step) 续跑所识别的因果修复。**

| Claim ID | 科学问题、来源与结果 | SIS Program / Framework / estimand | Evidence Role / I/T | 第一编码者决定 |
|---|---|---|---|---|
| 075-C1 | 在保留的轨迹家族中排序可能有影响的分支；Branch Recall@5 提升，但指标是对既有重放标签的匹配 | ASR/BGT; DR/ID/MEAS/TD/BT; `ZERO_REPLAY_ORACLE_EFFECT_RANK_PREDICTION` | Prediction instrument; I1/T1 | **CL1 CONFIRM**。不能直接作为 CL2 因果故障定位 |
| 075-C2 | Deterministic replay Oracle 生成标签；被训练的零重放预测器运行时没有重新执行对应的反事实 | SDR/BGT; TD/ID/EG/BT; `ORACLE_SURROGATE_VS_TRUE_REPLAY_VALIDITY` | Identification limit; I0–I1/T0 | 条件性 Oracle 定义 **CL0** + 经验对齐 **CL1**；不得解释成中介机制 |
| 075-C3 | 预测阶段减少重放调用，但总体训练 Oracle 建造/维护成本以及修复后任务净收益未独立定量 | ASR/BGT; DR/MEAS/BT; `REPLAY_BUDGET_TRIAGE_NET_VALUE` | Cost boundary; I1/T0 | **CL1** 条件性成本，未确认操作收益或迁移 |

**Boundary:** replay Oracle 正确性、轨迹家族分布、预测置信度、修复预算与下游状态不可逆性。**Kill Test:** 冻结原始轨迹，预测分支 vs 真实 replay oracle vs 随机/图中心性基线，同等预算下真正执行候选修复并测量成功、净计算成本与轨迹状态一致性。全文表格待复核；Second coder PENDING。

## SIS-LIT-082｜BATON: Dual-Axis Policy Optimization for LLM Agents

StudyVersionRecord: https://arxiv.org/abs/2609.19830 ; original 2026-09-17, PREPRINT, source qualification PRIMARY_ABSTRACT_VERIFIED_2026-11-08_FULLTEXT_PENDING. 作者将 Bayesian Feedback Attribution（BFA，轨迹内贡献分配）与 Trajectory Mass Normalization（TMN，轨迹间权重控制）组合，在 ALFWorld、WebShop、SearchQA 报告优于 GRPO/GiGPO；**组合性能不等于单个算子的因果中介证据**。

| Claim ID | 科学问题与原始证据 | SIS Program / Framework / estimand | Evidence Role / I/T | 第一编码者决定 |
|---|---|---|---|---|
| 082-C1 | BFA 根据反馈对轨迹内步骤分配信号；全文原始消融表及等预算设置未独立复核 | ASR/BGT; DR/ID/TD/MEAS/BT; `INTRA_TRAJECTORY_FEEDBACK_ATTRIBUTION_INDEPENDENT_GAIN` | Operator candidate; I1 / I2-local candidate, T1 | **CL1** 初步，局部 **CL2 candidate** 待全文+随机对照，不能晋升 |
| 082-C2 | TMN 规范不同轨迹整体训练权重；长度分布、样本质量和更新预算可能共同变化 | ASR/BGT; DR/MEAS/ID/BT; `INTER_TRAJECTORY_MASS_NORMALIZATION_POLICY_EFFECT` | Regulation/measurement candidate; I1 / I2-local candidate, T1 | **CL1**，局部 **CL2 candidate** 待验证 |
| 082-C3 | BFA+TMN 的整体策略改进相对比较算法，但缺明确定义独立交互的2×2因子实验 | ASR/CSCI/BGT; DR/MI/MEAS/BT; `BFA_BY_TMN_INTERACTION_NET_VALUE` | Composite implementation/performance; I1/T1 | **CL1** 整体效果；没有已证实的 CL3 机制或 T3 迁移 |

**Boundary:** 奖励稀疏程度、轨迹长度、样本质量、模型能力、计算 token 和 rollout 种子。**Kill Test:** 2×2 BFA×TMN、相同轨迹样本/资源/奖励、独立冻结测试、报告交互项及置信区间。全文表格待复核；Second coder PENDING。

## SIS-LIT-114｜STEVE: Stabilizing Textual Gradient-Based Prompt Optimization

StudyVersionRecord: https://arxiv.org/html/2609.23716v1 ; original 2026-09-20. 原始 arXiv HTML 的 Methods 2.3–2.4、Results 3.3–3.4、Tables 2–3 已重查。作者声称 2026 Findings AACL-IJCNLP 录用，但正式存档未独立核实，source class **PREPRINT**, qualification PRIMARY_HTML_REAUDITED_2026-11-08_ARCHIVAL_UNCONFIRMED。

| Claim ID | 来源锚点与实验结果 | SIS Program / Framework / estimand | Evidence Role / I/T | 第一编码者决定 |
|---|---|---|---|---|
| 114-C1 | Table 3 GSM8K：Correct-only 76.5，Full dataset 82.5，完整 STEVE 86.2；「只在错误样本计算梯度」与最终验证门共同影响表现 | ASR/BGT; DR/MI/MEAS/ID/BT; `ERROR_ONLY_GRADIENT_SELECTION_VALUE` | Local ablation and conditional gain; I1/I2-local candidate, T1 | **CL1** 局部实验支持；没有独立验证特定语义梯度中介 |
| 114-C2 | Table 3：无 regularized verification GSM8K/StrategyQA/ObjectCounting 为84.1/91.5/92.2，完整方案为86.2/93.2/95.7 | ASR/BGT; DR/EG/MEAS/ID/BT; `HOLDOUT_REGRESSION_GATE_ADMISSION_EFFECT` | Intervention/regression gate candidate; I2-local/T1 | **CL1**，仅局部 **CL2 candidate**；不能视作通用安全保证 |
| 114-C3 | Table 2：TextGrad→STEVE，Object Counting 44→52，Geometric Shapes 34→44，GSM8K-Platinum 98.2→98.3，DS-1000 32.0→32.5；优化器额外调用增加 | SCF/ASR+BGT; MI/DR/MEAS/BT; `TEXTUAL_OPTIMIZATION_GENERALIZATION_NET_COMPUTE` | Performance + compute boundary; I1/T1 | **CL1**，非 T3 因果迁移、非已识别全系统净价值 |

**Boundary:** 初始 Prompt 正确率、数据集、样本错误类型、验证集重用和优化 token 预算。**Kill Test:** error-only×regression-gate 全 2×2 因子，对齐候选/评价器调用与 token 预算；分离独立冻结 Gold，报告新收益与旧正确样本回归；预注册拒绝阈值。Second coder PENDING。

## P0 Governance Decision & Handoff

- Today: 3 preexisting Study IDs, 9 claim-level split records, 0 formal promotions, 0 confirmed T3/T4.
- 075/082: **claim source not fully qualified**; maintain provisional first-coder status, do not inherit original candidate CL2; do not assert source appendix verified.
- 114: conditional ablation confirmed against original HTML tables, but **source archival version remains unconfirmed**; local effects do not establish complete mechanism mediation.
- First coder: AUTOMATED_FIRST_CODER_2026-11-08; second coder PENDING; adjudication PENDING. Next audit must independently inspect 075/082 experimental tables, 114 compute-matched full factorial and blinded held-out Gold.
