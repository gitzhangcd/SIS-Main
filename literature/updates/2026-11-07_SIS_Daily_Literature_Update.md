# SIS Daily Literature Update｜2026-11-07

基准：SIS v0.3.1 FROZEN、Registry v1.3、P0 ClaimRecord v0.1。上一次更新 2026-11-06。arXiv cs.AI 2026-11-06 列表总计 361 条，其中首次新投稿分类 75 条；入选的十项均于 11-04 或 11-05 首次提交，且本次与 Registry arXiv ID 精确去重。未检出足以独立确认的新同行评审存档版本；社区评论 DISCOVERY_ONLY。永久编号与历史 10 月 9–23 日候选仍待全局谱系对账。

## 10 项本期研究及科学语义

### 1. Benchmarks as Software: Terminal-Bench and the Case for Continuous Benchmarks｜Must Read

- Source: https://arxiv.org/abs/2611.08417（2026-11-05 v1；PREPRINT）。
- 核心创新与证据：审计Terminal-Bench 2.0发现约30%任务存在问题；2.1修订后准确率变化超过10个百分点、排名最大变化三位，时间预算改变Harness差距。
- SIS：Primary `ROUTING_ABSTAIN`；Cross-cutting `BGT`；Framework `MEAS/EG/ID/BT`；primary estimand `BENCHMARK_VERSION_BUDGET_CONDITIONAL_RANKING`；Claim/I/T `CL1/I1-I2local/T0`；Evidence Role `INSTRUMENT+NEGATIVE`。
- 识别、测量、迁移边界：人工门控修订有选择偏差；新评价器并非独立绝对Gold，任务修复和资源预算需正交控制。
- Impact：SHARPENS ROUTING_ABSTAIN/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 2. When Verification Is Not Agreement: Cross-Agent LLM-to-Dafny Formalization｜Must Read

- Source: https://arxiv.org/abs/2611.07073（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：96份临床试验文档；同模型独立抽取仅59.3%一致；强模型担任实施者或规范者时一致率分别53.0%与14.3%，且发现直接调用谓词的验证捷径。
- SIS：Primary `SCF`；Cross-cutting `CSCI/BGT`；Framework `MI/EG/MEAS/ID/BT`；primary estimand `ROLE_SWAP_FORMAL_SPECIFIER_IMPLEMENTER_AGREEMENT`；Claim/I/T `CL1/I2local/T1`；Evidence Role `NEGATIVE+BOUNDARY`。
- 识别、测量、迁移边界：形式正确不意味着独立重建或真实临床意图；角色对调改变组件能力；Workshop接收为作者声明，非正式存档。
- Impact：SHARPENS SCF/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 3. BabyTheorist: A Benchmark for Learning to Theorize the World from Observation Alone｜Must Read

- Source: https://arxiv.org/abs/2611.08177（2026-11-05 v1；PREPRINT）。
- 核心创新与证据：隐藏组合程序连续生成状态转移，训练时不暴露规则标签、任务身份及支持集；七种基线随课程复杂度升高持续落后。
- SIS：Primary `SCF`；Cross-cutting `BGT`；Framework `MI/TD/MEAS/ID/BT`；primary estimand `CONTINUAL_OBSERVATIONAL_COMPOSITIONAL_THEORY_INDUCTION`；Claim/I/T `CL1/I1/T0`；Evidence Role `INSTRUMENT+NEGATIVE`。
- 识别、测量、迁移边界：合成DSL及课程先验限定构念；不能当作真实科学发现或跨域机制迁移。
- Impact：SHARPENS SCF/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 4. Trust Responsive Runtime Authorization for Agentic AI with Empirical Characterization of Policy Behavior and Parameter Sensitivity｜Must Read

