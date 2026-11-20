# SIS v0.3.1 Daily Literature Update｜2026-11-20

**Authority:** `specs/System_Intelligence_Science_v0.3.1.md` (ScientificCoreDelta=0 frozen), Literature Registry, `literature/evidence-map/SIS_P0_Audit_Queue.csv` and P0 audit history.
**Baseline:** 2026-11-19 previous daily note and GitHub main; do not interpret discovery date as first publication.
**Discovery:** https://arxiv.org/list/cs.AI/new (Thursday 2026-11-19 batch, 362 total and 82 cs.AI new) plus https://arxiv.org/list/cs.AI/recent, primary arXiv abstracts/HTML, ACL Anthology November 2026 (AACL-IJCNLP), OpenReview/NeurIPS/ICLR/ICML/ACL/EMNLP sweeps and technical discovery-only analyses.
**Inclusion:** 10 unique qualifying StudyVersionRecords, 1 official peer-reviewed AACL paper (November 2026 delayed indexing), 9 arXiv preprints (eight first posted Nov 18 and one Nov 17 delayed cross-discovery); no raw publish-date inflation. First-coder discovery only; official paper does not inherit higher CL. No new independently reproduced community evidence.
**Dedup:** exact arXiv identifiers / ACL anthology ID and title-identity checked against Registry, distinct from prior 'Agent Architecture Cost-Success Trade-offs' and previously recorded memory/handoff studies. Historical broader candidate lineage backlog remains open.
**P0:** three existing studies (005/046/063) split into nine claim units with provenance and falsification tests; no formal promotion, no second coder, no T3/T4.
**Formal impact:** MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; CorePressure WATCH; ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO. Existing SCF/SDR/ASR+CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG express all observed scientific questions.

## 1. Peer-reviewed (newly indexed)
### SIS-CAND-20261120-01｜AgentArch: A Benchmark for Evaluating Agent Architectures in Enterprise Workflows — Must Read
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.44/ ; initial/archive date **2026-11 (AACL-IJCNLP 2026)**; source PEER_REVIEWED; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 18种架构配置，交叉比较组织方式、ReAct/函数调用、记忆与思考工具；最佳模型复杂任务成功率35.3%，简单任务70.8%。
- **Evidence quality & limitations:** 正式会议论文；结构化多维比较有价值，但样本仅覆盖有限企业任务，各维度实现和模型选择未完成充分随机正交，不能认定普适架构因果效应。
- **Scientific recoding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/MEAS/ID/BT`; primary estimand `ENTERPRISE_MODEL_BY_ORCHESTRATION_MEMORY_STYLE_THINKING_TOOL_INTERACTION`; Evidence Role `COMPONENT_INTERACTION / BENCHMARK`; claim maturity ceiling `CL1 (paper-level outcomes, no formal CL2)`; identification/transport `I1 / T1`.
- **Boundary variables:** 模型能力、任务难度、工具实现、架构交互、token/latency预算.
- **Impact:** SHARPENS：能力取决于组件×组织×任务的交互，已有CSCI可表达。
- **Priority:** **Must Read**. **Kill test:** 固定任务与执行器，四因子平衡实验×等计算预算×独立交付物Gold；对比交互与NoOp。

## 2. Preprints (first posted Nov 17–18; surfaced by Nov 19)
### SIS-CAND-20261120-02｜Training Language Models for Introspective Oversight — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.23365 ; initial/archive date **2026-11-17**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 分离第三人称观察者角色并以实际行为核查训练；五项留出监督任务平均AUROC 0.907，优于honesty training 0.864、transcript monitor 0.828、activation oracle 0.796。
- **Evidence quality & limitations:** 有五种留出评价和行为核验；但观察者与被观察模型共享权重及训练分布，干预后模型行为亦变化，存在共同盲区与自我报告有效性问题。
- **Scientific recoding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; primary estimand `INTROSPECTIVE_OBSERVER_BEHAVIOR_VERIFIED_MONITOR_AUROC_AND_OBSERVER_INDEPENDENCE`; Evidence Role `OBSERVABILITY_INSTRUMENT / NEGATIVE_BOUNDARY`; claim maturity ceiling `CL1; local training contrast candidate (no adjudicated CL2)`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** 监督标签真实性、隐藏行为分布、角色分离、共同训练、模型家族与部署事件.
- **Impact:** SHARPENS：可观测性提升不等于独立的机制识别，要求外部Gold和对抗验证。
- **Priority:** **Must Read**. **Kill test:** 同一冻结Actor×独立Observer训练×盲法真实执行日志×隐藏reward-hack/欺骗注入×跨模型迁移。

### SIS-CAND-20261120-03｜Knowing What You Know: A Trait Theory of Reviewer Value in Human-AI Cognitive Systems — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24932 ; initial/archive date **2026-11-18 (author reports ACS 2026 acceptance; proceedings not independently verified)**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 在483名审阅者、541621条生产事件中研究人类复核校准与增量价值；指出单次判断及多数投票下个体因果价值可能不可识别。
- **Evidence quality & limitations:** 生产规模大，含审阅结局；但处理分配、案件难度及存活反馈具有混杂/选择偏差。'人类校准与模型自知属于相同构念'属于有待检验理论，不应视为已确立机制。
- **Scientific recoding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `IA/MEAS/ID/EG/BT`; primary estimand `HUMAN_MODEL_ITEM_CONDITIONAL_CALIBRATION_REVIEWER_ADDED_VALUE_IDENTIFIABILITY`; Evidence Role `HUMAN_AI_INTERACTION / IDENTIFICATION_BOUNDARY`; claim maturity ceiling `CL0 theoretical claims + CL1 observational`; identification/transport `I1 / T1`.
- **Boundary variables:** 任务难度、审阅分配机制、真实Gold、反馈延迟、聚合规则、专业领域.
- **Impact:** SHARPENS/WATCH：人机调节权与价值的可识别性；仍可由CSCI/IA/ID表示。
- **Priority:** **Must Read**. **Kill test:** 随机指派复核者×冻结模型预测×盲法外部真值×校准层分层×多数投票对照。

### SIS-CAND-20261120-04｜Choosing What to Observe: Budget-Paired Counterfactual Audits for Credible Evaluation of Visual Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24867 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 固定公开证据和区域绑定，配对改变剩余观察预算，并利用精确续行价值区分获取信息失败与终端决策失败；40个配对路由锚点、五个开放模型。
- **Evidence quality & limitations:** 方法与附录中明确区分观测策略和终端回答，具较强受控参考；但精确值依赖人工构造任务及已知世界，无法自动外推真实文档与不完备Gold。
- **Scientific recoding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/TD/MEAS/ID/EG/BT`; primary estimand `FIXED_EVIDENCE_BUDGET_PAIRED_ACQUISITION_VS_TERMINAL_DECISION_LOSS`; Evidence Role `COUNTERFACTUAL_MEASUREMENT / VALUE_OF_INFORMATION`; claim maturity ceiling `CL0 exact task-model reference + CL1 model findings; local controlled comparison candidate`; identification/transport `I2-local / T0`.
- **Boundary variables:** 观察预算、区域绑定、先验、观测噪声、证据选择器、终端答复.
- **Impact:** SHARPENS：将主动观测价值从最终正确率中拆分，是现有DR+ID的精细化。
- **Priority:** **Must Read**. **Kill test:** 同一证据世界×预算随机分配×固定reader与终端策略×真实文档留出×伪观测/信息缺失。

