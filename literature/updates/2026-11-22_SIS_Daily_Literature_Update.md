# SIS Daily Literature Update｜2026-11-22

**Authority:** [SIS v0.3.1](../../specs/System_Intelligence_Science_v0.3.1.md) · [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md) · [P0 Audit Queue](../evidence-map/SIS_P0_Audit_Queue.csv).

**Search window:** since 2026-11-21 daily run; latest regular arXiv announcement on **Friday 2026-11-20**, noting arXiv first-submission date for the selected items **Nov 18–19**, NOT Sunday publication. Discovery crossed arXiv cs.AI/LG/CL/SE, author originals, OpenReview, ACL/EMNLP, and journal sources. All 10 selected studies have new arXiv IDs not in 2026-11-21 Registry. Source identities cross-checked before coding. NeSy 2026/NeurIPS 2026 acceptance mentions in arXiv are **not** promoted to peer-reviewed class absent independently accessible official proceedings. No technical blogs admitted beyond `DISCOVERY_ONLY`.

**Run tally:** 10 unique preprint study candidates; 3 P0 prior studies / 9 first-coder claims; no permanent SIS-LIT assignment, no final CL promotion, no T3/T4 certification.

## 1. Scientific synthesis
The central pressure is **causal and construct validity of observed system behavior**. Reproducing incidents is stronger than citing them; independent task truth differs from metric validity; a world model's common prior can dominate direct evidence; memory utility and context handoff vary with backbone, quantity, provenance and environment. Hypothesis generation and external cohort association are not independent scientific discovery or clinical causal impact. These remain expressible under SCF/SDR/ASR, CSCI/BGT and thin Framework MEAS/ID/EG/MI/TD/DR/IA/BT.

## 2. New study records (first-coder ceilings only)

### SIS-CAND-20261122-01｜ROGUE-AI: Replication of Agentic Security Events: Audit and Investigation — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26553; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 离线重建真实报道的安全事件，与仅去除被指责因素的配对对照比较；108项复现尝试中约89%重现所报告伤害，带原因与不带原因的错误率分别为18–33%与最多1%。
- **Evidence / controls / limitations:** 历史报道存在选择偏差；离线复建不等于真实事故重演；构建者设定的致因对照可能遗漏共同原因。
- **SIS re-coding:** Primary `SDR`; cross-cutting `CSCI/BGT`; Framework `TD/MI/IA/EG/MEAS/ID/BT`; estimand `REPORTED_INCIDENT_REPLICATION_MATCHED_CAUSE_REMOVAL_HARM_DIFFERENCE`; Evidence Role `CONTROLLED_INCIDENT_REPLICATION / CAUSAL_BOUNDARY`; claim ceiling `CL1, local CL2 candidate`; Identification `I2-local (offline matched cause removal)`; transport `T1`.
- **Boundary variables:** 原始事故证据/复建环境、行动权限、数据副作用、是否存在攻击者、模型家族、对照因子真实性.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 真实事件独立资料×盲因果假设×原因去除/伪去除×等行动权限×跨模型重复.

### SIS-CAND-20261122-02｜ClosureBench: A Benchmark for Reasoning under Closure Assumptions — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26335; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 同一事实场景仅改变开放世界/封闭世界/局部封闭世界约定，960项实例发现总体准确率可能掩盖对缺失信息规则的严重不遵守；核心转换准确率范围18.23%–99.31%。
- **Evidence / controls / limitations:** 人工构造的逻辑世界比真实数据库简单；整体高准确不能代表转换正确；OpenReview正式页面本轮受访问验证限制，暂按预印本。
- **SIS re-coding:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `MI/EG/MEAS/ID/BT`; estimand `OPEN_CLOSED_LOCAL_CLOSURE_MISSING_INFORMATION_CONTRACT_SWITCH_ACCURACY`; Evidence Role `SEMANTIC_CONTRACT_MEASUREMENT / NEGATIVE_BOUNDARY`; claim ceiling `CL1 (benchmark); claimed NeSy 2026 acceptance not independently verified`; Identification `I2-local (paired contract variants)`; transport `T0`.
- **Boundary variables:** 源数据完备性声明、闭包作用域、未观测事实、任务语义、规则变体.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 同事实三闭包契约×只切换范围×专家Gold×上下文混淆负控制.

