# SIS v0.3.1 Daily Literature Update｜2026-11-19

**Authority:** `specs/System_Intelligence_Science_v0.3.1.md`; `literature/SIS_v0.3.1_Literature_Re-Coding_Registry.md`; `literature/evidence-map/SIS_P0_Audit_Queue.csv`.
**Baseline:** GitHub main 61a4755fb941a58f716d750a5d429a7efa088293 (2026-11-19 run starts); previous daily note 2026-11-18. **Discovery:** arXiv 2026-11-18 public announcement (109 cs.AI new, 150 cross-lists, 142 replacements; secondary discovery index https://arxane.org/cs.AI), original arXiv/author full-text pages, ACL Anthology/OpenReview checks and community discovery-only checks.
**New studies:** 10 separate arXiv preprint StudyVersionRecords, first submitted 2026-11-17, not 2026-11-19. **Peer-reviewed new:** 0 independently verified. **Technical/community CL-qualified:** 0. No filler. Direct arXiv ID deduped against main registry; other historical backlog not fully reconciled.
**Status:** FIRST_CODER_DISCOVERY, NOT_ADJUDICATED. `CL2 candidate` is not a normative level. No automatic study-level promotion or T3/T4.
**Note:** `arXiv:2611.21651` has inconsistent surfaced metadata (Nov ID vs Oct initial-submission date); not used without independent source resolution.

## New evidence and SIS claim-level provisional recoding

### SIS-CAND-20261119-01｜The Resolution Hypothesis: Agent Evolution's Key Is Identifying Improvements — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.23068 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 七种自演化方法、六种模型、超过1000万次LLM调用；存在有益候选，但评估对好坏候选的识别接近随机，方法间几百分点差距可能小于独立运行方差。
- **Evidence quality / confounders:** 模型输出随机性、评分器噪声、候选集采样、基准任务与冻结权重设置限制泛化；作者主张不能自动外推到确定性真实执行评分。
- **Scientific coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/MEAS/ID/EG/BT`; Estimand `EVALUATION_RESOLUTION_CANDIDATE_SELECTION_AND_METHOD_RANK_STABILITY`; Evidence Role `NEGATIVE_MEASUREMENT / ADAPTIVE_SELECTION`; claim maturity ceiling `CL1 (author-reported comparison); no final CL2`; identification/transport `I1 / T1`.
- **Boundary variables:** evaluation noise, candidate pool, outcome instrument, model, repeated seeds, budget.
- **Impact:** SHARPENS; 当前SIS需要把候选产生能力与候选选择统计分辨率独立建模；不构成新增Core。
- **Priority:** Must Read. **Kill test:** 固定候选池×独立重复执行×盲法真实Gold×等预算选择；候选选择是否显著优于随机、方法排名是否稳定.

### SIS-CAND-20261119-02｜Multi-Agent Memory Inconsistency: Where Factual Conflicts Disappear in LLM Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22245 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 强制委托使冲突证据双向读取率由50.2%升至68.7%，但最终冲突检出由16.2%降至13.2%；证据分散在不同worker导致交接损失。
- **Evidence quality / confounders:** 文档审查平台、三种模型、有限执行次数、上下文分配与委托策略共变；证据覆盖与最终归因不是同一端点。
- **Scientific coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/EG/MEAS/ID/BT`; Estimand `DELEGATION_PARTITION_HANDOFF_EVIDENCE_PAIR_PRESERVATION_CONFLICT_DETECTION`; Evidence Role `NEGATIVE_BOUNDARY / INTERACTION / EVIDENCE_FLOW`; claim maturity ceiling `CL1; delegation contrast local CL2 candidate`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** delegation topology, partitioning, handoff compression, worker model, evidence overlap, dollar budget.
- **Impact:** SHARPENS; 更多信息获取可以伴随更少共同证据和更低系统判断能力。
- **Priority:** Must Read. **Kill test:** 固定检索到的冲突事实×同worker/分worker随机分配×统一handoff字数×lead盲判.

### SIS-CAND-20261119-03｜When Agent Skills Go Stale: Runtime Behavior and Selective Maintenance in Evolving Environments — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22525 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 四类任务环境、两模型：过期技能可使成功率比无技能低逾10pp或成本增近40%；无需新增模型调用的选择性维护最多提升67pp准确率、降低37%步骤。
- **Evidence quality / confounders:** 变化种类、维护检查覆盖、任务可重放性、模型校正行为决定净效用；最大值不是整体平均增益。
- **Scientific coding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/DR/MI/EG/MEAS/ID/BT`; Estimand `ENVIRONMENT_DRIFT_STALE_SKILL_REUSE_MAINTENANCE_COST_ACCURACY_RECOVERY`; Evidence Role `DYNAMIC_NEGATIVE_BOUNDARY / RECOVERY`; claim maturity ceiling `CL1; local maintenance contrast CL2 candidate`; identification/transport `I2-local / T1`.
- **Boundary variables:** environment volatility, drift type, observation delay, skill granularity, checks, maintenance cost.
- **Impact:** SHARPENS; 能力资产可由正贡献转成负贡献，必须动态评估维护净效用。
- **Priority:** Must Read. **Kill test:** 技能新旧×环境变更×无技能基线×维护/重建×回归保留集.

### SIS-CAND-20261119-04｜RAG in a Trenchcoat: When Minimal Memory Is Enough for Agentic Systems, and When It Isn't — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22179 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 简洁BRIDGE记忆在LongMemEval-S/BEAM与复杂方法统计近似，EverMemBench高约5.7–6.3分；但未显式提示规则的执行探针显示原子事实记忆与块摘要在规则应用/模式归纳上互有胜负。
- **Evidence quality / confounders:** 探针与grader设计、输入呈现、不同reader与总token费用、相同任务族；检索正确不代表行动使用证据。
- **Scientific coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/EG/MEAS/ID/BT`; Estimand `MINIMAL_VS_COMPLEX_MEMORY_RETRIEVAL_AND_APPLIED_RULE_PATTERN_DECISION_EFFECT`; Evidence Role `NEGATIVE_BOUNDARY / MEASUREMENT`; claim maturity ceiling `CL1; controlled probe candidate not CL3`; identification/transport `I1/I2-probe / T1`.
- **Boundary variables:** memory representation, recall vs applied behavior, reader, prompt prominence, token budget, domain.
- **Impact:** CHALLENGES以检索指标声称普遍记忆能力增益；现有MEAS/SCF可表述。
- **Priority:** Must Read. **Kill test:** 固定检索内容×不同记忆表征×证据可见位置×实际行动Gold.

### SIS-CAND-20261119-05｜Do LLM Agents Still Need to Be Told How to Self-Improve? — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.23219 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 冻结权重的teacher/player只给通用改善目标、工具及预算，自发构造练习任务、评估和上下文更新，形成某些模型有效的自我学习流程，并在不同游戏规则/时域出现迁移改善。
- **Evidence quality / confounders:** 封闭PuzzleScript游戏、三次teacher种子、工具可用性与模型能力高度相关；学习循环发现不等于真实科学系统递归优化的普遍机制。
- **Scientific coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/MI/TD/EG/MEAS/ID/BT`; Estimand `SELF_ORGANIZED_LEARNING_LOOP_VS_PRESCRIBED_LOOP_HELDOUT_CONTEXT_GAIN`; Evidence Role `CAPABILITY_FORMATION / REGULATION_IMPLEMENTATION`; claim maturity ceiling `CL1; limited local controlled contrast candidate`; identification/transport `I1/I2-local / T2 performance-only`.
- **Boundary variables:** teacher backbone capability, self-play budget, tool set, game horizon, frozen weights, transfer family.
- **Impact:** SHARPENS; 自组织调节策略是ASR的对象而非新primitive；需与显式循环等预算比较。
- **Priority:** Must Read. **Kill test:** 自组织循环×手工固定循环×sham工具×同预算×隐藏游戏与更长期未见任务.

### SIS-CAND-20261119-06｜What Does an Agent Need? Bundle-Aware Agent Resource Composition — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22030 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 5060个已执行配置、模型与工具技能包联合选择；十候选内找回完整参考配置67.73%，代理评分器选优配置执行得分从7.58升8.37，实际执行反馈提高至8.78。
- **Evidence quality / confounders:** 参考配置不是唯一最优、代理critic学习数据与后验评分之间可能共享偏好；成本、组合规模及目标域分布变化需对照。
- **Scientific coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/IA/MI/MEAS/ID/BT`; Estimand `TASK_CONDITIONAL_MODEL_TOOL_SKILL_BUNDLE_SELECTION_REAL_EXECUTION_VALUE`; Evidence Role `REGULATION / COMPONENT_INTERACTION`; claim maturity ceiling `CL1; local execution contrast CL2 candidate`; identification/transport `I1/I2-local / T2 performance-only`.
- **Boundary variables:** backbone capability, bundle interactions, resource catalog, task domain, critic feedback, evaluation cost.
- **Impact:** SHARPENS; 组件价值不可独立相加，优化路由应评估整个配置净价值。
- **Priority:** Must Read. **Kill test:** 固定模型×技能包组合正交干预×真实执行Gold×等算力候选选择×新工具.

### SIS-CAND-20261119-07｜CrossEnv: Synthesizing Verifiable Cross-Environment Tasks for Long-Horizon Agent Training — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22777 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 使用实体—工具图生成跨服务依赖一致的任务与课程，从单环境到多环境再到用户交互；四项外部基准报告更少训练样本下的竞争力及新环境组合迁移。
- **Evidence quality / confounders:** 合成数据自洽不等于真实服务副作用/权限约束真实，课程、数据规模和环境组合同时变化。
- **Scientific coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/IA/EG/MEAS/BT`; Estimand `CROSS_ENV_ENTITY_DEPENDENCY_CURRICULUM_VS_REAL_TASK_TRANSFER`; Evidence Role `BENCHMARK / PERFORMANCE_TRANSFER`; claim maturity ceiling `CL1; no causal transport confirmation`; identification/transport `I1 / T2 performance-only`.
- **Boundary variables:** entity consistency, cross-service side effects, environment combinations, curriculum, task length, user behavior.
- **Impact:** FILLS EXISTING FRAMEWORK; T2性能迁移不能写成T3机制可迁移。
- **Priority:** Worth Skimming. **Kill test:** 合成跨环境×真实跨环境holdout×等样本/计算×实体一致性缺陷注入.

### SIS-CAND-20261119-08｜RegimeCouncil: Paired-Evidence Routing For Memory Conflict Governance In LLM Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22113 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 对事实失效的延迟反馈选择本地或全局传播范围；理论显示固定策略有线性遗憾的条件，双顾问策略在30个保留设置、主争议样本上比最佳固定策略高5.2–7.3分。
- **Evidence quality / confounders:** 所述保证依赖反馈时延和效用可比，误报反馈、数据隐私与长期反馈延迟未充分检验。
- **Scientific coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/TD/EG/MEAS/ID/BT`; Estimand `LOCAL_VS_GLOBAL_MEMORY_FEEDBACK_SCOPE_ONLINE_POLICY_VALUE_UNDER_DELAY`; Evidence Role `THEORETICAL_BOUNDARY / REGULATION`; claim maturity ceiling `CL0 conditional theory + CL1 experimental`; identification/transport `I0/I1 / T1`.
- **Boundary variables:** fact validity coupling, feedback delay, regime switching, no-memory anchor, model, drift rate.
- **Impact:** SHARPENS; 影响传播范围本身是条件性ASR决策变量。
- **Priority:** Must Read. **Kill test:** 隔离漂移×全局漂移×缺失/延迟反馈×相同查询预算×真实线上长期保留.

### SIS-CAND-20261119-09｜Thinking Harder Doesn't Lead to Better Choices: Reasoning Effort Increases the Confidence but Not the Correctness of LLM Shopping Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22033 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 十种前沿模型、三个电商商品选择测试中，更高推理努力未带来统计上可靠的正确率提升，却显著提高自报信心；部分错误在模型间共享。
- **Evidence quality / confounders:** 商品正确性标签、任务构造和努力档位影响统计效力；不能从未显著提高断言所有任务无收益。
- **Scientific coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/MEAS/ID/BT`; Estimand `REASONING_EFFORT_COST_VS_PURCHASE_CORRECTNESS_CONFIDENCE_CALIBRATION`; Evidence Role `NEGATIVE_NULL / MEASUREMENT`; claim maturity ceiling `CL1; local effort assignment not general mediation`; identification/transport `I1/I2-local / T1`.
- **Boundary variables:** task ambiguity, model family, thinking budget, confidence calibration, product Gold, common errors.
- **Impact:** CHALLENGES把更多推理预算视为单调提升的工程假设；SIS早已不预设Adaptive>Static。
- **Priority:** Must Read. **Kill test:** 随机预算×相同商品Gold×任务难度×成本与校准误差×跨模型相关错误.

### SIS-CAND-20261119-10｜SkillBuffBench: Measuring What Agent Skills Contribute across Harnesses, Models, Skill Access Modes and Memory — Watchlist
- **StudyVersionRecord:** https://arxiv.org/abs/2611.22017 ; initial submission **2026-11-17**; PREPRINT, surfaced in 2026-11-18 announcements and checked 2026-11-19; one provisional Study, not a permanent SIS-LIT ID.
- **Core idea / novelty and author evidence:** 提出Skill访问三水平（无/人工指定/从安装库自动发现）×记忆开关×四Harness×多个模型的配对实验，并以材料/生物领域工件确定性校验和配对bootstrap设计测量。
- **Evidence quality / confounders:** v1明确尚未公布实验结果；技能库部分材料未公开，不能视为系统能力收益证据。
- **Scientific coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/EG/MEAS/ID/BT`; Estimand `SKILL_ACCESS_MODE_BY_MEMORY_HARNESS_BACKBONE_TASK_OUTCOME_INTERACTION`; Evidence Role `MEASUREMENT_DESIGN_ONLY`; claim maturity ceiling `CL0 protocol; no empirical CL1 results released in v1`; identification/transport `I0 / T0`.
- **Boundary variables:** skill retrieval mode, memory exposure, harness, model capability, domain expert Gold, time/cost.
- **Impact:** FILLS EXISTING MEAS/CSCI; 强测量设计但不应据此提升任何Claim。
- **Priority:** Watchlist. **Kill test:** 结果正式释放×重复实验×模型预算匹配×自动选择错误归因×独立领域专家Gold.

## Synthesis and concrete experimental/measurement updates

1. **Evaluation resolution may bound self-improvement before proposal quality does.** Register a proposer-quality vs selector-resolution paired benchmark with repeated trials, random-selector placebo and measurement variance.
2. **Evidence may be found but lost at organization boundaries.** Independently audit read → worker output → lead input → contradiction detection, with same facts and randomized partition topology.
3. **Stored capabilities are time-conditional assets.** Explicitly compare old skill reuse, no skill, selective repair and complete rebuild after environment perturbation; count maintenance resource cost.
4. **Memory representation is task-conditional.** Ordinary retrieval QA does not establish implicit rule application or pattern induction; measure action outcome with independent Gold.
5. **Regulation controls include feedback scope, resource bundle, deliberation budget and whether a self-learning loop is discovered.** All are conditional policies, not new first-principles primitives.

| Priority | Proposed controlled fixture | Required negative / kill result |
|---|---|---|
| P0 | Fixed candidate pool × judge noise × independent repeated evaluation | Selector not reliably better than random; rank order flips under reseeding |
| P0 | Worker partition × handoff compression × fixed conflicting facts | Evidence read rises while contradiction detection falls |
| P0 | Skill age × environment drift × repair vs no-skill baseline | Stored skill reduces utility or repair fails to preserve earlier competence |
| P0 | Memory representation × implicit-rule task × reader and budget | Retrieval high but remembered rule not applied |
| P0 | Local/global feedback scope × delayed validity × no-memory paired anchor | Performance depends on hidden drift regime |
| P0 | Reasoning effort × correctness × confidence calibration | Cost and confidence increase with no decision gain |
| P1 | Bundle selection × backbone × real verifier vs proxy judge | Proxy ranking reverses in independently executed outcomes |
| P1 | Autonomous self-learning × prescribed loop × held-out mechanics | Self-improvement disappears at matched total training/eval cost |
| P1 | Cross-environment curriculum × true cross-service integrity Gold | Synthetic verifiability fails under real side effects |
| P1 | SkillBuff factorial preregistration | CL0 design cannot be reported as verified CL1 until runs published |

## P0 Claim-level re-audit
See [SIS_P0_Reaudit_2026-11-19](../evidence-map/audits/SIS_P0_Reaudit_2026-11-19.md). Existing study IDs **SIS-LIT-101 AIDE²**, **SIS-LIT-102 Growing Harness**, **SIS-LIT-105 ToolCompass** each decomposed into three estimand-specific claims, primary-source verified; first coder only, no automatic promotion. **9 claim reviews, 0 final CL2/CL3, 0 confirmed T3/T4.**

## Formal SIS Impact Decision
- **Primary:** `MEASUREMENT_IDENTIFICATION_DELTA`; **Secondary:** `BENCHMARK_DELTA`.
- **CorePressure:** `WATCH` (evaluation resolution and evidence lost across organization boundaries).
- **ScientificCoreDelta:** `0`; **SPEC_REVISION_CANDIDATE:** `NO`.
- **Reason:** All effects are expressible as SCF/SDR/ASR questions and CSCI/BGT with MI/TD/DR/IA/BT/MEAS/ID/EG; no verified missing estimand family, irreducible causal distinction, or non-replaceable scientific capability. Real pressure is on measurement and identification, not reopening Scientific Core.

## Provenance and version governance
- Full public arXiv paper URLs above are the primary provenance. Community indexing and blogs were discovery-only, and not CL evidence.
- No known duplication with dated candidates in Registry on direct source-ID matching. Preprint-to-proceedings lineage left unchanged; no inferred venue status.
- First-coder labels are provisional. Full second coder, controlled replication, and final adjudication pending.
