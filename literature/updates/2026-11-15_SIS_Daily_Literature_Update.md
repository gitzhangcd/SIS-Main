# SIS Daily Literature Update｜2026-11-15

**Authority:** SIS v0.3.1 Master Specification; Literature Registry v1.3; SIS Literature Evidence Map P0; ClaimRecord Schema; P0 Audit Queue. **Scientific Core FROZEN**.
**Discovery date:** 2026-11-15 (Asia/Shanghai). Official arXiv cs.AI latest bulletin: **Friday 2026-11-13**, 537 total listings / 113 new submissions (not 537 new studies). The new preprints below were FIRST SUBMITTED 2026-11-10–12 and are DELAYED-DISCOVERY/INDEXING candidates, not newly posted on Sunday.
**Scope and integrity:** Primary arXiv/ACL records checked; AACL 2026 venue 2026-11-06–10, one new delayed-discovery **peer-reviewed survey**. Targeted OpenReview/NeurIPS/ICML/ACL/EMNLP searches yielded no independently verified, stronger and nonduplicate replacement. All 10 candidate titles + identifiers checked against current Registry before admission. Existing 2026-11-14 candidate ledger preserved. Community analyses = DISCOVERY_ONLY; no claimed independent reproduction. arXiv workshop/conference statements not treated as proceedings unless matched.
**Limitations:** Most new papers screened at official abstract; EGE and selected prior audit studies examined in original HTML. Not all experimental appendices independently audited. Candidate labels are NOT CL2/CL3 adjudications, and not permanent SIS-LIT IDs.

## Peer-reviewed / late-indexed archive
### SIS-CAND-20261115-01｜Is There a Dr. House in the Machine? Towards Clinical and Diagnostic Reasoning in LLM-based Medical Agents — **Must Read**
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-aacl.82/; 2026-11 AACL-IJCNLP Findings; discovered 2026-11-15; **PEER_REVIEWED_SURVEY**; unique study candidate (no permanent ID).
- **Core novelty:** 综述围绕推理范式、组织架构、工具、自治程度与具身性五维检视医疗 Agent 的诊断表现是否具备临床因果与知识论基础；不把 Agent 架构当科学原语。
- **Evidence and limitations:** 正式 AACL-IJCNLP 2026 Findings 归档，但属叙述综述而非受控对照或新临床试验；引用研究存在模型、疾病和流程异质性。
- **SIS routing:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `MEAS/ID/EG/BT`; primary estimand `CLINICAL_DIAGNOSTIC_OUTPUT_VS_CAUSAL_EPISTEMIC_PROCESS_GAP`.
- **Claim maturity:** CL0 evidence synthesis (no new independent causal estimate); identification I0; transport T0; evidence role `SYNTHESIS / MEASUREMENT_AGENDA`; claim nature `REVIEW / IDENTIFICATION_GAP`.
- **Boundary variables:** 临床决策环节、医生工作流、病例组合、参考真值、临床结局、风险和责任边界。
- **SIS effect:** SHARPENS SIS-MED 的 Measurement 与 Evidence Independence；提示诊断输出正确不等于过程或患者效用有效。 **Reading:** Must Read. Proposed fixture: 临床病例固定 × 外部独立 Gold × 决策轨迹 × 医生复核 × 结局约束。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