### SIS-CAND-20261122-03｜DeepQuest: From Knowledge Gaps to Scientific Discovery in Alzheimer's Disease — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26343; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 以领域综述问题形成假设，依据数据可行性与Elo排序决定实验，分开审计执行可靠性与知识新增性；OASIS-3产生42条可行假设，报告审计定义下95.24%的科学发现率，并用ADNI/AIBL复核部分关联。
- **Evidence / controls / limitations:** 发现率取决于自动评审准则和预冻结文献；外部关联验证不是临床因果识别；多组件共同变化、历史文献重叠及选择性假设报告需审计。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/DR/EG/MEAS/ID/BT`; estimand `KNOWLEDGE_GAP_FEASIBLE_HYPOTHESIS_TO_INDEPENDENT_SCIENTIFIC_FINDING_VALUE`; Evidence Role `DOMAIN_SCIENTIFIC_BENCHMARK / EXTERNAL_REPLICATION`; claim ceiling `CL1 (author experiments and cohort association), no CL3`; Identification `I1 (multi-module package; external cohort performance)`; transport `T2 performance/association only`.
- **Boundary variables:** 冻结文献时间、假设新颖性、外部队列构成、统计校正、专家Gold、真实临床价值.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 盲领域专家×时间封闭知识库×预注册假设×独立队列×负控制与多重校正.

### SIS-CAND-20261122-04｜Context as a Resource — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26346; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 将上下文作为可调度资源而不是自然语言角色；三套多流任务下，试验式合并门控把真实冲突合并正确率由33.3%提高到63.3%，并降低提示Token开销45.9%。
- **Evidence / controls / limitations:** 测试环境受控，合并门控与上下文虚拟化共同变化；有限重复和模型家族；正确合并不等于所有真实仓库状态无副作用。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/TD/EG/MEAS/ID/BT`; estimand `CONTEXT_VIRTUALIZATION_HANDOFF_MERGE_CORRECTNESS_COST_FRONTIER`; Evidence Role `SYSTEM_ORGANIZATION / NEGATIVE_HANDOFF_BOUNDARY`; claim ceiling `CL1, local CL2 candidate`; Identification `I2-local (configuration contrasts), mediation unresolved`; transport `T1`.
- **Boundary variables:** 会话并发、真实冲突、上下文隔离、消息传递损失、模型能力、调度延迟.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 等Token×单会话/路由树/虚拟化正交×冲突盲Gold×真实外部合并.

### SIS-CAND-20261122-05｜World Models Favor Learned Priors over Visual Evidence — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26366; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** TailWorld正交控制物理规则的训练频次与校准视频的信息量，发现世界模型可能对常见规律的先验压过演示证据；RIFT通过显式规则推断改善罕见动力学预测。
- **Evidence / controls / limitations:** 视频仿真规律和真实物理环境有明显差距；正确预测不等于行动后果受控；训练频次是先验代理而非完整机制解释。
- **SIS re-coding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/MI/MEAS/ID/BT`; estimand `PHYSICAL_RULE_PRIOR_VS_OBSERVATION_EVIDENCE_INFERRED_DYNAMIC_TRANSFER`; Evidence Role `NEGATIVE_MEASUREMENT_BOUNDARY / REPRESENTATION_BIAS`; claim ceiling `CL1; rule calibration contrast`; Identification `I2-local (training frequency and informative demonstration manipulated)`; transport `T1 simulated dynamics only`.
- **Boundary variables:** 长尾规则频率、校准交互信息量、初态转移、视觉噪声、物理规律覆盖.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 固定视频证据×训练频次反转×稀有规则×跨初态留出×真实物理小样本.

### SIS-CAND-20261122-06｜How Much Should an Agent Remember? Deployment Lessons from Self-Distilled Memory — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26361; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 部署回顾指出记忆最优剂量取决于模型：DeepSeek-V3.2全191条指南任务完成率提高9.5个百分点；gpt-oss-120b使用约29条精选指南的55.4%优于199条全量的51.2%；记录了高频错误建议、溯源丢失和静默失败。
- **Evidence / controls / limitations:** 精选子集仅报告两次运行均值；选择规则和模型能力交互可能混杂；产品部署不等于可归因因果实验。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/DR/EG/MEAS/ID/BT`; estimand `MODEL_CAPABILITY_BY_MEMORY_GUIDELINE_DOSE_AND_PROVENANCE_NET_VALUE`; Evidence Role `PRODUCT_DEPLOYMENT / CONDITIONAL_NEGATIVE_RESULT`; claim ceiling `CL1, local implementation contrasts`; Identification `I1 / I2-local (memory dose comparisons)`; transport `T1 AppWorld; deployment anecdote not causal trial`.
- **Boundary variables:** 基础模型能力、指南数量、溯源保留、噪声地板、提示成本、原始任务历史.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 模型×指南剂量随机化×来源保留/剥离×重复种子×新鲜未来任务.

