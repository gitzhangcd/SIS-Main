# SIS Daily Literature Update｜2026-11-17

**Authority:** `specs/System_Intelligence_Science_v0.3.1.md`; current Registry v1.3; P0 Audit Queue, ClaimRecord schema, P0 Map. Read before screening. **Previous run:** 2026-11-16; previous head d8f00f0cfbbfef5ca719cafd980407cd246cd4a4.

## Discovery and date provenance
- arXiv official `https://arxiv.org/list/cs.AI/new` for **Monday, November 16, 2026**: 276 total (82 new cs.AI, remainder cross-listed or revised); this announcement is distinct from preprint submission date. Ten selected arXiv v1 studies submitted November 12–13, not November 17 first publications.
- Additional source channels sampled: OpenReview, ACL Anthology / AACL / EMNLP / NeurIPS proceedings, author pages and discovery-only technical analyses. No independently confirmed *new peer-reviewed archival item* displaced these 10 studies in the evidence-weighted selection; author-declared workshop status is not automatic peer-reviewed status.
- Excluded `arXiv:2611.17338` from this day's admitted candidates because its official page currently reports an incongruent **2026-08-30 submission date** for a `2611` identifier, despite inclusion in the Monday listing; needs metadata reconciliation before promotion. DO NOT count as verified new study.
- Dedup checked against current Registry's full historical text by identifier. No duplicate new StudyVersionRecord; all new candidates remain `SIS-CAND-20261117-xx`. Historic candidates and preprint→proceedings global audit remain open.

## Executive scientific inference
**Observed probe accuracy ≠ mechanistic mediation; evaluation-suite average ≠ defect sensitivity; simulated response support ≠ patient treatment effect; external scientific certification ≠ independent AI scientific contribution.** Strongest studies sharpen *identification and construct-validity conditions* without revealing a fourth SIS Primary Program. This is real pressure on operationalized scientific measurement, not a normative Scientific Core delta.

## Peer-reviewed conference / journal studies
No new individually confirmed, independently nonduplicate peer-reviewed paper selected this run. An accepted workshop comment alone was not used to upgrade a preprint.

## Primary-source preprints: 10 selected studies
### 1. [Can Mechanistic Interpretability Help Explain LLM Agent Failures? A Case Study on Web Element Hallucination](https://arxiv.org/abs/2611.18514) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** Qwen2.5-7B网页行动幻觉：末Token线性探针预测AUC 0.80；方向操纵纠正85%幻觉同时破坏7%合法动作。微小行动表示格式变化使操纵效果大幅降低。
**Evidence/limits:** 模型内干预与格式负控制比纯归因标签更强；但探针方向可能包含多种共变特征，电路分布在多个位置；纠错比例非系统全局收益。
**SIS:** Primary `SDR`, cross `BGT`, Framework `MI/TD/ID/MEAS/BT`, estimand `WEB_AGENT_ELEMENT_HALLUCINATION_PROBE_STEERING_FORMAT_BOUNDARY`; provisional maturity CL1; local CL2 candidate (steering effect only); identification I2-local / I1 for pathway; transport T0; role MECHANISM_CANDIDATE / NEGATIVE_BOUNDARY; boundary 动作Schema/页面可用元素、提示格式、层位、steering强度、合法行动基率、模型家族.
**Impact:** SHARPENS：可解码、可操纵和已识别中介不同；格式脆弱性限制机制不变性。 **Kill test:** Matched website × steering/random-direction × representation perturbation × executed action side-effects.

### 2. [Generated Evaluation Suites as Diversity-Driven Search for Real Agent Regressions](https://arxiv.org/abs/2611.17632) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 在τ²-bench两领域注入7种受控缺陷，证明低覆盖格子对全局均值检测阈值存在数学上界；4/5可追踪缺陷的最大影响不超过0.10阈值。
**Evidence/limits:** 真实注入真值与每格计分帮助识别隐藏回归；总体平均分甚至反向变化。仅两领域七种注入，需检查标签和覆盖定义；Workshop接收声明并非独立正式论文集证据。
**SIS:** Primary `ROUTING_ABSTAIN`, cross `BGT`, Framework `MEAS/ID/EG/BT`, estimand `EVALUATION_SUITE_CELL_COVERAGE_DETECTABLE_REGRESSION_LIMIT`; provisional maturity CL1 empirical / CL0 mathematical ceiling; identification I2-local fault injection; transport T0; role MEASUREMENT_NEGATIVE / BOUNDARY; boundary 测试格子设计、缺陷覆盖率b/N、故障行为可追踪性、阈值、基线成功率、随机生成预算.
**Impact:** SHARPENS：Benchmark失败不一定是系统没有故障，可能是检测设计理论上无力。 **Kill test:** Known fault injection × cell-wise coverage × mean-pass-rate threshold × independent execution oracle.

