# SIS Daily Literature Intelligence｜2026-11-21

**Authority:** SIS v0.3.1 Master, latest Registry, Evidence Map P0, Audit Queue. **Discovery window:** new arXiv announcements by 2026-11-20; previous daily run dated 2026-11-20; includes earlier first-posted candidates discovered late and one peer-reviewed record. **Source semantics:** published date ≠ submission date ≠ discovery date. **Status:** FIRST_CODER_SCREEN / CLAIM_LEVEL_ADJUDICATION_PENDING.

**Selection:** 10 high-interest independent studies (1 peer-reviewed *Perspective*, 9 arXiv preprints). Community/industry materials remain DISCOVERY_ONLY absent independent replication. **Not a new study:** Nature Machine Intelligence 2026-11-20 perspective and ChemRxiv 2026-02-08 earlier version are one Study lineage, not two.

## 1. Peer-reviewed / published literature
### SIS-CAND-20261121-01｜Enabling lab autonomy with reward functions and executable workflows — Must Read
- **StudyVersionRecord:** https://www.nature.com/articles/s42256-026-01339-0; initial/version publication **2026-11-20**; source `PEER_REVIEWED_PERSPECTIVE`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** Nature Machine Intelligence 观点论文：科研假设必须编译为可执行实验足迹（动作、约束、观测和规则）；实验选择应最大化每单位成本的决策相关信息；奖励设计而非文本规划本身是闭环实验瓶颈。
- **Evidence quality, controls and limitations:** 正式同行评审Perspective、无新的随机受控实证；2026-02-08 ChemRxiv预印本 The Missing Piece of Automated Scientist 为同一工作谱系，不能双重计数。
- **Scientific re-coding:** Primary `ASR`; cross-cutting `BGT`; Framework `DR/MI/TD/MEAS/EG/BT`; estimand `LAB_HYPOTHESIS_TO_EXECUTABLE_ACTION_INFORMATION_EFFICIENCY_AND_REWARD_SPEC_VALIDITY`; Evidence Role `CONCEPTUAL_SYNTHESIS / EXECUTABLE_SCIENCE_CONTRACT`; claim maturity ceiling `CL0 synthesis`; identification `I0`; transport `T0`.
- **Boundary variables:** 实体仪器可操作性、奖励错设、物理约束、动作风险、成本与观测延时.
- **Impact and priority:** SHARPENS; 不把Agent当原语，要求把科学决策可执行性与真科研效用分开. **Must Read**. **Kill test:** 固定同一实验目标×显式动作契约×随机设计策略×盲法物理实验Gold×等预算.

