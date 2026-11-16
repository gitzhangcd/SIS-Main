# SIS Daily Literature Update｜2026-11-16

**Source of truth:** `specs/System_Intelligence_Science_v0.3.1.md`; Registry v1.3 (living); `literature/evidence-map/SIS_Literature_Evidence_Map_P0.md`; P0 Audit Queue, latest 2026-11-15 ledger. **Scientific Core FROZEN**.
**Discovery/analysis date:** 2026-11-16 (Asia/Shanghai). Most recent available regular arXiv cs.AI bulletin at this run: Friday 2026-11-13 (113 new cs.AI submissions, 208 crosslists and 216 replacements; 537 total listing entries, not 537 independent new works). Monday 2026-11-16 bulletin had not been published by local 08:00. All selected new studies were FIRST SUBMITTED 2026-11-10–12 and are **delayed-discovery selections**, not first-posted on Monday.
**Repository read:** full 9,895-line SIS Master, current living Registry, entire CSV Audit Queue, P0 Evidence Map and 2026-11-15 update/audit. Dedup checked against entire living Registry by original arXiv ID and title; current historical 2026-10-09–23 ledger remains global identity-reconciliation backlog. Do not create new permanent identifiers, and do not confuse preprint / peer-reviewed version.
**Primary-source screening:** official arXiv pages for ten papers; targeted ACL Anthology proceedings, arXiv current postings and selected conference/author pages; official EACL and EMNLP primary publication versions of existing studies 009/011 verified. No independently verified newly archived high-value peer-reviewed study in this selection. Community technical analyses may inform discovery, never CL promotion.
**Evidence limit:** abstract and selected method/result verification. The ten new studies have not all had tables/appendices independently reproduced or second-coded; no formal CL2+ or T3/T4 conclusion.

## New peer-reviewed studies
None admitted: no stronger nonduplicate recently indexed official proceedings item qualified for a new Study on this date. **Existing StudyVersionRecord lineage updates are below, not counted as new papers.**