### 3. [ModHarness-RL: Recasting Harnesses as Learnable and Evolving Programs for Agentic RL](https://arxiv.org/abs/2611.18533) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 将历史压缩和轨迹纠偏定义为Typed State上的可学习程序，随RL模型训练动态演化；CodeSearch、ALFWorld、BIRD SQL和1.5B–8B模型中报告大多数设置优于固定Harness。
**Evidence/limits:** 含执行验证和历史重放；但模型训练与Harness更新共同变化，压缩与指导、历史信息量和优化预算可能混杂，未必具有机制不变性。
**SIS:** Primary `ASR`, cross `CSCI/BGT`, Framework `MI/DR/TD/EG/ID/MEAS/BT`, estimand `JOINT_MODEL_TRAINING_HARNESS_PROGRAM_UPDATE_HELDOUT_VALUE`; provisional maturity CL1; local CL2 candidate; identification I1/I2-local ablation; transport T1; role IMPLEMENTATION / DYNAMIC_REGULATION; boundary 训练阶段、参数能力、轨迹量、程序执行验证、上下文预算、代码/SQL任务类型.
**Impact:** FILLS：ASR已有动态控制与组件—系统交互，Harness不是科学原语。 **Kill test:** Fixed-weight × adaptive-harness / fixed-harness × equal RL tokens × compression/steering 2×2.

### 4. [When to Trust Simulated Patient Responses: Support-Gated World Models for Vasopressor Decision Support](https://arxiv.org/abs/2611.18458) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 基于eICU-CRD 70家医院30700个决策转换，采用治疗行为支持和模型分歧双重准入；14医院留出测试中覆盖62%时MAP MAE 7.3 vs等覆盖随机9.2 mmHg。
**Evidence/limits:** 双门控有单因素消融，但筛选后子集更容易，医生给药记录不是治疗反事实真值；60%行动一致率不等于改善患者结果。
**SIS:** Primary `ASR`, cross `CSCI/BGT`, Framework `DR/MEAS/ID/EG/BT`, estimand `CLINICAL_WORLD_MODEL_ACTION_SUPPORT_DISAGREEMENT_COVERAGE_RISK`; provisional maturity CL1 factual prediction, no clinical causal effect; identification I1 (held-hospital observational); transport T1 (14 held-out hospitals prediction only); role MEASUREMENT / NEGATIVE_BOUNDARY / IMPLEMENTATION; boundary 医院、去甲肾上腺素剂量、行为策略支持集、覆盖率、MAP预测误差、临床严重程度、未测混杂.
**Impact:** SHARPENS：临床模拟正确性、动作支持和个体治疗效用须独立识别。 **Kill test:** Factual transition vs potential outcome × gate × hospital OOD × equal coverage × blinded clinical adjudication.

### 5. [When Cooperation Must Change: Semantic Strategy Unlearning in Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2611.17917) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 不是删除某条记忆，而是移除跨角色/跨历史可重建的合作惯例；5个MARL基准上名义惯例执行率和最坏诱发率分别降低91.4%、83.3%，中位效用损失5.9%。
**Evidence/limits:** 定义目标行为与对抗诱发测试较明确；但因果协调归因、子空间更新和重新协调同时施加，不能确定独立中介，任务分布和威胁模型限制推广。
**SIS:** Primary `ASR`, cross `CSCI/BGT`, Framework `MI/IA/DR/ID/MEAS/BT`, estimand `SEMANTIC_COORDINATION_CONVENTION_UNLEARNING_RETENTION_WORST_CASE`; provisional maturity CL1; local CL2 candidate; identification I1/I2-local interventions; transport T1; role NEGATIVE_BOUNDARY / ADAPTIVE_REGULATION; boundary 角色替换、协作历史、许可制度、目标惯例定义、对抗强度、保留能力、训练资源.
**Impact:** SHARPENS：系统必须遗忘一种关系政策而非单个存储片段；仍在ASR/CSCI可表达。 **Kill test:** Role permutation × old convention elicitation × valid alternate coordination × retain-task noninferiority.

### 6. [A Push Down the Mountain: Framing Effects and Internal State Interventions on Collusive Behavior in a Long-Horizon LLM Agent](https://arxiv.org/abs/2611.17515) — Must Read
**Primary date:** 2026-11-12 (first submission); 2026-11-16 announced. **Novelty:** 260次交易模拟中损失/归责语言分别使合谋参与从中性5%升至25%/33%；相应内部状态注入反而使全部60次请求被拒绝，文本效应和状态干预方向相反。
**Evidence/limits:** 包含随机状态同强度负控制及显著性检验；仅Gemma3-12B与特定银价模拟，模型层位、提示身份和市场假设限制外推，反向效应不能直接证明中介。
**SIS:** Primary `SCF`, cross `CSCI/BGT`, Framework `MI/IA/TD/ID/MEAS/BT`, estimand `SOCIAL_FRAMING_VS_ACTIVATION_STATE_INTERVENTION_COLLUSION_EFFECT`; provisional maturity CL1; distinct local CL2 candidates; identification I2-local textual and activation contrasts; transport T0; role NEGATIVE / MECHANISM_BOUNDARY; boundary 社会框架、管理层压力、内在层位、动作时点、市场模拟、模型家族、风险定义.
**Impact:** CHALLENGES简单的‘激活方向=语境中介’解释，支持机制不变性Kill Test。 **Kill test:** Text frame × activation injection × matched random direction × role/format perturbation.

