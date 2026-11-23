# SIS Daily Literature Update｜2026-11-23

**Authority:** [SIS Master](../../specs/System_Intelligence_Science_v0.3.1.md), [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md), [P0 Queue](../evidence-map/SIS_P0_Audit_Queue.csv).

**Actual search/publication chronology:** This is a **Monday 2026-11-23** run; latest verified regular arXiv cs.AI batch is **Friday Nov 20** (the new Sunday-evening US announcement has not yet appeared at this local run time). Today's 3 arXiv candidates were originally submitted **Thursday Nov 19**, not new Nov 23 publications. Six official AACL-IJCNLP 2026 papers were published in **November**; the seventh official EMNLP paper was published in **October**. All seven are *delayed SIS discoveries*, not freshly published this morning. Primary sources: ACL Anthology, arXiv abstracts/HTML, author reports; discovery scans also included arXiv, OpenReview/ICLR/NeurIPS venues, major journals and technical/community posts. Secondary posts discovery-only. Exact source IDs and titles checked against registry; no duplicate primary Study.

**Run tally:** 10 unique first-coder candidates: **7 peer-reviewed archival papers + 3 preprints**; 3 previously catalogued studies and 9 claim-level re-audit units; formal promotions=0; new T3/T4=0. No new first-principles SIS primitive is inferred from an Agent/Memory/Workflow implementation.

## 1｜Scientific synthesis
1. Memory relevance and temporal validity do not imply admissibility: `retrieved ≠ permitted; current truth ≠ historical visibility`. MemGov and MemFSM raise governed state-selection and temporal evidence contracts, but both fit SIS EG/DR/TD.
2. An evaluator with better benchmark scores is not necessarily independent: VERGE exposes strict-subset insufficiency; J-ToRL explicitly addresses reward shortcuts while retaining reference-answer validity limits.
3. Correct performance contrasts require a valid *null interaction*: LLM GerryMandering shows that additive attribute effects can produce false-positive intersectional claims, a direct caution for SIS CSCI.
4. Conditional regulation includes *when to stay silent* and *whether simulated candidate actions merit real execution* (FLUID, Seer). Neither new method is a scientific primitive.
5. Representation surprise can indicate potential memory formation, but future utility is a different estimand (ReSuME). CROP/CRAFT add implementational accuracy–cost and semantic contrast examples, not Core coverage gaps.

## 2｜Peer-reviewed studies (archive verification, delayed discovery)

### SIS-CAND-20261123-01｜Beyond Retrieval: Deterministic Memory Governance with Pairwise Constraints and Certified Repair for Long-Term Language Agents — Must Read
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.246/; AACL-IJCNLP 2026, November 6–10, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** MemGov 将检索到的记忆作为带权限/生命周期/互斥约束的对象，应用 must-link/cannot-link 判定与可审计修复或拒绝；不是优化相似度，而是确定可准入集合。
- **Evidence / experimental strength / limitations:** 在所测试的受控治理场景，原检索返回47–51%不安全组合；MemGov降至0%，答案效用约损失2–4个百分点。该0%只在已编码约束及测试分布内成立，不能推广成所有安全风险为零。
- **SIS re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework Capability `DR/EG/MI/MEAS/ID/BT`; primary estimand `CONSTRAINT_ADMISSIBLE_MEMORY_SELECTION_UNSAFE_MERGE_VS_ANSWER_UTILITY`; Evidence Role `CONTROLLED_GOVERNANCE / NEGATIVE_BOUNDARY`; first-coder ceiling `CL1; local CL2 candidate for constraint-mediated selection`; Identification `I2-local for governance switch; independent constraint Gold limited`; transport `T1`.
- **Key boundary variables:** 缺失/错误的约束、时间有效性、访问权限、检索候选固定、拒绝成本、用户意图
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 相同候选集随机启用/停用门控×未知互斥约束×独立权限Gold×任务效用/拒绝成本

