# SIS P0 Claim-Level Re-Audit｜2026-11-16

**Scientific authority:** SIS v0.3.1 Master + Evidence Map P0 + ClaimRecord v0.1. **First-coder review of 3 existing studies, 9 distinct ScientificClaims.** The historical Registry Primary and ClaimLevel are triage metadata, NOT final routing or maturity.
**Scope/provenance:** official archived EACL/EMNLP publication records for 009/011, original arXiv full HTML for 011/012. 009 official abstract only; detailed EACL experimental tables remain pending. Full independent replication and second coder unavailable this run.
**Governance:** All `final_claim_level` remain `PENDING_CLAIM_LEVEL_AUDIT`, second coder PENDING, adjudication PENDING; **CL2/CL3 new confirmed = 0, T3/T4 new confirmed = 0**. Explicitly separate controlled local contrasts from mechanism/pathway claims.

## SIS-LIT-009｜Don’t Generate, Classify! Low-Latency Prompt Optimization with Structured Complementary Prompt
**StudyVersionRecord / provenance:** https://aclanthology.org/2026.eacl-long.204/ (EACL 2026 official archived study; abstract verified 2026-11-16; full main tables/appendices pending)
**Source qualification:** `PRIMARY_ANTHOLOGY_ABSTRACT_VERIFIED_2026-11-16_FULLTEXT_PENDING`. **First coder only**; full independent second-coder and adjudication pending.
| Claim | Primary estimand / scientifically distinct question | Routing & Framework | Ceiling / identification / transport | Evidence role & main boundary | Kill test |
|---|---|---|---|---|---|
| `009-C1` | `STRUCTURED_PROMPT_FIELD_CLASSIFICATION_COST_QUALITY_EFFECT` | Primary `SCF`; Cross `BGT`; `MI/MEAS/ID/BT` | CL1; I1/T1 | MEASUREMENT / IMPLEMENTATION — 分类式字段优化相对自由生成带来的整体质量-延迟效果；最多26.5% win-rate和最高1956x latency等作者摘要数字仅对应特定对照；质量与延迟同任务约束、基线算力及模型预算混杂 | Same corpus × same base model × iso-quality and iso-cost field-classify vs prompt generation |
| `009-C2` | `PROMPT_FIELD_ABLATION_INDEPENDENT_UTILITY` | Primary `SCF`; Cross `BGT`; `MI/ID/MEAS/BT` | CL1, local CL2 candidate; I1/T0 | MECHANISM_CANDIDATE — 结构化互补字段有助于优化但信息组织/搜索策略共同变化；未对所有字段进行独立随机化，不能声称已识别单字段中介 | 2×2 matched-budget prompt-field toggles × independent final model outputs |
| `009-C3` | `PROMPT_FIELD_JUDGE_HUMAN_AGREEMENT` | Primary `ROUTING_ABSTAIN`; Cross `BGT`; `MEAS/EG/ID/BT` | CL1 measurement validity warning; I1/T0 | MEASUREMENT / BOUNDARY — 自动Judge或少量人工偏好无法直接代表跨域真实质量；判别标签准确与任务收益必须分开 | Blind independent human Gold × judging rubric × model-choice stability |
**Audit decision:** Do not inherit study-level CL2 candidate; no mechanistic CL3 without mediator measurement/manipulation and competing pathways; no T3 from task or executor performance transfer.

## SIS-LIT-011｜Polished but Unresolved: Identifying Late-Stage Pressure States in Long-Horizon Tool-Use Agents
**StudyVersionRecord / provenance:** https://aclanthology.org/2026.emnlp-main.1143/ and https://arxiv.org/html/2609.00823 ; official EMNLP 2026 + original arXiv full HTML verified 2026-11-16; same study
**Source qualification:** `PRIMARY_ANTHOLOGY_AND_ARXIV_HTML_REAUDITED_2026-11-16`. **First coder only**; full independent second-coder and adjudication pending.
| Claim | Primary estimand / scientifically distinct question | Routing & Framework | Ceiling / identification / transport | Evidence role & main boundary | Kill test |
|---|---|---|---|---|---|
| `011-C1` | `HIDDEN_PRESSURE_PROBE_DISCRIMINATION` | Primary `SDR`; Cross `BGT`; `TD/MEAS/ID/BT` | CL1; I1/T0 | MEASUREMENT / BOUNDARY — 从隐藏激活预测后期执行压力、未完成约束的分类相关；线性可解码不等于压力状态为唯一因果变量 | Matched-length terminal traces × task hardness × independent pressure annotation |
| `011-C2` | `ACTIVATION_STEERING_LATE_STAGE_TERMINATION_EFFECT` | Primary `SDR`; Cross `BGT`; `MI/TD/ID/MEAS/BT` | CL1, local CL2 candidate; I2-local/T0 | MECHANISM_CANDIDATE — 作者对激活方向操纵影响结束/继续行为，但干预可能同时改变其他隐变量；不等于CL3中介因果识别 | Target steering × random orthogonal direction × matched activation magnitude × actual constraints completed |
| `011-C3` | `PSPR_CONSTRAINT_MAPPING_POLICY_NET_VALUE` | Primary `ASR`; Cross `BGT`; `DR/TD/EG/MEAS/ID/BT` | CL1; I1/T1 | IMPLEMENTATION / REGULATION — 后期约束识别插件改变任务完成率但新增提示/工具检查成本和信息量；必须审计约束满足而非回答润色 | PSPR on/off × equal task budget × independent completion oracle × early-stop negative controls |
**Audit decision:** Do not inherit study-level CL2 candidate; no mechanistic CL3 without mediator measurement/manipulation and competing pathways; no T3 from task or executor performance transfer.