## New primary preprints｜10 qualifying items
### SIS-CAND-20261116-01｜Controlling the Probability of Unknown Unknowns in Pre-Deployment Testing of AI Systems — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.15835; first submitted 2026-11-11; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 对后续测试首次出现未知故障模式的概率（missing mass）构造 anytime-valid 置信上界，在连续测试中允许依据预设阈值决定是否停止；研究对应 Good–Turing 的序贯版本。
- **Evidence, design, confounders:** 理论统计保证及 SWE-Chat 代码执行轨迹上的示例，而非证明真实部署无未见风险；故障类别定义、事件可观测性、任务抽样制度及任务分布偏移决定有效性。
- **SIS routing:** Primary `ASR`; cross-cutting `BGT`; Framework Capability `DR/MEAS/ID/EG/BT`; primary estimand `UNSEEN_FAILURE_MASS_SEQUENTIAL_TEST_STOPPING_BOUND`.
- **ScientificClaim maturity ceiling:** CL0 conditional guarantee; CL1 empirical demonstrations; identification `I0/I1`; transport `T0`; evidence role `MEASUREMENT / BOUNDARY / THEORETICAL_STOPPING`; claim nature `BOUNDARY / MEASUREMENT`.
- **Key boundary variables:** failure-mode identity, test-sampling distribution, exchangeability, partial observability, distribution shift, risk severity, stopping threshold.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Sequential unseen-failure stopping × failure taxonomy quality × shifted test distribution × independently verified catastrophic outcome.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-02｜NIBench: benchmarking autonomous AI agents for execution, skill evolution and scientific judgment in neuroimaging — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.15831; first submitted 2026-11-11; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 以七种神经影像工具生态的56项执行/重建任务、轨迹技能蒸馏与36条阿尔茨海默病科学判断问题，拆分执行能力、经验获得和科学证据判断。
- **Evidence, design, confounders:** 19个模型的工具与任务实验具有领域价值；已见任务技能增益不代表未见任务、跨模型或科学结论的可靠迁移。工作流可复现≠神经影像分析有效，临床/科研专家独立Gold缺位。
- **SIS routing:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/TD/EG/MEAS/ID/BT`; primary estimand `NEUROIMAGING_EXECUTION_SKILL_TRANSFER_VS_SCIENTIFIC_JUDGMENT_GAP`.
- **ScientificClaim maturity ceiling:** CL1 observed performance only; identification `I1`; transport `T2-performance-only (unseen tasks/other models)`; evidence role `MEASUREMENT / NEGATIVE_BOUNDARY / TRANSPORT_GAP`; claim nature `NEGATIVE / TRANSPORT_GAP`.
- **Key boundary variables:** scanner/modality, MRI/PET workflow, software versions, task familiarity, expertise, evidence provenance, skills cost, model capabilities.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Fixed executor × skill learned/held-out/cross-model × neuroimaging ground-truth analysis × blinded domain expert scientific judgment.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-03｜AgentSSL: Can MLE Agents Leverage Unlabeled Data? — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.17323; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 将半监督学习定义为程序搜索；等计算预算下8/12情形自动合成程序优于人工比较方案最高21.8%，但依赖系统反馈指标选程序时性能可下降47%，并发布16977程序的ProgramSelectBench。
- **Evidence, design, confounders:** 等预算比较有价值；反馈指标与真正未见集效用不一致，生成器、程序库质量、选择器、标注密度及跨生态域迁移尚不能唯一归因。
- **SIS routing:** Primary `ASR`; cross-cutting `BGT`; Framework Capability `MI/DR/MEAS/ID/BT`; primary estimand `PROGRAM_GENERATION_VS_FEEDBACK_BASED_SELECTION_VALUE_UNDER_SPARSE_LABELS`.
- **ScientificClaim maturity ceiling:** CL1 task performance and negative selection results; local CL2 candidate; identification `I1/I2-local`; transport `T1 (controlled/real ecology)`; evidence role `NEGATIVE_BOUNDARY / MEASUREMENT / IMPLEMENTATION`; claim nature `NEGATIVE / BOUNDARY`.
- **Key boundary variables:** labeled/unlabeled ratio, program candidate set, evaluator calibration, compute, dataset shift, ecology domain, feedback leakage.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Fixed generated candidate pool × surrogate-feedback selector × independent held-out Gold × equal total compute.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-04｜Singularity-Bench: Can Agents Build Agents? — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.16591; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 将预训练、中训练、后训练、推理、Agent Harness、集群管理六项完整AI系统构建任务在相同硬件上与人类成熟实现比较，并构造Breakwater对自动生成系统的奖励投机/攻击审计。
- **Evidence, design, confounders:** 多个系统和任务真实实现提供成本与端到端证据；评价器只覆盖已测试攻击，局部优于人类基线不等于一般自我改善、独立因果机制或安全保证。
- **SIS routing:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/IA/EG/MEAS/ID/BT`; primary estimand `END_TO_END_AI_SYSTEM_BUILD_CAPABILITY_VS_HUMAN_BASELINE_AND_EVAL_INTEGRITY`.
- **ScientificClaim maturity ceiling:** CL1 benchmark performance only; identification `I1`; transport `T1 multi-workload performance`; evidence role `BENCHMARK_INSTRUMENT / IMPLEMENTATION / EVALUATOR_GOVERNANCE`; claim nature `MEASUREMENT / IMPLEMENTATION`.
- **Key boundary variables:** human reference quality, hardware parity, compute allowance, grader correctness, workload selection, reward-hacking threat model.
- **SIS impact:** **SHARPENS** (CorePressure=NONE); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Same hardware + budget × task-specific system construction × blind functional grader × held-out adversarial breakwater tests.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-05｜LiveGeo: Benchmarking Geographic Agents in Continuously Evolving Worlds — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.17267; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 提出GeoWorld/LiveGeo，让外部地理环境按照自己的时间过程变化且留下可验证历史；要求系统检查旧依据是否过期、主动获取新信息并修订计划。
- **Evidence, design, confounders:** 静态任务成绩不保证动态可靠性，且环境有时间标记；但地理模拟器可控的状态变化不能证明现实规划的可靠性，证据刷新成本和任务难度需控制。
- **SIS routing:** Primary `SDR`; cross-cutting `BGT`; Framework Capability `TD/MI/DR/EG/MEAS/BT`; primary estimand `DYNAMIC_WORLD_CHANGE_EVIDENCE_REFRESH_PLAN_VALIDITY`.
- **ScientificClaim maturity ceiling:** CL1 simulation task evidence; identification `I1`; transport `T1 multi-task simulated`; evidence role `NEGATIVE_BOUNDARY / DYNAMICS_BENCHMARK`; claim nature `BOUNDARY / NEGATIVE`.
- **Key boundary variables:** world update rate, evidence latency, time horizon, sensing permission, routing data, simulated-real mismatch, plan reversibility.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Frozen vs evolving world × evidence-refresh permission × delay × equal retrieval budget × state-grounded endpoint.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-06｜Actor, Judge, or Teacher? Understanding Decision Models in Long-Horizon Agents — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.17167; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 对同一决策模型分离行动者、轨迹结束后评价者和教师：模型前瞻行动容易被即时子目标吸引，但事后拥有完整轨迹时可能正确评价长期动作；教师方案在ALFWorld/WebShop优于比较训练。
- **Evidence, design, confounders:** 同一模型跨角色比较控制了部分能力混杂；但角色变化也改变可见信息、时间方向、训练数据与反馈粒度，不能推断纯粹角色的因果机制。
- **SIS routing:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/IA/TD/MEAS/ID/BT`; primary estimand `ACTOR_VS_RETROSPECTIVE_JUDGE_VS_TEACHER_ROLE_EFFECT`.
- **ScientificClaim maturity ceiling:** CL1; local controlled role candidate; identification `I1/I2-local`; transport `T1 multi-environment`; evidence role `ROLE_BOUNDARY / IMPLEMENTATION / COMPONENT_INTERACTION`; claim nature `BOUNDARY / IMPLEMENTATION`.
- **Key boundary variables:** trajectory visibility, posthoc information, model size, task horizon, reward specification, teacher training budget.
- **SIS impact:** **SHARPENS** (CorePressure=NONE); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Fixed base model × actor/judge/teacher role × matched state information × blind final task outcome.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-07｜Ballad: Bandit-Based LLM Routing for Automated Heuristic Discovery — **Worth Skimming**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.17241; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 面向非平稳的自动启发式发现，通过搜索谱系DAG分配延迟收益与折扣旧信息，动态选择不同费用的LLM；挑战始终使用最强大模型的路由假设。
- **Evidence, design, confounders:** 报告组合优化问题上相近或更高结果质量且某些场景相对昂贵单模型最多节约65.6%成本；启发式变异谱系关联导致收益非平稳，DAG归因未必等同独立因果贡献。
- **SIS routing:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework Capability `DR/IA/MEAS/ID/BT`; primary estimand `NONSTATIONARY_GENEALOGY_CONDITIONAL_MODEL_ROUTING_COST_QUALITY_EFFECT`.
- **ScientificClaim maturity ceiling:** CL1; local CL2 candidate; identification `I1/I2-local`; transport `T1 optimization families`; evidence role `IMPLEMENTATION / ROUTING_BOUNDARY`; claim nature `IMPLEMENTATION / BOUNDARY`.
- **Key boundary variables:** candidate genealogy, NP-hard task type, model tariff, reward nonstationarity, search budget, shared context, delayed reward.
- **SIS impact:** **SHARPENS** (CorePressure=NONE); no uncovered first-principles estimand. **Reading:** Worth Skimming. **Kill test:** Model routing × genealogy credit vs random credit × equal quality/compute × nonstationary task shifts.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-08｜How Should Planning Agents ReSHAPE Their Search Space? — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.16466; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 将用户初始请求当可检验偏好假设，主动展示备选方案以识别可接受权衡，并测量搜索空间质量与固定规划器实际可到达的可接受方案。
- **Evidence, design, confounders:** 5800个人工核对模拟用户任务显示正确权衡能大幅提高可接受计划发现；模拟用户反应、接受判据和人类真实长期偏好不是同一真值。
- **SIS routing:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework Capability `DR/IA/MEAS/ID/BT`; primary estimand `PREFERENCE_ELICITATION_SEARCH_SPACE_REVISION_ACCEPTABLE_PLAN_EFFECT`.
- **ScientificClaim maturity ceiling:** CL1; local CL2 candidate; identification `I1/I2-local`; transport `T1 simulated travel/shopping`; evidence role `HUMAN_SYSTEM_BOUNDARY / REGULATION`; claim nature `BOUNDARY / IMPLEMENTATION`.
- **Key boundary variables:** user tradeoff uncertainty, user attention, preference revision cost, planner frozen state, simulator validity, domain.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Must Read. **Kill test:** Ask preference vs show concrete plans × same planner × human-validated acceptability × interaction budget.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-09｜Scale-Induced Semantic Shift in Visual Prompt Injection Against VLMs and Web Agents — **Worth Skimming**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.16744; first submitted 2026-11-12; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 缩放/压缩可以改变视觉模型能读取的文本语义；构造双尺度对照显示图片被模型看懂的风险不等于Web Agent实际执行越权。
- **Evidence, design, confounders:** 300例测试中图片攻击平均成功率58.75% vs 41.08%基线，独立Web Agent实际行为妥协约4%；不同尺度、图像渲染与下游代理能力显著调节结果。
- **SIS routing:** Primary `SDR`; cross-cutting `BGT`; Framework Capability `TD/MI/EG/MEAS/ID/BT`; primary estimand `IMAGE_SCALE_SEMANTIC_DISCONTINUITY_TO_EXECUTED_COMPROMISE`.
- **ScientificClaim maturity ceiling:** CL1; local I2 presentation control; identification `I2-local for representation, I1 end-to-end`; transport `T1 VLM/web-agent`; evidence role `NEGATIVE_BOUNDARY / MEASUREMENT`; claim nature `NEGATIVE / BOUNDARY`.
- **Key boundary variables:** image dimensions, compression algorithm, OCR perception, browser rendering, model family, actual action reach, defense.
- **SIS impact:** **SHARPENS** (CorePressure=NONE); no uncovered first-principles estimand. **Reading:** Worth Skimming. **Kill test:** Image scale × same semantic content × perception-only vs executed side effects × unchanged tool permissions.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.

### SIS-CAND-20261116-10｜Rational Use of Time for Social Coordination in Humans and AI — **Worth Skimming**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14766; first submitted 2026-11-10; discovered 2026-11-16; **PREPRINT**, no independently confirmed peer-reviewed archive; provisional unique study, no permanent SIS-LIT ID.
- **Core novelty:** 考察不允许显式沟通、只能依赖时间间隔协调的合作卡牌游戏；150名人类与两类AI系统对比，区分理解伙伴时间线索和随合作史实际调整策略。
- **Evidence, design, confounders:** 模型表现可以呈现近似贝叶斯推断线索，却没有像人类一样高效调整跨轮行为；任务特定游戏规则及时间编码可能限制推广。
- **SIS routing:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `IA/TD/MEAS/ID/BT`; primary estimand `IMPLICIT_TEMPORAL_SIGNAL_INFERENCE_VS_PARTNER_ADAPTATION_EFFECT`.
- **ScientificClaim maturity ceiling:** CL1 behavioral gap only; identification `I1`; transport `T0 game / T1 model comparisons`; evidence role `NEGATIVE_BOUNDARY / HUMAN_INTERACTION`; claim nature `NEGATIVE / BOUNDARY`.
- **Key boundary variables:** timing signal precision, partner diversity, adaptation horizon, real-time experience, reward regime, policy memory.
- **SIS impact:** **SHARPENS** (CorePressure=WATCH); no uncovered first-principles estimand. **Reading:** Worth Skimming. **Kill test:** Timing cue × partner change × repeated interaction × signal validity × adaptive policy retention.
- **Evidence governance:** Official arXiv primary-source abstract/method claims verified; not independently adjudicated full experimental tables. Second coder and adjudication PENDING; CL2/CL3 not automatically promoted.


## Technical and community analysis
No independently reproduced technical/community analysis promoted into the evidence map; any items encountered remain `DISCOVERY_ONLY`. No padding.

## Version lineage and de-duplication
- `SIS-LIT-009` is already a study; its EACL 2026 archival identity is `2026.eacl-long.204` (official ACL Anthology). Verified archive identity; no new candidate ID.
- `SIS-LIT-011` is already a study; original arXiv:2609.00823 → official EMNLP 2026 Main `2026.emnlp-main.1143`. Reclassified queue source as peer-reviewed archive, **no new study** and no CL maturity promotion.
- `SIS-LIT-012` remains arXiv:2609.04611 preprint, original HTML examined. A task-level benchmark cannot be treated as mechanism evidence.
- Neither historical 145 permanent coded items nor the prior dated candidate ledger is silently renumbered. The P0 queue covers its existing 131 audited slots; no new row for daily temporary candidates.

## P0 first-coder claim-level re-audit
Nine distinct claims from existing `SIS-LIT-009/011/012`; details and source anchors in `literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-16.md`. No automatic inheritance of paper-level labels; second coder and adjudication **PENDING**. Confirmed CL2/CL3 promotions **0**, new T3/T4 **0**.

## Scientific synthesis and benchmark candidates
1. **Unseen failure mass / stopping:** counting known failures cannot establish absence of unknown failure families. Proposed P0: anytime-valid missing-mass stop test × taxonomy granularity × shifted task distribution × severity.
2. **Scientific capability disaggregation:** reliable neuroimaging execution, cross-model procedural skill and independent domain scientific judgment must be separately graded; NIBench provides an operational starting point relevant to SIS-MED.
3. **Candidate generation vs independent selection:** semi-supervised program synthesis can excel while feedback-based selection loses utility, exposing evaluator and selection confounding; pair with independent untouched Gold.
4. **Component role and conditional capability:** actor, posthoc judge and teacher are different intervention/information regimes. Fix model and role-information set; vary access, look-ahead and update costs orthogonally.
5. **Dynamic world and human interaction:** static success does not certify fresh-state decisions, and observing a timing signal does not guarantee adapting to a partner.

| Priority | Proposed fixture | Kill / negative criterion |
|---|---|---|
| P0 | Unseen failure missing-mass upper bound × shifting test distribution | Confidence guarantee invalid after taxonomy change or task shift |
| P0 | Scientific procedural execution × held-out skill × blind expert neuroimaging Gold | Strong execution but scientific claims unsupported |
| P0 | SSL candidate pool × selection metric × matched compute and independent test | Generated candidate gains reverse under selected deployment |
| P0 | Actor–Judge–Teacher × full vs limited trajectory × same model | Apparent role benefit vanishes under information matching |
| P0 | Dynamic GeoWorld × evidence refresh age × fixed retrieval budget | Static plan retained after verified world change |
| P1 | Same hardware system-build tasks × independent red-team/grader | Benchmark apparent completion disappears under hidden tests |
| P1 | Nonstationary routing × genealogical credit placebo × cost | DAG credit loses advantage to random allocation |
| P1 | Visual resize × perception × executed compromise | Attack success reported at perception level without execution |

## Formal SIS Impact Decision
**Primary: MEASUREMENT_IDENTIFICATION_DELTA**; secondary: **BENCHMARK_DELTA**; CorePressure: **WATCH**; **ScientificCoreDelta=0**; **SPEC_REVISION_CANDIDATE=NO**. New evidence sharpens test-stopping under unseen failures, selection-measurement validity, scientific judgment, dynamic-world state validity and human–component role interaction, all expressible under SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG; no fourth program or scientifically irreducible new object.

**Core Reopen Watchlist:** unseen-failure epistemic stopping, scientific judgment and cross-executor skill, selection-vs-generation, simulation-to-real and hidden authority limits. None yet reveals a non-expressible scientific estimand. Proceed with P0 measurement/identification and Benchmark fixtures, not Scientific Core revision.