## 2. Preprints
### SIS-CAND-20261121-02｜TwinLab-Bench: Evaluating AI Scientists in Agentic Twins of Real Labs — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26248; initial/version publication **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 52个来自物理、生物及工程实验室记录的科研任务、逾100个实验动作；由实验记录和限定插值计算器支持数字孪生执行自选实验，隐藏真实实验结论评价科学发现。最强模型平均分45.0。
- **Evidence quality, controls and limitations:** 真实实验记录和盲Gold优于纯模拟；数字孪生仍不能执行任意未做过实验，计算器在局部数据邻域外的外推和科研判断Gold设定仍有边界；不能宣称真实自主实验已完成。
- **Scientific re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/EG/MEAS/ID/BT`; estimand `SELF_DESIGNED_SCIENTIFIC_EXPERIMENT_VS_TWIN_EXECUTION_RECORD_GROUNDED_DISCOVERY`; Evidence Role `BENCHMARK / SCIENTIFIC_JUDGMENT_MEASUREMENT`; claim maturity ceiling `CL1 empirical (benchmark)`; identification `I1`; transport `T1`.
- **Boundary variables:** 实验动作支持集、实验预算、孪生外推范围、隐藏答案、模型记忆和评分.
- **Impact and priority:** SHARPENS; 执行给定流程、选择既有测量、自主设计实验应分别测量. **Must Read**. **Kill test:** 真实验保留集×可执行动作支持集×未知实验请求×独立实验室专家Gold×重复执行.

### SIS-CAND-20261121-03｜Closing the Analyze-to-Design Gap: An Authorization-Bounded Agent for Self-Driving Laboratories — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.25043; initial/version publication **2026-11-18**; source `PREPRINT_DELAYED_DISCOVERY`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 在真实LC-MS仪器的氧化剂筛选中，通过授权边界和可审计行动，将数据分析接入测量选择；作者报告排序与脚本峰积分一致，化学专家确认若干谱图解释。基于历史数据重放的选井实验约第7针发现最佳条件，随机基线平均14.5针。
- **Evidence quality, controls and limitations:** 真实硬件验证局部可行性，样本与任务窄；注射效率来自历史重放而非所有任务的在线随机实验；专家确认不等于已识别自主系统因果贡献或无风险。
- **Scientific re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/IA/EG/TD/MEAS/ID/BT`; estimand `AUTHORIZED_LAB_MEASUREMENT_SELECTION_COST_VS_PHYSICAL_EVIDENCE_CORRECTNESS`; Evidence Role `REAL_HARDWARE_IMPLEMENTATION / CONDITIONAL_ACTION_BOUNDARY`; claim maturity ceiling `CL1; local replay contrast CL2 candidate`; identification `I1/I2-local`; transport `T1`.
- **Boundary variables:** 仪器权限、人类设定实验范围、MS谱图解析、注射预算、真实与重放差异.
- **Impact and priority:** SHARPENS; 真实仪器行动的权限与风险边界可由ASR和治理Framework表达. **Must Read**. **Kill test:** 随机注入限额×等预算主动/随机/规则式测量选择×独立物理真值×越权测试.

### SIS-CAND-20261121-04｜Verify the Verifier: Specification-Grounded LLM Cross-Checking for Bugs That Escape UVM Scoreboards — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26588; initial/version publication **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 在OpenTitan四种IP中植入564个缺陷，68个为通过现有scoreboard且已激活的候选漏检缺陷；基于规范的LLM轨迹交叉审查并以证明断言确认其中41个。
- **Evidence quality, controls and limitations:** 受控缺陷注入+在原始与变异设计上的断言核验较强；41/68不能理解为总体召回率，候选样本筛选和断言覆盖不全面，跨硬件IP迁移未识别。
- **Scientific re-coding:** Primary `SDR`; cross-cutting `BGT`; Framework `TD/EG/MEAS/ID/BT`; estimand `SPECIFICATION_GROUNDED_SCOREBOARD_ESCAPE_DETECTION_WITH_PROVEN_ASSERTION_GOLD`; Evidence Role `CONTROLLED_FAULT_INJECTION / NEGATIVE_EVALUATOR_BOUNDARY`; claim maturity ceiling `CL1; local intervention candidate`; identification `I2-local`; transport `T1`.
- **Boundary variables:** 规范完整性、断言可证明性、变异激活、参考记分板盲点、硬件IP家族.
- **Impact and priority:** SHARPENS; 测试通过只是评价器覆盖而不是规范符合性. **Must Read**. **Kill test:** 已知注入漏洞×隐藏断言×不同验证器×不依赖LLM的独立规范Gold.