## Recent preprints — 9 independent new candidates
### SIS-CAND-20261115-02｜Together Compiler: Continual Compilation for AI Inference — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14681; 2026-11-10 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 将持续推理编译的候选搜索与常驻执行引擎结合，以分层测量减少发动引擎的开销，同时在不同并行配置之间选择优化路线；面向真实生产负载。
- **Evidence and limitations:** 报告在某些工作负载达 1.7× 对手工 Megakernel 和至多 2.6× 对开源引擎的吞吐增益，并称服务生产 token；最大值不是平均因果效应，硬件/批量/内核与负载变化相互混杂。
- **SIS routing:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/MI/TD/MEAS/ID/BT`; primary estimand `CONTINUAL_COMPILER_MEASUREMENT_FIDELITY_THROUGHPUT_POLICY_VALUE`.
- **Claim maturity:** CL1 reported production performance; local CL2 candidate; identification I1/I2-local; transport T2 performance-only claimed; evidence role `IMPLEMENTATION / MEASUREMENT_FIDELITY_BOUNDARY`; claim nature `IMPLEMENTATION / BOUNDARY`.
- **Boundary variables:** GPU 与 kernel、MoE 路由、batch、持续负载、测量保真度、启动成本、部署配置。
- **SIS effect:** SHARPENS ASR 选择策略的测量保真度与资源条件，但新编译器属于可替换实现。 **Reading:** Must Read. Proposed fixture: 固定硬件/负载 × tiered engine 开关 × 候选搜索预算 × 测量误差 × 端到端吞吐。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-03｜SynthCorp: A Platform for Creating Benchmarks for Data Agents — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14765; 2026-11-10 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 以带时间线的业务事件生成关系库、文档与目录；保留事件执行日志，自动生成可执行 Gold 并进行因果数据溯源。
- **Evidence and limitations:** 7 个 data estates、256 项任务、5 个领域，覆盖最多千张表；确定性一致性检查和自动真值仅保证模拟器内部自洽，不能替代外部业务真值。
- **SIS routing:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `TD/MI/EG/MEAS/ID/BT`; primary estimand `EVENT_LOG_DERIVED_EXECUTABLE_GOLD_SEMANTIC_VALIDITY`.
- **Claim maturity:** CL1 synthetic benchmark instrument; identification I1; transport T0; evidence role `BENCHMARK_INSTRUMENT / GOLD_CONSTRUCT`; claim nature `MEASUREMENT / IMPLEMENTATION`.
- **Boundary variables:** 事件模拟规则、文档—表一致性、生成任务分布、隐含因果规则、数据规模。
- **SIS effect:** SHARPENS MEAS/EG 的 event-log Gold，但必须有外部语义审查及未见事件迁移。 **Reading:** Must Read. Proposed fixture: Synthetic Gold × 独立专家判定 × 注入错误事件 × 跨数据资产一致性。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-04｜Robust Task-Aware State Estimation from Pre-trained Perception — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14781; 2026-11-10 v1; discovered 2026-11-15; **PREPRINT (author states NeurIPS 2026; proceedings not independently matched)**; unique study candidate (no permanent ID).
- **Core novelty:** 提出基于感知模型概率的最小信念状态集合 MBSθ，不将最大概率状态强行当真值；用任务约束筛选状态并在规划环节消费不确定性。
- **Evidence and limitations:** 给出无约束场景的计算性质，并报告实验规划收益；结论依赖概率校准、特征依赖与状态约束，不能将覆盖概率等同于真实环境安全保证。
- **SIS routing:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/MI/DR/MEAS/ID/BT`; primary estimand `BELIEF_MASS_STATE_SET_VS_POINT_ESTIMATE_TASK_VIABILITY`.
- **Claim maturity:** CL0 conditional algorithmic guarantee / CL1 experiments; identification I0/I1; transport T0; evidence role `MEASUREMENT / BOUNDARY`; claim nature `BOUNDARY / IMPLEMENTATION`.
- **Boundary variables:** θ 阈值、VLM 校准、状态相关性、观测缺失、任务规划 horizon、符号约束。
- **SIS effect:** SHARPENS SDR 的部分可观测状态与 Viability 测量；未发现缺失 Core Estimand。 **Reading:** Must Read. Proposed fixture: 点估计 vs belief set × 感知校准 × 未观测状态 × 任务安全性。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-05｜RSI-PDEbench: A Benchmark for Self-Improving Agents in PDE Solving — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14949; 2026-11-11 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 1,001 个 PDE 案例、42 种模板，分无噪声、50% RMS 噪声和未知模板/参数范围 Hard-OOD；用方程残差与 L2 反馈验证候选，并门控政策/记忆更新。
- **Evidence and limitations:** 四模型中作者报告相对单次运行较大相对通过率增益、对原生 Harness 3.0–19.6% 相对增益及减少 46.9% 记录的模型调用；组合模块与任务适配未正交，仍非真实独立科学发现证明。
- **SIS routing:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/MI/EG/MEAS/ID/BT`; primary estimand `VALIDATION_GATED_PDE_SELF_IMPROVEMENT_NOISY_OOD_NET_VALUE`.
- **Claim maturity:** CL1 package performance; local CL2 candidate; identification I1/I2-local; transport T2 performance-only; evidence role `BENCHMARK / IMPLEMENTATION / BOUNDARY`; claim nature `IMPLEMENTATION / TRANSPORT_GAP`.
- **Boundary variables:** PDE 家族、噪声强度、方程模板 OOD、数值离散、模型预算、验证器正确性。
- **SIS effect:** SHARPENS ASR 的 noisy/OOD 校验与自改进回归门控；不将 Harness 当独立纲领。 **Reading:** Must Read. Proposed fixture: 残差验证 × 更新门控 × 独立数值 Gold × 模板 OOD × 等计算预算。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-06｜Termination Lag: Coding Agents Solve Early but Stop Late — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.14960; 2026-11-11 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 测试执行过程中每个不同代码补丁，区分首次正确时间与最终停机时间；38–82% 成功轨迹的第一轮源码修改即正确，但随后大量额外步骤用于校验和探索。
- **Evidence and limitations:** 五模型、两执行框架、三 SWE-bench 数据集；部分模型成功轨迹中后续步骤中位比例达 35–60%，1–8% 实际撤销正确补丁。对最终成功条件选择会产生幸存者偏倚，尚没有随机停止干预。
- **SIS routing:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/TD/MEAS/ID/EG/BT`; primary estimand `FIRST_CORRECT_PATCH_TO_STOP_POLICY_COST_REGRESSION_EFFECT`.
- **Claim maturity:** CL1 trace audit; stopping treatment untested; identification I1; transport T1; evidence role `NEGATIVE_BOUNDARY / MEASUREMENT`; claim nature `NEGATIVE / BOUNDARY`.
- **Boundary variables:** 模型、任务、patch 测试器、验证时长、检验成本、停机时点、错误回滚。
- **SIS effect:** SHARPENS ASR 的 stopping estimand：探索更多不总有正价值；需要随机对照的 stop/continue。 **Reading:** Must Read. Proposed fixture: 同一首次正确 patch 状态 × STOP/CONTINUE 随机续跑 × 资源成本 × 失效回归。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-07｜guardscope: Measuring Which Actions Runtime Controls Check in LLM Agent Systems — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.15223; 2026-11-11 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 将控制器检查范围和内核层真实执行动作逐条对账；静态推断15类行动路径，实测8种部署拓扑下动作是被检查、绕过还是阻止。
- **Evidence and limitations:** 已在两个 Harness 和实际控制器上测试；日志与内核对账能验证覆盖面，但覆盖到动作不代表理解动作，更不保证最终安全结果。
- **SIS routing:** Primary `SDR`; cross-cutting `CSCI/BGT`; Framework `TD/IA/EG/MEAS/ID/BT`; primary estimand `RUNTIME_CONTROL_TOPOLOGY_KERNEL_VERIFIED_ACTION_COVERAGE`.
- **Claim maturity:** CL1 instrumentation, not safety-effect identification; identification I1/I2 measurement intervention; transport T1; evidence role `MEASUREMENT / NEGATIVE_BOUNDARY`; claim nature `MEASUREMENT / BOUNDARY`.
- **Boundary variables:** 工具/非工具执行路径、gateway 位置、容器内核证据、部署拓扑、未观测副作用。
- **SIS effect:** SHARPENS SDR/EG 的 action-level observability；可直接作为 Evidence Integrity Fixture。 **Reading:** Must Read. Proposed fixture: 固定任务 × 八类 topology × action-path ground truth × control logs × bypass negative controls。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-08｜MemCredit: From Relevance to Utility for Decision-Time Memory in Long-Horizon Web Agents — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.15600; 2026-11-11 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 在固定 token 预算下先用相关性召回候选，再用受控反事实估计单条记忆对当前行动的条件性净贡献，蒸馏轻量预测器选择真正有用记忆。
- **Evidence and limitations:** ALFWorld 500-token 历史记忆下报告 SR@50=86.57，BM25=65.67；局部曝光效应依赖状态、上下文与执行策略，不能直接解释为跨策略的永久记忆因果价值。
- **SIS routing:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/DR/TD/MEAS/ID/BT`; primary estimand `STATE_POLICY_CONDITIONAL_MEMORY_EXPOSURE_MARGINAL_DECISION_VALUE`.
- **Claim maturity:** CL1 performance; local CL2 candidate; identification I2-local/T policy-confounded; transport T1; evidence role `MECHANISM_CANDIDATE / BOUNDARY`; claim nature `BOUNDARY / IMPLEMENTATION`.
- **Boundary variables:** memory token 预算、状态、ReferenceContext、行动策略、记忆交互、任务分布、token cost。
- **SIS effect:** SHARPENS SCF/CSCI；与前一日 CoReMem 属互补独立研究，需区分历史片段选择与未来任务效用，不合并。 **Reading:** Must Read. Proposed fixture: Memory exposure × policy × state × matched tokens × future unseen tasks。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-09｜Evidence-Governed Adoption of Self-Generated Updates in Autonomous AI Agents — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.16378; 2026-11-12 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 分离候选生成和确认性采用；冻结候选，在独立配对审计上做准入和既有能力非劣效约束，使用独立参考校准应对评价器乐观偏差，并用桥接试验替换版本参照。
- **Evidence and limitations:** 提供有限样本条件边界与 Monte Carlo 压力测试，作者明确尚未执行真实 Agent 受控实验；形式保证假设评分有界、样本新鲜与参照有效。
- **SIS routing:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/EG/ID/MEAS/BT`; primary estimand `FRESH_PAIRED_AUDIT_CALIBRATED_UPDATE_ADMISSION_RETENTION_VALUE`.
- **Claim maturity:** CL0 conditional statistical theory / CL1 stylized Monte Carlo; identification I0/I1 simulated; transport T0; evidence role `THEORETICAL_ADMISSION / MEASUREMENT_GOVERNANCE`; claim nature `BOUNDARY / THEORY`.
- **Boundary variables:** 候选自适应选择、评价器漂移、独立样本、版本链、非劣效边界、分布迁移、更新成本。
- **SIS effect:** SHARPENS ASR/EG 的更新准入设计，不能因数学形式而宣称全场景安全；核心已有表达。 **Reading:** Must Read. Proposed fixture: 真实候选提议 × 冻结确认集 × 偏差评价器 × 独立 Gold × 版本桥接。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

