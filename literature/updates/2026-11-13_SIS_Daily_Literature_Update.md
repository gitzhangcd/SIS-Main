# SIS Daily Literature Update｜2026-11-13

**Source of truth:** SIS v0.3.1 Master, Registry v1.3, P0 Audit Queue, existing audit files through 2026-11-12. **First-coder literature intelligence, not final causal adjudication.**

## Discovery and lineage

- Search date 2026-11-13 at ~00:03 UTC. At that moment the latest published cs.AI arXiv list showed **Wednesday 11 November 2026, 381 records / 105 new submissions**; no confirmed later arXiv regular cs.AI listing. Avoid confusing discovery/indexing with first submitted date.
- **10 newly discovered distinct preprints** first submitted 2026-11-09 or 10. All arXiv IDs checked against existing Registry, not numbered as permanent SIS-LIT. No duplicate preprint→conference Study created. NeurIPS/IEEE acceptance claimed on two papers but formal proceedings identity not independently established; remain PREPRINT.
- Cross-source scanning includes official arXiv listing and abstracts, ACL Anthology recent AACL/EMNLP proceedings, conference/OpenReview targeted discovery, author/project pointers, and discovery-only technical commentary. No independent community replication qualifies for Claim promotion.
- No padding: 10 candidates meet scientific relevance, but primary abstract checks precede any full-text CL decision.

## Peer-reviewed new items

No newly matched *independently archived and unduplicated* peer-reviewed paper at this cut-off that displaced the ten selected items. Author-reported acceptance alone is not a formal archived paper version.

## Preprints — qualified candidates (10)

### 1. Agreeing on the Answer but Not the Reason: Measurement Limits of LLM Reasoning Failure Taxonomies — **Must Read**

- Original: https://arxiv.org/abs/2611.13140 (v1 2026-11-09; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 12模型、11语言、2316条记录，失败类别重叠50.1%；类别检查次序改变后占比26.4%–76.4%；答案正确性与失败原因标签的Kappa差距巨大。
- Evidence strength / confounders: 标签次序、标注器Prompt、翻译缺漏、人工分歧改变推断；不能用此估计真实系统故障发生率。
- SIS re-coding: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**, Framework **MEAS/EG/ID/BT**; estimand `FAILURE_TAXONOMY_LABEL_ORDER_PROMPT_GOLD_AGREEMENT_SENSITIVITY`; CL1 measurement; no causal failure mechanism promotion; identification **I1 (label-order manipulation I2-local only)**; transport **T0**; evidence role **MEASUREMENT_NEGATIVE / construct validity**. Nature **NEGATIVE / MEASUREMENT**.
- Boundary: 语言、类别共现、tie-break次序、标注提示、Gold翻译.
- SIS effect: **SHARPENS MEAS/ID；失败分类比例是测量操作条件性的，不是天然的系统故障性质**.

### 2. Dependable Long-Horizon LLM Agents: A Trajectory-Centered Empirical Study of Where Errors Enter and Which Controls Reach Them — **Must Read**

- Original: https://arxiv.org/abs/2611.13254 (v1 2026-11-09; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 对95条完整失败轨迹建立起点—传播—检测—响应—结局记录；72%失败轨迹中已有反证但88%未行动；部分故障由provider过滤器崩溃及Harness替代输出引发。
- Evidence strength / confounders: 样本为失败案例且人为标签依赖判断，不能从轨迹可观测反证推导执行修复效果或普遍发生率。
- SIS re-coding: Primary **SDR**, cross-cutting **BGT**, Framework **TD/EG/MEAS/ID/BT**; estimand `FAULT_ORIGIN_PROPAGATION_OBSERVED_CONTRADICTION_CONTROL_REACH`; CL1 observational trajectory audit; CL0 proposed control efficacy; identification **I1**; transport **T0**; evidence role **TRAJECTORY / negative descriptive finding**. Nature **NEGATIVE / BOUNDARY**.
- Boundary: 轨迹完整性、外部过滤器、task contract、反证可达性、行动权限.
- SIS effect: **SHARPENS SDR；区分可见反证、实际行动、可执行修复与第三方基础设施故障**.

### 3. ExpertCrowd-SWE: Measuring Frontier Coding Agents on Expert-Authored Engineering Tasks in Unfamiliar Codebases — **Worth Skimming**

