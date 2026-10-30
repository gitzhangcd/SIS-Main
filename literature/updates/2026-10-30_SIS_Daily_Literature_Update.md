# SIS Daily Literature Update | 2026-10-30

**Authority:** SIS v0.3.1 (Core frozen), Registry v1.3, SIS-LEM-P0 and ClaimRecord v0.1. **Discovery:** latest arXiv cs.AI page accessible was 2026-10-28 (407 listed; 95 new); EMNLP 2026 records below were published in October, newly discovered from archival proceedings now, **not** published 2026-10-30. New preprints first submitted Oct 26–27. Primary source version and reading priority in every item; community discussion discovery-only.

**De-dup and governance:** 10 source URLs/titles checked against 145 canonical studies plus 59 synced Oct 24–29 provisional records. Unmerged Oct 9–23 history still requires complete backfill/lineage reconciliation; no new permanent SIS-LIT IDs. **No paper-wide CL2/CL3; no causal transport T3, mechanism invariance T4, or second-coder promotion.**

**Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA` (secondary `BENCHMARK_DELTA`). Real pressure on independent evaluator observations, blind scientific-optimization evaluation, process-level citation provenance, dynamic viability, semantic program validity, and CSCI effect modification. All expressible in existing SIS v0.3.1: **CORE_DELTA_NONE; SPEC_REVISION_CANDIDATE=NO**.

## StudyVersionRecords / First-coder scientific coding

### SIS-CAND-20261030-01 — Beneath the Diff: Diagnosing and Mitigating Algorithmic Mode Collapse in Code-Level Autonomous Research Loops
- **Primary version:** [EMNLP 2026 Main (October; delayed archival discovery)](https://aclanthology.org/2026.emnlp-main.1029/); **priority 代码级自动科研循环的编辑表面多样但语义机制趋同；DAPS结合语义覆盖、历史记忆与验证准入**.
- **Scientific routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `DR/MI/MEAS/ID/EG/BT`; primary estimand `SEMANTIC_PROPOSAL_DIVERSITY_HELDOUT_OPTIMIZATION_EFFECT`.
- **Claim ceiling:** CL1; local CL2 candidate, identification/transport I1/I2-local/T1; evidence role `NEGATIVE_OPTIMIZER_DYNAMICS`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 作者报告语义类别衰减减少69.1%，blind/audit相对faithfulness提升83.7%/81.6%
- **Reported evidence:** 三组件联合变化，机制中介未独立识别；盲测保持隔离但仅测试所研究的科研循环
- **Limits, confounders, transport:** 挑战in-loop成功=真实算法发现；提出语义提案坍缩与评价可见性的边界
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-02 — Gaming the Judge: How Unfaithful Chain-of-Thought Can Undermine Agent Evaluation
- **Primary version:** [Findings EMNLP 2026 (October; delayed archival discovery)](https://aclanthology.org/2026.findings-emnlp.1636/); **priority 固定真实动作与观察，只修改推理叙述，检验Judge是否被不忠实解释误导**.
- **Scientific routing:** Primary `ROUTING_ABSTAIN`; Cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; primary estimand `COT_REWRITE_JUDGE_FALSE_POSITIVE_EFFECT`.
- **Claim ceiling:** CL1; local CL2 candidate, identification/transport I2-local/T1; evidence role `NEGATIVE_MEASUREMENT_CONSTRUCT`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 800条Web轨迹中部分Judge假阳性率相对基线最多增加117%
- **Reported evidence:** 117%是相对幅度不是百分点；人为轨迹操纵不是生产发生率；受Judge和任务分布影响
- **Limits, confounders, transport:** 强化评价信息与原始执行事件分离；CoT不是真值证据
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-03 — Who is the Agent to Blame? Localizing Faithfulness and Citation Mistakes in Agentic Deep Research
- **Primary version:** [EMNLP 2026 Main (October; delayed archival discovery)](https://aclanthology.org/2026.emnlp-main.1681/); **priority 逐组件比较输入与输出，定位虚构、丢失来源或不足引用**.
- **Scientific routing:** Primary `SDR`; Cross-cutting `CSCI/BGT`; Framework `TD/IA/EG/ID/MEAS/BT`; primary estimand `LOCAL_CITATION_ERROR_PROPAGATION_AND_REPAIR`.
- **Claim ceiling:** CL1; local repair candidate, identification/transport I1/I2-local/T0; evidence role `TRACE_FAITHFULNESS_BOUNDARY`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 三套开源深度研究系统中AI-Q的84.7%最终错误被标记起源于编排器；针对性干预使引用召回提高约5%
- **Reported evidence:** 错误来源标签不等于执行反事实因果源；单个AI-Q比例不可推广；修复有多变量混杂
- **Limits, confounders, transport:** 支持组件间证据传递的诊断；需要citation loss到outcome flip验证
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-04 — AgentRx: Diagnosing AI Agent Failures from Execution Trajectories
- **Primary version:** [Findings EMNLP 2026 (October; delayed archival discovery)](https://aclanthology.org/2026.findings-emnlp.598/); **priority 生成局部约束并逐步审查，输出可追溯违反证据和故障类别**.
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/ID/EG/MEAS/BT`; primary estimand `AUDITABLE_CONSTRAINT_FAILURE_LOCALIZATION_ACCURACY`.
- **Claim ceiling:** CL1; local label comparison, identification/transport I1/T1; evidence role `DIAGNOSTIC_MEASUREMENT_INSTRUMENT`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 170条人工标注失败轨迹、11类任务；作者报告步骤定位比对照平均提高75%
- **Reported evidence:** 人工关键错误标签不等于经真实修复验证的因果源；规模有限
- **Limits, confounders, transport:** 增强轨迹诊断证据接口，保持预测标签与因果干预分离
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-05 — The Cold-Start Safety Gap in LLM Agents
- **Primary version:** [EMNLP 2026 Main (October; delayed archival discovery)](https://aclanthology.org/2026.emnlp-main.1973/); **priority 改变风险请求前经历的普通任务数量，测试系统安全行为随执行历史变化**.
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; primary estimand `PRECEDING_TASK_DEPTH_CONDITIONAL_SAFETY_EFFECT`.
- **Claim ceiling:** CL1; local session-depth candidate, identification/transport I2-local/T1; evidence role `DYNAMIC_VIABILITY_BOUNDARY`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 7个模型4个家族、最多20个前序任务；作者报告安全评价改善9%–52%
- **Reported evidence:** 历史长度、普通任务类型与上下文内容可能共同作用；隐层变化不是独立因果中介
- **Limits, confounders, transport:** 明确系统安全具有session-depth条件性；不能把预热视为通用安全保证
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-06 — Evolving Agent Teams
- **Primary version:** [arXiv:2610.36848 v1, 2026-10-27 (preprint)](https://arxiv.org/abs/2610.36848); **priority 监督器诊断局部最优并重构团队，持久文件保存搜索证据**.
- **Scientific routing:** Primary `ASR`; Cross-cutting `CSCI/BGT`; Framework `DR/IA/MI/MEAS/ID/BT`; primary estimand `TEAM_RESTRUCTURING_LOCAL_OPTIMUM_POLICY_NET_VALUE`.
- **Claim ceiling:** CL1; local ablation candidate, identification/transport I1/I2-local/T2-performance; evidence role `IMPLEMENTATION_AND_CAPABILITY_INTERACTION`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 匹配token预算优于对照，延长预算下47个FlashInfer负载赢36个，报告生产基线平均1.2倍
- **Reported evidence:** 匹配与延长预算对照不能混同；重组、记忆与总计算共同变化；单项内核性能不是完整系统成本
- **Limits, confounders, transport:** ASR组织策略有价值但独立因果中介未识别
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-07 — MARQ: A Modular, LLM-Agnostic Requirement Quality Assessor Infused with Systems Engineering Knowledge
- **Primary version:** [arXiv:2610.36234 v1, 2026-10-26 (preprint)](https://arxiv.org/abs/2610.36234); **priority 将INCOSE标准转为分准则外部专家知识，检验不同模型对NASA工程要求缺陷的检测**.
- **Scientific routing:** Primary `SCF`; Cross-cutting `CSCI/BGT`; Framework `MI/EG/MEAS/ID/BT`; primary estimand `CRITERION_KNOWLEDGE_INFUSION_REQUIREMENT_DEFECT_F1_EFFECT`.
- **Claim ceiling:** CL1; local knowledge contrast candidate, identification/transport I1/I2-local/T1; evidence role `MEASUREMENT_INSTRUMENT`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 100次模型重复执行：Claude F1 .80 vs .55、GPT-5.6 Sol .62 vs .52、Gemma .53 vs .18
- **Reported evidence:** 重复次数不等于独立任务数量；不同模型误报与漏报代价不同；专家Gold覆盖有限
- **Limits, confounders, transport:** 科学任务规范与模型能力交互，应独立测量Precision/Recall和误报代价
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-08 — Grounding LLM Agents in Business Processes: Process-Aware Knowledge Graphs for Reliable Multi-Step Service Invocation
- **Primary version:** [arXiv:2610.37242 v1, 2026-10-27 (preprint)](https://arxiv.org/abs/2610.37242); **priority 将OData与BPMN流程约束编码到类型图，辅助端点检索与合法调用**.
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/TD/EG/MEAS/ID/BT`; primary estimand `TYPED_PROCESS_GRAPH_CONTEXT_API_CONFORMANCE_EFFECT`.
- **Claim ceiling:** CL1; local schema contrast candidate, identification/transport I1/I2-local/T0; evidence role `REPRESENTATION_EXTERNALIZATION_BOUNDARY`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 42服务、81多步骤任务完成率38.7% vs 10.3%，完整类型信息非法调用3/101
- **Reported evidence:** 没有流程元数据的OpenAPI场景无收益；检索、字段与过程上下文同时变化
- **Limits, confounders, transport:** 流程契约外部化是可替换MI能力，非新科学原语
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-09 — From Structural Feedback to Prompt Policies: Learning Faithful Text-to-Image Prompt Editors
- **Primary version:** [arXiv:2610.36146 v1, 2026-10-26 (preprint)](https://arxiv.org/abs/2610.36146); **priority 场景图约束可重用的提示编辑策略，优化审美同时保护对象和关系**.
- **Scientific routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `DR/MI/EG/MEAS/ID/BT`; primary estimand `GRAPH_CONDITIONED_PROMPT_EDIT_RELATIONAL_FIDELITY_EFFECT`.
- **Claim ceiling:** CL1; local ablation candidate, identification/transport I1/I2-local/T1; evidence role `SEMANTIC_INVARIANT_OPTIMIZER`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 三个不重合的2K提示集、4个冻结生成器，独立指标与15名人工标注支持关系忠实度收益
- **Reported evidence:** 图谱标定、编辑与图像奖励共同变化；标注样本有限；图未表示的语义无法保证
- **Limits, confounders, transport:** 提示优化须加入不可变语义约束，属于ARSO算子实现
- **SIS relationship & new boundary:** undefined

### SIS-CAND-20261030-10 — Agentic Distributional Regression: Conditional Density Estimation through Agent-Written Programs
- **Primary version:** [arXiv:2610.37611 v1, 2026-10-27 (preprint)](https://arxiv.org/abs/2610.37611); **priority 系统搜索可执行条件密度公式，输出可独立审计的统计程序**.
- **Scientific routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `MI/DR/EG/MEAS/ID/BT`; primary estimand `EXPLICIT_DENSITY_PROGRAM_SEARCH_VALIDATED_VALUE`.
- **Claim ceiling:** CL0 theorem + CL1 empirical, identification/transport I0/I1/T1; evidence role `FORMAL_PROGRAM_SEARCH`. Paper metadata != ClaimRecord adjudication.
- **Novelty / hypothesis:** 明确条件下推导有限样本界和验证选择不等式；12真实数据集及训练后数据集比较
- **Reported evidence:** IID、程序长度、优化误差和独立验证是保证前提；不能把最优结果等同于搜索机制可迁移
- **Limits, confounders, transport:** 程序外部化使科学输出可验证，但仍受验证数据与模型选择偏差制约
- **SIS relationship & new boundary:** undefined

## P0 claim-level advance / evidence-map

Re-audited **SIS-LIT-023, SIS-LIT-031, SIS-LIT-045** as **9 distinct ClaimRecords**. The 023 predeclared H1/H4a five-point hypotheses are not supported; H2 and H7a locally supported. The 031 compiler is a bundled outcome improvement, not proven full semantic equivalence. The 045 nonsignificant interaction F-test is not proof of no interaction; diagnostic pretest not prospectively validated. See [source-anchored audit](../evidence-map/audits/SIS_P0_Reaudit_2026-10-30.md). First coder only; second coder & adjudication pending.

## Recommended fixtures

| P | Fixture | Main measurement |
|---|---|---|
| P0 | Semantic Proposal Diversity × Sealed Blind Metric | semantic mode collapse, genuine unseen gain, selection leakage |
| P0 | CoT-only Rewrite × Fixed Action/Observation | evaluator false-positive construct validity |
| P0 | Multi-Stage Citation Provenance × Interventions | transmission loss vs causal source |
| P0 | Memory Migration × Reader/Writer/Embedding Swap | capability retention and recoverability with raw-source control |
| P0 | Session History × Risk Response | cold-start viability and resource/history confounding |
| P0 | Requirement Quality × Expert Gold | model-stratified false alarms, misses and repeatability |
| P1 | Team Restructure × Matched Full Compute | net benefit beyond local optimum |
| P1 | Typed BPMN Process × No-Process Negative Control | specification-conditional API validity |
| P1 | Explicit Scientific Program × Independent Validation | post-selection model validity |

**Source/governance:** independent peer-reviewed archival IDs stored per study; arXiv items not misclassified as reviewed; community commentary discovery-only. Claim ceilings are first-coder hypotheses, not final scientific Gold.