### SIS-CAND-20261120-05｜When Figures Disagree with Text: Evaluating Autonomous Visual Evidence Verification in Scientific Papers — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24353 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 31份含评审记录矛盾的完整论文、六种视觉模型、1445次开放审稿；60.6%提及问题图但仅3.3%获评分准则接受为正确诊断，指定图编号的独立对照4.3%→20.4%。
- **Evidence quality & limitations:** 使用原始完整论文与多种提示干预，设盲审审计；自动rubric本身偏宽松，31份样本小且有选择性，不能将分数作为绝对科研审稿能力。
- **Scientific recoding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; primary estimand `FULL_MANUSCRIPT_FIGURE_SELECTION_VS_CONTRADICTION_DIAGNOSIS_VALIDITY`; Evidence Role `NEGATIVE_MEASUREMENT / SCIENTIFIC_EVIDENCE_GOLD`; claim maturity ceiling `CL1; local provided-figure contrast candidate`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** 是否指定图、渲染页可见性、rubric严格度、证据定位、学科与模型.
- **Impact:** SHARPENS：选择要验证的证据与对已给定证据判断正确是两个测量终点，直连SIS-MED证据审计。
- **Priority:** **Must Read**. **Kill test:** 全文自主定位×指定图×给定矛盾线索阶梯，专家盲裁判×未见医学论文×可重复冲突位置。

