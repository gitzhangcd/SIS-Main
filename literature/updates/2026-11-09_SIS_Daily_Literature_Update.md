# SIS Daily Literature Update｜2026-11-09

**Authority:** SIS v0.3.1 Master Specification, Registry v1.3, P0 Audit Queue and prior 2026-11-08 note. **As-of:** Monday 2026-11-09 (Asia/Shanghai). Previous qualified daily intake: 2026-11-08. As of this run no new regular arXiv weekly public batch since Friday Nov 6; expanded delayed-indexing search of EMNLP 2026 Main/Findings and REALM 2026 October archives (plus arXiv/OpenReview/official sources). **Nine unique October peer-reviewed studies newly discovered for Registry plus one peer-reviewed version reconciliation (SIS-LIT-004)**. Therefore 10 valuable reading items but **not** ten newly published November papers. No padding with weak preprints; preprints category has zero qualifying newly checked items.

Search/dedup: exact paper title, ACL Anthology ID and Registry scan of 145 permanent studies plus prior daily candidates. A prior arXiv candidate **DCFA is already SIS-LIT-004**, so 2026 EMNLP archival version is a StudyVersionRecord update ONLY, not a new Study ID. Oct 9–23 historical candidate/global lineage backlog unresolved. Community analyses DISCOVERY_ONLY unless independently replicated. Paper-level intake is provisional; CL2 candidates are NOT formal ClaimRecord promotions; I*/T* are Registry-only aids.

## Selected paper-level entries (nine NEW studies, October delayed discoveries)

### SIS-CAND-20261109-01｜Causal Decomposition of LLM Agent Failure via Oracle-State Intervention

- StudyVersionRecord: https://aclanthology.org/2026.realm-1.6/; published 2026-10, class REALM_2026_WORKSHOP, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 420条WebArena失败轨迹、2模型；失败后替换真实结构化状态恢复率低于10%，持续oracle-state使成功率提升19–38%；58–74%故障在上下文与环境恢复后仍失败。
- Primary: **SDR**; cross-cutting: **BGT**; Framework Capability: **MI/TD/ID/MEAS/BT**; primary estimand: `POSTHOC_VS_CONTINUOUS_ORACLE_STATE_RECOVERY_EFFECT`.
- Claim maturity (provisional): **CL1; local CL2 candidate**; Identification **I2-local**; Transport **T1**; Evidence Role: **Negative mechanism boundary / state-timing intervention**.
- Evidence strength/limitations and key boundaries: 失败后修复与从一开始持续给予真实状态是不同制度；oracle-state是不可自然获得的特权信息；条件效应不证明全部失败机制。
- SIS impact: SHARPENS SDR：后验修复价值与连续状态治理价值分离。 Reading priority **Must Read**.

### SIS-CAND-20261109-02｜When Failures Propagate: Causal Failure Attribution in Agentic Retrieval-Augmented Generation

- StudyVersionRecord: https://aclanthology.org/2026.realm-1.46/; published 2026-10, class REALM_2026_WORKSHOP, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 在多跳检索中注入已知故障并重执行后缀；覆盖率型诊断在首跳准确0.91、后二跳0.00，过度依赖首跳启发式。
- Primary: **SDR**; cross-cutting: **BGT**; Framework Capability: **MI/TD/ID/EG/MEAS/BT**; primary estimand: `INJECTED_FAULT_HOP_CONDITIONAL_LOCALIZATION_ACCURACY`.
- Claim maturity (provisional): **CL1; local intervention target CL2 candidate**; Identification **I2-local**; Transport **T0**; Evidence Role: **Intervention benchmark / negative late-hop attribution**.
- Evidence strength/limitations and key boundaries: MuSiQue三跳与特定模型样本；已知注入位置是实验真值，但诊断正确率不是修复效应；后缀重执行会改变故障显现。
- SIS impact: SHARPENS SDR：注入位置、传播位置、故障被观察位置和实际修复收益分离。 Reading priority **Must Read**.

### SIS-CAND-20261109-03｜Beyond Consensus: Downward Bias and Role Asymmetry in Multi-Agent LLM Judges for Subjective Evaluation

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.243/; published 2026-10, class FINDINGS_EMNLP_2026, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 六种Judge模型、两类主观评分任务；多人共识反而降低人类对齐；三种消融将主要退化指向严格/宽松角色不对称及严格立场主导。
- Primary: **ROUTING_ABSTAIN**; cross-cutting: **BGT**; Framework Capability: **IA/MEAS/ID/EG/BT**; primary estimand: `ASYMMETRIC_JUDGE_ROLE_CONSENSUS_HUMAN_ALIGNMENT_EFFECT`.
- Claim maturity (provisional): **CL1; local CL2 candidate**; Identification **I2-local**; Transport **T1**; Evidence Role: **Negative evaluator-construct / role intervention**.
- Evidence strength/limitations and key boundaries: 人类评分自身有不确定性；角色、评分共享和讨论轮次均可改变分布；不能推断所有共识机制失效。
- SIS impact: SHARPENS MEAS/CSCI：共识一致性不等于独立人类真值。 Reading priority **Must Read**.