- Original: https://arxiv.org/abs/2611.13246 (v1 2026-11-09; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 100个专家工程任务，87个项目、11种语言，提供sealed reference、must-pass blockers与对抗控制补丁；七个模型、五次重复共3495次评分。
- Evidence strength / confounders: 任务按前沿模型难度筛选可能选择偏差；评分器校准不代表独立语义真值；平台统一但工具接口原生并不完全相同。
- SIS re-coding: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**, Framework **MEAS/EG/ID/BT**; estimand `EXPERT_AUTHORED_PARTIAL_CREDIT_GRADER_AND_STOCHASTIC_RELIABILITY`; CL1 benchmark instrument; identification **I1; control-patch challenge I2-local (grader only)**; transport **T1 performance only**; evidence role **BENCHMARK / MEASUREMENT_INSTRUMENT**. Nature **MEASUREMENT**.
- Boundary: Repo版本、执行接口、参考补丁覆盖、grader语义、任务选择.
- SIS effect: **SHARPENS BGT：连续评分、grader负控制和重复性纳入能力前沿测量**.

### 4. Multimodal Abstention That Preserves Acquired Correct Answers — **Must Read**

- Original: https://arxiv.org/abs/2611.14311 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 同一SFT检查点上比较弃权策略，独立228问簇确认66.05%正确弃权、保留已答对题；默认阈值反而丢失298个正确答案。
- Evidence strength / confounders: 单一模型/任务集，校准上的零回归不是总体零回归；静态阈值表现与真实长期拒答效用不同。
- SIS re-coding: Primary **ASR**, cross-cutting **BGT**, Framework **DR/MEAS/ID/EG/BT**; estimand `SELECTIVE_ABSTENTION_CORRECT_REPAIR_VS_ACQUIRED_ANSWER_REGRESSION_BUDGET`; CL1, local CL2 candidate for fixed-model threshold contrast; identification **I2-local provisional**; transport **T1**; evidence role **NEGATIVE_BOUNDARY / regulation value**. Nature **NEGATIVE / POLICY**.
- Boundary: 阈值、校准独立性、无答案问题比例、模型、数据漂移.
- SIS effect: **SHARPENS ASR；弃权要联合计算修复错误、损失原有正确答案与保留学习收益**.

### 5. Don't Just Trust Your Memory: Evidence-Linked Memory Reduces Memory-Induced Degradation in LLM Agents — **Must Read**

- Original: https://arxiv.org/abs/2611.14320 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: WikiTrace将经验摘要与原始轨迹证据链接，读取时可以回溯核对经验，在五个基准上降低错误经验导致的任务退化。
- Evidence strength / confounders: 额外轨迹读取、上下文预算与工具调用成本可能同时变化；对模型是否真正使用原始证据缺少随机暴露因果确认；ACL ARR仍在审稿。
- SIS re-coding: Primary **SCF**, cross-cutting **BGT**, Framework **MI/TD/EG/ID/MEAS/BT**; estimand `TRAJECTORY_LINKED_MEMORY_EVIDENCE_ACCESS_VS_MEMORY_INDUCED_DEGRADATION`; CL1, local CL2 candidate for same-insights comparison; identification **I1/I2-local**; transport **T1**; evidence role **MECHANISM_CANDIDATE / negative boundary**. Nature **MECHANISM_CANDIDATE / NEGATIVE**.
- Boundary: 经验来源成功/失败、上下文预算、证据锚定精度、读取门槛.
- SIS effect: **SHARPENS SCF/EG：记忆结论应能回溯证据并有任务条件适用范围**.

### 6. When Should Agents Remember? Falsification-Gated Self-Evolution for LLM Agents — **Must Read**

- Original: https://arxiv.org/abs/2611.14326 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 把经验更新表述为前提-行动-预期效应-验证器的假设，并在暂存状态进行反证/迁移/回归测试；作者报告回归伤害1.3%、有害提交3.6%。
- Evidence strength / confounders: 验证器与任务覆盖可能错设；性能收益混合候选生成、反证测试与门控；不可直接推断真实部署安全率。
- SIS re-coding: Primary **ASR**, cross-cutting **BGT**, Framework **DR/EG/ID/MEAS/BT**; estimand `FALSIFICATION_REGRESSION_GATED_PERSISTENT_UPDATE_ADMISSION_NET_VALUE`; CL1 package; local CL2 candidate, no proven mediation; identification **I1/I2-local provisional**; transport **T1**; evidence role **REGULATION / GOVERNANCE**. Nature **REGULATION / BOUNDARY**.
- Boundary: 候选经验选择、反证样本、回归任务库、不可逆外部副作用、测试预算.
- SIS effect: **SHARPENS ASR；update admission是关于保存哪种经验的条件性调节决策，不是Memory新原语**.