### SIS-CAND-20261123-02｜VERGE: Verification-Enhanced Generation of Multi-Hop Evaluation Datasets for Task-Specific RAG — Must Read
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.139/; AACL-IJCNLP 2026, November, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 把多证据片段的必要性与问答完整性检查放进样本生成循环，以严格子集消融和删除片段来审查问题是否真需要多个证据来源。
- **Evidence / experimental strength / limitations:** 11052个候选筛选出2854道题；250题分层样本中，闭卷不可答者有69.8%在任意严格子集下仍不可答；人工校验Kappa=0.903。但多片段必要性并非所有题目成立，也未验证真实行动中因果证据使用。
- **SIS re-coding:** Primary `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework Capability `MEAS/EG/ID/BT`; primary estimand `EVIDENCE_CHUNK_STRICT_NECESSITY_BENCHMARK_GOLD_VALIDITY`; Evidence Role `MEASUREMENT_INSTRUMENT / CONTRASTIVE_NEGATIVE_CONTROL`; first-coder ceiling `CL1 measurement; no mechanistic promotion`; Identification `I2-local chunk removal; source composition confounds`; transport `T1 six domains, no causal transfer`.
- **Key boundary variables:** 片段相似性、题型、闭卷知识泄露、选项提示、自动验证器与人工Gold
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 随机删片段×严格子集×开放问答格式×盲专家标注×新源域

### SIS-CAND-20261123-03｜J-ToRL: Tool-Integrated LLM-as-a-Judge via Reinforcement Learning — Must Read
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.46/; AACL-IJCNLP 2026, November, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 通过RL训练评价模型主动调用计算工具，并用参考答案的辅助可验证奖励抑制仅猜对两两胜负的捷径学习。
- **Evidence / experimental strength / limitations:** 五领域两两比较的作者实验中优于基础评价器与若干对照；但法定/科学真值不必然被参考答案完整表达，工具使用与奖励调整共同变化；不能把评价器自身打分认作独立Gold。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/EG/MEAS/ID/BT`; primary estimand `TOOL_VERIFIED_JUDGE_TRAINING_INDEPENDENT_VERDICT_VALIDITY_VS_SHORTCUT_RATE`; Evidence Role `EVALUATOR_INSTRUMENT / REWARD_SHORTCUT_NEGATIVE`; first-coder ceiling `CL1 package evidence, local CL2 candidate`; Identification `I1/I2-local; reward and tool interaction unseparated`; transport `T1`.
- **Key boundary variables:** 参考答案可信度、工具错误、RL奖励捷径、领域差异、评价器与训练者信息泄漏
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 冻结评价集×计算工具开关×辅助奖励开关2×2×人类/可执行Gold×未知任务

### SIS-CAND-20261123-04｜CROP: Token-Efficient Reasoning in Large Language Models via Regularized Prompt Optimization — Worth Skimming
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.45/; AACL-IJCNLP 2026, November, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 在文本Prompt优化目标中加入输出长度正则与相应反馈，将只求正确率的搜索变为明确的准确率—Token成本前沿搜索。
- **Evidence / experimental strength / limitations:** GSM8K、LogiQA和BIG-Bench Hard上报告平均节约68%输出Token，最高80.6%，准确率名义小幅下降；具体效果随任务、模型、预算和评分方式变化，不能推出不损能力。
- **SIS re-coding:** Primary `ASR`; cross-cutting `BGT`; Framework Capability `DR/MI/MEAS/ID/BT`; primary estimand `PROMPT_LENGTH_REGULARIZATION_ACCURACY_TOKEN_PARETO_EFFECT`; Evidence Role `RESOURCE_CONSTRAINED_POLICY_VALUE`; first-coder ceiling `CL1 performance; local CL2 candidate`; Identification `I1/I2-local; prompt content and regularization co-vary`; transport `T1`.
- **Key boundary variables:** 模型规模、任务难度、输出长度、推理轨迹有效性、模型成本/延迟
- **SIS relation:** `FILLS EXISTING FRAMEWORK`. **Reading priority:** `Worth Skimming`. **Kill test:** 等候选搜索与等Token预算×隐藏准确率Gold×重复种子×全生命周期成本

