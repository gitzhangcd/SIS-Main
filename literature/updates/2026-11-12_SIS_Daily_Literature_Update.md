# SIS Daily Literature Update｜2026-11-12

Authoritative SIS v0.3.1 Master and Registry v1.3. Discovery window after the 2026-11-11 daily update. arXiv cs.AI 2026-11-11 list includes 381 entries and 105 new submissions; cited manuscripts submitted Nov 6-10. 1 archival AACL November paper; 9 original preprints. Search against already synchronized registry found no same source identifier; earlier historical candidate reconciliation remains pending. Author-claimed NeurIPS acceptance of 2611.13596 is NOT independently verified. Primary abstract and official record screenings; no 10-study fulltext audit and no community analysis elevated beyond DISCOVERY_ONLY.

## Ten independent study-version candidates

### SIS-CAND-20261112-01 — RAGCap-Bench: Benchmarking Capabilities of LLMs in Agentic Retrieval Augmented Generation Systems
- StudyVersionRecord: https://aclanthology.org/2026.aacl-long.245/; PEER_REVIEWED_AACL_NOV_2026; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 官方11月AACL论文：迭代检索中间能力与端到端表现的关联；相关性无法识别各环节的独立因果贡献。
- Primary Program: ROUTING_ABSTAIN; Cross-cutting: BGT; Framework Capability Profile: MI/TD/MEAS/ID/BT.
- Primary estimand: INTERMEDIATE_RETRIEVAL_CAPABILITY_END_TO_END_PREDICTIVE_VALIDITY; claim maturity ceiling: CL1; identification: I1; transport: T1; evidence role: INSTRUMENT / boundary.
- Key boundary variables: 检索步难度、任务信息密度、评分标签、模型、工具权限. SIS impact: SHARPENS MEAS：需要独立测量中间能力与终点净收益。. Reading priority: Worth Skimming. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-02 — Agent Architecture Cost-Success Trade-offs: A Controlled Evaluation across Enterprise-Style SOPs
- StudyVersionRecord: https://arxiv.org/abs/2611.12953; PREPRINT_2026_11_07; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 13项企业SOP与8个架构条件比较。复杂组织多耗1.4–4.7倍token和2.6–5.8倍延迟，整体成功差异通常不显著；定向重构后75.6% vs 67.4%。任务少且架构实现质量可能混杂。
- Primary Program: SCF; Cross-cutting: CSCI/BGT; Framework Capability Profile: MI/IA/MEAS/ID/BT.
- Primary estimand: FIXED_EXECUTOR_SOP_CONDITIONAL_ORGANIZATION_COST_SUCCESS_FRONTIER; claim maturity ceiling: CL1; local CL2 candidate; identification: I2-local provisional; transport: T1; evidence role: NULL / boundary / cost frontier.
- Key boundary variables: SOP复杂度、技能质量、token、延迟、拓扑、模型. SIS impact: SHARPENS SCF/CSCI；不预设多组件优于单组件。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-03 — Seeing Is Not Believing: Counterfactual Lesion Erasure Teaches a Small Medical Vision-Language Agent to Report Only What the Image Shows
- StudyVersionRecord: https://arxiv.org/abs/2611.13006; PREPRINT_2026_11_08; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 507例内部评估中抹除病灶反事实训练改善影像证据敏感性；外部48例气胸检测为0，临床净效用反而下降。编辑图像也有分布偏移风险。
- Primary Program: SCF; Cross-cutting: BGT; Framework Capability Profile: MI/MEAS/ID/EG/BT.
- Primary estimand: LESION_ERASURE_EVIDENCE_GATING_VS_RARE_DISEASE_DETECTION_NET_UTILITY; claim maturity ceiling: CL1; local CL2 candidate; identification: I2-local provisional; transport: T1; evidence role: NEGATIVE_BOUNDARY / measurement.
- Key boundary variables: 病种患病率、外部中心、图像编辑、危重病敏感度和误报成本. SIS impact: CHALLENGES抗幻觉率可替代临床净效用的假设；无需SIS原语修订。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-04 — From Questions to Decisions: Benchmarking How LLM Agents Acquire Decision-Relevant Information from Human Beings
- StudyVersionRecord: https://arxiv.org/abs/2611.13015; PREPRINT_2026_11_09; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: Ask2Decide 43项任务、19名真实参与者79次互动。人类纠正被遗漏事实比模拟用户频繁；询问数量不等于决策信息价值。真人意图及优化器目标可能不同。
- Primary Program: ASR; Cross-cutting: CSCI/BGT; Framework Capability Profile: DR/IA/ID/MEAS/BT.
- Primary estimand: DECISION_RELEVANT_HUMAN_QUERY_VALUE_OF_INFORMATION; claim maturity ceiling: CL1; local CL2 candidate; identification: I2-local provisional; transport: T1; evidence role: BOUNDARY / regulation measurement.
- Key boundary variables: 信息缺失模式、回复真实性、专家时间、目标与可行集. SIS impact: SHARPENS ASR；应测量真实决策改变和人类负担。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-05 — Counting Under Disagreement: Dollar-Weighted Measurement, Selective Machine Labelling and Budgeted Human Review from Disagreeing AI Readers of Administrative Text
- StudyVersionRecord: https://arxiv.org/abs/2611.13215; PREPRINT_2026_11_09; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 651条三人独立标注及12.1万文本；不同读者令美元加权总量相差约39.3亿美元，是抽样不确定性区间2.2倍。主动复核收益主要是模拟，尚未完成真实部署误差认证。
- Primary Program: ROUTING_ABSTAIN; Cross-cutting: BGT; Framework Capability Profile: MEAS/EG/ID/DR/BT.
- Primary estimand: HUMAN_READER_DISAGREEMENT_VS_SAMPLING_VARIANCE_AND_REVIEW_ALLOCATION; claim maturity ceiling: CL0 conditional theory; CL1 empirical; identification: I1/I2-design-specific; transport: T0; evidence role: NEGATIVE / measurement / governance.
- Key boundary variables: 专家规则、权重、抽样、独立Gold、分歧裁决、审核预算. SIS impact: SHARPENS MEAS/EG：人类分歧不能合并进抽样方差。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-06 — Agent-Guided Discovery of Exchange-Correlation Functionals with Physics-based Validation
- StudyVersionRecord: https://arxiv.org/abs/2611.13329; PREPRINT_2026_11_09; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 大模型提出密度泛函O159，并用自洽物理计算及保留集检验；报告MGCDB84较ωB97M-V误差下降11.7%。领域结果有独立性，但候选搜索、人工选择与资源预算未能识别AI独立科研贡献。
- Primary Program: SCF; Cross-cutting: CSCI/BGT; Framework Capability Profile: MI/TD/EG/MEAS/ID/BT.
- Primary estimand: AI_PROPOSED_SCIENTIFIC_FUNCTIONAL_INDEPENDENT_PHYSICAL_HOLDOUT_GAIN; claim maturity ceiling: CL1 external validation; not CL3 mechanism; identification: I1; transport: T1; evidence role: SCIENTIFIC_VALIDATION / boundary.
- Key boundary variables: 候选生成预算、独立物理计算、留出集污染、重复实验. SIS impact: SHARPENS SCF：区分科学结果获验证与系统发现机制。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-07 — Veritas: A Verifier Generation Harness for Agent Tasks
- StudyVersionRecord: https://arxiv.org/abs/2611.13336; PREPRINT_2026_11_09; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 生成证据头、领域规则与迭代准则，使任务验证器在四个Benchmark中更贴近官方验证器。官方评价器不等于独立任务真值，几个模块没有等预算正交消融。
- Primary Program: ASR; Cross-cutting: BGT; Framework Capability Profile: DR/EG/MEAS/ID/BT.
- Primary estimand: AUTOMATIC_VERIFIER_GENERATION_AGREEMENT_VS_INDEPENDENT_TASK_GOLD; claim maturity ceiling: CL1; local CL2 candidate; identification: I1/I2-local provisional; transport: T1; evidence role: INSTRUMENT / implementation / identification.
- Key boundary variables: 官方评分器有效性、隐藏规则、过拟合、模型族、判定成本. SIS impact: SHARPENS ASR/EG：验证器一致性不等于任务正确性。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-08 — Agent Benchmarks Stop Ranking Before They Run Out of Tasks
- StudyVersionRecord: https://arxiv.org/abs/2611.13541; PREPRINT_2026_11_10; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 八个Benchmark执行工件重评分，发现二值通过率及人类参考上限可能抹平前列模型差异；Terminal-Bench中二值结果相似系统的原始连续指标可差十倍以上。连续评分本身仍需构念与标尺校准。
- Primary Program: ROUTING_ABSTAIN; Cross-cutting: BGT; Framework Capability Profile: MEAS/EG/ID/BT.
- Primary estimand: PASS_FAIL_CEILING_VS_CONTINUOUS_UTILITY_RANKING_DISCRIMINATION; claim maturity ceiling: CL1 measurement audit; identification: I2-local re-scoring; transport: T0; evidence role: MEASUREMENT_INSTRUMENT / null ranking.
- Key boundary variables: Benchmark版本、评分分辨率、人类参考、成本、噪声. SIS impact: SHARPENS MEAS：排名饱和未必代表任务已被解决。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-09 — Towards Reliable VLM Judges: State-Conditional Invariance and Presentation-Aware Diagnostics
- StudyVersionRecord: https://arxiv.org/abs/2611.13596; PREPRINT_2026_11_10_ACCEPTANCE_UNVERIFIED; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 用MiniGrid环境比较真实状态反事实与仅改变呈现方式的轨迹，发现视觉Judge对呈现敏感且对因果变化辨别不足。arXiv总列表核验，单篇全文尚未复核；作者声称NeurIPS接收，未独立证实。
- Primary Program: ROUTING_ABSTAIN; Cross-cutting: BGT; Framework Capability Profile: MI/TD/MEAS/ID/EG/BT.
- Primary estimand: STATE_CONDITIONAL_JUDGE_PRESENTATION_INVARIANCE_VS_CAUSAL_SENSITIVITY; claim maturity ceiling: CL1 initial screening; identification: I1/I2-local provisional; transport: T0; evidence role: MEASUREMENT / negative boundary.
- Key boundary variables: 图像编码、状态恢复、无关呈现变动、模型、评审环境. SIS impact: SHARPENS MEAS/ID：应检验呈现不变性及真实状态因果敏感性。. Reading priority: Must Read. First coder initial screening only; independent reproduction and adjudication pending.