### SIS-CAND-20261120-06｜Semantic Context Handoff with On-Demand Evidence for Long-Horizon Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24357 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 将紧凑语义状态与可重访执行证据分离，按需返回过去证据；150项SWE-bench受控设置证据恢复使Pass@1由80.0%升至86.9%，完整系统对比节省43% tokens和41% walltime。
- **Evidence quality & limitations:** 对照明确且涉及真实软件工件；但任务与模型选择、回访成本、历史摘要和其他缓存策略可能混杂，局部增益不是所有长期流程的普遍机制。
- **Scientific recoding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/TD/EG/MEAS/ID/BT`; primary estimand `STATE_EVIDENCE_SEPARATION_RECALL_ON_DEMAND_HANDOFF_TASK_SUCCESS_COST`; Evidence Role `ORGANIZATION_EFFECT / EVIDENCE_PRESERVATION`; claim maturity ceiling `CL1; local recovery ablation candidate`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** 交接长度、证据索引精度、检索时机、错误历史、模型、执行成本.
- **Impact:** SHARPENS：前日跨组件证据丢失结果的可干预对照；已有SCF/CSCI/EG足够。
- **Priority:** **Must Read**. **Kill test:** 冻结同一证据×摘要/状态证据拆分/完整历史×相同tokens×证据再访随机遮蔽×独立任务Gold。

### SIS-CAND-20261120-07｜F³: What Makes Good Experience in World-Action Models? — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24708 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 将成功/失败轨迹转为已核验操作记录，学习何时匹配并将经验融合入动作策略；仅200个训练实例，跨MolmoSpaces和未训练RoboLab分别报告+12.0/+10.8pp成功率，回归减少57%。
- **Evidence quality & limitations:** 跨环境任务执行较有说服力，但Form/Fit/Fusion和经验库规模共同变化，未见训练域的测试仅是性能迁移，非机制迁移。
- **Scientific recoding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/DR/MEAS/ID/BT`; primary estimand `EXPERIENCE_FORM_FIT_FUSION_CONDITIONAL_ACTION_POLICY_GAIN_REGRESSION`; Evidence Role `CAPABILITY_FORMATION / NEGATIVE_BOUNDARY / PERFORMANCE_TRANSFER`; claim maturity ceiling `CL1; component ablation CL2 candidate only`; identification/transport `I1/I2-local / T2 performance-only`.
- **Boundary variables:** 经验质量、记录形式、使用时点、融合位置、环境分布、退化阈值.
- **Impact:** SHARPENS：经验有效必须经行动效用验证，检验能力资产的回归边界。
- **Priority:** **Must Read**. **Kill test:** 成功/失败经验×Form/Fit/Fusion三因子消融×随机经验×任务状态匹配×真实执行保留集。

### SIS-CAND-20261120-08｜Risk-Triggered Search: Behavior-Preserving Safe Control — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24409 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 冻结JEPA世界模型，通过动作条件风险前缀触发局部搜索，不触发时保留正常策略；1968条配对轨迹中安全到达率提高、控制时间减少17.71%–70.41%；给出条件下100%安全名义动作一致性。
- **Evidence quality & limitations:** 成对轨迹、明确条件性证明很有价值；但风险头和world-model错误、未模拟危险、训练分布及安全定义限定保证，不可解释为真实部署零风险。
- **Scientific recoding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/TD/MI/ID/MEAS/BT`; primary estimand `LATENT_PREFIX_RISK_TRIGGER_SEARCH_SAFETY_NOMINAL_IDENTITY_COST`; Evidence Role `CONDITIONAL_REGULATION / SAFETY_BOUNDARY`; claim maturity ceiling `CL0 conditional equivalence proof + CL1 empirical; local CL2 candidate`; identification/transport `I2-local / T1`.
- **Boundary variables:** 风险阈值、latent预测保真、动作代价、障碍/环境shift、模型预测时域.
- **Impact:** SHARPENS：自适应控制应同时测量安全干预收益和原有正确行为保留。
- **Priority:** **Must Read**. **Kill test:** 冻结同一世界×真实危险注入×阈值扫描×风险头校准×同计算预算全时/触发搜索。

### SIS-CAND-20261120-09｜WorldRuler: Interactive World Modeling under Configurable Rules — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24869 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 以可执行三维规则图管理规则依赖、对象状态和保存/恢复，结合视频生成在对象尚不可见时维持先行规则；GTA-V/Habitat构建RuleVerse。
- **Evidence quality & limitations:** 包含状态/事件标注与规则受控场景，但模拟器标注的语义正确性和生成画面忠实性仍受合成规则与感知器限制。
- **Scientific recoding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/MI/EG/MEAS/ID/BT`; primary estimand `RULE_STATE_PERSISTENCE_UNSEEN_OBJECT_BEHAVIOR_CONSISTENCY`; Evidence Role `STATE_SEMANTICS / IMPLEMENTATION / MEASUREMENT`; claim maturity ceiling `CL1 (author-reported simulation)`; identification/transport `I1 / T0`.
- **Boundary variables:** 隐藏对象、状态保存/加载、规则冲突、对象绑定、画面可视化.
- **Impact:** FILLS EXISTING FRAMEWORK：形式规则与视觉表现一致性是TD/MI的可替换测量实例。
- **Priority:** **Worth Skimming**. **Kill test:** 随机隐藏对象与规则冲突×状态保存恢复×独立符号模拟器Gold×未见规则组合。

