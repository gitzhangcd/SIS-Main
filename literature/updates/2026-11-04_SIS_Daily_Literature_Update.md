# SIS Daily Literature Update | 2026-11-04

Source: SIS v0.3.1 frozen Master + GitHub Registry v1.3 + P0 Queue. Current arXiv cs.AI listing Tuesday 2026-11-03 (816 total, 222 new); original manuscript dates 2026-10-30 to 2026-11-02. Ten strong primary preprints; no added peer-reviewed or independently reproduced community claims. Dated intake only; historic October 9–23 lineage reconciliation is pending.

**Formal SIS Impact Decision: MEASUREMENT_IDENTIFICATION_DELTA.** Secondary: BENCHMARK_DELTA. ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO.

## Selected papers and coding

| Source | Primary / Cross | Framework | Primary estimand | Claim ceiling | Priority |
|---|---|---|---|---|---|
| [Top-k Retrieval Leaves Memory Value Undetermined](https://arxiv.org/abs/2611.03289) | ROUTING_ABSTAIN / BGT | ID/MEAS/EG/BT | TOPK_MEMORY_VALUE_IDENTIFIABILITY_FROM_RETRIEVAL_DESIGN | CL0 theory + CL1 empirical; I0/I1/T0 | Must Read |
| [Can Coding Agents Sustain Continual Evolution without Forgetting?](https://arxiv.org/abs/2611.03219) | SDR / CSCI/BGT | TD/DR/ID/MEAS/BT | SEQUENTIAL_HARNESS_EVOLUTION_BACKWARD_RETENTION_EFFECT | CL1; local CL2 candidate; I1/I2-local/T1 | Must Read |
| [SelfImprove-Bench: Evaluating Generalization in Self-Improving Agents](https://arxiv.org/abs/2611.02797) | ROUTING_ABSTAIN / BGT | MEAS/EG/ID/BT | RSI_GAIN_GENERALIZATION_LADDER_CONSTRUCT_VALIDITY | CL1 benchmark; I1/T1 | Must Read |
| [Delivered, Not Used: Evaluating Agent Memory at Its Point of Use](https://arxiv.org/abs/2611.01718) | ROUTING_ABSTAIN / BGT | TD/MEAS/EG/ID/BT | DELIVERED_MEMORY_OBSERVED_USAGE_AND_EFFECT_VALIDITY | CL1; I1/T0 | Must Read |
| [Accessed, never disclosed: Silent access to protected health information by medical artificial intelligence agents](https://arxiv.org/abs/2611.02319) | SDR / BGT | TD/EG/ID/MEAS/BT | UNNECESSARY_PHI_TOOL_ACCESS_CONDITIONAL_POLICY_GATE_EFFECT | CL1; local CL2 candidate; I1/I2-local/T1 | Must Read |
| [LEANGUARD: Lean-Verified Guardrails for Tool-Using Agents](https://arxiv.org/abs/2611.02332) | ASR / BGT | MI/DR/EG/ID/MEAS/BT | FORMAL_TOOL_CALL_ADMISSION_AND_PROOF_GUIDED_REPAIR_EFFECT | CL0 conditional formal + CL1 empirical; I0/I2-local/T1 | Must Read |
| [CARE: Grounded Recursive Self-Improvement for Production Customer-Service Agents](https://arxiv.org/abs/2611.02839) | ASR / CSCI/BGT | DR/TD/EG/ID/MEAS/BT | VERSION_CONDITIONED_GOVERNED_RSI_UPDATE_ADMISSION_VALUE | CL1 composite; I1/T1 | Must Read |
| [Early Stopping in Large Reasoning Models: A Survey and Empirical Audit of Efficiency and Reliability](https://arxiv.org/abs/2611.00166) | ASR / BGT | DR/ID/MEAS/BT | EARLY_STOP_TOKEN_EFFICIENCY_JUSTIFICATION_VALIDITY | CL1 audit; I1/T1 | Worth Skimming |
| [Exo: An Architecture for Self-Improving Systems at Runtime](https://arxiv.org/abs/2611.00463) | ASR / CSCI/BGT | DR/MI/TD/EG/MEAS/BT | PROTECTED_RUNTIME_POLICY_EVOLUTION_COST_ADJUSTED_VALUE | CL1 composite; local candidate; I1/I2-local/T2-performance-only | Must Read |
| [ScienceCUA: Resource-to-Skill Construction and Execution-Guided Skill Evolution for Scientific Computer Use Agents](https://arxiv.org/abs/2611.03238) | SCF / BGT | MI/TD/EG/ID/MEAS/BT | SCIENTIFIC_DOCUMENTATION_TO_EXECUTABLE_SKILL_VALIDATED_VALUE | CL1; local candidate; I1/T1 | Must Read |

## Evidence, limitations and impact per study

### 1. Top-k Retrieval Leaves Memory Value Undetermined

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.03289.
- Idea / evidence: 证明 top-k 共检索日志无法识别单条记忆价值；14 基准、55 配置均无单项识别；LEDGER 经主动检索使 HotpotQA 可识别比例约 0.001→0.797。
- Limitations/confounders: 研究依赖特定 Shapley 价值定义及支持集设计；HotpotQA 准确率损失 2.6 点，可识别不等于有净收益。
- SIS: ROUTING_ABSTAIN; Cross BGT; Framework ID/MEAS/EG/BT; Estimand TOPK_MEMORY_VALUE_IDENTIFIABILITY_FROM_RETRIEVAL_DESIGN; CL0 theory + CL1 empirical; I0/I1/T0; evidence role Identification limit / negative.
- Boundary: 检索支持集、共同曝光、探索成本. SIS impact SHARPENS. Reading Must Read.

### 2. Can Coding Agents Sustain Continual Evolution without Forgetting?

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.03219.
- Idea / evidence: 三数据集六演化顺序比较；一个模型配置的 SWE-Bench 94%→32%，下降 62 个百分点，后续优化破坏原能力。
- Limitations/confounders: 需验证顺序、模型、预算和保留集独立性；不能泛化为所有模型必然遗忘。
- SIS: SDR; Cross CSCI/BGT; Framework TD/DR/ID/MEAS/BT; Estimand SEQUENTIAL_HARNESS_EVOLUTION_BACKWARD_RETENTION_EFFECT; CL1; local CL2 candidate; I1/I2-local/T1; evidence role Negative / retention boundary.
- Boundary: 任务顺序、执行器、版本、非回归门控. SIS impact CHALLENGES. Reading Must Read.

### 3. SelfImprove-Bench: Evaluating Generalization in Self-Improving Agents

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.02797.
- Idea / evidence: 游戏可控任务及 G0–G4 泛化阶梯评估自我优化是否超出训练场景；不同方法各阶梯收益不一致。
- Limitations/confounders: 作者 G0–G4 不等于 SIS T0–T4，游戏成绩不能证明 T3 因果传输。
- SIS: ROUTING_ABSTAIN; Cross BGT; Framework MEAS/EG/ID/BT; Estimand RSI_GAIN_GENERALIZATION_LADDER_CONSTRUCT_VALIDITY; CL1 benchmark; I1/T1; evidence role Measurement / transport boundary.
- Boundary: 难度、训练/测试隔离、系统变化. SIS impact SHARPENS. Reading Must Read.

### 4. Delivered, Not Used: Evaluating Agent Memory at Its Point of Use

- First submission: 2026-11-01. Original source: https://arxiv.org/abs/2611.01718.
- Idea / evidence: MemUse 分别审查记忆交付、内容新颖性、使用与后果；8000 条 SWE-bench 执行中三种记忆系统成功率与无记忆差距均在 0.4 百分点以内。
- Limitations/confounders: 影响标注依赖轨迹 Judge；没有随机记忆替换，不能把观察到的影响作为单条记忆因果效应。
- SIS: ROUTING_ABSTAIN; Cross BGT; Framework TD/MEAS/EG/ID/BT; Estimand DELIVERED_MEMORY_OBSERVED_USAGE_AND_EFFECT_VALIDITY; CL1; I1/T0; evidence role Measurement / conditional null.
- Boundary: 记忆冗余、交付时机、Judge 独立性. SIS impact SHARPENS. Reading Must Read.

### 5. Accessed, never disclosed: Silent access to protected health information by medical artificial intelligence agents

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.02319.
- Idea / evidence: 合成患者 Canary 与工具调用日志识别隐藏 PHI 读取；五模型四级权限七类攻击条件，三模型发生不必要读取，执行前门控接近消除。
- Limitations/confounders: 合成数据及构造攻击不是真实临床事故率；输出不泄漏不能证明访问合规。
- SIS: SDR; Cross BGT; Framework TD/EG/ID/MEAS/BT; Estimand UNNECESSARY_PHI_TOOL_ACCESS_CONDITIONAL_POLICY_GATE_EFFECT; CL1; local CL2 candidate; I1/I2-local/T1; evidence role Viability / controlled boundary.
- Boundary: 访问必要性、工具权限、声称授权、审计. SIS impact SUPPORTS. Reading Must Read.

### 6. LEANGUARD: Lean-Verified Guardrails for Tool-Using Agents

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.02332.
- Idea / evidence: Lean4 前置动作审查及可证明修复；Tau-Bench 未防护至少 33 条违规调用，防护 0 条；DTap 注入成功 57.9%→5.9%。
- Limitations/confounders: 形式证明只覆盖已编码规则；不能证明规范完整或真实用户意图正确。
- SIS: ASR; Cross BGT; Framework MI/DR/EG/ID/MEAS/BT; Estimand FORMAL_TOOL_CALL_ADMISSION_AND_PROOF_GUIDED_REPAIR_EFFECT; CL0 conditional formal + CL1 empirical; I0/I2-local/T1; evidence role Formal constraints / implementation.
- Boundary: 规范覆盖、Fail-closed、状态、工具副作用. SIS impact SUPPORTS. Reading Must Read.

### 7. CARE: Grounded Recursive Self-Improvement for Production Customer-Service Agents

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.02839.
- Idea / evidence: 生产自改进依据当时 SOP 版本独立盲审，分离模型与工具/技能故障，冻结模拟+离线评价+在线比较+人类批准完成准入。
- Limitations/confounders: 多个更新机制及策略变化共同作用；摘要没有足够随机效应数字支持单独因果晋升。
- SIS: ASR; Cross CSCI/BGT; Framework DR/TD/EG/ID/MEAS/BT; Estimand VERSION_CONDITIONED_GOVERNED_RSI_UPDATE_ADMISSION_VALUE; CL1 composite; I1/T1; evidence role Deployment governance / implementation.
- Boundary: SOP 版本、历史评估、更新准入、人类审查. SIS impact SHARPENS. Reading Must Read.

### 8. Early Stopping in Large Reasoning Models: A Survey and Empirical Audit of Efficiency and Reliability

- First submission: 2026-10-30; 2026-11-03 listed. Original source: https://arxiv.org/abs/2611.00166.
- Idea / evidence: 五推理模型的共同重放协议、TITE 指标；较晚出口不保证更正确，部分提前终止后支持理由更弱。
- Limitations/confounders: 重放不等于在线干预，成本需含停止判定与校准；同时含综述性内容。
- SIS: ASR; Cross BGT; Framework DR/ID/MEAS/BT; Estimand EARLY_STOP_TOKEN_EFFICIENCY_JUSTIFICATION_VALIDITY; CL1 audit; I1/T1; evidence role Measurement / stopping boundary.
- Boundary: 目标正确率、退出点、证据质量、预算. SIS impact SHARPENS. Reading Worth Skimming.

### 9. Exo: An Architecture for Self-Improving Systems at Runtime

- First submission: 2026-10-30; 2026-11-03 listed. Original source: https://arxiv.org/abs/2611.00463.
- Idea / evidence: 固定受保护的执行历史与策略激活层，允许实时修改执行政策；AppWorld/SREGym 相近正确率时模型费用下降约 35–61%。
- Limitations/confounders: 模型费用不等于全系统成本；多个实现因素同步变化且旧能力保持未充分识别。
- SIS: ASR; Cross CSCI/BGT; Framework DR/MI/TD/EG/MEAS/BT; Estimand PROTECTED_RUNTIME_POLICY_EVOLUTION_COST_ADJUSTED_VALUE; CL1 composite; local candidate; I1/I2-local/T2-performance-only; evidence role Framework / performance transfer.
- Boundary: 保护层、工作负载、成本账、更新准入. SIS impact SHARPENS. Reading Must Read.

### 10. ScienceCUA: Resource-to-Skill Construction and Execution-Guided Skill Evolution for Scientific Computer Use Agents

- First submission: 2026-11-02. Original source: https://arxiv.org/abs/2611.03238.
- Idea / evidence: 科学软件文档转为可执行技能与动态参考，并按成败轨迹验证更新；初始收益最多 7.23 点，演化后总收益最多 17.12 点。
- Limitations/confounders: 文档版本、执行条件和更新预算混杂；需独立测试严格正确性。
- SIS: SCF; Cross BGT; Framework MI/TD/EG/ID/MEAS/BT; Estimand SCIENTIFIC_DOCUMENTATION_TO_EXECUTABLE_SKILL_VALIDATED_VALUE; CL1; local candidate; I1/T1; evidence role Scientific capability / implementation.
- Boundary: 文档版本、任务隔离、软件状态、规范完整性. SIS impact SUPPORTS. Reading Must Read.

## Scientific synthesis and benchmark work

1. **Retrieval support-set identification:** prove whether memory value is estimable *before* fitting an optimizer; top-k logs may preclude individual effects.
2. **Continual self-improvement retention:** pair every new-task gain with old-task performance, full training/rollout budget, and versioned non-regression gates.
3. **Evidence-delivery ≠ evidence-use:** separate retrieval, use, influence and realized action; independent memory substitution is stronger than trace Judge scores.
4. **Viability is action-based:** output-only auditing misses PHI tool access; formal admission only certifies encoded policy obligations.
5. **Transport and scientific representations:** benchmark-internal G0–G4 is not SIS transport T0–T4; science software documentation requires executable provenance and disjoint gold.

| Priority | Proposed fixture | Measure / kill test |
|---|---|---|
| P0 | Top-k support-set × randomized memory exposure | identifiable value fraction, accuracy and exploration cost |
| P0 | Sequential evolution × old-task retention | old/new task delta, rollback, non-regression and full budget |
| P0 | PHI access gate × actual tool logs | unnecessary reads independent of output disclosure |
| P0 | Delivered memory × counterfactual action replay | use and independent marginal decision effect |
| P0 | Lean policy × specification completeness | forbidden-call reduction vs unencoded harms and repair costs |
| P0 | RSI generalization ladder × SIS transport | disjoint new problems; separate G0–G4 and T0–T4 |
| P1 | Science software version × skill verification | exact action/sequence/task conformance, cost |
| P1 | Stopping policy × justification | accuracy, token cost, answer support and drift |

P0 first-coder re-audit: SIS-LIT-115, 118, 127 (9 independent ClaimRecords). See evidence-map/audits/SIS_P0_Reaudit_2026-11-04.md. No final CL promotion or T3/T4. All impacts fit existing SIS core; no revision candidate.