- Source: https://arxiv.org/abs/2611.06996（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：100条匹配Monte Carlo轨迹下非对称门控对突发退化迅速收紧；渐进退化下多数轨迹没有及时收权，20段中的15.9–18.9段处于过高权限。
- SIS：Primary `ASR`；Cross-cutting `CSCI/BGT`；Framework `DR/TD/MEAS/ID/BT`；primary estimand `ABRUPT_VS_GRADUAL_RISK_AUTHORITY_GATE_EFFECT`；Claim/I/T `CL1/I2local/T0`；Evidence Role `NEGATIVE_BOUNDARY+POLICY`。
- 识别、测量、迁移边界：后者为探索性事后试验； readiness人为构造，不是独立的真实信任Gold。
- Impact：SHARPENS ASR/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 5. Formalizing inverse problems in the age of AI: possibilities, pitfalls, and an invitation｜Must Read

- Source: https://arxiv.org/abs/2611.06962（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：AutoIP以Lean形式化逆问题与正则化理论；数学证明检查只保证形式陈述，对教科书条件过宽的案例展示规范核对必要性。
- SIS：Primary `ROUTING_ABSTAIN`；Cross-cutting `BGT`；Framework `MI/EG/MEAS/ID/BT`；primary estimand `FORMAL_THEOREM_NATURAL_INTENT_FIDELITY`；Claim/I/T `CL0-CL1/I0-I1/T0`；Evidence Role `CONSTRUCT_WARNING`。
- 识别、测量、迁移边界：方法论文及案例而非代表性失败率；证明有效和数学陈述符合原意须独立核查。
- Impact：SHARPENS ROUTING_ABSTAIN/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 6. Autonomous AI Agents Systematically Diverge From Human Preferences in Proof Formalization｜Worth Skimming

- Source: https://arxiv.org/abs/2611.06995（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：研究九个Lean合作项目、470万定义和六千余次提交，模拟Agent与人类选择证明缺口、中心节点和复杂目标的偏好不同。
- SIS：Primary `SCF`；Cross-cutting `CSCI/BGT`；Framework `IA/MI/MEAS/ID/BT`；primary estimand `HUMAN_AGENT_PROOF_PATH_PREFERENCE_GAP`；Claim/I/T `CL1/I1/T1`；Evidence Role `INTERACTION_BOUNDARY`。
- 识别、测量、迁移边界：历史人类行为不是最优Gold，模拟组件与人类资源不同；没有真实联合协作的因果效率试验。
- Impact：SHARPENS SCF/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 7. Adapting the Process of Adaptation: Darwinian, Lamarckian, and Agent-Directed Evolution in AI｜Worth Skimming

- Source: https://arxiv.org/abs/2611.07048（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：理论比较达尔文式、拉马克式与定向演化：当评价目标错设时，提高搜索强度可能更快收敛于错误目标。
- SIS：Primary `ASR`；Cross-cutting `BGT`；Framework `DR/MI/EG/ID/BT`；primary estimand `SEARCH_EFFORT_WITH_MISSPECIFIED_OBJECTIVE_REGULATION_VALUE`；Claim/I/T `CL0/I0/T0`；Evidence Role `THEORY+NEGATIVE`。
- 识别、测量、迁移边界：理论假设尚未实证推广为系统规律，须独立测量真实目标与代理指标。
- Impact：SHARPENS ASR/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 8. KDASO: Knowledge-Data Dual-Driven Automated Skill Optimization for Liability Adjudication Tasks｜Worth Skimming

- Source: https://arxiv.org/abs/2611.06972（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：最近裁决案例驱动技能更新，执行轨迹用于对齐改写，预算约束决定路由；作者报告相似概念转移改进8.96%。
- SIS：Primary `ASR`；Cross-cutting `BGT`；Framework `DR/MI/TD/EG/ID/BT`；primary estimand `SKILL_STALENESS_ALIGNMENT_ROUTING_COMPOSITE_VALUE`；Claim/I/T `CL1/I1/T2-performance`；Evidence Role `IMPLEMENTATION+TRANSFER`。
- 识别、测量、迁移边界：归纳、改写与路由共同变化，缺少独立机制中介；仅性能迁移不等于T3因果迁移。
- Impact：SHARPENS ASR/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 9. BlockLock: Reproducible LLM Inference with Fixed Batch Geometry｜Must Read