### SIS-CAND-20261115-10｜ReA-Bench: Benchmarking Responsible Agent Auditing — **Must Read**
- **StudyVersionRecord:** https://arxiv.org/abs/2611.16493; 2026-11-12 v1; discovered 2026-11-15; **PREPRINT**; unique study candidate (no permanent ID).
- **Core novelty:** 基于生产/红队轨迹构建六个梯度：安全知识、轨迹内矛盾、长上下文证据检索、来源核验、间接诱导、缺失信息，并包括合法但表面可疑的负例。
- **Evidence and limitations:** 设置剪短轨迹、补充信息的配对版本检查审计员是否真正利用证据；人工选择/改写可能偏置，静态审计结果不是上线风险降低的因果效应。
- **SIS routing:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; primary estimand `TRAJECTORY_AUDIT_MISSING_INFORMATION_SOURCE_VERIFICATION_RECALL_FALSE_POSITIVE_FRONTIER`.
- **Claim maturity:** CL1 benchmark construction, not intervention validation; identification I1; transport T1; evidence role `MEASUREMENT_INSTRUMENT / NEGATIVE_BOUNDARY`; claim nature `MEASUREMENT / BOUNDARY`.
- **Boundary variables:** 真实/模拟轨迹比例、审计信息可见性、风险标签、合法行为负例、误报成本、工具来源。
- **SIS effect:** SHARPENS MEAS/EG 的 false-positive 和 missingness 分解，提供优先 P0 审计任务。 **Reading:** Must Read. Proposed fixture: paired full/short trajectory × missing evidence supplied × independent risk Gold × FPR/Recall。
- **Governance:** abstract-level or explicitly stated method verification only; second coder/adjudication PENDING; no automatic CL2/CL3 promotion.