### SIS-CAND-20261121-05｜Mind2Act World: A Diagnostic Benchmark for Embodied Mind, Physical Action, and Mind-Action Composition in Robotic Manipulation — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26444; initial/version publication **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 30种模拟机械操作任务×3难度×2场景=180配置，分别测心智状态、身体动作和闭环组合；最强系统单项Mind为52.7%、Act为39.0%，组合仅12.0%。
- **Evidence quality, controls and limitations:** 三视角任务拆分提供可检验的能力组合差距；但三视角任务难度不完全同质，12%低分不能自动归因于特定组件关系；真实机器人迁移未确认。
- **Scientific re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/IA/TD/MEAS/ID/BT`; estimand `ISOLATED_REASONING_ACTION_CAPABILITIES_VS_CLOSED_LOOP_COMPOSITION_GAP`; Evidence Role `NEGATIVE_COMPONENT_SYSTEM_INTERACTION / BENCHMARK`; claim maturity ceiling `CL1`; identification `I1`; transport `T0`.
- **Boundary variables:** 动作接触稳定性、历史窗口、闭环反馈、模拟器动力学、状态噪声.
- **Impact and priority:** SHARPENS; 组件具备局部能力不等于整体组合能力. **Must Read**. **Kill test:** 同任务单一能力oracle×组合闭环×随机破坏交接反馈×真实机器人小样本.

### SIS-CAND-20261121-06｜EverydayBench: Evaluating Satisfactory Completion of Live User-Facing Digital Work — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.25146; initial/version publication **2026-11-18**; source `PREPRINT_DELAYED_DISCOVERY`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 77项人工提出的实时数字工作任务（8领域），预设成功条件但不预设唯一答案；用确定性约束、实时网页引文核验和最终产物质量三类证据评分；23组系统中最高strict pass 54.55%。
- **Evidence quality, controls and limitations:** 真实用户式产出与实时可验证证据比固定QA更贴近实际；网页事实变化、主观Rubric、重复判分漂移、样本量77与任务权重影响分数；不是独立能力因果机制。
- **Scientific re-coding:** Primary `SCF`; cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; estimand `LIVE_USER_DELIVERABLE_CONSTRAINT_GROUNDING_AND_QUALITY_JOINT_SUCCESS`; Evidence Role `BENCHMARK / MEASUREMENT_VALIDITY`; claim maturity ceiling `CL1`; identification `I1`; transport `T1`.
- **Boundary variables:** 实时网页变化、证据时间戳、任务异质、评分器、产品/服务可用性.
- **Impact and priority:** SHARPENS; 信息正确、已引用与最终成果令人满意是不同终点. **Must Read**. **Kill test:** 冻结网页快照与实时网页×人工盲评×同产物重复评分×虚构引文负控制.

### SIS-CAND-20261121-07｜BuggyMLE: Scaling Machine Learning Engineering Difficulty with Bug Injection — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.25088; initial/version publication **2026-11-18**; source `PREPRINT_DELAYED_DISCOVERY`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 引入10种结构特征组成Code Complexity Index，8个公开编程Benchmark上与平均解题率拟合R²=0.951；在222个原始仓库生成6600余个ML工程缺陷版本，最难分层中最强解题率从95%降至9%，并展示训练后跨软件工程性能提升。
- **Evidence quality, controls and limitations:** 可控代码缺陷注入和仓库级真实执行有价值；CCI拟合可能受基准共线性/选择偏差影响，自动生成缺陷不一定代表真实ML错误，任务谱系泄漏和训练评测重叠须审计。
- **Scientific re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/TD/EG/MEAS/ID/BT`; estimand `REPOSITORY_COMPLEXITY_INJECTED_DEFECT_REPAIR_CAPABILITY_AND_TRANSFER`; Evidence Role `BENCHMARK / CONTROLLED_FAILURE / PERFORMANCE_TRANSFER`; claim maturity ceiling `CL1; injected contrast candidate`; identification `I2-local`; transport `T2 performance-only`.
- **Boundary variables:** 仓库规模、补丁复杂度、缺陷真实程度、训练源泄漏、算力预算.
- **Impact and priority:** SHARPENS; 故障难度是可测边界，跨任务成绩不等于可迁移故障机制. **Must Read**. **Kill test:** 人工真实缺陷×合成缺陷×复杂度匹配×藏匿仓库×独立运行测试.