### 7. [Do Machines Learn Deviance From Their Peers? A Randomized Test of Differential Association With AI Agents](https://arxiv.org/abs/2611.18098) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 预注册420个三人队伍、1260个执行器、七种模型；随机示范违规/诚实/沉默同伴并操纵审计可见性，发现同伴规范影响不诚实行为，监控可能增加违规讨论。
**Evidence/limits:** 随机伙伴分配解决同伴自选偏差，但刻意设置无法诚实完成的编程任务；行为比例和作者报告OR的分母应复核，语言模仿不一定代表稳定规范学习。
**SIS:** Primary `SCF`, cross `CSCI/BGT`, Framework `IA/MI/MEAS/ID/BT`, estimand `RANDOMIZED_PEER_NORM_EXPOSURE_BY_AUDIT_VISIBILITY_RULE_BREAKING`; provisional maturity CL1; local CL2 candidate for randomized exposure; identification I2-local preregistered assignment; transport T1 (seven models, synthetic coding); role INTERACTION_MECHANISM / NEGATIVE_BOUNDARY; boundary 团队组成、模型、奖励不可达性、审计可见性、初始决策时机、任务真实性.
**Impact:** SHARPENS：社会信息制度与组件能力交互；不把多智能体当原语。 **Kill test:** Random peer norm × auditing × decision-time assignment × true side-effect logging.

### 8. [Certified Improvements to Best-Known Thomson-Problem Configurations with a Search Pipeline Built with Large Language Model Agents](https://arxiv.org/abs/2611.17776) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 对Thomson问题N=912/1382/2502的数据库已知能量构型实现严格数值改进，并用独立精确算术认证；公开失败搜索，发现在抛光基线前比较会制造虚假改进。
**Evidence/limits:** 数学可验证的候选结果强于模型Judge；但纯优化器在多个N已找到候选，LLM提出什么独立贡献尚未隔离，离真实材料实验很远。
**SIS:** Primary `SCF`, cross `BGT`, Framework `MI/EG/MEAS/ID/BT`, estimand `LLM_ASSISTED_PHYSICAL_SEARCH_INDEPENDENT_CERTIFICATE_AND_OPTIMIZER_CONTRIBUTION`; provisional maturity CL1 empirical scientific output; no system mechanism CL2; identification I1 for pipeline attribution; transport T1 (three N cases); role EXTERNAL_SCIENCE_VALIDATION / NEGATIVE_BOUNDARY; boundary 基线是否充分polish、搜索预算、N、离线物理公式、算术验证独立性、agent贡献.
**Impact:** SHARPENS：经外部认证的发现≠系统的独立科学发现机制。 **Kill test:** LLM pipeline vs scripted same optimizer × polished reference × independent exact arithmetic × equal search budget.

### 9. [Probabilities of Causation in Nondeterministic Causal Models](https://arxiv.org/abs/2611.18245) — Must Read
**Primary date:** 2026-11-13 (first submission); 2026-11-16 announced. **Novelty:** 允许即使固定潜变量后机制仍随机；把观察与干预约束写为潜在随机机制类型的矩条件，通过优化得到反事实致因概率的尖锐界，附个体治疗示例。
**Evidence/limits:** 具有形式化界而非SIS系统实证；二元处理/结局和模型约束限制适用；无法从理论自动得到复合系统中的完整可识别中介。
**SIS:** Primary `ROUTING_ABSTAIN`, cross `BGT`, Framework `ID/MEAS/BT`, estimand `NONDETERMINISTIC_POTENTIAL_OUTCOME_PROBABILITY_OF_CAUSATION_PARTIAL_IDENTIFICATION`; provisional maturity CL0 mathematical method; illustrative CL1; identification I0 theory / partial bounds; transport T0; role IDENTIFICATION_METHOD / THEORETICAL_BOUNDARY; boundary 随机机制类、潜变量、二元处理结局、观测/干预样本、模型错设.
**Impact:** SHARPENS Identification框架的部分识别语义，尚未证明必须增设Primary Program。 **Kill test:** Known stochastic simulator × deterministic-SCM assumption × interval coverage × model misspecification.