## Technical / community analyses
No separately reproduced community analysis admitted to scientific evidence. All such sources remain DISCOVERY_ONLY.

## Version/duplicate reconciliation
- The October archive is not a new initial publication merely because surfaced on 2026-11-15; the AACL survey is a late-discovery peer-reviewed **synthesis**.
- No overlap with 2026-11-14 (CoReMem is a prospective **future-task** cost study; today's MemCredit is a **decision-time conditional memory-exposure** study, distinct methods and identity).
- 2026-10-09–23 historical candidates remain a known global lineage reconciliation backlog; no false assertion that all permanent+daily candidates are globally deduplicated.

## P0 claim-level backlog progress
First-coder re-audit of existing SIS-LIT-008 / 053 / 056: **nine atomic claims**; paper-level CL labels cannot be inherited; **zero confirmed CL2/CL3 upgrades, zero T3/T4**. Detailed audit: `literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-15.md`.

## Synthesis and P0 experiment priorities
1. **STOP / CONTINUE**: termination lag → stopping policy must be valued relative to compute and risk of undoing correct work.
2. **CONTROL REACH**: kernel action coverage ≠ authorization validity ≠ deployment safety; audit actual action paths, not gateway logs alone.
3. **MEMORY EXPOSURE**: utility depends on state, policy and reference context; a frequent/relevant memory is not necessarily causally useful; compare future-task and decision-time valuations.
4. **UPDATE ADMISSION**: repeated candidate exploration needs fresh independent paired audits, non-inferiority of retained abilities, calibrated evaluators, and version bridge tests.
5. **GOLD REPRESENTATION**: event-log synthetic executable Gold and clinical diagnostic rubric both require external semantic validation; partial observability and real-world ground truth constrain transport.

| Priority | Fixture | Null / kill condition |
|---|---|---|
| P0 | STOP vs CONTINUE randomized at first verified correct patch | No net policy gain or early test oracle non-independent |
| P0 | Kernel action-path × topology × control audit | Gateway inspected logs do not cover true executed actions |
| P0 | Memory utility exposure × matched token/policy/state | Relevant memory marginal effect null or reverses across states |
| P0 | Frozen candidate × fresh independent Gold × evaluator calibration | Positive apparent update disappears / capability regression |
| P0 | Event-log Gold × independent semantic domain Gold | Simulation self-consistency fails external task meaning |
| P0 | Robust belief-set θ × calibration × planning safety | Claimed belief coverage collapses under missingness/OOD |
| P1 | PDE noise/OOD × gate on/off × fixed computation | Package benefit vanishes against equal compute/native baselines |

## Formal SIS Impact Decision
**Primary: MEASUREMENT_IDENTIFICATION_DELTA.** Secondary: **BENCHMARK_DELTA**. **CorePressure: WATCH** (stopping, unobserved action paths and long-lived update validity); **ScientificCoreDelta=0**; **SPEC_REVISION_CANDIDATE=NO**.
These are real pressures on measurable estimands, independent evaluators, action observability and causal identification, but are still expressible within SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG. No demonstrated uncovered first-principles scientific object or irreplaceable capability.