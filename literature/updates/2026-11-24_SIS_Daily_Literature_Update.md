# SIS Daily Literature Update｜2026-11-24
Authority: [Master](../../specs/System_Intelligence_Science_v0.3.1.md), [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md), [P0 Queue](../evidence-map/SIS_P0_Audit_Queue.csv), parent 388cfbcefaa3062d7813ede7d24fabbd47f39328.
Search: arXiv cs.AI Nov 23 list (214 entries), targeted title screening, not exhaustive all abstracts; all 10 selected first submitted Nov 20. Targeted searches also OpenReview, ACL Anthology, NeurIPS/ICLR and technical reports. No new independently verified archival paper selected. METR Nov 20 report https://metr.org/blog/2026-11-20-q4-2026-capability-update/ discovery-only in this run. Full-text retrieval attempts failed; abstract-level first coder. All IDs and exact titles checked against complete Registry; no permanent ID assigned.

## Selected preprints
### SIS-CAND-20261124-01｜Recoverable Symbols, Unstable Execution: Auditing Internal Pathways and Decision Identity in Visual State Tracking — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27715v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 冻结ViT，3526对完全可解码符号视图中背景变化使准确率降17.13点；恢复相位修复351/391新增错误，但仍有142个预测不同；192个未见程序族锁定测试复现局部路径；一致性训练未胜普通增强。
- **SIS:** Primary SCF; cross-cutting BGT; Framework MI/ID/MEAS/BT; canonical family MEDIATED_MECHANISM_EFFECT; operational estimand CONTEXT_PHASE_SWAP_DECISION_IDENTITY; role 机制候选及训练负结果; provisional ceiling CL1 (CL0 for untested mechanism), I2-local/T1; pathway candidate. No formal promotion.
- **Boundary:** 背景、旋转头、解码器、决策身份. Impact SHARPENS; **Kill test:** 固定符号×背景×双向通道交换×随机通道×逐例一致性.

### SIS-CAND-20261124-02｜MetaRigor: From Agentic Automation to Verifiable End-to-End Meta-Analysis Through Scientific Decision Boundaries — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27713v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** Study×Target绑定来源与结果；模型解释语义、程序执行形式规则。完整结果F1 86.29%，证据确定性一致80.20%；7例端到端F1 77.01%，较最强基线+9.78点；三系统归档追踪显示身份错配改变统计输入及偏倚评价。
- **SIS:** Primary SDR; cross-cutting BGT; Framework TD/MI/EG/MEAS/ID/BT; canonical family PROPAGATION_EFFECT; operational estimand STUDY_TARGET_IDENTITY_ERROR_PROPAGATION; role 测量及传播边界; provisional ceiling CL1 (CL0 for untested mechanism), I1/T1; propagation observed, no isolated mediation. No formal promotion.
- **Boundary:** 研究类型、结局时点、Gold、7例样本. Impact SHARPENS; **Kill test:** 注入人群/时点错配×独立专家Gold×逐阶段追踪.

### SIS-CAND-20261124-03｜Double counting in LLM evidence fusion: exact posteriors separate rule compliance from posterior gain — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27138v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 2976个精确后验世界、四依赖等级及四配置；部分强模型增加指令后误差增0.044，另一模型改善0.0140（95%区间0.0064–0.0219）；预注册端点增益差0.0342（0.0303–0.0382），分组差0.0004（-0.0023–0.0031）。
- **SIS:** Primary SCF; cross-cutting BGT; CSCI hypothesis; Framework MI/MEAS/ID/EG/BT; canonical family CAUSAL_MECHANISM_EFFECT; operational estimand SOURCE_DEDUP_INSTRUCTION_POSTERIOR_GAIN; role 负边界及测量; provisional ceiling CL1 (CL0 for untested mechanism), I2-local/T1. No formal promotion.
- **Boundary:** 来源依赖、基线校准、提示、概率模型. Impact SHARPENS; **Kill test:** 固定事实×共享来源依赖×指令/安慰剂×精确后验.

