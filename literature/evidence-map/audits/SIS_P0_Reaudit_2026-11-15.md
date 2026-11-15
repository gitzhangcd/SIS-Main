# SIS P0 Claim-Level Re-Audit｜2026-11-15

**Source of truth:** SIS v0.3.1, Literature Evidence Map P0 and ClaimRecord Schema. **First coder**: 3 existing studies, 9 atomic claims. **Second coder / adjudication PENDING**. Original paper-level ClaimLevel is historical triage metadata. Claim final-level fields unchanged PENDING, no formal CL2/CL3 upgrade and no confirmed T3/T4.

## SIS-LIT-008｜MAPRO
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-eacl.233/ ; https://arxiv.org/html/2510.07475
- **Primary provenance:** Official EACL Findings and arXiv 2510.07475v1 HTML §3.2–3.4, §4 and Appendix C
- **Qualification:** PRIMARY_ANTHOLOGY_AND_HTML_REAUDITED_2026-11-15 ; peer-review status = ARCHIVED_PEER_REVIEWED.
- **Reconciliation:** Existing SIS-LIT ID retained; verified later official/archive or revised version is a lineage event, not second study.
- **First-coder audit:** each below is a separate ScientificClaim (not paper-level CL inheritance).

| Claim | Distinct question / primary estimand | Routing and Framework | Identification; maturity ceiling | Critical confound / decision |
|---|---|---|---|---|
| 008-C1 | 联合提示搜索相比人工/独立优化的端到端收益 — `JOINT_PROMPT_SET_OPTIMIZATION_PACKAGE_EFFECT` | SCF/CSCI/BGT; MI/IA/MEAS/ID/BT | I1/I2-local/T1; **CL1; local CL2 candidate** | 组合优化含初始化、反馈更新和搜索，模型/预算/任务未正交；不能断言相互作用中介 |
| 008-C2 | MAP 消息传递相对其它联合搜索的独立增量 — `MAP_MESSAGE_PASSING_VS_COMPUTE_MATCHED_SEARCH` | ASR/BGT; DR/MI/ID/MEAS/BT | I1/T0; **CL1 performance; CL2 pending** | 证明近似 MAP 搜索算法性质不等于 LLM reward model 校准或独立系统因果机制 |
| 008-C3 | 拓扑下游 blame 对特定 Prompt 的归因是否成立 — `DOWNSTREAM_BLAME_CAUSAL_PROMPT_CREDIT_VALIDITY` | SDR/CSCI/BGT; TD/IA/ID/EG/MEAS/BT | I1/T0; **CL0 mechanistic claim; CL1 heuristic utility** | 下游责备信号与真正干预修复不同；需步骤级替换和续跑 |

**Kill Test:** 同一候选池、等模型调用/FLOPs 的 MAP vs uniform/beam × 有无下游 blame × 固定拓扑执行器；已知扰动点执行反事实修复。
**Source / mechanism / transport gates:** No automatic CL2 via named optimizer or published venue; no CL3 without measured and manipulated mediator with competing-path controls; no T3 from cross-dataset performance alone.
**Lineage:** first coder audited 2026-11-15, second coder PENDING, blind adjudication PENDING.

## SIS-LIT-053｜ReflecTool-Bench
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-acl.86/
- **Primary provenance:** Official ACL Findings 2026 abstract and archived metadata (10 domains/88 APIs/968 dialogues/12 models); full appendix/table independent audit PENDING
- **Qualification:** PRIMARY_ANTHOLOGY_ABSTRACT_VERIFIED_2026-11-15_FULLTEXT_TABLES_PENDING ; peer-review status = ARCHIVED_PEER_REVIEWED.
- **Reconciliation:** Existing SIS-LIT ID retained; verified later official/archive or revised version is a lineage event, not second study.
- **First-coder audit:** each below is a separate ScientificClaim (not paper-level CL inheritance).

