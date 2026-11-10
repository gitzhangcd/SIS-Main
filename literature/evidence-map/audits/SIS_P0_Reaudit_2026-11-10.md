# SIS P0 Claim-Level Re-Audit｜2026-11-10

Authority: SIS v0.3.1 Master; Registry v1.3; P0 Queue. First-coder assessment based on original arXiv abstract and identified available claims, NOT full-text table or appendix verification. Paper-level CL2/CL3 candidate labels are NOT inherited. Second coder/adjudication pending.

## SIS-LIT-086｜Flag Game: A Toy Model for Mechanistic Swarm Interpretability
Original source: https://arxiv.org/abs/2609.19124; PRIMARY_ABSTRACT_REAUDITED_2026-11-10_FULLTEXT_PENDING.

| Claim | Precise estimand | Scientific route / evidence tier | First-coder decision |
|---|---|---|---|
| 086-C1 | GROUP_SIZE_BELIEF_COLLAPSE_POLARIZATION_REGIME | SDR/CSCI/BGT; IA/TD/MEAS/BT; I1/T1 | CL1 CONFIRM：规模与沟通制度条件下观察到信念坍缩和极化，不得外推普适规律。 |
| 086-C2 | PATCHED_AGENT_EVIDENCE_COLLECTIVE_OUTCOME_EFFECT | SDR/CSCI/BGT; MI/IA/ID/MEAS/BT; I2-local/T0 | CL1; local CL2 candidate：干预单个agent私有证据后群体结果改变；规模、位置、证据分布仍是边界。 |
| 086-C3 | SOCIAL_CIRCUIT_ATTRIBUTION_STATMECH_MEDIATION | SDR/BGT; IA/ID/MEAS/BT; I0/I1/T0 | CL0理论+CL1现象拟合；相图相似不足以证明唯一因果中介或跨群体规模机制不变。 |

Boundaries / Kill Tests: 群体规模×crop分布×Agent位置×对话结构正交试验，保留匹配随机干预、预测未见规模极化相变。原CL2到CL3整篇候选不继承。

## SIS-LIT-087｜Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation
Original source: https://arxiv.org/abs/2609.20822; PRIMARY_ABSTRACT_REAUDITED_2026-11-10_FULLTEXT_PENDING.

| Claim | Precise estimand | Scientific route / evidence tier | First-coder decision |
|---|---|---|---|
| 087-C1 | OBSTACLE_ACKNOWLEDGED_BUT_COLLISION_OCCURRED | SDR/BGT; TD/MEAS/EG/BT; I1/T0 | CL1：语言识别约束却在路径规划中仍碰撞，不唯一识别内部故障源。 |
| 087-C2 | GEOMETRIC_OBSTACLE_HARNESS_TASK_COLLISION_EFFECT | SDR/SCF/BGT; MI/TD/ID/MEAS/BT; I1/I2-local/T0 | CL1; local CL2 candidate：组合SafeHarness报告任务成功71.9%、避障87.5%，较比较方法提高6.5及27.0个百分点；需固定模型任务后归因。 |
| 087-C3 | ROUTE_PLANNING_VS_CONTACT_POLICY_CAUSAL_MEDIATION | SDR/BGT; MI/TD/ID/EG/BT; I0/I1/T0 | CL0机制假设/CL1组合实现：路线规划和触碰约束两个模块缺独立等预算2x2消融。 |

Boundaries / Kill Tests: 固定执行器和初始状态，路线规划×碰撞约束2x2、障碍位置扰动、真实接触及任务完成率双指标；不能将高避障分数当真实连续机器人安全证据。

## SIS-LIT-097｜Emergent Collusion in Long-Horizon LLM Agent Interaction
Original source: https://arxiv.org/abs/2609.24967; PRIMARY_ABSTRACT_REAUDITED_2026-11-10_FULLTEXT_PENDING.

| Claim | Precise estimand | Scientific route / evidence tier | First-coder decision |
|---|---|---|---|
| 097-C1 | REPEATED_INTERACTION_VERIFICATION_VIOLATION_PREVALENCE | SDR/CSCI/BGT; TD/IA/MEAS/BT; I1/T1 | CL1：构造奖励与监督冲突中的10模型实验有94%轨迹出现定义的合谋；不能推断现实发生率。 |
| 097-C2 | PEER_BEHAVIOR_INTERVENTION_COLLUSION_EFFECT | SDR/CSCI/BGT; MI/IA/ID/BT; I2-local/T0 | CL1; local CL2 candidate：同伴行为的控制性改变影响合谋；需明确定义do变量并控制反馈与历史。 |
| 097-C3 | HISTORY_SCOPE_REWARD_FEEDBACK_COLLUSION_MECHANISM | SDR/CSCI/BGT; TD/DR/IA/EG/ID/BT; I1/I2-local/T0 | CL1条件性：限制共享历史减少合谋现象；非已证明唯一中介，更不是T3跨任务机制。 |

Boundaries / Kill Tests: 按历史可见×奖励强度×伙伴干预正交设计，分别报告规范违规、真实任务利益和错误拒绝；不将模拟偏差称系统法则。

## Governance handoff
- 3 studies / 9 preliminary claim records. All source-qualified at abstract level only; full text and appendix pending.
- Promotions 0. Splits/demotions: 086 CL3 mechanistic paper-level candidate not adopted; 087 independent module mediation held CL0; 097 historical mediation and general collusion causal law not claimed.
- No confirmed T3/T4. Second coder and adjudication pending. Scientific core remains frozen.
