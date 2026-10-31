# SIS Daily Literature Update | 2026-11-01

**Authority:** `specs/System_Intelligence_Science_v0.3.1.md` (Core frozen), Registry v1.3, P0 Evidence Map and ClaimRecord schema. **Latest regular arXiv cs.AI batch:** Friday 2026-10-30, 605 total listed, 158 new submissions; no Saturday/Sunday regular arXiv batch. **Discovery:** three October EMNLP 2026 archival papers + seven arXiv preprints first submitted October 27–29. These are **delayed discoveries / newly indexed relevant studies**, not 2026-11-01 newly published work.

**Dedup:** exact official venue IDs and arXiv IDs checked against 145 permanent registry items plus 79 provisional items from Oct 24–31. Earlier unsynced Oct 9–23 studies not exhaustively reconciled; provisional `SIS-CAND` IDs only. Future preprint→venue matches should update StudyVersionRecord lineage, not create a second study.

**Evidence standard:** Primary author/ACL Anthology/arXiv abstracts checked; this is a **first-coder scope/ceiling**, not full supplemental reproduction. `CL2 candidate` is triage only, not final CL2. `ROUTING_ABSTAIN` means scientific primary-program routing abstention, not a fourth program. Community analyses are discovery-only.

**Decision:** `MEASUREMENT_IDENTIFICATION_DELTA` (secondary `BENCHMARK_DELTA`); `SPEC_REVISION_CANDIDATE=NO`, `CORE_DELTA_NONE`. Real pressure arises from authority/provenance transfer, hidden redundant safety, local recovery, measurement of exact scientific protocol comprehension and cost-conditioned stopping. Existing SCF, SDR, ASR, CSCI, BGT and replaceable framework capacities express all of them.

## Source-verified StudyVersionRecords and SIS first-coder coding

### SIS-CAND-20261101-01 — TraceProbe: An Execution-Based Benchmark for Diagnosing Safety Failures in LLM Agents

