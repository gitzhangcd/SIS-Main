# SIS Daily Literature Update | 2026-11-03

Authority: SIS v0.3.1 frozen Core; canonical Registry and P0 Queue consulted before this run. Date of processing: 2026-11-03 Asia/Shanghai. arXiv cs.AI publicly listed 297 entries (98 new submissions) on Monday 2026-11-02. Selected papers were first submitted 2026-10-29 or 2026-10-30 UTC, and surfaced in the Nov 2 new listing; they were NOT newly submitted on Nov 3. All ten are PREPRINTS, with no verified archival peer-reviewed version.

Study-level source identifiers checked against the existing Registry (145 permanent entries plus dated provisional entries); no exact arXiv ID duplicates. Unreconciled October 9–23 provisional lineage still requires global reconciliation. No automatic CL2/CL3 or T3/T4 promotion.

## Intake index

| ID | Study | Primary | Cross | Claim ceiling | Reading |
|---|---|---|---|---|---|
| SIS-CAND-20261103-01 | [Does Recursive Knowledge Construction Help Agents Verify Consensus Claims in Science?](https://arxiv.org/abs/2610.40906) | SCF | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-02 | [ReplayRCA: Measuring Post-hoc Diagnosis and Live Oversight of Agent Failures by Counterfactual Replay](https://arxiv.org/abs/2610.41025) | SDR | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-03 | [More Rules, Longer Lists? Benchmarking Self-Evolving Agents on a Hidden-Rule Curriculum](https://arxiv.org/abs/2610.40758) | SCF | CSCI/BGT | CL1 | Must Read |
| SIS-CAND-20261103-04 | [BABA-Bench: Evaluating Long-Horizon Patient-Advocacy Agents](https://arxiv.org/abs/2610.41076) | SDR | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-05 | [Beyond Plausible Prediction: Safety Sufficiency in Web World Models](https://arxiv.org/abs/2610.40798) | SCF | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-06 | [Agentic World Modeling for Agent Test-time Scaling without Environment Replica](https://arxiv.org/abs/2610.40927) | SCF | BGT | CL1 | Must Read |
| SIS-CAND-20261103-07 | [Evidence-Guided Recovery for AI Agents with Ambiguous Tool Outcomes and Partial Execution](https://arxiv.org/abs/2610.41453) | SDR | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-08 | [When Should AI Agents Ask? Clarification Requests Under Limited Human Attention](https://arxiv.org/abs/2610.41129) | ASR | CSCI/BGT | CL0 theoretical + CL1 empirical | Must Read |
| SIS-CAND-20261103-09 | [Can Personal Requirements Become Supervision for Planning?](https://arxiv.org/abs/2610.40992) | SCF | BGT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261103-10 | [Counterfactual Pairwise Augmentation Improves Small Pointwise LLM Judges](https://arxiv.org/abs/2610.41149) | ROUTING_ABSTAIN | BGT | CL1; local CL2 candidate | Worth Skimming |

## Claim-level preliminary evidence coding

### SIS-CAND-20261103-01 — Does Recursive Knowledge Construction Help Agents Verify Consensus Claims in Science?

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40906 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 外部结构化证据状态与停止 Judge 分离测试，718 条由五个专家数据库标注的科学共识 Claim；外部状态优于纯上下文积累，独立训练 Judge 在五个子集中的三个达到最优或并列水平。
- Limitations and confounders: 专家共识不是普遍真值；检索覆盖、时间新鲜度、数据集独立性限制跨域因果推断。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/DR/EG/ID/MEAS/BT; primary estimand EXTERNAL_EVIDENCE_STATE_AND_STOP_JUDGE_CLAIM_VERIFICATION.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T1.
- Evidence role: Measurement / evidence externalization. Boundary variables: 证据结构、停止预算、Gold 独立性、领域、时效.
- SIS Impact: SHARPENS：既有 SCF 表示能力与 ASR 停止应拆为独立 Claim。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-02 — ReplayRCA: Measuring Post-hoc Diagnosis and Live Oversight of Agent Failures by Counterfactual Replay

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41025 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 同状态替换行动并配对原动作 placebo 重放，比较事后故障诊断和不知道最终结局的在线监督；62 个校准失败任务最佳事后修复 +51.3 点；87 次在线监督有系统反而 -14.5 点。
- Limitations and confounders: 生成式确定性 OpsWorld 不能代表真实系统；选择失败轨迹带来选择性，模型名次差异不全显著。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/ID/MEAS/BT; primary estimand PAIRED_REPLAY_POSTHOC_VS_LIVE_CAUSAL_REPAIR_EFFECT.
- Claim ceiling: CL1; local CL2 candidate; identification I2-local; transport T0.
- Evidence role: Controlled recovery / negative transport. Boundary variables: 已知失败、介入时间、不可逆性、重复执行、预算.
- SIS Impact: CHALLENGES：后验归因分数不能替代在线监督净收益。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-03 — More Rules, Longer Lists? Benchmarking Self-Evolving Agents on a Hidden-Rule Curriculum

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40758 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: CLR-Bench 测试从反馈中抽象未明示规则而非累积例外；20 条链、10 领域、六种自演化方法；部分模型收益不超过 5 点，不如保留原始历史，较强模型部分方法达到 78% 准确率。
- Limitations and confounders: 规则来自公开群体名称，预训练已知知识和模型识别性是关键混杂；不能证明自演化一般无效。
- Scientific routing: Primary SCF; Cross-cutting CSCI/BGT; Framework MI/ID/MEAS/BT; primary estimand HIDDEN_RULE_INDUCTION_VS_EXCEPTION_MEMORIZATION.
- Claim ceiling: CL1; identification I1; transport T1.
- Evidence role: Negative/boundary + capability interaction. Boundary variables: 组件能力、规则可识别性、历史记录、反馈量.
- SIS Impact: SHARPENS：能力形成区别于例外记忆；CSCI 是核心调节变量。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-04 — BABA-Bench: Evaluating Long-Horizon Patient-Advocacy Agents

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41076 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 47 个由去标识患者倡导案例改写的交互世界、14 模型和 1,974 次执行；921 次达成最终结果，其中 254 次（约 28%）走了不被允许的过程；提供经过验证的计划明显改善严格通过率。
- Limitations and confounders: 模拟场景不代表患者结局；路线提供的规范信息和规划能力提升耦合。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/EG/MEAS/BT; primary estimand GOAL_COMPLETION_CONDITIONAL_PROCEDURAL_AUTHORIZATION.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Clinical viability measurement. Boundary variables: 许可、证据、禁止动作、长时程协调、人类 Gold.
- SIS Impact: SUPPORTS：最终任务成功不等于系统 Viability。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-05 — Beyond Plausible Prediction: Safety Sufficiency in Web World Models

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40798 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 十个冻结模型的 3,000 个预测中 86.1% 被认为语义合理，却不能稳定支持 EXECUTE/ASK/BLOCK；安全微调可提高证据保留却降低授权判断。
- Limitations and confounders: 人类主观合理性不是安全授权 Gold；校准效果受基础模型与类别分布影响。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/DR/ID/MEAS/EG/BT; primary estimand PREDICTIVE_PLAUSIBILITY_VS_AUTHORIZATION_SUFFICIENCY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Negative construct-validity boundary. Boundary variables: 授权条件、ASK 召回、读出校准、证据缺失.
- SIS Impact: SHARPENS：预测合理和决策充分性应分开测量。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-06 — Agentic World Modeling for Agent Test-time Scaling without Environment Replica

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40927 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 以安全只读查询和可执行计算预测假设动作的后继观察，避免共享不可复位环境被多个轨迹修改；在 τ-bench、AppWorld、OfficeBench 相对单次模拟和训练世界模型有报告收益。
- Limitations and confounders: 隐藏写入副作用及不可见环境状态可能未被只读接口捕获；仿真提升不代表部署安全保证。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/TD/EG/MEAS/BT; primary estimand READ_GROUNDED_SIMULATION_NONRESETTABLE_STATE_VALUE.
- Claim ceiling: CL1; identification I1; transport T1.
- Evidence role: Implementation and observability boundary. Boundary variables: 可观察性、工具只读能力、状态更新、资源.
- SIS Impact: SUPPORTS：作为外部化状态估计的 Framework 实现。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-07 — Evidence-Guided Recovery for AI Agents with Ambiguous Tool Outcomes and Partial Execution

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41453 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 对超时、已提交与仍执行等未知结果做状态可行集和权限检查；预注册 58 个配对单元中指导接口认证完成 30 次、对照 9 次，差 36.2 个百分点，116 条轨迹独立重放通过。
- Limitations and confounders: 检验的是共同安全约束下的 Advice 接口，不是搜索算法独立收益；提供者契约、合成任务限制外推。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/EG/ID/MEAS/BT; primary estimand ADVICE_INTERFACE_CONDITIONAL_CERTIFIED_RECOVERY_EFFECT.
- Claim ceiling: CL1; local CL2 candidate; identification I2-local; transport T0.
- Evidence role: Controlled recovery / boundary. Boundary variables: 授权时效、未知效果、幂等性、残留效果.
- SIS Impact: SUPPORTS：受限状态下的证据引导恢复，不是普适 Exactly-Once。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-08 — When Should AI Agents Ask? Clarification Requests Under Limited Human Attention

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41129 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 把提问、检索和继续独立工作作为多任务共享人类注意力的动态策略；PCP 在至多两项未决要求时理论最优；864 合成实例平均距离最优成本 0.07%，比简单规则节约 18–31%。
- Limitations and confounders: 模型是理想化人类答复与任务耗时；小型 LLM 案例不能证明真实临床专家负担。
- Scientific routing: Primary ASR; Cross-cutting CSCI/BGT; Framework DR/IA/ID/MEAS/BT; primary estimand SHARED_HUMAN_ATTENTION_CLARIFICATION_NET_COST.
- Claim ceiling: CL0 theoretical + CL1 empirical; identification I0/I1; transport T0.
- Evidence role: Shared-resource regulation. Boundary variables: 注意力容量、任务关联、等待时间、询问成本.
- SIS Impact: SHARPENS：ASR 交互调节需要联合优化，而不是单任务贪心。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-09 — Can Personal Requirements Become Supervision for Planning?

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40992 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: Noura 利用可执行个人营养约束同时验证多日计划并生成训练目标；4,993 名保留参与者上同一执行闭环 Qwen3-14B 完整合规率 24.0% 至 72.5%，与模型生成目标相比执行目标在匹配比较中减少违规 41%。
- Limitations and confounders: 合规与营养质量是模拟计划指标，不能推广为临床疗效；指南约束、食品数据库和训练同时变化。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/EG/ID/MEAS/BT; primary estimand EXECUTABLE_PERSONAL_SPECIFICATION_SUPERVISION_PLAN_VALIDITY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T1.
- Evidence role: Clinical scientific specification. Boundary variables: 多疾病条件、用药冲突、专家 Gold、指南更新.
- SIS Impact: SUPPORTS：可执行科学规范作为数据构建、训练和评价桥梁。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-10 — Counterfactual Pairwise Augmentation Improves Small Pointwise LLM Judges

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41149 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 对同一查询构造并审核反向标签的配对样本训练判定器；六种二分类标准 Qwen3-8B 宏平均 F1 比点标注单独训练高 2.5 点。
- Limitations and confounders: 生成式反事实可能改变多项语义属性；Workshop 接收为作者自述，不作已正式归档会议论文证据。
- Scientific routing: Primary ROUTING_ABSTAIN; Cross-cutting BGT; Framework MEAS/EG/ID/BT; primary estimand COUNTERFACTUAL_PAIR_JUDGE_BOUNDARY_VALIDITY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Measurement instrument. Boundary variables: 反事实最小性、Gold 可靠性、标准分布.
- SIS Impact: SHARPENS：判定器准确率和独立科学真值需要分离。 Reading priority: Worth Skimming.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

## Formal SIS Impact Decision

Primary: MEASUREMENT_IDENTIFICATION_DELTA; secondary: BENCHMARK_DELTA; SPEC_REVISION_CANDIDATE=NO; ScientificCoreDelta=0.

Actual scientific pressure concerns post-hoc versus live causal repair, external evidence-state and stopping separation, viability versus terminal success, world prediction versus authorization, and model-capability-dependent rule learning. These are expressible in SCF/SDR/ASR, CSCI/BGT and existing thin Framework capabilities; none establishes an uncovered scientific primitive.

Recommended P0 fixtures: External Evidence State × Independent Judge × Expert Gold; Matched Replay × Post-hoc / Live; Hidden Rule Induction × Component Capability; Goal Success × Authorized Procedure; Predicted World × ASK/EXECUTE/BLOCK; Recovery Advice × Provider Capability; Human Attention × Task Dependencies; Executable Clinical Specification × Independent Dietitian Gold.

P0 re-audit separately covers SIS-LIT-089, SIS-LIT-068, SIS-LIT-088 (nine claim decisions, first coder only; second coder PENDING).