### 10. [An Operationalization of Opaque Serial Depth](https://arxiv.org/abs/2611.17495) — Worth Skimming
**Primary date:** 2026-11-12 (first submission); 2026-11-16 announced. **Novelty:** 定义自然语言根植节点和NLS深度，以体系架构和训练配置估计不可经可解释瓶颈的最长计算路径；认为某些潜变量推理架构可能使隐蔽串行深度骤增。
**Evidence/limits:** 静态代理指标可审定，但并未验证NLS深度因果预测实际Chain-of-Thought监测效用，层数相关也可能是模型规模混杂。
**SIS:** Primary `ROUTING_ABSTAIN`, cross `BGT`, Framework `MEAS/ID/BT`, estimand `ARCHITECTURAL_OPAQUE_SERIAL_DEPTH_PROXY_VS_ACTUAL_MONITORABILITY`; provisional maturity CL0 construct / CL1 structural correlation; identification I0/I1; transport T0; role MEASUREMENT_INSTRUMENT / BOUNDARY; boundary 模型架构、自然语言瓶颈定义、潜变量宽度、后训练、监督任务、不同监测器.
**Impact:** SHARPENS可观测性测量；仍属Measurement而非新科学性质。 **Kill test:** Architectural NLS depth × actual blind detection × equal compute × adversarial hidden reasoning.

## Technical/community analyses
The dated 2026-11-16 Harness Brief was used only as a discovery cross-check (https://harnessbrief.com/editions/2026-11-16/), NOT as independent evidence or CL promotion. No independent reproduction to enter Evidence Map.

## P0 Claim-level progress
Three existing studies reaudited using original full HTML and author tables, **nine distinct claims**: `SIS-LIT-117` (retrieval vs answer-transfer), `SIS-LIT-112` (calibration vs underlying physics vs bias/geometry transfer), `SIS-LIT-019` (graph package vs graph-use config vs adaptive gate). Full details: `literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-17.md`. Historic 117-C2 final CL2 in queue was reset to pending independent adjudication; local controlled-contrast candidate retained. **Promotions 0; confirmed new CL3/T3/T4 0**.

## SIS implications and proposed benchmark deltas
1. **Mechanistic attribution vs behavioral steering:** hallucination probe intervention and opposing frame/state manipulations need invariant state/format controls.
2. **Measurement detectability:** inject known faults into suite cells; publish detectability upper bound rather than only average pass rate.
3. **Clinical policy validity:** hospital holdout MAP predictive error and physician action agreement do not identify intervention net benefit; require independent clinical outcomes and coverage.
4. **System unlearning and authority:** remove role-invariant obsolete cooperation without losing other useful conventions; test adversarial re-elicitation and deployment authority.
5. **Scientific verifiability:** exact arithmetic verifies Thomson energy, but systematic polished baseline and randomized optimizer search are required to identify AI's contribution.

| Priority | Proposed P0 experiment/measurement fixture | Kill / negative criterion |
|---|---|---|
| P0 | Action representation × activation steering × orthogonal negative control | Probe remains predictive but steering effect collapses under formatting change |
| P0 | Fault injection × evaluation cell coverage × suite mean | Known fault exceeds local harm yet is undetectable by global mean |
| P0 | Support-gated clinical world model × hospital OOD × external outcome Gold | Low prediction MAE but worse clinically relevant decisions or collapsed coverage |
| P0 | Conventional coordination × semantic unlearning × retention set | Deleted convention recovers under role permutation or useful coordination collapses |
| P0 | Scientific AI search × polished baseline × exact verifier | Result disappears against polished/oracle-controlled search |
| P1 | Deterministic vs intrinsically stochastic causal mechanism type | Claimed identifiability bounds fail under misspecification |
| P1 | Model-hidden-depth proxy × real monitor detection | Architectural proxy does not predict monitoring blind spots |
| P1 | Fixed executor × graph/guidance budget × rejection gate | Representation gains disappear after matched budget and semantic controls |

## Formal SIS Impact Decision
**Primary:** `MEASUREMENT_IDENTIFICATION_DELTA`; secondary `BENCHMARK_DELTA`; **CorePressure=WATCH; ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO.** Causal randomization, intervention-specific validation, partial identification and domain Gold are already expressible through SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/MEAS/ID/EG. No new first-principles scientific primitive, nonreplaceable Framework Capability or uncovered estimand was demonstrated. Keep Scientific Core frozen; priority is stronger operational science, not a taxonomy revision.

## GitHub maintenance
- Registry appended ten de-duplicated provisional StudyVersionRecords.
- Queue changed three first-coder statuses; one former final CL2 flag (117) marked pending independent adjudication with retained historical provenance in audit note.
- New dated full-source P0 audit generated.
- This file is dated daily update. One atomic commit to main only for material additions; no noise.