## SIS-LIT-012｜τ^τ-Bench: An Environment for End-To-End, Realistic Agent Construction
**StudyVersionRecord / provenance:** https://arxiv.org/html/2609.04611 and https://arxiv.org/abs/2609.04611 ; original arXiv method/result sections verified 2026-11-16, not independently peer-reviewed
**Source qualification:** `PRIMARY_ARXIV_HTML_METHOD_RESULTS_REAUDITED_2026-11-16`. **First coder only**; full independent second-coder and adjudication pending.
| Claim | Primary estimand / scientifically distinct question | Routing & Framework | Ceiling / identification / transport | Evidence role & main boundary | Kill test |
|---|---|---|---|---|---|
| `012-C1` | `AGENT_CONSTRUCTED_SYSTEM_HELDOUT_TASK_SUCCESS_VS_EXPERT_CEILING` | Primary `SCF`; Cross `BGT`; `MI/MEAS/EG/BT` | CL1; I1/T1 | BENCHMARK / NEGATIVE — 53任务四个领域，作者所报告23.9%最佳vs 82.2%专家参考任务通过率；任务和参考实现难度限定结论，不是自治科研机制 | Same held-out tasks × independent expert acceptance × grader negative controls |
| `012-C2` | `SPECIFICATION_QUESTIONING_INHERITED_CODE_BUDGET_FAILURE_SUBTYPE` | Primary `SDR`; Cross `BGT`; `TD/MEAS/ID/EG/BT` | CL1 descriptive; I1/T0 | FAILURE_TAXONOMY / BOUNDARY — 构造任务失败可能来自需求澄清、已有代码适配、预算耗尽等；观察故障类别不能声称唯一因果来源 | Known injected requirement ambiguity × actual fix replay × equal budget |
| `012-C3` | `SERVING_BUDGET_CLIENT_SIMULATION_GOLD_VALIDITY` | Primary `ROUTING_ABSTAIN`; Cross `BGT`; `MEAS/EG/ID/BT` | CL0 specification / CL1 benchmark; I0/I1/T0 | MEASUREMENT / GOLD_CONSTRUCT — 模拟最终用户、服务预算和执行通过器内部一致性不等于真实客户需求已忠实建模 | Simulated client assertions × external expert semantic Gold × unforeseen deployment constraints |
**Audit decision:** Do not inherit study-level CL2 candidate; no mechanistic CL3 without mediator measurement/manipulation and competing pathways; no T3 from task or executor performance transfer.


## Cross-study decision and Core pressure
- Three StudyVersionRecords reconciled; 009 and 011 official proceedings are **same existing studies**, not newly created candidate identities; 011 source class corrected from PREPRINT to PEER_REVIEWED in P0 queue.
- 009: implementation quality/cost ≠ isolated representation mechanism or evaluator truth.
- 011: probe decodability ≠ mechanistic causal state; pressure-steering local effect ≠ proven mediator; not judging unfinished work as successful due to polished terminal text.
- 012: executable synthetic client Gold ≠ independent semantic truth; benchmark score difference ≠ inferred system-causal mechanism.
- **Program routing:** 009-C3 and 012-C3 use ROUTING_ABSTAIN; 011-C3 routes ASR rather than automatically inheriting study-level SDR. This demonstrates ScientificClaim routing rather than paper-level routing.
- **CorePressure WATCH** remains in identification/measurement; ScientificCoreDelta=0, no uncovered primitive. Primary ImpactDecision: MEASUREMENT_IDENTIFICATION_DELTA; Secondary BENCHMARK_DELTA.