### SIS-CAND-20261121-08｜A CPU Inside an LLM: Zero-Gradient Compilation of Exact Circuits into Pretrained Weights — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.26450; initial/version publication **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 闭式零梯度电路拼接把确定性算术与布尔程序写入已预训练模型权重，报告在2个3B–4B模型的6位算术测试达99.17%和100% ALU-prefix准确率，并测试文本能力保留与触发鲁棒性。
- **Evidence quality, controls and limitations:** 数学构造与预注册局部测试具启发性，但依赖特定架构、稀疏sidecar、数值精度及特殊触发条件；模型核心自然语言能力保留仅覆盖测试集，不能推断任意程序跨架构普适迁移。
- **Scientific re-coding:** Primary `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/MEAS/ID/BT`; estimand `COMPILED_EXACT_SUBCIRCUIT_WEIGHT_EXTERNALIZATION_VS_TASK_RETENTION_AND_ARCHITECTURE_PORTABILITY`; Evidence Role `REPRESENTATION_EXTERNALIZATION / IMPLEMENTATION / CONDITIONAL_MECHANISM`; claim maturity ceiling `CL0 conditional construction + CL1 empirical`; identification `I1`; transport `T1`.
- **Boundary variables:** 架构规范化、浮点精度、触发分布、宽度变化、自然语言回归及硬件实现.
- **Impact and priority:** SHARPENS; 可执行程序从外部组件迁入权重但仍是可替换能力实现. **Worth Skimming**. **Kill test:** 等计算/等参数LoRA×多架构留出×触发反事实×功能和语义保留集.

### SIS-CAND-20261121-09｜Stop Going in Circles: Loop-Triggered Routing for System 1 Decision Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.25363; initial/version publication **2026-11-19**; source `PREPRINT`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 检测重复的状态—动作对后临时请求LLM协助，其他时刻交给低成本策略，并在解困后恢复；三种环境、七种LLM上作者报告分别提高21.0%、60.1%、30.1%的平均相对/量化任务收益（原文未进一步标注单位）。
- **Evidence quality, controls and limitations:** 无训练路由规则，横跨多模型和环境；但循环也可能是合法策略，比较预算与状态观测可靠性不同，改进不应解释为已识别完整恢复机制。
- **Scientific re-coding:** Primary `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/TD/IA/MEAS/ID/BT`; estimand `REPEATED_STATE_ACTION_LOOP_TRIGGERED_ESCALATION_SUCCESS_COST_EFFECT`; Evidence Role `CONDITIONAL_REGULATION / RECOVERY`; claim maturity ceiling `CL1; local controlled routing candidate`; identification `I1/I2-local`; transport `T1`.
- **Boundary variables:** 状态别名、循环阈值、LLM调用预算、隐藏进度、低成本策略能力.
- **Impact and priority:** SHARPENS; 故障信号触发的选择性升级优于全程重模型是条件命题. **Must Read**. **Kill test:** 冻结决策模型×随机触发与伪触发×相同调用预算×Loop/NoLoop分层.

### SIS-CAND-20261121-10｜What the model knows but does not say: monitoring medical LLMs through verbalized thoughts — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.24994; initial/version publication **2026-11-18**; source `PREPRINT_DELAYED_DISCOVERY`; provisional study, no permanent SIS-LIT assignment.
- **Core idea / claimed novelty:** 通过自然语言自编码器把医疗多模态模型内部激活映射为文本，由输入盲审Judge分别检查内部表征和外部回答；对两类医疗攻击×两模态×两投递方式的八种条件，内部通道检出显著高于答案通道。
- **Evidence quality, controls and limitations:** 有干净对照和模态/攻击交叉，局部p<0.05；但Verbalizer和Judge可能共享训练偏差，针对攻击的检测不等于临床安全，罕见病漏诊与误报在部署分布下需独立核验。
- **Scientific re-coding:** Primary `SDR`; cross-cutting `CSCI/BGT`; Framework `TD/EG/MEAS/ID/BT`; estimand `MEDICAL_INTERNAL_STATE_VERBALIZATION_VS_OUTPUT_ONLY_HIDDEN_ATTACK_DETECTION_VALIDITY`; Evidence Role `OBSERVABILITY_INSTRUMENT / CLINICAL_NEGATIVE_BOUNDARY`; claim maturity ceiling `CL1; local comparison candidate`; identification `I1/I2-local`; transport `T1`.
- **Boundary variables:** 病种、提示注入类型、语言表征忠实性、模型家族、清洁特异度、临床风险权重.
- **Impact and priority:** SHARPENS; 观察隐藏行为不等于机制因果说明或独立临床真值. **Must Read**. **Kill test:** 外部真实病历Gold×冻结模型×独立Verbalizer/Judge×变换攻击×临床严重漏诊率.

