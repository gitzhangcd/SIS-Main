# SIS Daily Literature Update｜2026-11-11

Authority: `specs/System_Intelligence_Science_v0.3.1.md`, Registry v1.3, `SIS_P0_Audit_Queue.csv`, Evidence Map P0 and ClaimRecord schema.
Discovery window: after last completed 2026-11-10 daily run; checked arXiv cs.AI new list for Tuesday 2026-11-10 (887 listings including 166 new in cs.AI), ACL Anthology, official arXiv and project pages. Discovered Nov 11 Asia/Shanghai. **Publication date ≠ arXiv submission date ≠ discovery date.** The peer-reviewed DeepResearch RewardBench is an **October 2026 EMNLP Findings** paper with November 6 arXiv v1; one underlying study and only one candidate ID.
Primary source URLs are attached to each record. No independent reproduction from technical/community interpretations; those are DISCOVERY_ONLY.
Exact-title + arXiv-ID + known ACL venue dedup against current synced 145 permanent records and previously synced provisional candidates; historical unsynced Oct 9–23 global reconciliation is still PENDING. Claim maturity below is claim-family intake ceiling, not final ClaimRecord adjudication.

## Key scientific finding
Information, organizational and training artifacts are not automatically system capability. Data-composition counter-interactions, fixed-executor workflow differences, costly unrepeatable pretraining and evaluator confidentiality expose measurement/identification problems. **Formal impact: MEASUREMENT_IDENTIFICATION_DELTA** (secondary BENCHMARK_DELTA), NOT SPEC_REVISION_CANDIDATE.

