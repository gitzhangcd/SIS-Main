
# SIS Daily Literature Update | 2026-11-02

**Authority:** SIS v0.3.1 frozen scientific core; canonical Registry v1.3; current P0 Audit Queue. **Processing time:** 2026-11-02 08:00 China. **Source category:** October 2026 officially archived EMNLP Main / Findings / System Demonstrations papers, discovered/indexed late in this workflow. At 08:00 Asia/Shanghai, arXiv cs.AI new list still showed Friday, **2026-10-30** (605 list records; 158 new submissions); no verified new Nov 2 arXiv issue. **No invented same-day publication claims.**

**Duplicate rule:** match canonical paper title and official ACL Anthology ID against 145 permanent records and recent 89 provisional records. Ten items below had no exact ID/title duplicate; do not allocate permanent SIS-LIT IDs pending historical 2026-10-09 to 2026-10-23 reconciliation, and do not split a preprint/conference lineage.

**Scientific identity:** Agent/Workflow/Memory/Skill/Harness are implementations, not SIS primitives. Primary programs SCF/SDR/ASR; use `ROUTING_ABSTAIN` where primary system-mechanism estimand is not warranted. Cross-cutting CSCI requires explicit interaction/moderation, BGT benchmark/governance. Thin Framework capabilities remain replaceable.