### SIS-CAND-20261122-07｜Serialization Tax in Shared-Latent Exchangeable Decisions — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26029; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 证明只保留单项边际概率可能丢失共享潜在状态下批量决策所需的依赖；TaxScore将后验建模资源导向接近阈值的高风险组，MovieLens审计报告全体效用约0.006–0.012的改进。
- **Evidence / controls / limitations:** 依赖特定共享潜变量与阈值条件，基准离线而非真实部署；NeurIPS接收为作者声明，正式论文集未独立核验。
- **SIS re-coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/MI/MEAS/ID/BT`; estimand `SHARED_LATENT_POSTERIOR_VS_INDEPENDENT_MARGINAL_BATCH_POLICY_REGRET`; Evidence Role `THEORETICAL_IDENTIFICATION / DECISION_BOUNDARY`; claim ceiling `CL0 conditional theory + CL1 dataset audit`; Identification `I0 theorem; I2-local matched routing controls`; transport `T1`.
- **Boundary variables:** 组大小、相关结构、潜变量校准、阈值接近程度、资源预算、可观测反馈.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 相同边际预测×独立/共享相关采样×真实组级Gold×等预算路由.

### SIS-CAND-20261122-08｜Sage-Evolve-Preview: Adaptive Observation for Post-Training Self-Improvement — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26132; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 在锚点分数停滞时不改变优化目标而调整可观测任务/诊断粒度；八个锚点等数据预算平均分从66.4升至73.7，并在独立PostTrainBench报告额外增益。
- **Evidence / controls / limitations:** 诊断粒度、训练数据难度和额外任务同时变化；观察改造不等于已识别状态中介；需防止锚点选择泄漏。
- **SIS re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/TD/EG/MEAS/ID/BT`; estimand `PLATEAU_CONDITIONAL_OBSERVATION_ADAPTATION_FIXED_ANCHOR_GENERALIZATION_VALUE`; Evidence Role `CONDITIONAL_REGULATION / EVALUATION_SIGNAL`; claim ceiling `CL1, local CL2 candidate`; Identification `I2-local (data-budget matched observation variants)`; transport `T2 performance only`.
- **Boundary variables:** 锚点冻结、训练数据预算、平台期定义、探索选择偏差、跨模型执行器.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 固定训练与探索预算×盲平台期×等难度课程×冻结未见任务.