### SIS-CAND-20261123-05｜Episodic Memory from Compression Boundaries in Latent Representation Space — Worth Skimming
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.19/; AACL-IJCNLP 2026, November, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** ReSuME 将SAE重建残差的表示惊讶度作为记忆写入触发信号，不依赖预先写好的关键字重要性规则。
- **Evidence / experimental strength / limitations:** 长程对话上报告优于若干记忆和异常检测基线的性能—存储前沿，协方差归一化促进跨域校准；但高重建误差不等于任务相关性，输入分布变化或SAE错设可能放大噪声。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/TD/MEAS/ID/BT`; primary estimand `SAE_REPRESENTATION_SURPRISE_MEMORY_WRITE_FUTURE_TASK_NET_VALUE`; Evidence Role `REPRESENTATION_EXTERNALIZATION / BOUNDARY`; first-coder ceiling `CL1; no CL3 mediation`; Identification `I1; writing policy vs model representations confounded`; transport `T1 claims cross-domain calibration, no T3`.
- **Key boundary variables:** SAE训练分布、阈值、对话长度、模型尺度、写入成本、未来任务相关性
- **SIS relation:** `SHARPENS`. **Reading priority:** `Worth Skimming`. **Kill test:** 残差门控/随机/人类相关性门控×等写入量×未来任务×分布漂移

### SIS-CAND-20261123-06｜CRAFT: A Unified Counterfactual Reasoning Framework for Tabular Question Answering and Fact Verification — Worth Skimming
- **StudyVersionRecord:** https://aclanthology.org/2026.aacl-long.176/; AACL-IJCNLP 2026, November, peer reviewed (delayed discovery); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 通过同时构造原陈述及其逻辑对照，沿双向证据路线提取并整合表格QA/事实核验的判断信息。这里的反事实主要是语义反驳，不是因果do干预。
- **Evidence / experimental strength / limitations:** WikiTQ、TabFact等表格任务比部分基线好；但多路径推理、额外Token、证据筛选同时增加，尚不能把准确率提升解释为已识别因果中介。
- **SIS re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework Capability `MI/EG/MEAS/ID/BT`; primary estimand `BIDIRECTIONAL_CONTRASTIVE_TABLE_EVIDENCE_INTEGRATION_ACCURACY_EFFECT`; Evidence Role `EVIDENCE_SYNTHESIS / IMPLEMENTATION`; first-coder ceiling `CL1, mechanism CL0`; Identification `I1; no do-intervention/matched budget mechanism`; transport `T1`.
- **Key boundary variables:** 表格行列关系、查询复杂度、反事实语句正确性、推理预算、基线强度
- **SIS relation:** `FILLS EXISTING FRAMEWORK`. **Reading priority:** `Worth Skimming`. **Kill test:** 真假对照构造/两路推理/预算正交×完整表格独立Gold

### SIS-CAND-20261123-07｜Validity Is Not Visibility: A Lifecycle FSM for Agent Memory — Must Read
- **StudyVersionRecord:** https://aclanthology.org/2026.emnlp-main.260/; EMNLP 2026, October, peer reviewed (late indexing, not November publication); source class `PEER_REVIEWED`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 将事实是否仍有效（superseded/expired）与针对当前/历史查询是否应展示区分；用四状态FSM及意图路由控制检索可见性。
- **Evidence / experimental strength / limitations:** ValidMem为相同存储配对当前与历史查询，并在多记忆基准/多基础模型报告改善；但规则与查询意图判定共同变化，对错误时间戳和有歧义的意图缺少独立部署验证。
- **SIS re-coding:** Primary `SDR`; cross-cutting `BGT`; Framework Capability `TD/DR/EG/MEAS/ID/BT`; primary estimand `MEMORY_FACT_TEMPORAL_VALIDITY_VS_QUERY_CONDITIONAL_VISIBILITY`; Evidence Role `SEMANTIC_STATE_LIFECYCLE / NEGATIVE_BOUNDARY`; first-coder ceiling `CL1; local contrast candidate`; Identification `I1/I2-local; no mediation identification`; transport `T1`.
- **Key boundary variables:** 查询意图、时效/替代状态、历史证据可访问性、时间戳误差、权限规则
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 相同事实×当前/历史查询×状态误标×隐私规则×独立Gold

## 3｜Preprints (2026-11-19 submissions / 2026-11-20 announcements)

### SIS-CAND-20261123-08｜LLM GerryMandering: Separating Interactions from Additive Effects in LLM Audits — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26538; arXiv v1 first submitted 2026-11-19; in Friday Nov 20 announcement; delayed discovery; source class `PREPRINT`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 用加性模型与Freedman–Lane零假设区分单属性加和造成的表面差异与真正交互项，避免把相交子群的错误差异过度解释成机制。
- **Evidence / experimental strength / limitations:** 150个无交互合成数据中常用准则平均误报66.1子群，ADDIS 0.09；植入交互检出84%（原方法32%）；另测10000个人工画像和13个模型。人工合成基准可检验统计识别，真实人群的交互和公平性外推仍不足。
- **SIS re-coding:** Primary `ROUTING_ABSTAIN`; cross-cutting `CSCI/BGT`; Framework Capability `IA/MEAS/ID/BT`; primary estimand `ADDITIVE_MAIN_EFFECT_NULL_VS_TRUE_INTERACTION_DETECTION_FALSE_POSITIVE_RATE`; Evidence Role `MEASUREMENT_IDENTIFICATION_NEGATIVE / INTERACTION_CONTROL`; first-coder ceiling `CL1, local I2 controlled synthetic null`; Identification `I2-local planted interactions; real audit I1`; transport `T0/T1 models (no causal transport)`.
- **Key boundary variables:** 边际基率、群体样本量、模型输出评价标准、属性交互定义、零假设置换有效性
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 跨任务受控植入交互×匿名基准×校准零分布×低频子群×独立标签

### SIS-CAND-20261123-09｜FLUID: Flexible, Evidence-Grounded Situated Task Guidance — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26491; arXiv v1 first submitted 2026-11-19; Friday Nov 20 announcement; delayed discovery; source class `PREPRINT`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 实时人机协作的最优行动可能是延后、提示或者保持沉默；用支持证据、必要性和时间灵活性而非固定一句金标准评价任务引导。
- **Evidence / experimental strength / limitations:** 使用真实人类交互语料WTaG/HoloAssist，报告在正确率、干预精度、及时性和延迟之间较强的整体权衡；仍存在打断/语音重叠，离线自然行为不构成提示/沉默策略的随机因果效应。
- **SIS re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework Capability `DR/IA/TD/EG/MEAS/ID/BT`; primary estimand `EVIDENCE_CONDITIONED_TIMING_SPEAK_VS_SILENCE_GUIDANCE_NET_VALUE`; Evidence Role `INTERVENTION_TIMING / OBSERVATIONAL_BOUNDARY`; first-coder ceiling `CL1`; Identification `I1; timing-confounding and latent user intent`; transport `T1`.
- **Key boundary variables:** 用户当前状态、说话重叠、实时延迟、行动可逆性、必要性标注、模态可观测性
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 固定任务×随机提示/延迟/沉默×真实任务成功/中断成本×盲观察Gold

### SIS-CAND-20261123-10｜Seer: Guiding Small Deep-Research Agents with Shared Decision Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26423; arXiv v1 first submitted 2026-11-19; Friday Nov 20 announcement; delayed discovery; source class `PREPRINT`; provisional Study identity, no permanent SIS-LIT identifier. Citation is source metadata only, not claim-level validation.
- **Core idea / claimed novelty:** 将行动生成与离线学习的工具响应模拟器、价值估计器分离，只执行选中的真实工具动作，未执行候选的模拟输出不写入真实历史。
- **Evidence / experimental strength / limitations:** GAIA在Qwen3.5-4B上13.6%→41.7%，9B上22.3%→50.5%；但模拟预测误差、候选数量、价值模型训练轨迹与计算预算一起变化，不能断言模拟准确等于决策增益。
- **SIS re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework Capability `DR/MI/TD/EG/MEAS/ID/BT`; primary estimand `SHARED_SIMULATOR_VALUE_ESTIMATOR_COUNTERFACTUAL_TOOL_ACTION_ROUTING_GAIN`; Evidence Role `MODEL_BASED_REGULATION / SIMULATION_ERROR_BOUNDARY`; first-coder ceiling `CL1, local CL2 candidate`; Identification `I1/I2-local; simulator and value evaluator bundled`; transport `T2 performance across backbones only`.
- **Key boundary variables:** 模拟器误差、候选动作覆盖、工具费用、观察历史真实性、模型规模、任务分布
- **SIS relation:** `SHARPENS`. **Reading priority:** `Must Read`. **Kill test:** 固定动作候选×真模拟/错模拟/真实调用×价值估计器替换×等全部推理费用

## 4｜Technical and community analysis
Searched for high-quality commentary and implementation discussions. **None independently reproduced a scientific mechanism** or warranted standalone admission to scientific evidence. All analysis remains `DISCOVERY_ONLY`; no padding.

## 5｜P0 existing Study re-audit
- `SIS-LIT-076` SoL-Pi: 3 distinct claims, original https://arxiv.org/abs/2609.20519; arXiv原始全文的Method 2.1/2.2、Table 1–3、3.2跨Benchmark；NVIDIA研究页面版本身份核对. First-coder only, 0 formal promotions.
- `SIS-LIT-078` FORGE: 3 distinct claims, original https://arxiv.org/abs/2609.15209; arXiv原始全文Introduction/Experiments/Table 2累积消融及Transfer部分. First-coder only, 0 formal promotions.
- `SIS-LIT-094` SelfOp: 3 distinct claims, original https://arxiv.org/abs/2609.22792; arXiv原始全文Introduction/3.4 convergence/benchmark methods/ablation；未独立复现CyberGym执行. First-coder only, 0 formal promotions.
Full audit: [SIS_P0_Reaudit_2026-11-23.md](../evidence-map/audits/SIS_P0_Reaudit_2026-11-23.md).

## 6｜P0 proposals and kill tests
| Priority | Proposed scientific fixture | Key null / kill condition |
|---|---|---|
| P0 | Memory candidate set × eligibility constraint × query time | Memory is relevant but unauthorized/stale; safe selection loses utility or fails on unseen constraints |
| P0 | Multi-chunk evidence × strict-subset deletion × independent Gold | Benchmark answer does not actually need all claimed evidence; self-verifier passes false Gold |
| P0 | CSCI interaction inference × planted additive-only null × planted interaction | Standard analysis reports spurious interactions; model-composition claim disappears under additive control |
| P0 | Judge tool access × reference-reward × true judge correctness | Better self-scored verdicts but unchanged independent decision validity |
| P0 | Observation availability × real-time guidance/silence × user outcome | Timely advice degrades real task efficiency, increases interruption or lacks necessity |
| P0 | Shared simulator × value estimator × real tool effect × fixed budget | Predicted action value improves while executed decision value remains unchanged |
| P1 | Representational surprise × memory writing × future task shift | Surprise detects anomalies but provides no positive future-task net value |
| P1 | Cost-regularized prompt × full lifecycle tokens × non-inferiority | Reported token gain disappears when search cost / hidden correctness included |

## 7｜Formal SIS Impact Decision
**Primary:** `MEASUREMENT_IDENTIFICATION_DELTA`; **Secondary:** `BENCHMARK_DELTA`; **CorePressure:** `WATCH`; **ScientificCoreDelta:** `0`; **SPEC_REVISION_CANDIDATE:** `NO`.

**Real pressure:** on construct validity (governance, semantic evidence necessity), interaction-identification null models, and the relation between observable evidence and action value. **No new uncovered estimand/causal distinction or nonreplaceable Framework Capability**: all are already expressible by SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG. Thus new evidence fills and sharpens the existing SIS scientific programs, without revising the frozen Core.