| Candidate | Study | Primary | Cross | Claim evidence ceiling | Reading |
|---|---|---|---|---|---|
| 01 | [Messier: A High-Resolution Corpus for Cross-Benchmark Agent Evaluation](https://aclanthology.org/2026.emnlp-main.1398/) | ROUTING_ABSTAIN | BGT | CL1; counterfactual rescoring local measurement contrast (not mechanism) | Must Read |
| 02 | [STAGE: Diagnosing Semantic Transfer at Grounded Execution in Embodied Agents](https://aclanthology.org/2026.findings-emnlp.1148/) | SCF | BGT | CL1; local CL2 candidate for instruction-swap intervention only | Must Read |
| 03 | [SkillAlign: Aligning Skill Interfaces for LLM-based Agents](https://aclanthology.org/2026.emnlp-main.2565/) | SCF | BGT | CL1; local CL2 candidate | Must Read |
| 04 | [LegalWorld: A Life-Cycle Interactive Environment for Legal Agents](https://aclanthology.org/2026.emnlp-main.390/) | SDR | BGT | CL1 descriptive; no independent mechanism promotion | Must Read |
| 05 | [Asuka-Bench: Benchmarking Code Agents on Underspecified User Intent and Multi-Round Refinement](https://aclanthology.org/2026.findings-emnlp.1548/) | SDR | BGT | CL1; no CL2 promotion | Must Read |
| 06 | [CoEmbod: A Long-Horizon Benchmark for Multi-Agent Embodied Cooperation with Diverse Inter-Agent Dependencies](https://aclanthology.org/2026.emnlp-main.2247/) | SDR | CSCI/BGT | CL1 | Worth Skimming |
| 07 | [CUADebug: Diagnosing and Repairing Computer-Use Agent Failures](https://aclanthology.org/2026.findings-emnlp.530/) | SDR | BGT | CL1; local CL2 candidate conditional on matched rerollout | Must Read |
| 08 | [TopoCurate: Modeling Interaction Topology for Tool-Use Agent Training](https://aclanthology.org/2026.findings-emnlp.1969/) | ASR | BGT | CL1; no causal mediation promotion | Must Read |
| 09 | [OpenResearcher: A Fully Open Pipeline for Long-Horizon Deep Research Trajectory Synthesis](https://aclanthology.org/2026.emnlp-main.42/) | SCF | BGT | CL1; performance transfer only | Worth Skimming |
| 10 | [AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents](https://aclanthology.org/2026.emnlp-demos.52/) | SDR | BGT | CL1; demo evidence ceiling | Worth Skimming |

## Evidence and provisional ClaimRecord coding
### SIS-CAND-20261102-01 — Messier: A High-Resolution Corpus for Cross-Benchmark Agent Evaluation

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.1398/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 统一不同 Benchmark 的任务、执行器和验证器记录，并研究评分规则如何改变系统排序。
- **Reported evidence:** 957,611 条记录、30 个 Benchmarks、745 个 Agents、11,891 个 Tasks、74,263 个 Verifiers；不同多验证器规则的反事实重评分可改变排序，能力评分与 Epoch 指数 Spearman ρ=0.84。
- **Limitations/confounders:** 异质历史数据和验证器质量不同；重评分不是对系统实施新的因果干预；相关性不能证明能力测量的独立 Gold 有效。
- **Scientific routing:** Primary `ROUTING_ABSTAIN`; Cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; primary estimand `VERIFIER_SCORING_RULE_CONDITIONAL_AGENT_RANKING_VALIDITY`.
- **Evidence maturity:** CL1; counterfactual rescoring local measurement contrast (not mechanism); identification I1/I2-local measurement; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Measurement instrument; negative ranking-boundary evidence. **Boundary variables:** 验证器组合、all-pass 规则、任务领域、模型版本、执行预算.
- **SIS impact:** SHARPENS：强迫将 System Capability Frontier 与评分语义/验证器有效性分开；归入 BGT/MEAS，不构成第四 Primary。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-02 — STAGE: Diagnosing Semantic Transfer at Grounded Execution in Embodied Agents

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1148/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 固定视觉观察与系统状态，改变指令语义，直接测量语义已被解析时是否传递至连续动作控制。
- **Reported evidence:** LIBERO 目标和关系交换中语义恢复分别 100.0%、95.8%，OpenVLA 动作敏感性只有 6.8%、7.7%；另有 1,000 个组合和时序反事实，动作敏感性 6.1%。
- **Limitations/confounders:** 语义恢复与连续动作的匹配测量依赖阈值及物理仿真；低敏感性不自动意味着真实任务全部失败；未识别内部因果中介。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/ID/MEAS/BT`; primary estimand `FIXED_OBSERVATION_SEMANTIC_INTERVENTION_ACTION_SENSITIVITY`.
- **Evidence maturity:** CL1; local CL2 candidate for instruction-swap intervention only; identification I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Negative/boundary; semantic-to-action measurement. **Boundary variables:** 视觉状态、语义替换、连续动作幅度、控制器与物理任务.
- **SIS impact:** SHARPENS：语义理解与可执行能力分离；Representation Construct Validity 新 Fixture，不修订 Core。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-03 — SkillAlign: Aligning Skill Interfaces for LLM-based Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.2565/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 固定任务、执行器和候选技能，只切换完整说明、提示、摘要、工作流或不暴露等技能接口形式。
- **Reported evidence:** 在 ALFWorld 与 SkillsBench 上发现接口形式显著改变任务成功与上下文成本；紧凑 top-k 可能优于完整技能库注入，重放式学习显示自适应选择仍远离 Oracle。
- **Limitations/confounders:** 暴露形式会改变有效输入预算及信息密度；有限任务/技能分布；不应将接口作用归因于 Skill 内容本身或跨执行器机制不变性。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/ID/MEAS/BT`; primary estimand `FIXED_SKILL_CONTENT_EXPOSURE_INTERFACE_CAUSAL_EFFECT`.
- **Evidence maturity:** CL1; local CL2 candidate; identification I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Mechanism candidate; interface boundary. **Boundary variables:** 技能长度、接口压缩损失、模型上下文预算、技能适用性.
- **SIS impact:** SUPPORTS：SCF 中的 Representational Interface Effect；精细化 Skill Packaging 与能力之间的识别。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-04 — LegalWorld: A Life-Cycle Interactive Environment for Legal Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.390/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 将法律诉讼五阶段建成共享状态的因果连接过程，不再在每个子任务重置到独立真值。
- **Reported evidence:** 使用 75,309 对判决作为来源，五阶段七子场景；217 名法律背景评估者贡献 18,992 条评分；整体评分差距 4 分内的模型在单阶段可相差 15 个归一化点。
- **Limitations/confounders:** 法律模拟环境中的因果连锁由生成器定义；评估者程序忠实性不直接代表现实法律结果；反思 Skill 与环境作用组合。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/EG/MEAS/BT`; primary estimand `CROSS_STAGE_STATE_DEPENDENCE_LONG_HORIZON_CAPABILITY_GAP`.
- **Evidence maturity:** CL1 descriptive; no independent mechanism promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Benchmark instrument; state-history boundary. **Boundary variables:** 跨阶段历史、案件制度、时间跨度、前期错误不可逆性.
- **SIS impact:** SHARPENS：SDR 历史依赖与跨阶段后果；现实部署迁移未证明。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-05 — Asuka-Bench: Benchmarking Code Agents on Underspecified User Intent and Multi-Round Refinement

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1548/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 让欠完整用户需求经过网页生成—实际浏览器测试—自然语言反馈—多轮修订的闭环展开。
- **Reported evidence:** 50 个网站任务、784 项评价准则、2,402 个期望结果；8 个模型和 2 个执行框架；加权通过率跨模型相差 38 个百分点，最强模型三轮后只完成 52%。
- **Limitations/confounders:** 用户反馈来自 User LLM，可能偏离真实用户意图；不同轮次项目状态、算力和反馈同时改变；真实主观满意度未被证明。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/DR/MEAS/EG/BT`; primary estimand `UNDERSPECIFIED_INTENT_FEEDBACK_CONDITIONAL_REFINEMENT_EFFECT`.
- **Evidence maturity:** CL1; no CL2 promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Measurement and dynamic user-feedback boundary. **Boundary variables:** 规范欠完整程度、反馈质量、浏览器验证有效性、轮次预算.
- **SIS impact:** SHARPENS：用户意图动态演化和系统恢复；现有 SDR + MEAS 充分表达。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-06 — CoEmbod: A Long-Horizon Benchmark for Multi-Agent Embodied Cooperation with Diverse Inter-Agent Dependencies

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.2247/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 在长时程具身模拟中分别构造空间分配、并行约束与失败恢复三类组件依赖，并联合测量任务成功、合作忠实性及资源效率。
- **Reported evidence:** 155 项人工设计任务、40 个场景、10,845 个对象；作者称最强被测多模态执行流程成功率仅 20.23%。
- **Limitations/confounders:** 模拟任务和人工依赖设计限制外推；低成功率不单独识别某类协作机制的因果贡献；缺少正交任务/组织对照。
- **Scientific routing:** Primary `SDR`; Cross-cutting `CSCI/BGT`; Framework `TD/IA/MEAS/BT`; primary estimand `INTER_AGENT_DEPENDENCY_CONDITIONAL_COOPERATIVE_RECOVERY_VALUE`.
- **Evidence maturity:** CL1; identification I1; transport T0; no automatic whole-paper CL2/CL3.
- **Evidence role:** Benchmark instrument; dependency and failure boundary. **Boundary variables:** 组件间前置约束、时间协调、可观察性、恢复资源.
- **SIS impact:** SUPPORTS：SDR/CSCI 的多组件依赖测量；不是 Multi-Agent primitive。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-07 — CUADebug: Diagnosing and Repairing Computer-Use Agent Failures

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.530/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 联合低层 GUI 动作、前后截图和人工根因标签，定位故障再重新执行，避免将最终失败位置等同于根因。
- **Reported evidence:** 204 条 OSWorld 失败轨迹、30 个故障子类型；Gemini 2.5 Pro 的 Tag+Step exact 从 11.1% 到 19.4%；单次重新执行恢复率从 13.89% 到 29.86%。
- **Limitations/confounders:** 人工标签不等于可干预因果真值；某些重跑比较由人工标注固定重启点，诊断器与重试流程的独立效应仍需拆分。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/ID/EG/MEAS/BT`; primary estimand `TRAJECTORY_DIAGNOSIS_GUIDED_REEXECUTION_RECOVERY_EFFECT`.
- **Evidence maturity:** CL1; local CL2 candidate conditional on matched rerollout; identification I1/I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Failure recovery; local intervention candidate. **Boundary variables:** 界面状态、截图粒度、恢复起点、重试次数、模型版本.
- **SIS impact:** SHARPENS：故障定位和修复净收益可拆分；建议反事实重启点冻结 Fixture。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-08 — TopoCurate: Modeling Interaction Topology for Tool-Use Agent Training

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1969/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 不用最终成功/失败筛选训练样本，而是从多次尝试形成的执行交互拓扑中选择含恢复路径、多样策略和高错误分支的示例。
- **Reported evidence:** 在 BFCLv3、Tau2 Bench 作者报告 SFT +4.2%、RL +6.9% 的收益（原文未在摘要澄清是绝对点还是相对幅度，此处仅按报告数值记）。
- **Limitations/confounders:** 样本选择会改变难度、token、训练分布及奖励信噪比；拓扑指标与真实训练机制的中介作用未单独识别。
- **Scientific routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `DR/TD/MI/ID/MEAS/BT`; primary estimand `INTERACTION_TOPOLOGY_CONDITIONAL_TRAINING_EXAMPLE_SELECTION_VALUE`.
- **Evidence maturity:** CL1; no causal mediation promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Regulation/operator selection; mechanism candidate. **Boundary variables:** 任务分支比、失败与恢复密度、训练预算、模型能力、评估域.
- **SIS impact:** SHARPENS：ASR 训练数据/任务选择策略与最终收益的独立对照。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-09 — OpenResearcher: A Fully Open Pipeline for Long-Horizon Deep Research Trajectory Synthesis

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.42/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 将文献语料初始化和多轮 search/open/find 轨迹生成分离，在可记录、可复现的离线环境生成长轨迹。
- **Reported evidence:** 1,500 万文档，超过 97,000 条训练轨迹；30B-A3B 模型在 BrowseComp-Plus 达 54.8%，相较基础模型提高 34.0 个百分点。
- **Limitations/confounders:** 语料中答案存在性、检索质量和训练分布均影响成绩；离线文献与真实网络的时效、来源权威及引证充分性不同；多组件共同改变。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/TD/EG/MEAS/BT`; primary estimand `OFFLINE_RESEARCH_TRAJECTORY_SYNTHESIS_HELDOUT_CAPABILITY_EFFECT`.
- **Evidence maturity:** CL1; performance transfer only; identification I1; transport T2-performance-only; no automatic whole-paper CL2/CL3.
- **Evidence role:** Implementation plus training/measurement instrument. **Boundary variables:** 文献覆盖、检索工具、答案泄漏、训练量、评估独立性.
- **SIS impact:** SUPPORTS：SCF 科研系统的训练环境机制；实际科学 Claim 证据治理仍须独立评价。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-10 — AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 System Demonstrations (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-demos.52/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 提供 Detect–Attribute–Recover–Rerun 可重放诊断闭环和可选的去敏故障记忆库。
- **Reported evidence:** Who When 的严格 agent+step 定位准确率 28.8% vs 21.7% 单次分析基线；GAIA 73 次失败中单次重跑修复 13 项，对照为 4–6 项；总体准确率 55.8% 至 63.6%。
- **Limitations/confounders:** 系统演示论文不等于多中心机制验证；诊断器、重试策略和先验记忆共同变化；受控复制集有限。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/DR/ID/EG/MEAS/BT`; primary estimand `MULTI_TURN_ROOT_CAUSE_DEBUGGING_GUIDED_RERUN_RECOVERY_VALUE`.
- **Evidence maturity:** CL1; demo evidence ceiling; identification I1; transport T0; no automatic whole-paper CL2/CL3.
- **Evidence role:** Implementation + initial recovery comparison. **Boundary variables:** 故障分类质量、诊断深度、重启点、重试预算、日志脱敏与遗忘.
- **SIS impact:** IMPLEMENTATION：已有 SDR/EG 能承载；建议作为多步诊断与真实重跑实施基准。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.


## Separate technical and community analyses
Project repositories and community posts were discovery aids only; no independently reproduced new community findings were used to promote CL. AgentDebugX is a **peer-reviewed demonstration**, not equivalent to a controlled mechanism-identification study.

## P0 audit linkage
[SIS P0 Re-Audit 2026-11-02](../evidence-map/audits/SIS_P0_Reaudit_2026-11-02.md): 059/077/096; nine claim-level first-coder decisions. Independent second coder/adjudication remain PENDING. Chronicle workshop metadata is the canonical current version of its September preprint; update lineage in the Registry/Queue, not new Study.

## Five integrated SIS implications
1. **Scoring rules can reorder measured agent capability:** require rescoring sensitivity and verifier provenance (MESSIER).
2. **Semantic decoding need not reach motor/action control:** fixed-state semantic swaps isolate a representational-execution gap (STAGE).
3. **Skill benefit is conditional on presentation interface and resource budget:** separate packaged knowledge content from exposure policy (SkillAlign).
4. **Long-horizon and feedback phases are scientifically distinct:** stateful legal, code, embodied and GUI failure/recovery metrics are not one-shot success (LegalWorld/Asuka/CoEmbod/CUADebug).
5. **Optimization/training sample selection needs unbiased, trajectory-grounded evaluation:** outcome-filtered datasets and synthetic research rollouts may create selection/coverage bias (TopoCurate/OpenResearcher).

## Proposed experiment and benchmark deltas

| Priority | Fixture | Independent contrast and outcome |
|---|---|---|
| P0 | Verifier Rule × Same Agent Outputs | counterfactual rescoring, ranking stability, independent task Gold |
| P0 | Fixed Scene × Semantic Swap × Action | semantic recovery vs native action sensitivity and task consequences |
| P0 | Fixed Skill × Exposure Interface × Frozen Executor | utility, context budget, constraint fidelity, stress OOD |
| P0 | Failure Locus × Cut-point Replay | diagnosis vs live rerun, matched tool/state and cost |
| P0 | Memory Over/Under-use × Independent Gold | appropriate memory influence, directional intervention value |
| P0 | Long-horizon State Dependency × Feedback | cross-stage propagation, revision/recovery, budget and viability |
| P1 | Training Trajectory Topology × Data Budget | selected sample quality and truly held-out performance |
| P1 | Offline Research Corpus × Live Source | answer leakage, provenance validity, live-domain transport |

**Formal SIS Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA`; secondary `BENCHMARK_DELTA`; `SPEC_REVISION_CANDIDATE=NO`; `ScientificCoreDelta=0`. There is *genuine measurement pressure*, especially ranking construct validity and semantic-to-action construct gap, **but no uncovered estimand or irreducible scientific capability**. Do not revise SIS core.