- **Primary source / version:** [EMNLP 2026 Main, October 2026, delayed discovery](https://aclanthology.org/2026.emnlp-main.1233/); **Reading:** Must Read.
- **Core idea / novelty:** 可执行沙盒中联结最终安全结果、潜在规则违规和步骤级运行重放，区分原计划风险与实际执行路径。
- **Reported empirical or formal evidence:** 155 scenarios, 3 risk-source classes, 12 models; reported mean attack success rate 0.347. EMNLP archival paper.
- **Evidence limitations, confounders, and claim ceiling:** 刻意构造的可执行风险分布不代表真实部署事故率；轨迹回放的诊断标签并非自动构成有因果识别力的修复实验。
- **SIS routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/ID/EG/MEAS/BT`; primary estimand `EXECUTABLE_TRACE_LATENT_VIOLATION_LOCALIZATION_VALIDITY`.
- **Claim maturity / identification / transport:** CL1; local replay-based CL2 candidate only for executed substitutions; I1/I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `NEGATIVE_DYNAMIC_VIABILITY_AND_MEASUREMENT`; classification: PEER_REVIEWED.
- **SIS impact:** 强化SDR故障轨迹与Viability测量；挑战仅依赖终态安全评分的实现假设。
- **Boundary variables:** 风险来源类别、内部权限妥协、执行路径、日志覆盖和违规规则有效性. **Transport:** 未提供跨真实部署的T3因果迁移.
- **Provenance note:** 正式会议论文；不可将ASR 0.347视为现实发生率.

### SIS-CAND-20261101-02 — Trust Cascade through Provenance Erasure: How Multi-Agent Delegation Breaks Single-Agent Safety

- **Primary source / version:** [EMNLP 2026 Main, October 2026, delayed discovery](https://aclanthology.org/2026.emnlp-main.1005/); **Reading:** Must Read.
- **Core idea / novelty:** 区分信息改写与委托通道权威变化，检测自然语言转交时来源、角色和授权元信息丢失。
- **Reported empirical or formal evidence:** 460 delegation pairs: 98% format markers, 100% authority entities and 44% attribution lost; 0% to 33–63% attack success in reported comparisons across eight open-weight models; TBA 86–100% conditional detection. EMNLP archive.
- **Evidence limitations, confounders, and claim ceiling:** 攻击条件和标记格式经过设计；局部通道对照不能自动确立跨模型/实际组织的完整因果传播；0% false positives是指定数据条件下结果。
- **SIS routing:** Primary `SDR`; Cross-cutting `CSCI/BGT`; Framework `TD/IA/EG/ID/MEAS/BT`; primary estimand `DELEGATION_PROVENANCE_ERASURE_AUTHORITY_ESCALATION_EFFECT`.
- **Claim maturity / identification / transport:** CL1; local controlled delegation/channel candidate CL2; I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `MECHANISM_CANDIDATE_AND_NEGATIVE_BOUNDARY`; classification: PEER_REVIEWED.
- **SIS impact:** 直接强化CSCI组件边界及EG来源权威的联动；不需新增原语。
- **Boundary variables:** 来源元数据保留、系统角色、委托通道、执行模型与攻击类型. **Transport:** T1多模型重复，不是T3.
- **Provenance note:** 与10月31日LogicInception不同Study，机制相近但不合并.

### SIS-CAND-20261101-03 — Tracing Error Propagation in Reasoning Language Models

- **Primary source / version:** [EMNLP 2026 Main, October 2026, delayed discovery](https://aclanthology.org/2026.emnlp-main.1559/); **Reading:** Worth Skimming.
- **Core idea / novelty:** 使用反事实重新采样区分可恢复与不可恢复推理轨迹，研究早期持续错误在终点内部表示的累积信号。
- **Reported empirical or formal evidence:** 官方EMNLP论文报告邻近步骤错误可预测，持续错误信号在末步表示上可分离并可回溯解码。
- **Evidence limitations, confounders, and claim ceiling:** 可解码特征不等于具有中介作用；重新采样条件改变后续路径，无法单独证明表示导致最终失败；需追踪真实修复结果。
- **SIS routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/ID/MEAS/BT`; primary estimand `PERSISTENT_REASONING_ERROR_RECOVERABILITY_SIGNAL_VALIDITY`.
- **Claim maturity / identification / transport:** CL1; counterfactual resampling local CL2 candidate; I1/I2-local/T0. No final CL2/CL3 promotion.
- **Evidence role:** `RECOVERY_BOUNDARY_AND_MEASUREMENT`; classification: PEER_REVIEWED.
- **SIS impact:** 细化SDR动态错误积累与恢复边界，属于已有TD/MEAS框架。
- **Boundary variables:** 模型层、错误持续时间、采样策略、任务类型、可恢复阈值. **Transport:** 没有T3/T4机制迁移证明.
- **Provenance note:** 正式EMNLP，不等同于2026-11-01新发表.

### SIS-CAND-20261101-04 — Masked Erosion: How Acceptance Gates Lose Redundant Safeguards in Self-Improving Agents

- **Primary source / version:** [arXiv:2610.38392v1, first submitted 2026-10-28, preprint](https://arxiv.org/abs/2610.38392); **Reading:** Must Read.
- **Core idea / novelty:** 强调性能准入Gate在多重防护冗余时看不到单层防护价值，进而允许自改进过程逐层侵蚀安全冗余。
- **Reported empirical or formal evidence:** four safeguards subset tests; 411 improvement loops over 10 gate rules in two environments; 20-task batches retained all protections whereas matched-cost 40-task batches lost all six tested harnesses' depth; GEPA 2/3 weaker-model executions misused credentials.
- **Evidence limitations, confounders, and claim ceiling:** 合成删改和特定Gate预算设计；弱模型替换是边界测试，不能推出普遍失效比例；门槛成本、抽样与筛选耦合。
- **SIS routing:** Primary `ASR`; Cross-cutting `CSCI/BGT`; Framework `DR/TD/EG/ID/MEAS/BT`; primary estimand `REDUNDANT_SAFEGUARD_DELETION_ACCEPTANCE_GATE_MASKING_EFFECT`.
- **Claim maturity / identification / transport:** CL1; controlled safeguard deletion CL2 candidate; I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `NEGATIVE_REGULATION_BOUNDARY_AND_MECHANISM_CANDIDATE`; classification: PREPRINT.
- **SIS impact:** 对ASR更新准入和CSCI能力依赖提出真实的测量压力；科学对象已存在。
- **Boundary variables:** 防护冗余、测试批次、审核预算、基础模型更换、门槛统计策略. **Transport:** T1受控运行，非真实部署T3.
- **Provenance note:** 不把保留文字等价于保留安全功能.

### SIS-CAND-20261101-05 — DynaRev: Benchmarking Web Agents under Dynamic Goal Revision

- **Primary source / version:** [arXiv:2610.40133v1, first submitted 2026-10-29, preprint](https://arxiv.org/abs/2610.40133); **Reading:** Must Read.
- **Core idea / novelty:** 在执行中语义里程碑时刻更改目标，分别评价新增要求、无条件覆盖和依赖运行状态的覆盖。
- **Reported empirical or formal evidence:** 181 tasks, five models; revision correctness, responsiveness and efficiency separated; instruction rewrite with retained browser state sometimes helps, browser reset harms.
- **Evidence limitations, confounders, and claim ceiling:** 修改任务在基准场景中受控；动态到达时机及任务源差异混杂；尚无真实多轮用户交互迁移结果。
- **SIS routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/DR/MI/ID/MEAS/BT`; primary estimand `SEMANTIC_MILESTONE_GOAL_REVISION_ADAPTATION_EFFECT`.
- **Claim maturity / identification / transport:** CL1; local revision/reset ablations need audit; I1/I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `DYNAMIC_GOAL_BOUNDARY_AND_BENCHMARK`; classification: PREPRINT.
- **SIS impact:** 强化SDR任务意图状态变化和ASR恢复策略的分离。
- **Boundary variables:** 修订类型、交付时机、浏览器状态是否保持、任务源与预算. **Transport:** T1场景和模型，不构成T3.
- **Provenance note:** 与SWE-Shift(环境变化)不同，研究对象是用户目标变更.

### SIS-CAND-20261101-06 — MemSteer: Turning User Histories into Supervision for Agent Memory Optimization

- **Primary source / version:** [arXiv:2610.39276v1, first submitted 2026-10-29, preprint](https://arxiv.org/abs/2610.39276); **Reading:** Must Read.
- **Core idea / novelty:** 从无标签历史自动建立证据支持的问答监督，通过盲答重建和来源检查生成优化器信号，调整存储、检索和上下文构造而不更新模型权重。
- **Reported empirical or formal evidence:** ATM-Bench Question Score relative BM25 +13.4 points; RHELM accuracy +4.1/+6.6 points without/with external data; tests on additional optimizers and new-user history.
- **Evidence limitations, confounders, and claim ceiling:** 生成Gold与优化器共享来源及审查策略可能造成自我确认；QA分数不等于真实长期决策价值；多机制同时变化。
- **SIS routing:** Primary `ASR`; Cross-cutting `CSCI/BGT`; Framework `DR/MI/EG/ID/MEAS/BT`; primary estimand `EVIDENCE_GROUNDED_SYNTHETIC_MEMORY_SUPERVISION_OPTIMIZATION_VALUE`.
- **Claim maturity / identification / transport:** CL1; local supervision-policy contrast candidate; I1/T1 (new-user results exploratory T2 performance). No final CL2/CL3 promotion.
- **Evidence role:** `OPTIMIZER_POLICY_AND_EVIDENCE_GOVERNANCE`; classification: PREPRINT.
- **SIS impact:** 强化ASR选择性调节与EG来源监督，要求独立封闭Gold。
- **Boundary variables:** 用户历史分布、来源质量、合成问答泄漏、外部数据可见性、检索预算. **Transport:** 仅性能层的有限新用户验证.
- **Provenance note:** 不要将合成监督当成人类专家金标准.

### SIS-CAND-20261101-07 — Detecting Covert Collusion between AI Agents through Partner-Outsider Positive Listening

- **Primary source / version:** [arXiv:2610.37849v1, first submitted 2026-10-27, work in progress preprint](https://arxiv.org/abs/2610.37849); **Reading:** Worth Skimming.
- **Core idea / novelty:** 把消息含义保持的改写对合作者与局外者的行为影响差定义为潜在私有通信检测量。
- **Reported empirical or formal evidence:** simulated five-condition market; encoded-channel conditions PoPLi 0.48–0.59 with reported positive intervals, no-code -0.10– -0.01; message-only monitors failed tested comparisons.
- **Evidence limitations, confounders, and claim ceiling:** 单一模拟市场与特定首字母编码；检测的是私密信道使用，不是合谋本身；意义携带的协议和纯激励合谋可能漏检。
- **SIS routing:** Primary `SDR`; Cross-cutting `CSCI/BGT`; Framework `IA/TD/ID/MEAS/BT`; primary estimand `PARTNER_OUTSIDER_PARAPHRASE_DIFFERENTIAL_CHANNEL_USE`.
- **Claim maturity / identification / transport:** CL1; local controlled wording perturbation candidate; I2-local/T0. No final CL2/CL3 promotion.
- **Evidence role:** `MEASUREMENT_INSTRUMENT_AND_NEGATIVE_BOUNDARY`; classification: PREPRINT.
- **SIS impact:** 加强CSCI信息交互测量与TD传播边界，不能形成普遍安全机制结论。
- **Boundary variables:** 编码通道、意义保持重写、伙伴/局外者能力、激励结构. **Transport:** T0单环境.
- **Provenance note:** work in progress，不进行机制CL2晋升.

### SIS-CAND-20261101-08 — Evaluating and improving AI agents for sequencing protocol understanding / LibStructBench

- **Primary source / version:** [arXiv:2610.37851v1, first submitted 2026-10-27, preprint](https://arxiv.org/abs/2610.37851); **Reading:** Must Read.
- **Core idea / novelty:** 以测序文库分子状态与实验流程连通性为独立真值，测量科学协议阅读器是否准确重建结构，而不只给出近似自然语言描述。
- **Reported empirical or formal evidence:** frontier agents often approximate but miss exact structures; model switches show larger mean differences than harness switches, statistically significant only for molecular state reconstruction; added knowledge pilot improves oligo family, not mean workflow; autonomous rules show no mean heldout gain.
- **Evidence limitations, confounders, and claim ceiling:** 协议文献/Gold覆盖和专家裁决定义有限；小样本知识增强及优化轨迹不能证明一般归纳规律；跨实验类型需迁移检验。
- **SIS routing:** Primary `SCF`; Cross-cutting `CSCI/BGT`; Framework `MI/TD/ID/MEAS/BT`; primary estimand `BIOPROTOCOL_EXACT_MOLECULAR_STATE_WORKFLOW_RECONSTRUCTION`.
- **Claim maturity / identification / transport:** CL1; controlled model/harness contrasts need full audit; I1/I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `NEGATIVE_SCIENTIFIC_CAPABILITY_AND_BENCHMARK`; classification: PREPRINT.
- **SIS impact:** 对生物医学SIS测量、CRISPR及NutriFoundation科学任务规范有直接价值；挑战近似回答即科学理解的假设。
- **Boundary variables:** 分子状态精度、连接拓扑、协议复杂度、模型能力、外部知识与正交效应. **Transport:** T1局部生物实验领域.
- **Provenance note:** 读后不把小型Pilot视为统计确定的机制效应.

### SIS-CAND-20261101-09 — ThinkJev: One Thought, Every Budget for Calibrated Typed Decisions

- **Primary source / version:** [arXiv:2610.37732v1, first submitted 2026-10-27, preprint](https://arxiv.org/abs/2610.37732); **Reading:** Must Read.
- **Core idea / novelty:** 用同一模型共享缓存将快速分类决策与逐步推理的概率输出放在同一选项空间，控制何时升级和何时停止。
- **Reported empirical or formal evidence:** Qwen3.5-27B at 5% dev-calibrated target: 24.5% of 8,359 held-out decisions fast path, realized 3.9% error; remaining thought stopping 81.6% vs always think 82.7%, using 72% tokens.
- **Evidence limitations, confounders, and claim ceiling:** 开发集校准前提、离散选项任务与分布变化限制；5%目标只是受控条件下的风险控制，非域外保证；尾部错误、真实成本尚需评价。
- **SIS routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `DR/ID/MEAS/BT`; primary estimand `CONFIDENCE_CONDITIONAL_REASONING_ESCALATION_AND_STOPPING_NET_VALUE`.
- **Claim maturity / identification / transport:** CL1; local budget contrast candidate; I1/I2-local/T1. No final CL2/CL3 promotion.
- **Evidence role:** `ADAPTIVE_REGULATION_BOUNDARY`; classification: PREPRINT.
- **SIS impact:** 加强ASR停止策略和验证成本测量，现有框架足够。
- **Boundary variables:** 基础模型能力、目标误差阈值、类别概率校准、任务分布、token与延迟成本. **Transport:** T1多任务，不支持T3.
- **Provenance note:** 准确率差不等于证明非劣效性.

### SIS-CAND-20261101-10 — WebAnything: From the Wild Web to Scalable Agent Environments

- **Primary source / version:** [arXiv:2610.37786v1, first submitted 2026-10-27, preprint](https://arxiv.org/abs/2610.37786); **Reading:** Worth Skimming.
- **Core idea / novelty:** 从真实网站构造可重置、可执行的环境镜像，冻结候选由独立验证器检查并局部修复，提高训练环境覆盖。
- **Reported empirical or formal evidence:** 244 reconstructed site artifacts, 14 domains, 53 categories, 12,984 accepted tasks; blind fidelity comparison reported 12 wins, 2 ties; fixed harness fine-tuned model improved REAL +9.9 pp and WebArena +13.33 pp.
- **Evidence limitations, confounders, and claim ceiling:** 环境冻结镜像与真实持续变化网站存在差异；构造、验证、训练和数据多样性同时变化；环境质量优于基准不意味因果迁移可推广。
- **SIS routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/TD/EG/ID/MEAS/BT`; primary estimand `SOURCE_GROUNDED_RECONSTRUCTED_WEB_ENVIRONMENT_FIDELITY_AND_TRAINING_VALUE`.
- **Claim maturity / identification / transport:** CL1; local independent verifier contrast candidate; I1/T2-performance-only. No final CL2/CL3 promotion.
- **Evidence role:** `REPLACEABLE_BENCHMARK_ENVIRONMENT_IMPLEMENTATION`; classification: PREPRINT.
- **SIS impact:** 丰富SCF训练环境与BGT性能迁移实验，实施技术而非SIS原语。
- **Boundary variables:** 网站类别、交互覆盖、镜像保真度、权限可用性、行为漂移和训练预算. **Transport:** T2仅为训练模型的测试性能迁移.
- **Provenance note:** 不得用模拟成功自动代替真实部署效果.

## Synthesis, scientific impact and concrete benchmark updates

1. **Authority provenance becomes a dynamical variable:** delegation loses source trust; require information/authority preservation across components, fixed-content control, and downstream outcome checks.
2. **Optimizer admission can erase redundancy:** task success and harm-at-current-model are insufficient to certify defense-in-depth or capability retention under model replacement.
3. **Correct behavior under changing goals is not static task success:** milestone-defined user revisions and dynamic state retention require paired trajectory metrics and recovery budgets.
4. **Evidence-based synthetic supervision remains self-confirmation prone:** memory optimization needs independent QA/answer Gold, temporal source freshness, blinded recovery, and sealed test users.
5. **Domain scientific comprehension and stopping are conditional:** exact molecular protocol state/connectivity and confidence-conditional cost/accuracy must be measured separately from fluent answers, approximate structure, and mean token savings.

| Priority | Fixture | Independent measurement and contrast |
|---|---|---|
| P0 | Delegation Provenance × Role/Channel | original vs rephrased payload, metadata survival, unauthorized effect, do(delegate) |
| P0 | Redundant Safeguard × Acceptance Gate × Model Swap | task score, depth loss, violation after single safeguard failure; full search and audit costs |
| P0 | Dynamic Goal Revision × Browser State | same prefix, milestone-timed revision, responsiveness, previous side-effect reversal |
| P0 | Synthetic Memory QA × Independent Sealed Gold | generated evidence-plan validity, independent expert/heldout QA, memory-policy net value |
| P0 | Biological Protocol State × Workflow Connectivity | exact molecule reconstruction vs approximation, model × harness interaction, external expert Gold |
| P0 | Reasoning Escalation × Error Bound × Cost | conditional coverage, achieved risk, tail failures, token+latency cost across shifts |
| P1 | Replayed Covert Channel × Outsider Control | channel detection vs behavioral collusion, semantic rephrases, false positives |
| P1 | Source-Grounded Web Mirror × Live Site | replay fidelity, failure regimes, training-to-live transport |
| P1 | Persistent Error Signal × Real Repair | decodability vs causal state replacement/recovery |

**P0 audit advancement:** see [SIS_P0_Reaudit_2026-11-01.md](../evidence-map/audits/SIS_P0_Reaudit_2026-11-01.md) for 126,130,131 and nine claim decisions (first coder only).

**Formal SIS Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA`, secondary `BENCHMARK_DELTA`, `SPEC_REVISION_CANDIDATE=NO`. This is genuine pressure on identification/measurement but still a **framework/benchmark delta within frozen scientific semantics**, not evidence of a new non-replaceable capability.