### SIS-CAND-20261109-04｜The Autonomy Tax: Defense Training Breaks LLM Agents

- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.52/; published 2026-10, class EMNLP_2026_MAIN, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 97项代理任务、1000次对抗提示；防御训练模型在干净任务上产生动作拒绝或无效调用，部分设置的超时99%而基线13%；作者称存在表面模式捷径学习。
- Primary: **SDR**; cross-cutting: **CSCI/BGT**; Framework Capability: **TD/IA/MEAS/ID/BT**; primary estimand: `DEFENSE_TRAINING_BENIGN_EXECUTION_AND_ATTACK_ROBUSTNESS_TRADEOFF`.
- Claim maturity (provisional): **CL1; local intervention candidate**; Identification **I1/I2-local**; Transport **T1**; Evidence Role: **Negative viability / cascading failure boundary**.
- Evidence strength/limitations and key boundaries: 模型训练和推理配置不同，不能完全归因于单一训练信号；攻击集不代表自然风险；99%仅为指定测试条件。
- SIS impact: SHARPENS SDR/CSCI：安全性更新必须联合监测任务能力与长时程失效放大。 Reading priority **Must Read**.

### SIS-CAND-20261109-05｜Leaving the Past Behind: Breaking Personalization Inertia in Long-Term LLM Agents

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.1744/; published 2026-10, class FINDINGS_EMNLP_2026, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: Pivot以轨迹独立证据判断既有偏好是否失效，并在局部回滚时保留可信前缀、重写后缀，报告个性化准确性和轨迹忠实度改善。
- Primary: **SDR**; cross-cutting: **BGT**; Framework Capability: **TD/DR/EG/ID/MEAS/BT**; primary estimand: `STALE_PREFERENCE_ROLLBACK_CURRENT_INTENT_CONFORMANCE_EFFECT`.
- Claim maturity (provisional): **CL1; local CL2 candidate**; Identification **I1/I2-local**; Transport **T1**; Evidence Role: **Temporal evidence boundary / local recovery**.
- Evidence strength/limitations and key boundaries: 历史偏好标签和当前意图Gold存在时效歧义；回滚策略、外部证据、修复均同时改变；缺真实长时程决策净收益。
- SIS impact: SHARPENS SDR：历史记忆可成为当前意图的错误约束，需状态时效和纠偏价值测量。 Reading priority **Must Read**.

### SIS-CAND-20261109-06｜Causal Episodic Memory for Feedback-Driven Agent Repair

- StudyVersionRecord: https://aclanthology.org/2026.realm-1.70/; published 2026-10, class REALM_2026_WORKSHOP, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 仅检索先前已结束episode的正负修复记忆；Spider执行准确率66.34→69.79%，BIRD 47.35→48.44%；Spider配对证据较清楚，BIRD较弱。
- Primary: **SCF**; cross-cutting: **BGT**; Framework Capability: **MI/TD/EG/ID/MEAS/BT**; primary estimand: `PRIOR_FINALIZED_REPAIR_MEMORY_CONDITIONAL_SQL_EXECUTION_GAIN`.
- Claim maturity (provisional): **CL1; local CL2 candidate**; Identification **I1/I2-local**; Transport **T1**; Evidence Role: **Conditional benefit / modest negative-null subtype evidence**.
- Evidence strength/limitations and key boundaries: Oracle辅助的真实答案反馈不一定生产可得；类型化检索与非类型检索未可靠区分；训练和运行成本应独立计。
- SIS impact: SHARPENS SCF：记忆效果是任务、Schema局部性与反馈制度条件性的。 Reading priority **Worth Skimming**.

### SIS-CAND-20261109-07｜Aligning Progress and Feasibility: A Neuro-Symbolic Dual Memory Framework for Long-Horizon LLM Agents

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.227/; published 2026-10, class FINDINGS_EMNLP_2026, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 分别构造语义进度记忆与从失败转移合成的可执行可行性检查函数，在ALFWorld、WebShop、TextCraft报告组合改进。
- Primary: **SDR**; cross-cutting: **BGT**; Framework Capability: **MI/TD/DR/EG/ID/MEAS/BT**; primary estimand: `GLOBAL_PROGRESS_VS_LOCAL_FEASIBILITY_CONSTRAINT_EFFECT`.
- Claim maturity (provisional): **CL1**; Identification **I1**; Transport **T1**; Evidence Role: **Composite implementation / failure-mode distinction**.
- Evidence strength/limitations and key boundaries: 同时增加上下文与逻辑检查，未独立证实各模块因果中介；检测到的可行性条件可能不完整。
- SIS impact: FILLS EXISTING FRAMEWORK：进度漂移与局部可行性违反应分别测量。 Reading priority **Worth Skimming**.

### SIS-CAND-20261109-08｜Drift No More: Spectral Locking for Long-Horizon Open-Weight Multi-Agent AI

- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.1796/; published 2026-10, class EMNLP_2026_MAIN, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 14,832标注轮次中三种漂移相关；联合task-role-state子空间的消融损失7.2分，等秩随机子空间损失0.8分；报告跨模型和扰动收益。
- Primary: **SDR**; cross-cutting: **CSCI/BGT**; Framework Capability: **MI/TD/IA/ID/MEAS/BT**; primary estimand: `TASK_ROLE_STATE_SUBSPACE_INTERVENTION_LONG_HORIZON_RETENTION`.
- Claim maturity (provisional): **CL1; local CL2 candidate**; Identification **I2-local**; Transport **T2-performance-only**; Evidence Role: **Representation intervention / conditional mechanism candidate**.
- Evidence strength/limitations and key boundaries: 隐藏态相关与激活操纵不必然证明单一中介；只适用于可访问内部状态模型；迁移为性能级非T3。
- SIS impact: SHARPENS CSCI/SDR：可观测轨迹漂移与表示层控制作用需分开。 Reading priority **Must Read**.

### SIS-CAND-20261109-09｜IterInject: Indirect Prompt Injection Against LLM Agents via Feedback-Guided Iterative Optimization

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.808/; published 2026-10, class FINDINGS_EMNLP_2026, discovered 2026-11-09 (delayed indexing).
- Novelty/primary evidence: 诊断反馈驱动的间接注入优化在AgentDojo/InjectAgent优于静态方法；在Claude Code 9个目标中5个完全成功，附带三项注意力层干预。
- Primary: **SDR**; cross-cutting: **BGT**; Framework Capability: **TD/DR/EG/ID/MEAS/BT**; primary estimand: `ADAPTIVE_UNTRUSTED_INPUT_ATTACK_SUCCESS_AND_ATTENTION_PATHWAY`.
- Claim maturity (provisional): **CL1; local CL2 mechanism candidate pending**; Identification **I1/I2-local**; Transport **T1**; Evidence Role: **Adversarial boundary / mechanism candidate**.
- Evidence strength/limitations and key boundaries: 构造攻击成功率不能代表实际发生率；训练预算与攻击迭代次数可能不同；注意力通路证据需独立复核，不能直接晋升CL3。
- SIS impact: SHARPENS SDR/EG：不可信输入的自适应攻击与证据权限边界。 Reading priority **Must Read**.

## Existing StudyVersionRecord reconciled — NOT a new study
- **SIS-LIT-004 DCFA**, existing arXiv https://arxiv.org/abs/2609.04749, has official peer-reviewed archive **https://aclanthology.org/2026.emnlp-main.1887/** (October 2026). Maintain ONE study identity, document preprint→EMNLP version lineage. Study-level classifier remains SDR / ASR cross-cutting (or BGT on transport question), Framework ID/IA/TD. The official abstract reports up to **8.27%** step-level attribution accuracy improvement across six LLMs on Who&When; structured graph + counterfactual-*inspired* reasoning is not executed causal repair. Existing source-level CL1/CL2 candidate not promoted, previous 2026-10-29 first-coder decision unchanged; independent re-audit needed for CL2.
- Version update is evidence/provenance change, not a tenth new unique study.

## P0 first-coder claim re-audit
- Full detail: [SIS_P0_Reaudit_2026-11-09](../evidence-map/audits/SIS_P0_Reaudit_2026-11-09.md).
- 123/125/129 → **9 claims** separated; 123 & 125 primary abstract only; 129 HTML Sections 6.5–6.8 verified. No whole-paper CL2/CL3 promotion; 123-C3, 129-C2/3 remain CL0 hypotheses or prospective protocols. Second coder pending.

## Science synthesis and candidate fixtures
1. **Context repair paradox:** post-failure oracle state rarely rescues agent but continuous state support has distinct value; do(pre-failure continuous vs do(post-failure replacement) with matched models and budgets, preserve intervention regime as boundary.
2. **Failure localization is not executed causal correction:** known injected hop can be missed after suffix changes. Inject@hop × ReplayPlacebo × RepairSuccess, report exact-hop and true recovery separately.
3. **Safety–competence trade-off:** adversarial defense can impair benign long-horizon action; SafetyUpdate × BenignTask × AttackType × ToolFault × ModelCapability, jointly report authorization, success, retry loops and actual security.
4. **Consensus is not independent Gold:** evaluator role asymmetry biases group scores; JudgeRoleAsymmetry × Debate × SharedScores × BlindedHumanGold and false-correction cost.
5. **History and representation must be conditional and causal:** stale personalization, dual memory, role steering, and episodic memory each change different system states; matched-policy exposure and tool-state evidence required. Representation intervention ≠ proven universal mechanism.

**Formal SIS Impact Decision: MEASUREMENT_IDENTIFICATION_DELTA**, secondary **BENCHMARK_DELTA**. This is real pressure on the measurement and identification of the existing P2/SDR and P1/SCF mechanisms, not uncovered core ontology. Scientific Core Delta=0; SPEC_REVISION_CANDIDATE=NO; no T3/T4 confirmation.