### SIS-CAND-20261120-10｜Think Offline, Act in Real Time: Self-Improving Visual Game Agents through Code — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24590 ; initial/archive date **2026-11-18**; source PREPRINT; one provisional Study, no permanent SIS-LIT assignment.
- **Core idea / author claim:** 面对持续推进的实时视觉游戏，比较实时模型决策和试跑间修改的外部程序策略；170项GameWorld任务、最多8次一分钟试跑，代码策略平均进展47.8%，训练控制器30.9%。
- **Evidence quality & limitations:** 固定试跑上限具有可比性，但代码策略和模型策略在离线思考、动作时延、编译/调试与权限上不同，需完整计算成本和相同反馈做公平对照。
- **Scientific recoding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/MI/TD/MEAS/ID/BT`; primary estimand `OFFLINE_PROGRAM_POLICY_REWRITE_VS_ONLINE_MODEL_ACTION_REALTIME_NET_VALUE`; Evidence Role `REPRESENTATION_EXTERNALIZATION / ADAPTIVE_REGULATION`; claim maturity ceiling `CL1; local policy-mode contrast candidate`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** 实时环境时钟、试跑预算、程序执行速度、代码风险、状态可观测性.
- **Impact:** SHARPENS：表示外部化让控制具有新的时间条件，但属已有ASR与MI，不是新的原语。
- **Priority:** **Must Read**. **Kill test:** 等walltime+tokens+工具机会×程序策略/动作模型×实时速度×随机规则变化×未见任务。

## 3. Technical/community analyses
No independently reproduced mechanism evidence qualified. DISCOVERY_ONLY; no CL upgrade. No filler used.

## 4. P0 claim-level re-audit
Detailed 9-claim audit: [SIS_P0_Reaudit_2026-11-20.md](../evidence-map/audits/SIS_P0_Reaudit_2026-11-20.md). Full-text HTML independently checked for 005 and 046; 063 source primary text/result extraction verified, detailed table independence still needs second coder. Original study-level CL2/CL3 candidates do not convey a normative status.

## 5. Synthesis, boundary implications and benchmark backlog
1. **Evidence acquisition vs evidential judgment:** scientific figure selection, visual region-value audits, and state/evidence handoff show why evidence **exists**, **was selected**, **was retained**, and **changed decisions** are different endpoints; none is a new primitive.
2. **Verifier and observer independence:** observer-trained internal monitoring is useful but correlated with the system it watches; independent execution Gold and joint failure injections remain mandatory.
3. **Human–AI contribution cannot be read off activity:** reviewer calibration estimates depend on assignment, outcomes and aggregation; majority-vote individual contributions may be non-identifiable without extra intervention.
4. **Experience and rule-conditioned dynamics:** F³, WorldRuler, and code-as-policy show representations can be valuable yet contextual, and require future-action/retention tests, not artifact counts.
5. **Conditional regulation & preserved capability:** trigger-gated safety requires falsifiable nominal-action preservation and OOD risk calibrations; budget-matched counterfactuals should separate selection vs terminal-decision loss.

| Priority | Proposed fixture | Distinguishing test / kill condition |
|---|---|---|
| P0 | Fixed Evidence × Observation Budget × Terminal Reader | 观察价值随reader或可见成本变化后丧失；量化acquisition vs decision regret |
| P0 | Full Scientific Paper × Figure Selection × Independent Expert Gold | 找到目标图不等于识别矛盾；自动rubric偏宽松 |
| P0 | Worker Context × Evidence Handoff × Recoverability | 证据确实存在、已读却在handoff后不可检索 |
| P0 | Observer Role × Hidden Behavior × External Execution Gold | 自检探针共享偏差，对未知作弊失效 |
| P0 | Human Review Randomization × Item Difficulty × Calibration | 生产关联不具备个体增量因果识别 |
| P0 | Risk Trigger × OOD World Dynamics × Nominal Action Identity | 风险头漏警或触发搜索错误改写安全行动 |
| P1 | Experience Form/Fit/Fusion × New Task × Cost | 经验复用造成历史正确行为回归 |
| P1 | Offline Code Policy × Model Policy × Equal Lifecycle Budget | 程序外部化优点被离线成本抵消 |

**Core reopen gate:** Only new inexpressible estimand, distinction, identification necessity, or non-replaceable framework would warrant SPEC_REVISION_CANDIDATE. None meets that standard today. Keep Scientific Core frozen.