### SIS-CAND-20261112-10 — Auditable Human-Agent Teams for Autonomous X-ray Experimentation
- StudyVersionRecord: https://arxiv.org/abs/2611.12933; PREPRINT_2026_11_06_DELAYED_INDEXING; source discovery 2026-11-12; new distinct source ID, no permanent number.
- Novelty / evidence audit: 三次真实同步辐射X射线实验保留人机多方执行记录，59–68%的修正涉及多方。真实仪器证据有价值，但缺少人力和AI的独立对照，不能归因独立系统能力。
- Primary Program: SDR; Cross-cutting: CSCI/BGT; Framework Capability Profile: TD/IA/EG/MEAS/ID/BT.
- Primary estimand: AUDITABLE_HUMAN_AGENT_EXPERIMENT_DECISION_PROVENANCE_AND_CORRECTION; claim maturity ceiling: CL1 descriptive implementation; identification: I0/I1; transport: T1 domain demonstration; evidence role: IMPLEMENTATION / evidence lineage.
- Key boundary variables: 专家劳动、仪器状态、研究目标变化、记录完整性. SIS impact: FILLS SDR/CSCI：真实物理科研审计案例，未形成新机制证据。. Reading priority: Worth Skimming. First coder initial screening only; independent reproduction and adjudication pending.

