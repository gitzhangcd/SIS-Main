# SIS Daily Literature Update｜2026-11-18

**Authority:** [SIS v0.3.1](../../specs/System_Intelligence_Science_v0.3.1.md); [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md); [P0 Audit Queue](../evidence-map/SIS_P0_Audit_Queue.csv).
**Search window:** since 2026-11-17 last committed daily run. Official [arXiv cs.AI listing 2026-11-17](https://arxiv.org/list/cs.AI/new) (135 primary cs.AI new submissions; 293 cross-lists; 289 replacements), arXiv original abstracts/full HTML, ACL Anthology AACL November 2026, ICLR 2026 author archive and OpenReview reference, other venue/index checks. Only independently verified primary papers receive scientific claims; community interpretations remain DISCOVERY_ONLY.
**Intake:** 10 unique candidate studies: 1 November peer-reviewed late-discovered AACL study; 9 preprints (8 first submitted 2026-11-16 and 1 cs.SE preprint 2026-11-13 cross-listed later). Explicitly separate first submission, listing, and discovery date.
**Quarantine:** arXiv:2611.18642 appeared in 17 November list but official abstract page oddly says "Submitted on 14 Oct 2026" despite an arXiv:2611 identifier. Hold as metadata lineage ambiguity; do not create scientific Study candidate before correction/verification.

## Peer-reviewed archival delayed discovery

### SIS-CAND-20261118-01｜ATOD: An Evaluation Framework and Benchmark for Agentic Task-Oriented Dialogue Systems — Worth Skimming
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.109/; **initial/version publication:** 2026-11 (AACL-IJCNLP archival publication); **source status:** PEER_REVIEWED; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 1000合成长期对话，六类目标生命周期属性；符号—向量记忆评价器在中等复杂度上同时超过90%目标检出F1与条件状态准确率，跨评价器复核、人工审计一致率94%。
- **Evidence audit / confounders:** 固定轨迹而非真实交互；记忆、状态规则和检索联合变化；人工一致率不意味着生命周期语义独立Gold充分。
- **SIS:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/MI/MEAS/EG/ID/BT`; primary estimand `GOAL_LIFECYCLE_STATE_DEPENDENCY_MEMORY_CONDITIONAL_STATUS_ACCURACY`; role `MEASUREMENT_INSTRUMENT / IMPLEMENTATION`; provisional maturity `CL1 (goal-state tracking); no causal claim`; identification / transport `I1 / T0`.
- **Boundaries:** 对话复杂度、模拟目标依赖、语言、评价器、交互权限.
- **Impact:** SHARPENS：目标存在、状态推进与真实任务完成不能互换。
- **Required kill test:** Fixed dialogue trace × perturbed dependencies × blind human lifecycle Gold × intervention replay.

## Newly posted / delayed-indexed preprints
### SIS-CAND-20261118-02｜SciResearch-Eval: Evaluating Scientific Judgment in Autonomous Experimental Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21541; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 热传导实验设计与故意漏掉物理项的模拟器；留出93任务、9模型、2511次episode，要求95%参数区间。部分模型面对错设模拟器覆盖仅20%–62%，高计算量可改变表现。
- **Evidence audit / confounders:** 模拟实验有已知真值但不是真实实验室；任务解法、计算预算及模型族共变；区间覆盖不直接等于现实科学发现价值。
- **SIS:** Primary `SCF`; cross-cutting `BGT`; Framework `MI/DR/EG/MEAS/ID/BT`; primary estimand `DESIGNED_EXPERIMENT_MISSPECIFIED_SIMULATOR_INTERVAL_CALIBRATION_AND_JUDGMENT`; role `MEASUREMENT_INSTRUMENT / NEGATIVE_BOUNDARY`; provisional maturity `CL1; exact physical truth used for outcome scoring, not mechanism proof`; identification / transport `I1 / T1-task`.
- **Boundaries:** 模拟器错设类型、实验激励、计算预算、参数可识别性、实验设计.
- **Impact:** SHARPENS：科学执行、模型错设诊断及校准科学判断必须分开。
- **Required kill test:** Matched physics omissions × equal experiment budget × blinded true parameter coverage × decision utility.

### SIS-CAND-20261118-03｜Harness Leverage Across Model Size: A Ladder of Five Local Agent Harnesses from 0.75B to 4.7B — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21407; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 五种Harness×四款小模型及大模型锚点、18项产出工件任务；360个实验格，127/357无所需工件且85个正常退出；撤销重复阻断规则可使弱模型表现恶化。
- **Evidence audit / confounders:** 小任务集，规模阶梯仅四个小模型，模型家族与大小混杂；完成门控消融并非收益来源，不能推断单调scale law。
- **SIS:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/TD/MEAS/ID/BT`; primary estimand `MODEL_CAPABILITY_BY_HARNESS_COMPLETION_POLICY_ARTIFACT_DELIVERY_EFFECT`; role `COMPONENT_INTERACTION / NEGATIVE_BOUNDARY / MEASUREMENT`; provisional maturity `CL1 package; local CL2 candidate for ablations, pending independent audit`; identification / transport `I2-local / T1`.
- **Boundaries:** 模型能力、工件存在性、重复次数、退出码、执行预算、规则组合.
- **Impact:** SHARPENS：进展控制与产出工件真值不同于进程退出；CSCI条件交互须量化。
- **Required kill test:** Matched artifact checker × model scale/family × rule ablation × equal calls × state persistence.

### SIS-CAND-20261118-04｜Procedure without Judgment: What Small Language Models Learn under an Exact Verifier — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21529; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 确定性权限策略下计算最小充分理由，4B模型用2000算法轨迹微调在已见策略达到92%，但三项未见策略中充分性94%、最小性48%；精确奖励RL并未提高留出表现。
- **Evidence audit / confounders:** 小型可枚举的权限政策，不代表开放式制度；训练教师、轨迹类型和评估分布相互作用。
- **SIS:** Primary `SCF`; cross-cutting `BGT`; Framework `MI/DR/EG/MEAS/ID/BT`; primary estimand `EXACT_POLICY_VERIFIER_TRAINING_IN_DOMAIN_MINIMAL_REASON_VS_OOD_GENERALIZATION`; role `NEGATIVE_BOUNDARY / MEASUREMENT`; provisional maturity `CL1; local training contrast candidate; no generalized mechanism`; identification / transport `I1/I2-local / T2 performance-only`.
- **Boundaries:** 策略形式、训练教师类型、查询预算、未知政策、最小性定义.
- **Impact:** CHALLENGES：精确Verifier可教会执行程序，不保证获得可迁移判断能力。
- **Required kill test:** Train-policy swap × policy complexity × strict sufficiency+minimality × matched oracle calls.

### SIS-CAND-20261118-05｜Benchleaking Is Accelerating: Benchmark contamination has worsened sharply in the past month — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21315; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 20个benchmark、4个公开base模型的few-shot continuation检测：某模型可复现96% HumanEval题及85% OpenBookQA题；提出泄漏题目判错的Anti-Hack分数。
- **Evidence audit / confounders:** 记忆式复现表明暴露风险但不证明训练数据从何处进入；不同基座模型训练来源不透明，评分扣减是保守压力测试非因果去污染。
- **SIS:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; primary estimand `BENCHMARK_EXAMPLE_RECALL_CONTAMINATION_VS_MEASURED_GENERALIZATION`; role `NEGATIVE_MEASUREMENT / EVIDENCE_INTEGRITY`; provisional maturity `CL1 observational recall evidence, no independently established training-data provenance`; identification / transport `I1 / T1`.
- **Boundaries:** 基准公开程度、训练截止日期、提示方式、模型家族、泄漏定义.
- **Impact:** SHARPENS：基准高分必须报告泄漏检查和抗污染敏感性。
- **Required kill test:** Fresh hidden holdout × task perturbation × memorization continuation × training provenance.

### SIS-CAND-20261118-06｜EVIDENT: Evaluating Evidence Grounding in GUI Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.20488; **initial/version publication:** 2026-11-16; **source status:** PREPRINT (author reports EACL 2027 Findings acceptance; archival unverified); first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 220项英韩网页任务及人工证据元数据，分别测TSR结果成功、ESR必要证据观察、GSR最终Claim获证据支持；表面任务成功可能掩盖证据失配。
- **Evidence audit / confounders:** 观察到证据不等于因果使用；人工证据元数据存在选择偏差；英韩语言与GUI布局影响迁移。
- **SIS:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; primary estimand `GUI_TASK_SUCCESS_REQUIRED_EVIDENCE_OBSERVATION_AND_GROUNDED_CLAIM_SUPPORT`; role `MEASUREMENT_INSTRUMENT / NEGATIVE_BOUNDARY`; provisional maturity `CL1; metric design CL0; no executed causal evidence-use proof`; identification / transport `I1 / T1`.
- **Boundaries:** 语言、网页动态、截图可见性、证据标注、任务目标.
- **Impact:** SHARPENS：证据被观察、证据支持与真实行动变更是不同终点。
- **Required kill test:** Evidence swap × fixed navigation × independent human Gold × task success and trace replay.

### SIS-CAND-20261118-07｜Subprocess-Constrained Markov Decision Processes — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21471; **initial/version publication:** 2026-11-16; **source status:** PREPRINT (author reports NeurIPS 2026; proceedings unverified); first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 把初态累积成本约束加强为每条可达历史的后续策略仍需满足成本界；静态平稳策略可能严格次优且近似优化NP-hard，历史依赖策略可在ε最优、δ违规保证下多项式表达。
- **Evidence audit / confounders:** 理论依赖完整MDP/成本已知和条件历史可定义，真实系统状态不完全可观测、估计偏差未覆盖。
- **SIS:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/TD/ID/MEAS/BT`; primary estimand `HISTORY_CONDITIONAL_CONTINUATION_FEASIBILITY_POLICY_VALUE`; role `THEORETICAL_BOUNDARY / REGULATION_LAW_CANDIDATE`; provisional maturity `CL0 theorem; not empirical CL2`; identification / transport `I0 formal / T0`.
- **Boundaries:** 可达历史、条件风险预算、折扣率、模型已知性、不可观测状态.
- **Impact:** SHARPENS/WATCH：可行性不是初始期望成本，通过路径历史的条件约束已经可由SIS Dynamics/ASR表达。
- **Required kill test:** History-conditioned risk × stationary baseline × partial observation × mismatch to real side effects.

### SIS-CAND-20261118-08｜Language-model agents' beliefs can be manipulated via truthful evidence in open channel — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21235; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 1090个Rumour目标、6个Twitter事件中把真实片段串成误导性的隐含关系；14模型中12个的接受率超过65%，同证据投票/评审仍可能维持错误信念；独立支持校验的监控干预提高准确率。
- **Evidence audit / confounders:** 片段选择和叙事顺序会同时改变；真实事实组合诱发推论不等于模型内部具体机制已识别，平台世界迁移未测。
- **SIS:** Primary `SDR`; cross-cutting `CSCI/BGT`; Framework `IA/TD/EG/MI/MEAS/ID/BT`; primary estimand `TRUE_FRAGMENT_COMPOSITION_TO_UNSUPPORTED_BELIEF_PROPAGATION`; role `NEGATIVE_BOUNDARY / INFLUENCE_REGULATION`; provisional maturity `CL1; local fragment manipulation CL2 candidate only`; identification / transport `I2-local / T1`.
- **Boundaries:** 信息来源、片段组合、时间顺序、社会图传播、监控成本.
- **Impact:** SHARPENS：事实真实与由事实诱出的关系被证实不是同一回事。
- **Required kill test:** Fact-preserving order swap × same propositions × relationship Gold × downstream executed decision.

### SIS-CAND-20261118-09｜Benchmark Factory: Agentic Benchmark Creation via Dataset Curation and Label-Free Quality Anchors — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.18890; **initial/version publication:** 2026-11-13 (cs.SE; cs.AI cross-listed 2026-11-17); **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 从生产代码变更构造五组编码Benchmark，以已知模型顺序等无逐题Gold锚点过滤；测试了故意简单任务、损坏评分器和模型标签打乱的负控制。
- **Evidence audit / confounders:** 预设模型顺序可能偏向已知家族；5%人工样本不足以覆盖罕见严重评分错误；基准区分模型能力不等于测量构念正确。
- **SIS:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `MEAS/EG/DR/ID/BT`; primary estimand `LABEL_FREE_BENCHMARK_QUALITY_ANCHOR_EXTERNAL_ORDER_DISCRIMINATION`; role `MEASUREMENT_INSTRUMENT / NEGATIVE_CONTROL`; provisional maturity `CL1; no independent semantic correctness guarantee`; identification / transport `I1/I2-control / T1`.
- **Boundaries:** 企业代码分布、排序先验、评分器缺陷、抽样比例、未来模型.
- **Impact:** SHARPENS：代理有效性锚点是必要检查，不是充分真值证明。
- **Required kill test:** Model order inversion × unseen implementation family × independent blinded task Gold × corrupted grader.

### SIS-CAND-20261118-10｜Turing Agent: Agentic Formal Verification for Mathematical Research — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.21299; **initial/version publication:** 2026-11-16; **source status:** PREPRINT; first discovered/selected 2026-11-18; one unique provisional study; no permanent SIS-LIT ID.
- **Core idea and evidence:** 数学论文级定理形式化与辅助引理并行验证，在Formal TCS Bench报告约57%–62%忠实形式化成功，TCS子集RLMEval约83% pass@1，并报告三个难题正式证明。
- **Evidence audit / confounders:** 证明器仅保证形式表达定理成立，不保证该表达忠实对应自然语言命题；模型/资源配置与证明分解一起变化。
- **SIS:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/EG/MEAS/ID/BT`; primary estimand `RESEARCH_MATH_INFORMAL_TO_FORMAL_FAITHFUL_VERIFICATION_SUCCESS`; role `EXTERNAL_FORMAL_VALIDATION / IMPLEMENTATION`; provisional maturity `CL1; formal proof soundness conditional on encoded statement; semantic faithfulness separately`; identification / transport `I1 / T1`.
- **Boundaries:** 定理表达复杂度、形式系统、人工形式化Gold、工具调用预算、学科迁移.
- **Impact:** SHARPENS：形式正确性和自然语言科学主张一致性需要两条独立证据链。
- **Required kill test:** Blind math expert formalization match × checker proof × equal compute × unseen theorem family.

## Technical / community analysis
Discovery-only checking of announcement and institutional/project pages. No independent methodological replication qualified for separate CL promotion. Original source dates preserved.

## Synthesis: SIS pressure and scientific experiment work
1. **Post-execution outcome is not truth:** exit code, GUI task completion, policy sufficiency, and real artifact/semantic accuracy are separate end points. New benchmark fixtures must independently validate them.
2. **Scientific judgment and calibrated uncertainty:** deliberate simulator error and exact formal checkers reveal why procedural execution and semantic/physical scientific validity diverge.
3. **Component–system interaction:** five-harness model-size factorial study demonstrates why both completion policy and backbone capability are treatment variables, not implementation labels.
4. **Dynamic viability constraints:** history-conditional continuation constraints are stronger than initial expected cost, but already expressible in SIS SDR/ASR with MEAS/ID.
5. **Evidence governance:** benchmark leakage, synthetic true-fragment composition and self-authored quality anchors alter epistemic validity without necessarily changing underlying capability.

| Priority | Fixture | Estimand / negative kill |
|---|---|---|
| P0 | Model capacity × harness progress control × artifact checker | Identical exit status but missing artifacts; purported scale interaction disappears under equal budget |
| P0 | Experimental design × deliberately wrong simulator × interval coverage | High procedural completion with systematically under-covered physical truth |
| P0 | Exact verifier training × new policies | In-domain sufficiency transfers but minimality and counterfactual judgment collapse |
| P0 | Historical policy × every reachable continuation | Initial cost feasible but a reachable history violates continuation viability |
| P0 | Truthful fragments × relation support × order permutation | Factually true fragments induce false unsupported relation |
| P0 | Benchmark contamination × private perturbation × independent scoring | Score advantage vanishes when leaked examples are excluded |
| P0 | GUI evidence observed × counterfactual source swap × external Gold | Cited/seen evidence has no causal influence on final answer |
| P1 | Formal proof checker × natural-language semantic Gold | Valid Lean theorem differs materially from research statement |

## P0 backlog re-audit
- [Detailed 9-Claim audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-18.md): **SIS-LIT-109 BayesFlow**, **SIS-LIT-110 TPGO**, **SIS-LIT-111 Conductor**.
- 109: theorem applies to unrefined asymptotic posterior, not automatically full final search algorithm.
- 110: TPGO graphs, structural edits, historical optimization and cross-domain transfer separated; no CL3.
- 111: collaboration topology, tailored instructions, worker quality, recursion and token budget disentangled as independent estimands; no causal transport claim.
- Changes: 9 claims first-coded, **0 formal CL2/CL3 promotions, 0 confirmed T3/T4**. Second-coder independent adjudication PENDING.

## Formal SIS Impact Decision
**Primary:** `MEASUREMENT_IDENTIFICATION_DELTA` · **Secondary:** `BENCHMARK_DELTA` · **CorePressure:** WATCH · **ScientificCoreDelta:** 0 · **SPEC_REVISION_CANDIDATE:** NO.
**Rationale:** Empirical evidence raises real pressure to measure artifact validity, external scientific Gold, conditional viability, and mechanism invariance. These are already explicitly expressible using SCF/SDR/ASR, CSCI/BGT, and MI/TD/DR/IA/BT/MEAS/ID/EG. No new irreducible scientific primitive/estimand demonstrated; Core remains FROZEN.
