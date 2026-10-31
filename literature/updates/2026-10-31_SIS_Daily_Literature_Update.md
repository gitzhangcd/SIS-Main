# SIS Daily Literature Update | 2026-10-31

**Authority:** `specs/System_Intelligence_Science_v0.3.1.md` (Scientific Core frozen), Registry v1.3, current P0 Queue and previous 2026-10-30 audit. 
**Source window:** latest arXiv cs.AI public list Friday 2026-10-30: 605 listed, 158 new submissions; primary study initial postings 2026-10-27–29. EMNLP archival item is an October 2026 publication discovered in this run, not newly published on Oct 31.
**Dedup:** checked source URLs against 145 permanent records and 69 Oct 24–30 provisionals; Oct 9–23 unsynced history still requires global lineage reconciliation. Provisional IDs only, no permanent SIS-LIT allocations.
**Coding:** first-coder paper-level ceiling NOT final ClaimRecord judgment; no inherited CL2/CL3, no demonstrated T3/T4, no second coder adjudication.
**Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA` (secondary `BENCHMARK_DELTA`); `CORE_DELTA_NONE`, `SPEC_REVISION_CANDIDATE=NO`. Real pressure on source-governed evaluation, experimental design and bounded measurement, fully expressible in existing programs/frameworks.
**Community/technical analyses:** discovery-only; no independent reproduction evidence admitted.

## StudyVersionRecords and first-coder SIS coding

### SIS-CAND-20261031-01 — LogicInception: Discourse-Level Indirect Prompt Injection via Causal Chain Construction

- **Primary version:** [EMNLP 2026 Main; archival October 2026, delayed discovery](https://aclanthology.org/2026.emnlp-main.1831/). **Reading priority:** Must Read.
- **Core idea/novelty:** 不含显式命令的跨工具输出叙述片段，通过虚构因果依赖被模型合成为错误授权行动；高推理能力未必减少风险.
- **Reported evidence / quality:** 1,139 scenarios, five defenses; author reports 42.9–48.8% attack success, 88% per-fragment stealth, baseline composite success below 8%; official peer-reviewed anthology record.
- **Limitations, confounders & identification:** 构造攻击分布与具体防御机制；攻击成功不能推导真实生产发生率；相关能力-风险趋势不等于能力提升直接导致风险.
- **SIS routing:** Primary `SDR`; Cross `CSCI/BGT`; Framework `TD/IA/EG/ID/MEAS/BT`; estimand `DISCOURSE_CAUSAL_CHAIN_UNAUTHORIZED_ACTION_EFFECT`.
- **Evidence role / claim ceiling:** `NEGATIVE_VIABILITY_BOUNDARY`; CL1; local CL2 candidate (not adjudicated); identification/transport I1/I2-local/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 强烈细化SDR/CSCI的信息传播和权威推断边界；不触发Core修订.
- **Boundary variables / transport gaps:** 片段可见性、虚构因果链、组件推理能力、工具执行权限、监督规则.

### SIS-CAND-20261031-02 — What Does an Ontology Catch? Curated, LLM-Generated and Data-Derived Ontologies as Checkers of LLM Agents over Knowledge Graphs

- **Primary version:** [arXiv:2610.37809v1; first submitted 2026-10-27; preprint under review](https://arxiv.org/abs/2610.37809). **Reading priority:** Must Read.
- **Core idea/novelty:** 检验本体作为自动裁判是否真的可靠，比较手工本体、模型生成本体和数据派生本体.
- **Reported evidence / quality:** 跨公共图谱及接近10^9三元组私有图谱；UniProt手工本体在真实正确回答上产生更多误报，其真实回答标记精度仅略好于随机标记.
- **Limitations, confounders & identification:** 不同图谱本体/数据不一致；局部Gold和模型配置限制；检查精度差不等于本体永远无效.
- **SIS routing:** Primary `ROUTING_ABSTAIN`; Cross `BGT`; Framework `EG/MEAS/ID/BT`; estimand `ONTOLOGY_CHECKER_FALSE_FLAG_DECISION_VALIDITY`.
- **Evidence role / claim ceiling:** `NEGATIVE_MEASUREMENT_BOUNDARY`; CL1; no causal mechanism promotion; identification/transport I1/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 挑战本体检查天然可靠的实施假设，支持EG/MEAS的独立评价，不新增Primitive.
- **Boundary variables / transport gaps:** 本体版本、数据schema漂移、误报成本、图谱类型与缺陷覆盖.

### SIS-CAND-20261031-03 — Measuring Where Intent Gets Lost in Agentic Smart Contract Synthesis

- **Primary version:** [arXiv:2610.37830v1; first submitted 2026-10-27; preprint (2027 conference note not peer review)](https://arxiv.org/abs/2610.37830). **Reading priority:** Must Read.
- **Core idea/novelty:** 对同一交易在生成合约和独立答案键上实际执行，先澄清缺失需求再编码，而不是事后补丁.
- **Reported evidence / quality:** 600 tasks，三模型；作者报告常见评价器遗漏明显错误，仅检查共有函数会隐藏约一半流水线差异；前置澄清较事后修补更有价值.
- **Limitations, confounders & identification:** 答案键/执行评分依赖合约覆盖；澄清提问、规范补全和实现质量共同变化；不可直接泛化到开放式软件.
- **SIS routing:** Primary `SCF`; Cross `BGT`; Framework `MI/EG/MEAS/ID/BT`; estimand `PREGENERATION_ELICITATION_VS_POSTHOC_REPAIR_INTENT_CONFORMANCE`.
- **Evidence role / claim ceiling:** `SPECIFICATION_BOUNDARY_AND_MECHANISM_CANDIDATE`; CL1; local CL2 candidate; identification/transport I2-local/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 加强任务规范完整性与行为符合性分离，SCF/MEAS已可表达.
- **Boundary variables / transport gaps:** 未表达需求、不可逆外部作用、独立执行Oracle完整性.

### SIS-CAND-20261031-04 — OpenFrontiers: A Collection of Open Research Problems and a Benchmark for Scientific Rediscovery

- **Primary version:** [arXiv:2610.37739v1; first submitted 2026-10-27; preprint](https://arxiv.org/abs/2610.37739). **Reading priority:** Must Read.
- **Core idea/novelty:** 区分真正独立重新发现数学结论与检索已公开解答，通过封闭、冻结检索及开放网络制度评价.
- **Reported evidence / quality:** 12,151个研究问题记录；200问题中110项2026已解决、90项未解决；HQ-50含形式化Lean4和独立检查；七个系统下封闭测试最多解决40项已解题中的7项.
- **Limitations, confounders & identification:** 开放网络成功多为检索，形式化数学问题不等同全部科学发现；未来污染与问题筛选影响可解释性.
- **SIS routing:** Primary `ROUTING_ABSTAIN`; Cross `BGT`; Framework `MEAS/EG/ID/BT`; estimand `CLOSED_BOOK_REDISCOVERY_VS_SOLUTION_RETRIEVAL_VALIDITY`.
- **Evidence role / claim ceiling:** `MEASUREMENT_INSTRUMENT_AND_LEAKAGE_BOUNDARY`; CL1 measurement; no mechanism CL2; identification/transport I1/T0. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 直接加强研究能力测量与Evidence Independence，不触发Core.
- **Boundary variables / transport gaps:** 模型知识截止、检索制度、问题解答公开时间、独立形式化验证.

### SIS-CAND-20261031-05 — SciGame: Let Agents Play the Scientific Discovery Games in the Real and Counterfactual World

- **Primary version:** [arXiv:2610.37919v1; first submitted 2026-10-27; preprint](https://arxiv.org/abs/2610.37919). **Reading priority:** Must Read.
- **Core idea/novelty:** 文献科学定律构建原世界和量纲一致的反事实世界，分离预训练先验、固定证据与主动实验.
- **Reported evidence / quality:** 五种前沿模型；作者发现熟悉定律的先验在关系被修改后反而妨碍推断，主动实验帮助强模型但在有限预算下损害弱模型，正确解释未必意味着正确符号定律.
- **Limitations, confounders & identification:** 生成的反事实环境及可用实验动作有限；无法自动得出跨科学领域机制不变性.
- **SIS routing:** Primary `ASR`; Cross `BGT`; Framework `DR/ID/MEAS/BT`; estimand `COUNTERFACTUAL_LAW_DISCOVERY_ADAPTIVE_EXPERIMENT_NET_VALUE`.
- **Evidence role / claim ceiling:** `COUNTERFACTUAL_BOUNDARY_AND_NEGATIVE_RESULT`; CL1; intervention candidate subject to full controls; identification/transport I1/I2-local/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 强化ASR的信息获取净价值及CSCI候选边界，现有框架足够.
- **Boundary variables / transport gaps:** 原/反事实定律、模型能力、实验预算、精确形式恢复与时间泄漏.

### SIS-CAND-20261031-06 — Prefix Executability: Evaluating Tool-Using Agents Beyond Final Success

- **Primary version:** [arXiv:2610.40444v1; first submitted 2026-10-29; NeurIPS acceptance author-declared; archive not independently linked](https://arxiv.org/abs/2610.40444). **Reading priority:** Must Read.
- **Core idea/novelty:** 评价每个工具调用前缀是否满足schema、状态前置条件和数据依赖，而非仅看最终任务成功.
- **Reported evidence / quality:** BFCL-v3、ToolSandbox及tau^3-bench；提出PEC/FED/TER/AUC-PEC/RR；带未验证计划的系统可有更高终局成功但显著更低轨迹可执行性.
- **Limitations, confounders & identification:** 工具状态契约必须正确完整；部分任务采用采样，不能把通过前缀验证视为现实世界全部约束满足.
- **SIS routing:** Primary `SDR`; Cross `BGT`; Framework `TD/MEAS/ID/BT`; estimand `PREFIX_EXECUTABILITY_CONDITIONAL_TERMINAL_SUCCESS_GAP`.
- **Evidence role / claim ceiling:** `TRAJECTORY_MEASUREMENT_AND_RECOVERY_BOUNDARY`; CL1; local plan-checking contrast CL2 candidate; identification/transport I1/I2-local/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 深化SDR可执行轨迹测量，不构成新Primary Program.
- **Boundary variables / transport gaps:** 轨迹长度、计划检查、schema完整性、恢复语义.

### SIS-CAND-20261031-07 — Efficient Scalable Oversight via Rewinding

- **Primary version:** [arXiv:2610.40535v1; first submitted 2026-10-29; preprint](https://arxiv.org/abs/2610.40535). **Reading priority:** Must Read.
- **Core idea/novelty:** 可重置证明者状态的交互验证，使较弱验证器无需假定至少一个证明者诚实，并提高特定计算类别的验证效率.
- **Reported evidence / quality:** 给出依赖oracle答案小比例扰动稳健性的条件性理论；诚实证明者线性开销、验证近输入长度线性；初步MNIST原型.
- **Limitations, confounders & identification:** 要求可信快照/回退控制、可重放状态和计算的稳健性条件；MNIST不能支持生产LLM监管有效性.
- **SIS routing:** Primary `ROUTING_ABSTAIN`; Cross `BGT`; Framework `EG/ID/MEAS/BT`; estimand `REWINDABLE_VERIFICATION_SOUNDNESS_AND_COST_UNDER_ORACLE_ROBUSTNESS`.
- **Evidence role / claim ceiling:** `FORMAL_IDENTIFICATION_INSTRUMENT`; CL0 conditional theorem; CL1 preliminary prototype; identification/transport I0/I1/T0. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 细化可替换EG Framework的理论实现，无Core压力.
- **Boundary variables / transport gaps:** rewind控制权、状态一致性、oracle扰动稳健性、验证成本.

### SIS-CAND-20261031-08 — PCM: A Proof-Carrying Message Protocol for Verifiable Multi-Agent Communication

- **Primary version:** [arXiv:2610.39109v1; first submitted 2026-10-29; preprint cross-listed cs.AI](https://arxiv.org/abs/2610.39109). **Reading priority:** Must Read.
- **Core idea/novelty:** 代理间每个事实或授权声明都携带来自代理不可写的追加Merkle日志证据，接收方三值验证.
- **Reported evidence / quality:** 预设926条消息测试含712条谎言；接受10条陈旧证据谎言，两个独立验证器926条判断一致，验证约1ms.
- **Limitations, confounders & identification:** 不可信根签名者、错误授权源和陈旧证据仍可能通过；形式化安全仅适用明确证明前提.
- **SIS routing:** Primary `ROUTING_ABSTAIN`; Cross `BGT`; Framework `EG/MI/ID/MEAS/BT`; estimand `SIGNED_INDEPENDENT_EVIDENCE_MESSAGE_AUTHORITY_VALIDITY`.
- **Evidence role / claim ceiling:** `EVIDENCE_GOVERNANCE_IMPLEMENTATION_AND_NEGATIVE_BOUNDARY`; CL0 conditional security proof + CL1 benchmark; identification/transport I0/I1/T0. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 加强claim-evidence-authority separation；有明显stale-evidence失效边界，不新增Primitive.
- **Boundary variables / transport gaps:** 签名者可信性、日志不可变性、证据时效、授权链收缩规则.

### SIS-CAND-20261031-09 — Disparity Laundering: Consensus Without Fairness in Clinical Multi-Agent Systems

- **Primary version:** [arXiv:2610.38215v1; first submitted 2026-10-28; preprint; EACL 2027 noted but not peer reviewed archive](https://arxiv.org/abs/2610.38215). **Reading priority:** Must Read.
- **Core idea/novelty:** 模型家族与协作拓扑的全因子比较，显示多组件协商可能保留甚至放大既有临床差异；把反事实观点合并进最终决策可以部分缓解.
- **Reported evidence / quality:** 5模型家族×4拓扑×120真实MIMIC-IV急诊病例，人口统计反事实替换；20组合均未消除方向性差异；全轮合并多视角时作者报告差异降低67–94%.
- **Limitations, confounders & identification:** 反事实改写及标注情境不等同真实临床分诊；模型与拓扑交互，不能推广种族效应大小至患者；独立医生裁决仍需要.
- **SIS routing:** Primary `SCF`; Cross `CSCI/BGT`; Framework `IA/ID/MEAS/BT`; estimand `TOPOLOGY_BY_MODEL_COMMITTED_CLINICAL_DECISION_DISPARITY`.
- **Evidence role / claim ceiling:** `NEGATIVE_CSCI_VIABILITY_BOUNDARY`; CL1; local demographic-swap and pooling CL2 candidate; identification/transport I2-local/T1. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 强化CSCI的系统级可行性测量；模型层评估不能自动代表组合系统.
- **Boundary variables / transport gaps:** 模型家族、协作拓扑、反事实人口属性、决策聚合、临床样本分布.

### SIS-CAND-20261031-10 — Beyond fabrication: Misattributed numbers in papers written by AI research agents

- **Primary version:** [arXiv:2610.38691v1; first submitted 2026-10-28; preprint](https://arxiv.org/abs/2610.38691). **Reading priority:** Must Read.
- **Core idea/novelty:** 科学论文中的数字真实存在于文件中，但可能来自错误实验、指标或运行轮次；提出确定性上下文绑定验证.
- **Reported evidence / quality:** 复核540个既有判断并人工标注18份提交中的256个数字Claim；约五分之四不受支持的Claim引用了错误上下文中的真实数值；盲评对85个可验证项确认78个，kappa 0.89.
- **Limitations, confounders & identification:** 能验证的仅为子集；不通过验证不意味着不真实；不同厂商Judge通过率相差大，无法自动判定主观科学贡献.
- **SIS routing:** Primary `ROUTING_ABSTAIN`; Cross `BGT`; Framework `EG/MEAS/ID/BT`; estimand `NUMERIC_CLAIM_TO_EXPERIMENT_METRIC_RUN_PROVENANCE_VALIDITY`.
- **Evidence role / claim ceiling:** `NEGATIVE_CLAIM_PROVENANCE_AND_MEASUREMENT_INSTRUMENT`; CL1 measurement; no causal promotion; identification/transport I1/T0. StudyVersionRecord is not a finalized claim.
- **SIS relationship:** 直接强化SIS ClaimRecord与Evidence Map的run-metric-source provenance；无Scientific Core修订.
- **Boundary variables / transport gaps:** 记录粒度、指标名称、实验轮次、数值诱饵、盲评覆盖.

## Synthesis and proposed experimental deltas

1. **Evaluation validity**: compare ontology checkers, executable specification satisfaction, and claim-to-run provenance using independent Gold and false-positive/false-negative costs.
2. **Scientific ability construct**: sealed closed-book vs frozen retrieval vs live-web; original vs counterfactual scientific laws; record exact symbolic correctness, not only explanation fluency.
3. **System dynamics**: prefix executability with first-error depth, recovery and final outcome kept as separate targets.
4. **Governance**: evidence-signature freshness, communication authority and rewindable oversight require explicit trusted control and evidence source assumptions.
5. **CSCI/viability**: fully crossed model capability × organizational topology × independent system-level outcome. No claim of causal transport based only on 2026 domain experiments.

| Priority | Fixture | Measurement/identification target |
|---|---|---|
| P0 | Ontology Source × Independent Answer Gold | false flags, missed errors, checker net value |
| P0 | Elicitation × Complete Executable Requirement Gold | pre-generation vs after-the-fact repair effect |
| P0 | Prior-Only × Frozen Retrieval × Live Web | genuine scientific rediscovery vs source retrieval |
| P0 | Original Law × Counterfactual Law × Model Capability | adaptive experimental value under prior conflict |
| P0 | Prefix Executability × Terminal Success | executable trajectory, recovery and invalidity depth |
| P0 | Signed Evidence × Stale Record | claim/provenance/authorization freshness |
| P0 | Model Family × Organization Topology × Clinical Gold | committed-decision disparities, calibration, resource match |
| P0 | Numerical Claim × Run/Metric/Source Ledger | traceability, blinded accuracy, noncoverage and decoys |
| P1 | Rewind Control × Oracle Robustness | conditional soundness/cost, not real-world deployment proof |

**Formal:** Primary=`MEASUREMENT_IDENTIFICATION_DELTA`; Secondary=`BENCHMARK_DELTA`; Scientific Core remains frozen. These are genuine experimental/identification demands and framework fillings, not an uncovered nonreplaceable scientific capability.