- Source: https://arxiv.org/abs/2611.06977（2026-11-04 v1；PREPRINT）。
- 核心创新与证据：固定受保护请求的计算几何，保留批量prefill；五种模型、三种GPU报告在改变批次同伴后输出及Top20 logits位级一致，延迟相对基线下降约53.5%–55%。
- SIS：Primary `SCF`；Cross-cutting `BGT`；Framework `MI/TD/MEAS/ID/BT`；primary estimand `BATCH_COMPANION_INVARIANT_BITWISE_REPLAY_COST`；Claim/I/T `CL1/I2local/T1`；Evidence Role `REPLAY_INSTRUMENT`。
- 识别、测量、迁移边界：仅具体部署、精度与kernel合同下成立；推理数值可复现不代表完整工具/外部状态可重放。
- Impact：SHARPENS SCF/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

### 10. When Bigger Becomes Brittle: Why Compression Hurts More as Language Models Scale｜Must Read

- Source: https://arxiv.org/abs/2611.07891（2026-11-05 v1；PREPRINT）。
- 核心创新与证据：对检索注意力头的消融损失进行被其他组件恢复与传至输出部分的分解；报告大模型补偿较弱，同等压缩伤害更明显。
- SIS：Primary `SCF`；Cross-cutting `CSCI/BGT`；Framework `MI/IA/MEAS/ID/BT`；primary estimand `MODEL_SCALE_COMPENSATION_RETRIEVAL_HEAD_DAMAGE`；Claim/I/T `CL1/I2local/T1`；Evidence Role `BOUNDARY+MECHANISM_CANDIDATE`。
- 识别、测量、迁移边界：仅特定注意力头与检索任务，比较损伤和架构尺度存在边界；尚非通用系统机制。
- Impact：SHARPENS SCF/BGT 的测量或机制边界，仍由现有科学对象表达；不自动产生科学纲领或 Core 变更。

## P0 Re-audit 增量

本轮重新审核 AgentGrad（SIS-LIT-018）、TrajDebug（054）、Reasoning as Gradient（108），共 9 条独立 Claim；[详细初审](../evidence-map/audits/SIS_P0_Reaudit_2026-11-07.md)。018 旧的整篇 CL2_CONFIRMED 记录因缺 claim-specific mediator 验证，重新标记为第二编码者待裁决，不自动继承。第二编码者、正式 CL2 晋升、T3/T4 仍 Pending。

## 5 个科学结论与可执行变更

1. **Benchmark maintenance debt:** 版本化Task/Oracle/Environment/Budget 联合管理，同一冻结执行器在2.0/2.1和不同超时预算重跑。
2. **Formal verification ≠ independent semantic agreement:** 临床试验 Specifier×Implementer 角色对照、绕过谓词的结构 Kill Test、独立医生 Gold。
3. **理论形成不等于规律记忆:** 持续隐藏规则流、课程跳级、无需可见标签的零样本组合迁移，作为 SCF Benchmark。
4. **自适应权限调节可能漏掉缓慢风险演变:** 渐进/突发退化×阈值×观察延迟×越权成本实验。
5. **重放与组件补偿边界:** 批处理数值确定性并不等于外部工具可重放；模型尺度和隐性补偿需受控扰动。

## Formal Impact Decision

**MEASUREMENT_IDENTIFICATION_DELTA**（primary），**BENCHMARK_DELTA**（secondary）。本日对测量构念、临床规范独立一致性、调节边界形成真实科学压力，**仍由 SCF/SDR/ASR、CSCI/BGT、MI/TD/DR/IA/BT/MEAS/ID/EG 表达**。Scientific Core Delta = 0；SPEC_REVISION_CANDIDATE = NO。优先 P0 实验为 BenchmarkVersion×Budget、RoleSwap×IndependentGold、ContinualTheoryInduction、SlowRiskDrift。