### SIS-CAND-20261124-04｜CoEvoBench: Can LLMs Drive Recursive Co-Evolution of Agentic Systems? — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27116v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 五领域、24小时共同起点、独立测试；最强研究者弥合相对指令微调参考逾80%差距；交互任务有进展，长程编码少成功；首轮改善非持续递归。
- **SIS:** Primary ASR; cross-cutting BGT; CSCI candidate; Framework DR/MI/TD/MEAS/ID/BT; canonical family POLICY_VALUE; operational estimand RECURSIVE_MODEL_HARNESS_UPDATE_SELECTION; role 测量及递归边界; provisional ceiling CL1 (CL0 for untested mechanism), I1/T1; training and search bundled. No formal promotion.
- **Boundary:** 初始能力、训练预算、任务长度、选择器. Impact SHARPENS; **Kill test:** 仅模型/仅控制/联合×每轮隐藏测试×等预算.

### SIS-CAND-20261124-05｜GRACE: Controlled Evidence Interventions for Diagnosing and Improving Knowledge Integration in GraphRAG — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27350v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 4028题20140题图对，固定题目选项操纵支持路径及干扰；固定生成器和事实上下文，整体准确率57.17→62.78（95%CI差5.04–6.17点），断路径55.41→67.85，语义干扰仍过度弃权。
- **SIS:** Primary SCF; cross-cutting BGT; Framework MI/EG/MEAS/ID/BT; canonical family CAUSAL_MECHANISM_EFFECT; operational estimand GRAPH_SUPPORT_STATE_BY_GUIDANCE_ACCURACY_ABSTENTION; role 受控证据负边界; provisional ceiling CL1 (CL0 for untested mechanism), I2-local/T0; combined gate not isolated. No formal promotion.
- **Boundary:** 图谱覆盖、干扰、先验、校准、弃权损失. Impact SHARPENS; **Kill test:** 路径完整性×相关性×门控×风险覆盖率.

### SIS-CAND-20261124-06｜Evidence sufficiency assessment enables cost-effective review allocation in on-premise clinical AI agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27390v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 1605例；遮蔽推理诊断，按证据充分性校准；MIRA-v2前50%单次通过98.91%，节约约80%计算；CDM升级后测试达96%；跨专科/缺影像等全复核。
- **SIS:** Primary ASR; cross-cutting BGT; CSCI hypothesis; Framework DR/EG/MEAS/ID/BT; canonical family SELECTIVE_ACTION_UTILITY; operational estimand EVIDENCE_SUFFICIENCY_TRIAGE_RISK_COST; role 调节及风险边界; provisional ceiling CL1 (CL0 for untested mechanism), I1/T1; retrospective selective risk, not clinical benefit. No formal promotion.
- **Boundary:** 患病谱、缺失影像、Gold、复核能力、严重错误. Impact SHARPENS; **Kill test:** 冻结门槛×医院外部留出×随机复核×严重漏诊/工作量.

### SIS-CAND-20261124-07｜HookEvo: A Framework for Coordinated Plugin Evolution on Hook-Enabled Agent Runtimes — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27294v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 冻结Qwen3-4B，轨迹提议修改后匹配任务选择保留；四任务报告95.41/70.56/48.17/41.67%；三优化器×三范围中强优化器联合范围收益较大。
- **SIS:** Primary ASR; cross-cutting BGT; CSCI candidate; Framework DR/MI/TD/EG/MEAS/ID/BT; canonical family INTERVENTION_LOCUS_SELECTION_EFFECT; operational estimand TRACE_CONDITIONAL_EDIT_SCOPE_VALUE; role 实现及组件交互候选; provisional ceiling CL1 (CL0 for untested mechanism), I1/T1; selection and compute confounding. No formal promotion.
- **Boundary:** 优化器能力、候选数、编辑权限、回归、验证集重用. Impact SHARPENS; **Kill test:** 同预算×随机编辑范围×独立隐藏任务.