## P0 Claim-level re-audit

See literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-12.md. First-coder split 3 studies (SIS-LIT-016,017,021) into 9 claims; zero promotions, no T3/T4.

## Five scientific conclusions

1. More complex organizational forms lack unconditional benefit; matched task/model costs and skill implementation quality govern system frontier.
2. Binary score saturation and judge presentation sensitivity are measurement properties, not system capability laws.
3. Auto-verifier agreement cannot substitute for independent task semantic Gold; human reader disagreement can exceed sampling error.
4. Anti-hallucination training may fail rare critical diseases out-of-distribution; clinically meaningful utility must consider false negatives.
5. Real physical experiment / independent computational physics validates outcomes but does not automatically identify the causal contribution of the agent system.

## Proposed measurable benchmark updates

| Priority | Fixture | Main identification requirement |
|---|---|---|
| P0 | Fixed executor × SOP architecture × cost budget | Negative or conditional organization frontier |
| P0 | Binary vs continuous score × benchmark version | Score resolution independent of task modification |
| P0 | VLM judge × presentation swap × executed state CF | Presentation invariance and causal sensitivity |
| P0 | Verifier components × independent human/algorithmic Gold | Official agreement vs semantic correctness |
| P0 | Lesion erase × external rare critical disease | False-negative harm and clinical net utility |
| P0 | Clarification × decision-relevant information × expert effort | True value of human questions |
| P0 | Three independent experts × sample design × audit budget | Reader disagreement vs sampling variance |
| P1 | Physics scientific discovery × candidate generator × blind holdout | Domain value vs system causal contribution |
| P1 | Physical research log × human/agent correction | Provenance vs independent component value |

## Formal SIS Impact Decision

MEASUREMENT_IDENTIFICATION_DELTA (secondary BENCHMARK_DELTA). Real scientific measurement/identification pressure: ranking resolution, verifier/judge construct validity, clinical evidence-gating external negative boundary, human label disagreement, task-conditioned query value; not new SIS ontology. Existing SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG cover these questions; ScientificCoreDelta=0, SPEC_REVISION_CANDIDATE=NO, T3/T4 confirmed 0.