## Peer-reviewed archival paper (delayed discovery)
### 01. DeepResearch RewardBench: Evaluating Reward Models for Deep Research Report
- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.1611/; lineage https://arxiv.org/abs/2611.10156; 2026-10（EMNLP正式版）；arXiv v1 2026-11-06; PEER_REVIEWED; no duplicate Study.
- Novelty: 针对长篇深度研究报告建立query-specific rubric与人审过滤的成对、三元、四元排序测试；正式Findings EMNLP 2026版本早于新上传的arXiv。作者发现通用奖励模型处理连贯性较好，却不擅长评价科学报告，比较式判定优于直接打分。
- Evidence audit: Rubric与评价模型可能共享偏好；人审过滤不等于全样本独立Gold。未独立证明排序代理指标能预测真实科研发现或复现质量。
- Primary estimand: `RESEARCH_REPORT_COMPARATIVE_REWARD_JUDGE_VALIDITY`; Primary Program: `ROUTING_ABSTAIN`; Cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`.
- Claim maturity ceiling: **CL0 measurement contract; CL1 empirical**; identification I1; transport T1; evidence role INSTRUMENT / negative measurement boundary.
- Impact: SHARPENS：科学报告质量与实际证据支持应分离；评价器本身须接受跨版本、跨来源验证。 Key boundary / experimental action: 固定同一报告候选，正交改变rubric来源与评审器，独立专家盲审；校验报告内claim—source锚点。
- Reading priority: Must Read; second coder/adjudication pending.

## New or newly indexed preprints
### 02. Homeopathic Learning: Diluting poisoned fine-tuning data can strengthen its effect
- StudyVersionRecord: https://arxiv.org/abs/2611.10110; 2026-11-06（UTC首次提交）；11-10公告; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 少量含触发特征的污染样本单独训练未必形成隐藏行为，但加入格式相近、无触发的干净样本后反而出现后门；覆盖不同语言任务、奖励投机文本和MNIST，给出回归式解释。
- Evidence audit: 需明确训练步数、数据配比、触发词频率及梯度预算对照；回归解释不是已识别中介，构造后门不代表现实发生率。
- Primary estimand: `CONTRASTIVE_CLEAN_DATA_BY_TRIGGER_BACKDOOR_INTERACTION`; Primary Program: `SCF`; Cross-cutting `BGT`; Framework `MI/ID/MEAS/BT`.
- Claim maturity ceiling: **CL1; local CL2 candidate**; identification I2-local provisional; transport T1; evidence role LIMIT / unexpected interaction / negative safety result.
- Impact: SHARPENS SCF：安全风险可能源于数据组合交互，而非逐样本属性；不能以单数据集静态审计作保证。 Key boundary / experimental action: Poison×Clean×Trigger 2×2×2、固定训练Token与步数、跨模型和未见触发检验。
- Reading priority: Must Read; second coder/adjudication pending.

### 03. WorkflowArena: Benchmarking Executable Workflow Orchestration in LLM-Based Multi-Agent Systems
- StudyVersionRecord: https://arxiv.org/abs/2611.12856; 2026-11-09（UTC首次提交）；11-10公开; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 145项长时程任务、8专业领域、9模型；允许系统自主决定是否委派及如何组织交付。固定执行器并更换工作流作者时表现改变，直接揭示组织方案可独立成为系统能力条件。
- Evidence audit: 工作流包含任务说明及隐含知识，组织拓扑与信息内容未分开；32项作者迁移测试没有充分重复随机种子，单一模型与Harness组合混杂。
- Primary estimand: `FIXED_EXECUTOR_WORKFLOW_AUTHOR_ORGANIZATION_EFFECT`; Primary Program: `SCF`; Cross-cutting `CSCI/BGT`; Framework `MI/IA/MEAS/ID/BT`.
- Claim maturity ceiling: **CL1; local CL2 candidate**; identification I1/I2-local provisional; transport T1; evidence role SUPPORT / component-system interaction / boundary.
- Impact: SHARPENS SCF/CSCI，不把Workflow当SIS primitive；建议固定执行器、组织结构和指令信息正交控制。 Key boundary / experimental action: 固定执行器×固定任务×工作流作者，另对拓扑和指令信息进行2×2消融及等预算复跑。
- Reading priority: Must Read; second coder/adjudication pending.

### 04. No Second Run: Does RSI Stop at Frontier Pre-training?
- StudyVersionRecord: https://arxiv.org/abs/2611.10719; 2026-11-07（UTC首次提交）；11-10公告; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 报告一次无法端到端重做的大规模预训练：30B-A3B模型、11.8T Token、约三个月。采用多个可闭环的局部设计与修复循环，而不是声称完成整个预训练过程的反事实RSI。
- Evidence audit: 只有一个完整预训练实例，团队、数据、算力和工具共同变化；后续成绩不能识别各局部循环贡献或构成整场预训练的可重复因果效应。
- Primary estimand: `UNREPEATABLE_PRETRAINING_LOCAL_LOOP_ADAPTATION_NET_VALUE`; Primary Program: `ASR`; Cross-cutting `BGT`; Framework `DR/TD/MI/EG/MEAS/BT`.
- Claim maturity ceiling: **CL0 conditional RSI design; CL1 implementation/performance**; identification I0/I1; transport T1 performance only; evidence role IMPLEMENTATION / identification boundary.
- Impact: SHARPENS ASR：不可重复全局过程应降低可识别Claim上限；需把局部试验和全局结果的证据角色分离。 Key boundary / experimental action: 多次可重放小规模预训练局部循环、对照全局生产运行的决策日志与未执行备选及成本。
- Reading priority: Must Read; second coder/adjudication pending.

### 05. Embodied First Exam
- StudyVersionRecord: https://arxiv.org/abs/2611.12177; 2026-11-09（UTC首次提交）；11-10公开; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 1,156个任务、35套件、47机器人，区分只给传感器且不可重置的Standard、思考时环境仍变化的Realtime、全状态无限重置的Privileged；456核心任务最优被测系统标准设置通过率34%。
- Evidence audit: 多数情境在模拟器，Privileged并非现实可用上限；控制方式、模型、计算资源与实时思考延迟混杂，不能转成真实机器人安全率。
- Primary estimand: `RESET_PRIVILEGE_REALTIME_CONDITIONAL_EMBODIED_TASK_SUCCESS`; Primary Program: `SDR`; Cross-cutting `BGT`; Framework `TD/MI/MEAS/ID/BT`.
- Claim maturity ceiling: **CL1 measurement; no causal mechanism promotion**; identification I1; transport T1 simulated; evidence role INSTRUMENT / negative boundary.
- Impact: SHARPENS SDR/BGT：非重置性、持续时间与观测权限是必须独立测量的环境边界。 Key boundary / experimental action: 同一机器人任务×重置权限×实时环境推进×可观测状态，固定执行器与资源预算。
- Reading priority: Must Read; second coder/adjudication pending.

### 06. Reconfigurable Action Theories: A Formal Foundation for Dynamically Composable Agent Harnesses
- StudyVersionRecord: https://arxiv.org/abs/2611.12300; 2026-11-09（UTC首次提交）；11-10公开; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 形式化定义可在执行时加载/卸载模块的Action Theory；给出确定下一状态、模块加入后旧行为保持及加载顺序无关的充分条件，并编译为ASP。用实际Harness执行作为有限对照。
- Evidence audit: 保证仅在给定语法片段与前提成立时有效；形式化抽象可能漏掉真实工具副作用、信息权限和外部服务，不能推出通用Harness安全性。
- Primary estimand: `MODULE_LOAD_UNLOAD_BEHAVIOR_PRESERVATION_AND_COMPOSITION`; Primary Program: `SCF`; Cross-cutting `BGT`; Framework `MI/TD/ID/BT`.
- Claim maturity ceiling: **CL0 conditional formal results; CL1 implementation comparison**; identification I0/I1; transport T0; evidence role INSTRUMENT / conditional mechanism representation.
- Impact: FILLS EXISTING FRAMEWORK：可替换的语义/DSL与Conformance Instrument，而非第四个Primary Program。 Key boundary / experimental action: Module A×B 加载顺序×资源/权限条件，模型行为、可达目标和实际工具副作用独立验证。
- Reading priority: Must Read; second coder/adjudication pending.

### 07. Double Blind Evals: Resolving the Dual Confidentiality Dilemma in AI Safety Auditing
- StudyVersionRecord: https://arxiv.org/abs/2611.12604; 2026-11-09（UTC首次提交）；11-10跨列; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 以硬件安全执行环境保护专有模型和私有测试题互不泄露；在H100机密计算环境中将Gemini 2.5 Flash Lite与私有AILuminate样本进行实测。
- Evidence audit: 机密性条件取决于硬件信任根、密钥管理、远程证明与侧信道假设；安全交换不保证测量公平、任务构念有效或无基准污染。
- Primary estimand: `MUTUAL_CONFIDENTIALITY_ENCLAVE_EVALUATION_FEASIBILITY`; Primary Program: `ROUTING_ABSTAIN`; Cross-cutting `BGT`; Framework `EG/MEAS/ID/BT`.
- Claim maturity ceiling: **CL0 threat-model design; CL1 pilot**; identification I0/I1; transport T0; evidence role INSTRUMENT / implementation.
- Impact: FILLS EG/MEAS：可提升独立评价可实施性，但不能因加密保护自动提升CL。 Key boundary / experimental action: 端到端威胁模型、证明链/泄漏测试、盲评与公开Gold一致性对照。
- Reading priority: Worth Skimming; second coder/adjudication pending.

### 08. SciMARS: Multi-Agent Recursive Self-Improvement for Closed-Loop Scientific Discovery
- StudyVersionRecord: https://arxiv.org/abs/2611.12552; 2026-11-09（UTC首次提交）；11-10公开; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 共享证据图与角色、协调、记忆策略三个独立编辑器，迭代选择Harness；数字孪生/实验数据重放条件下，GPT-6 Astra 12/18 vs 8/18、ScienceAgentBench 14/38 vs 11/38。
- Evidence audit: 样本小、组合编辑器与证据图共同变化，模拟实验不是真实独立科学发现；测试集合及更新期间曝光风险需核。
- Primary estimand: `EVIDENCE_GRAPH_ROLE_MEMORY_POLICY_UPDATE_SCIENTIFIC_TASK_VALUE`; Primary Program: `ASR`; Cross-cutting `CSCI/BGT`; Framework `DR/MI/IA/EG/ID/MEAS/BT`.
- Claim maturity ceiling: **CL1 combination; local CL2 candidate only after controls**; identification I1; transport T1; evidence role IMPLEMENTATION / conditional policy value.
- Impact: SHARPENS ASR科学闭环，但不足以确立各编辑器独立机制或T3迁移。 Key boundary / experimental action: EvidenceGraph×RoleEditor×MemoryEditor 2×2×2，固定初始数据、盲最终独立实验Gold和预算。
- Reading priority: Must Read; second coder/adjudication pending.

### 09. Who Remembers What? Multi-Granularity Memory Extraction for Multi-User, Multi-Agent Interaction
- StudyVersionRecord: https://arxiv.org/abs/2611.10439; 2026-11-07（UTC首次提交）；11-10跨列; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: MixUA把经验分配到用户—执行器对、用户、执行器及全局四级作用域。在5用户7执行器实验中，完成率最多高于无记忆16个百分点，隐私探针发现不允许作用域中植入事实的比例最多0.02%。
- Evidence audit: 受控隐私探针低命中率不能证明现实无泄漏；受益性判定与权限标签可能由相同模型生成，真实跨组织信任边界未知。
- Primary estimand: `MEMORY_SCOPE_BY_USER_AGENT_TRANSFER_PRIVACY_UTILITY`; Primary Program: `SCF`; Cross-cutting `CSCI/BGT`; Framework `MI/IA/EG/ID/MEAS/BT`.
- Claim maturity ceiling: **CL1; local CL2 candidate**; identification I1/I2-local; transport T1; evidence role SUPPORT / boundary / privacy leakage measurement.
- Impact: SHARPENS CSCI/EG：知识共享收益与用途授权必须联合测量，并将跨用户性能和隐私边界作为独立估计量。 Key boundary / experimental action: Scope×Executor×User×Disclosure，独立隐私Gold、多随机种子和真正跨执行器保持评估。
- Reading priority: Must Read; second coder/adjudication pending.

### 10. Joi-Bench-Task: Benchmarking Task Coordination in Full-duplex Voice Agents through Interactive Simulation
- StudyVersionRecord: https://arxiv.org/abs/2611.12118; 2026-11-09（UTC首次提交）；11-10公开; PREPRINT v1; no confirmed peer-reviewed version.
- Novelty: 以语音打断、工具执行和结果播报的时间节点模拟动态用户修改；5个商用语音系统中最高请求变更完成率55%，4/5系统被打断后的平均信息遗漏率至少23%。
- Evidence audit: 语音系统同时存在ASR、模型、工具与音频播报变量，模拟用户打断策略与真实使用不同；对话中承诺和真实任务完成的测量应分开。
- Primary estimand: `SPEECH_INTERRUPTION_GOAL_REVISION_OBLIGATION_RETENTION`; Primary Program: `SDR`; Cross-cutting `BGT`; Framework `TD/DR/MEAS/EG/BT`.
- Claim maturity ceiling: **CL1**; identification I1; transport T1; evidence role INSTRUMENT / negative dynamic-boundary.
- Impact: SHARPENS SDR：长时程义务保持需要区分已执行、已播报和仍欠用户的信息。 Key boundary / experimental action: InterruptionTime×ToolCommitState×GoalRevisionType及任务/口头通报双轨真值。
- Reading priority: Worth Skimming; second coder/adjudication pending.


## Technical / community analyses
No independently reproduced new community analysis selected as primary evidence; DISCOVERY_ONLY, no claim promotion.

## P0 claim-level audit
See [2026-11-11 SIS P0 Reaudit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-11.md): SIS-LIT-002/007/015 = 9 claims, first-coder only. 0 promotions, 0 confirmed T3/T4. Fulltext and judge validation as specified.

## SIS scientific synthesis: five impacts
1. Workflow authorship with a fixed executor must distinguish topology and instruction information; CSCI capability interaction is testable, not a Multi-Agent primitive.
2. Clean training data can amplify poisoned triggers; safety evaluation requires contrastive dataset-composition factors and negative results.
3. Large-scale frontier pretraining cannot be repeated globally, so local update loops and full-production causal claims need different evidence ceilings.
4. Scientific-report scoring and blind scientific-discovery benchmarks require independent human/primary-source Gold, not just automated comparative rubrics.
5. Reset privilege, real-time state progression, confidential evaluator access, memory scope and user interruption determine what is observable/actionable; do not conflate instrumentation with system viability.

## Recommended measurable P0 fixture additions (not Core schema)
| Priority | Fixture | Estimand / kill condition |
|---|---|---|
| P0 | Fixed executor × workflow author × topology × instruction | Separate organization effect from source information and budget |
| P0 | Trigger × poison × contrasting clean data | Test non-monotonic safety backdoor with equal training compute |
| P0 | Independent evaluator × report rubric × blind human Gold | Check judge construct validity and circularity |
| P0 | Module reconfiguration × real side-effect oracle | Test composition guarantees beyond symbolic modules |
| P0 | Standard vs Realtime vs Privileged state | Quantify execution/resets/latency effects under controlled observation |
| P0 | Evidence graph × role edits × memory-policy edits | Identify SciMARS component effects and independent scientific Gold |
| P1 | Multi-user memory scope × privacy probes | Joint privacy and transfer payoff, independently labeled permissions |
| P1 | Goal revision × interruption × tool commitment | Measure obligations executed versus communicated |
| P1 | Local RSI loops vs unrepeatable global training | Report what causal contrast is actually feasible |

## Formal SIS Impact Decision
**MEASUREMENT_IDENTIFICATION_DELTA**, secondary **BENCHMARK_DELTA**. Real pressure on construct validity and causal identifiability, but all estimands expressible through SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG; scientific CoreDelta=0; SPEC_REVISION_CANDIDATE=NO. No T3 causal transport or T4 mechanism invariance verified.