### SIS-CAND-20261124-08｜Same Facts, Different Decision: Fact-Invariant Manipulation and Provenance-Based Defense in Typed Decision Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27016v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 三个基准检验未增加事实的外部评论；约三分之一原本正确决策变错；来源门控阻止所测变化。
- **SIS:** Primary SCF; cross-cutting BGT; Framework MI/EG/MEAS/ID/BT; canonical family CAUSAL_MECHANISM_EFFECT; operational estimand FACT_INVARIANT_COMMENT_EXPOSURE_DECISION_CHANGE; role 负边界及治理实现; provisional ceiling CL1 (CL0 for untested mechanism), I2-local/T1; fact-equivalence verifier limits. No formal promotion.
- **Boundary:** 事实等价、来源、初始正确性、合法新证据. Impact SHARPENS; **Kill test:** 固定事实×来源×语义专家盲核×合法新证据正控制.

### SIS-CAND-20261124-09｜Portable Active Recovery under Timed and Position-Dependent Visual Outages — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27121v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 时间黑障与空间遮挡初始观测相似；悬停等待93/96对0/96。预注册48场景1920次飞行测试，完整MPPI最坏条件完成88.5%，较基线+29.2点（17.7–40.6）；移至SimpleFlight +17.7点（7.3–28.1）。
- **SIS:** Primary SDR; cross-cutting BGT; Framework TD/DR/MI/MEAS/ID/BT; canonical family RECOVERY_EFFECT; operational estimand OUTAGE_REGIME_BY_ACTIVE_RECOVERY; role 恢复机制候选及迁移边界; provisional ceiling CL1 (CL0 for untested mechanism), I2-local/T2 performance only. No formal promotion.
- **Boundary:** 故障机制、位置/时间、传感器、控制器、速度. Impact SHARPENS; **Kill test:** 相同初始观测×故障制度×随机恢复动作×重新获取观测中介.

### SIS-CAND-20261124-10｜Beyond Linear Decodability: Understanding and Improving Instruction Following in World Action Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.27401v1; submitted 2026-11-20; announced 2026-11-23; PREPRINT; provisional Study ID. Abstract verified; full text and independent replication pending.
- **Evidence:** 不遵循指令的模型也编码目标但线性可解码性较弱；辅助监督后LIBERO-CF成功率74.6%、grounding 89.2%，较最强基线+26.8/42.9点；两种无训练干预支持竞争解释。
- **SIS:** Primary SCF; cross-cutting BGT; Framework MI/ID/MEAS/BT; canonical family MEDIATED_MECHANISM_EFFECT; operational estimand INSTRUCTION_PRIOR_COMPETITION_GROUNDING; role 机制候选; provisional ceiling CL1 (CL0 for untested mechanism), I2-local candidate/T1; pathway pending. No formal promotion.
- **Boundary:** 训练目标、架构、先验、视觉域、动作真值. Impact SHARPENS; **Kill test:** 先验/指令冲突×选择性信号干预×随机方向×动作Gold.

## P0
[Audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-24.md): 081,095,036; 9 provisional claim units. JTPRO version reconciliation; no formal promotions.
## Synthesis and experiments
- Evidence duplication and graph sufficiency: exact posterior references, correlated-source control, separate correctness and abstention.
- Scientific result identity: inject population, outcome or timepoint mismatch and trace propagation to meta-analysis using independent Gold.
- Mechanistic identity: channel swaps and per-decision identity, not aggregate recovery; distinguish decoding, mediation and training benefit.
- Recursion: model/harness factorial, equal lifetime budget, hidden evaluation every round.
- Recovery and clinical selective action: similar initial observations but distinct latent failure regimes; prospective hospital risk, coverage and workload.
Decision: MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA. Real measurement/identification pressure, no uncovered primitive. Scientific Core frozen; no SPEC_REVISION_CANDIDATE. CSCI only hypothesis when model IDs substitute capability constructs.