### 7. Evaluating LLM-Generated World Models for Neuro-Symbolic Reasoning — **Must Read**

- Original: https://arxiv.org/abs/2611.14419 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 44场景410次生成；135个参考游戏中134个机械有效，却只有28个准确匹配参考结构，结构F1仅0.366。
- Evidence strength / confounders: 参考模型可能并非唯一合法形式化；机械有效、结构一致与任务语义仍需独立专家核验。
- SIS re-coding: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**, Framework **MI/MEAS/EG/ID/BT**; estimand `WORLD_MODEL_EXECUTABILITY_VS_SEMANTIC_STRUCTURAL_FIDELITY`; CL1 measurement; no model-induced planning causal effect; identification **I1; deterministic validity audit**; transport **T0**; evidence role **MEASUREMENT_NEGATIVE / specification fidelity**. Nature **NEGATIVE / MEASUREMENT**.
- Boundary: 参考模型歧义、文化上下文、结构等价变换、观测假设.
- SIS effect: **SHARPENS MEAS/MI：可执行的形式世界模型不等于任务真实语义**.

### 8. Re-Search: Dissecting LLM Ideation Through a Two-Player Questioning Game — **Must Read**

- Original: https://arxiv.org/abs/2611.14487 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 用200篇ICML 2026研究构造20问式科研问题，在6个模型中大部分进展发生于前30/100次问题；控制实验显示好想法识别与产生存在瓶颈差异。
- Evidence strength / confounders: 重复发现已发表思路不等于原创科研；yes/no Oracle信息泄露、提示方式和搜索先验影响结果。
- SIS re-coding: Primary **SCF**, cross-cutting **BGT**, Framework **MI/TD/MEAS/ID/BT**; estimand `RESEARCH_IDEA_GENERATION_VS_RECOGNITION_CONDITIONAL_QUESTION_BUDGET`; CL1, local CL2 candidate for candidate-question interventions; identification **I1/I2-local**; transport **T0**; evidence role **CAPABILITY_MEASUREMENT / negative boundary**. Nature **NEGATIVE / CAPABILITY**.
- Boundary: 候选库覆盖、Oracle信息、问题预算、已发表思路先验.
- SIS effect: **SHARPENS SCF：产生候选能力与评价候选能力是独立可检验组件性质**.

### 9. ReTrace: Distilling Tool-Using Agents into Planner-Free Workflows — **Must Read**

- Original: https://arxiv.org/abs/2611.14492 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 从工具轨迹解释提取条件规则编译工作流；79个生产SOP完成率93.8% vs Agent96.8%，成本下降24%；τ² Bench执行时间1.3秒 vs 170秒但成功率降低。
- Evidence strength / confounders: 系统实现环境与工具运行时不同；成功率损失不能用速度单独抵消；修复环节使用训练失败需独立留出复核。
- SIS re-coding: Primary **SCF**, cross-cutting **CSCI/BGT**, Framework **MI/TD/IA/MEAS/ID/BT**; estimand `TRACE_TO_RULE_WORKFLOW_COMPILATION_COST_SUCCESS_FRONTIER`; CL1 package, local CL2 candidate for matched procedural comparison; identification **I2-local provisional**; transport **T1**; evidence role **IMPLEMENTATION / cost-boundary**. Nature **IMPLEMENTATION / BOUNDARY**.
- Boundary: SOP重复度、规则覆盖、任务分布漂移、修复训练数据、回滚.
- SIS effect: **SHARPENS SCF/CSCI：执行轨迹可外化为规则，能力—成本—风险前沿须联合测量**.

### 10. Contrastive Discovery: Open-Ended Scientific Discovery over Competing Explanations — **Must Read**