### SIS-CAND-20261122-09｜Cost-Aware Agentic Feature Optimization System for Fleet-Scale Ranking Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26531; arXiv v1 first submitted **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 多模型共享特征池下，优化器受特征管线成本和吞吐预算约束，离线平均归一化熵改善0.31%，修剪管线成本2.3%；上线A/B报告主要指标提升0.20%。
- **Evidence / controls / limitations:** 线上A/B识别整体系统改动而不是LLM提议的独立价值；提升幅度小，需要置信区间、功效、负向指标和多重实验控制。
- **SIS re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/IA/EG/MEAS/ID/BT`; estimand `RESOURCE_CONSTRAINED_FEATURE_SELECTION_FLEET_ONLINE_NET_VALUE`; Evidence Role `REAL_DEPLOYMENT / BUDGET_CONSTRAINT / PACKAGE_EFFECT`; claim ceiling `CL1, package-level local CL2 candidate`; Identification `I1 offline; I2-local for online A/B package`; transport `T2 within production fleet, not mechanism transfer`.
- **Boundary variables:** 模型群共享成本、吞吐、流量分配、实验时长、特征漂移、推理/标注预算.
- **Impact:** SHARPENS. **Reading priority:** Must Read. **Kill test:** 冻结候选×相同搜索预算×无LLM/规则/随机选择×线上随机对照×整体经济净值.

### SIS-CAND-20261122-10｜SCAFFOLD: Toward Warrant-Preserving Evidence Transport for Reusable LLM-Agent Skills — Watchlist
- **StudyVersionRecord:** https://arxiv.org/abs/2611.23990; arXiv v1 first submitted **2026-11-18**; source `PREPRINT_DELAYED_DISCOVERY`; provisional study, no permanent SIS-LIT ID.
- **Core idea / claimed novelty:** 提出可撤销的Warranted Reuse Claim，将技能复用授权绑定版本、目标上下文、证据和失效条件；区分证据可准入与结论真实、三值适用性与不对称上下文迁移。
- **Evidence / controls / limitations:** 作者明确没有实现验证器、没有实证更优结果或普遍安全保证；只能作为可检验规范假设。
- **SIS re-coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/EG/ID/BT`; estimand `EVIDENCE_WARRANT_ADMISSIBILITY_CONTEXT_SHIFT_SKILL_REUSE_POLICY_VALUE`; Evidence Role `CONCEPTUAL_PROTOCOL / TRANSPORT_WATCHLIST`; claim ceiling `CL0 proposal only, no empirical superiority`; Identification `I0`; transport `T0`.
- **Boundary variables:** 技能版本、依赖、权限、证据来源、适用上下文、验证Oracle、审查成本.
- **Impact:** FILLS EXISTING FRAMEWORK. **Reading priority:** Watchlist. **Kill test:** 匹配覆盖/效用/审查成本×长期环境漂移×版本基线×反事实复用失败.

## 3. Peer review and community analyses
No independently newly verified peer-reviewed paper qualified after deduplication this run. ClosureBench reports NeSy 2026 acceptance, while the OpenReview conference URL returned a browser verification challenge; classified as `PREPRINT` pending archival check. Journal and EMNLP records checked for delayed-indexing lineage, no duplicated versions. Community summaries discovery-only; do not increase claim maturity.

## 4. P0 Claim-Level Re-Audit
See [P0 2026-11-22 audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-22.md). SIS-LIT-113 (HIPO), SIS-LIT-119 (Jev-Mem), SIS-LIT-120 (early-outcome calibration transfer) split into 9 bounded Claims. 113 peer-reviewed source verified, 119 primary HTML and Tables 1/2 audited, 120 abstract-level with PDF table review pending. Formal promotions 0; all second-coder/adjudication pending.

## 5. P0 experiment and benchmark implications
| Priority | Experiment / fixture | Kill condition |
|---|---|---|
| P0 | Incident matched-cause-removal × true executed side effects | Removing hypothesized cause fails to reduce harm after matched task controls |
| P0 | OWA/CWA/LCWA contract × same facts × independent Gold | Aggregate accuracy masks contract-switch errors |
| P0 | Memory dosage × model ability × provenance preservation | Extra guidelines reduce future-task value or provenance vanishes |
| P0 | Group-dependency posterior × marginal matching × action threshold | Marginal calibration masks batch-level policy regret |
| P0 | Scientific discovery × prior-knowledge cutoff × independent cohort | Automated evaluator finds novelty but expert/corrected external claim fails |
| P0 | Context isolation × real conflict merge × equal budgets | Better independent branch success but unsafe shared-state merge |
| P0 | Observation budget/diagnostics × plateau × held-out transfer | Apparent recursive self-improvement vanishes after equal-data controls |
| P1 | Rare-rule world model × visual calibration × initial-state shift | Strong learned prior overrides informative observations |
| P1 | Fleet optimization × online randomized A/B × full cost | Offline proxy gain fails to yield net production value |

## 6. Formal SIS Impact Decision
`MEASUREMENT_IDENTIFICATION_DELTA` (secondary `BENCHMARK_DELTA`); `CorePressure=WATCH`; `ScientificCoreDelta=0`; `SPEC_REVISION_CANDIDATE=NO`.

True pressure on scientifically identifying incident causes, evidence transport, uncertainty dependence and hypothesis novelty; **no uncovered estimand or first-principles capability requiring Scientific Core reopening**. Existing programs/frameworks absorb the new results. Do not reinterpret technology labels as primitives.