| Claim | Distinct question / primary estimand | Routing and Framework | Identification; maturity ceiling | Critical confound / decision |
|---|---|---|---|---|
| 053-C1 | 旁观 Critique 与自己执行 Self-Reflection 的性能差距 — `EXTERNAL_CRITIQUE_VS_SELF_REFLECTION_DETECTION_GAP` | SDR/BGT; TD/MEAS/ID/BT | I1/T1; **CL1 observed comparison** | 不同对话上下文和可访问证据条件，非同一错误的完整随机对照 |
| 053-C2 | 用户源错误与助手源错误在检测/修复上存在差异 — `USER_VS_ASSISTANT_ORIGIN_ERROR_DETECTION_AND_CORRECTION_GAP` | SDR/CSCI/BGT; TD/IA/MEAS/ID/BT | I1/T1; **CL1 measured boundary** | 错误难度与类别、调用环境和 Gold 标注同时变化 |
| 053-C3 | 解释与修正评分是否代表真实工具状态已恢复 — `ANNOTATED_CORRECTION_VS_EXECUTED_REPAIR_VALIDITY` | SDR/BGT; TD/EG/MEAS/ID/BT | I1/T0; **CL0 causal repair; CL1 task-level correctness metrics** | 没有配对执行续跑和环境状态验证不能把文本修正当真实恢复 |

**Kill Test:** 匹配同一注入错误 × observer/self × user/assistant origin × 相同信息与预算，再执行真实修复续跑和状态一致性验证。
**Source / mechanism / transport gates:** No automatic CL2 via named optimizer or published venue; no CL3 without measured and manipulated mediator with competing-path controls; no T3 from cross-dataset performance alone.
**Lineage:** first coder audited 2026-11-15, second coder PENDING, blind adjudication PENDING.

## SIS-LIT-056｜The Router Within / Gavel
- **StudyVersionRecord:** https://arxiv.org/html/2609.15982v2
- **Primary provenance:** Original arXiv HTML v2 §3.2–3.5, §4.2–4.5, Appendix F/H; first submission 2026-09-14, revised v2 2026-09-28 (same study)
- **Qualification:** PRIMARY_HTML_V2_METHOD_RESULTS_REAUDITED_2026-11-15 ; peer-review status = PREPRINT.
- **Reconciliation:** Existing SIS-LIT ID retained; verified later official/archive or revised version is a lineage event, not second study.
- **First-coder audit:** each below is a separate ScientificClaim (not paper-level CL inheritance).

| Claim | Distinct question / primary estimand | Routing and Framework | Identification; maturity ceiling | Critical confound / decision |
|---|---|---|---|---|
| 056-C1 | 从冻结模型隐状态读出路由信号的条件性表现 — `FROZEN_BACKBONE_LATENT_ROUTING_VS_EXTERNAL_RETRIEVAL` | ASR/CSCI/BGT; DR/MI/IA/MEAS/ID/BT | I2-local/T1; **CL1; local CL2 candidate** | 仅训练少量投影头，但对照外部检索参数和上下文开销不相同；路由准确率不是任务增益 |
| 056-C2 | Glance+Verdict 双阶段各组件的独立贡献 — `GLANCE_VERDICT_FUSION_INCREMENTAL_ACTION_VALUE` | ASR/BGT; DR/MEAS/ID/BT | I2-local/T1; **CL1 ablation; CL2 pending** | 候选召回变化与最终精排混杂，需等候选池/预算消融 |
| 056-C3 | 跨基础模型、途中调用和技能库规模的因果迁移 — `BACKBONE_SCALE_SKILL_LIBRARY_ROUTER_TRANSFER` | ASR/CSCI/BGT; DR/IA/BT/MEAS/ID | I1/T2; **CL1; T2 performance-only, no T3** | 不同基座和 SkillTraj 模拟轨迹，未证明同一机制跨模型稳定，也不能据 Codex 对照隔离路由贡献 |

**Kill Test:** 固定 skill metadata × 候选召回 × 等预算 Glance/Verdict 因子 × 基座能力/库规模/途中状态；真实任务结果而非路由标签为主要终点。
**Source / mechanism / transport gates:** No automatic CL2 via named optimizer or published venue; no CL3 without measured and manipulated mediator with competing-path controls; no T3 from cross-dataset performance alone.
**Lineage:** first coder audited 2026-11-15, second coder PENDING, blind adjudication PENDING.

## Governance and CorePressure
**Operations:** 3 studies / 9 ClaimRecords re-coded; positives vs negative/boundary claims split; all final_claim_level / final_primary_program / transport_final remain PENDING_CLAIM_LEVEL_AUDIT. Correctly separates author assertion from observed experimental estimand. Full-text table verification for 053 not completed, thus source qualification explicitly restricted.  
**CorePressure:** WATCH only; no uncovered primary estimand. **ScientificCoreDelta=0, SPEC_REVISION_CANDIDATE=NO**. Evidence Map gaps needing research: executed repairs; component interaction; independent Gold; causal transport and evaluator independence.