- Original: https://arxiv.org/abs/2611.14514 (v1 2026-11-10; discovered 2026-11-13; **preprint**).
- Claimed novelty/observations: 与点假设/非假设相对，构建互斥完备解释候选集合；同一证据可将73%的被拒绝点假设归到替代解释，等预算搜索解决更多问题67%；38位盲审专家78%一致。
- Evidence strength / confounders: 候选解释集合是否真正互斥完备取决于人工规范；共识非唯一科学真值，跨6领域不能自动晋升T3；NeurIPS接收为作者声明未独立匹配正式归档。
- SIS re-coding: Primary **ASR**, cross-cutting **BGT**, Framework **MI/DR/EG/ID/MEAS/BT**; estimand `CONTRASTIVE_HYPOTHESIS_SET_EVIDENCE_REUSE_AND_SEARCH_POLICY_VALUE`; CL1, local CL2 candidate for same-evidence rescoring; no CL3 mechanism; identification **I2-local provisional**; transport **T1 performance only**; evidence role **MECHANISM_CANDIDATE / scientific measurement**. Nature **MECHANISM_CANDIDATE / IDENTIFICATION**.
- Boundary: 备择集合完整性、同一证据复用、先验分布、实验预算、专家一致性.
- SIS effect: **SHARPENS ASR/EG：证据不只用于否证，还应支持备择解释间的辨别及下一实验的信息价值**.


## Technical / community analyses

None promoted beyond DISCOVERY_ONLY. Source-independent replication lacking; commentary cannot raise CL levels.

## P0 re-audit (Claim-level)

literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-13.md: SIS-LIT-104, 106, 091; nine atomic claims. Selected methods/results audited in arXiv HTML; second coder/adjudication pending. **104 legacy CL2_PROMOTED and 106 legacy CL2_CONFIRMED labels withdrawn from final-claim fields pending independent claim-specific adjudication.** No new CL2/CL3 promotion and no confirmed T3/T4.

## Five highest-impact scientific implications

1. **Failure taxonomy is an instrument-dependent construct.** Label co-occurrence, tie-break order, annotation prompt and translated Gold can change purported failure proportions; published prevalence is not necessarily a property of the system.
2. **Preserving learned correct answers is part of adaptive regulation net value.** Abstention, evidence-gating and memory updates must measure corrected failures *and* newly lost correct outcomes; validation-only zero regression is not a general safety guarantee.
3. **Evidence provenance is not evidence use.** Long-horizon audits and linked-memory work support tracing trajectory-derived lessons back to receipts, while requiring explicit intervention tests to establish the decision impact of provenance.
4. **Mechanical correctness does not establish semantic fidelity.** Generated world models passed mechanical checks almost universally yet differed structurally from reference models; references also require independent semantic qualification.
5. **Scientific optimization needs contrastive alternatives and matched budgets.** Candidate generation, candidate judgment, evidence discrimination and search policy are separable estimands. Workflow distillation reveals real cost–success frontiers rather than unconditional organizational superiority.

## Benchmark / measurement proposals

| Priority | New fixture | Identification and negative-control requirement |
|---|---|---|
| P0 | Failure Taxonomy × Label Order × Independent Humans | Category co-occurrence, tie-break permutation, shared Gold, prompt/translation audit |
| P0 | Memory Evidence Link × Randomized Exposure × Equal Token Budget | Memory retrieval vs actual use vs correct action; harmful update rate |
| P0 | Admission Gate × Falsification × Regression Archive | Temporary change→holdout probes→admit/reject; independent verifier and cost |
| P0 | Abstain Threshold × Retained Capabilities × OOD | Gains, losses, correct abstentions, pretraining/SFT retention with frozen thresholds |
| P0 | Executable World Model × Semantic Gold × Structural Equivalence | Mechanical validity, reference equivalence, human-verified task intent |
| P0 | Scientific Hypothesis Set × Evidence Reuse × Fixed Budget | Pointwise vs contrast set; generation vs discrimination; independent scientific Gold |
| P1 | SOP Rule Compilation × Agent Replanning × Drift | Completion-rate, time, cost, exceptions, platform transfer |
| P1 | Inherited CL2 queue × Original HTML × Second Coder | Claim-specific evidence vs paper-level badges; prespecified contrast and mediation |

## Formal SIS Impact Decision

**MEASUREMENT_IDENTIFICATION_DELTA**, secondary **BENCHMARK_DELTA**. **ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO.** Real identification/measurement pressure rather than merely new implementation: instrument-dependent failure taxonomy, persistence regression risk, semantic fidelity, and dynamic evidence-use policies. All are expressible within SIS v0.3.1 SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG. **CorePressure=WATCH** (watchlist rather than reopening). Formal core remains frozen; new fixture definitions remain open.