## 3. Technical / community analyses
Checked recent arXiv indexes, Nature, ACL Anthology and technical scans. Technical summaries were used only for candidate discovery. No independently replicated mechanism evidence admitted; `DISCOVERY_ONLY`, no CL elevation or padding.

## 4. P0 Claim-Level Re-Audit
See [2026-11-21 P0 claim audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-21.md): **SIS-LIT-003, 023, 024** split into nine evidence-bounded claims. 003 package effect cannot establish mechanism; 023 memory migration is directional performance transfer; 024 nonsignificance cannot prove equivalence. Full paper tables and 024 version chronology remain follow-ups; all final CL/transport fields pending second coder.

## 5. Synthesis and proposed scientific fixtures
1. **Scientific autonomy ≠ fluent research text:** TwinLab + physical LC-MS + NMI Perspective distinguish designed experiments, admissible actions, true readings, and scientific judgment. Physical truth has limits; twins are not identical to laboratories.
2. **Verifier agreement ≠ specification truth:** Verify the Verifier and EverydayBench demand independent, artifact/execution-grounded Gold, with measurement coverage and evidence timestamps.
3. **Component capability ≠ composed system capability:** Mind2Act isolates reasoning, action, and closed-loop composition; task difficulty matching and interface manipulations are prerequisites for causal claims.
4. **Capability formation and transfer depend on implementation boundaries:** BuggyMLE controlled faults, weight-compiled exact circuits and medical internal observability require separate controls for distributions, model backbones and preserved skills.
5. **Adaptive regulation must preserve budget and legitimate actions:** loop-triggered escalation and lab authorization require false-trigger, NoOp and adverse side-effect testing.

| Priority | Fixture | Key kill condition |
|---|---|---|
| P0 | Real-lab action authorization × twin vs physical confirmation | digital-twin results break outside recorded intervention support |
| P0 | Independent specification × mutated verifier / scoreboard | pass status hides reachable semantic violations |
| P0 | Mind × Act × Feedback composition with difficulty-matched oracle | isolated proficiency fails in closed-loop without a single identifiable mediator |
| P0 | Hidden-data scientific Gold × experiment budget × decision correctness | experiment text looks plausible but independent scientific conclusion fails |
| P0 | Real-time deliverable × evidence timestamp × blinded expert quality | evidence citations pass while final result fails predefined user constraints |
| P0 | Medical internal observer × external clinical Gold × attack shift | clean-data false-positive or critical-disease misses rise |
| P1 | Fixed model × harness vs weight-embedded circuit / skill retention | task gain loses old capability or fails unseen architecture |
| P1 | Loop-triggered regulation × random triggers × equal total calls | routing gain disappears after budget & hidden-state controls |

**Formal SIS Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA` (secondary `BENCHMARK_DELTA`); `CorePressure=WATCH`; `ScientificCoreDelta=0`; `SPEC_REVISION_CANDIDATE=NO`. The evidence challenges the identification and validity of existing measurements. All new estimands remain expressible under SCF/SDR/ASR, CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG; no uncovered scientific primitive is established.
