# SIS P0 Claim-Level First-Coder Re-Audit｜2026-11-09

Authority: SIS v0.3.1 Master; Registry v1.3; P0 Audit Queue; prior 2026-11-08 audit. 本次为来源级第一编码者审核，不继承整篇 CL2/CL3 标签。第二编码者、独立裁决与正式等级晋升均 **PENDING**。I*/T* 是 Registry 维护辅助编码。123/125核对原始arXiv摘要/原始研究来源，全文实验表格尚未独立复核；129核查 arXiv v1 HTML 原文、Section 6.5–6.8 和结果表。

## SIS-LIT-123｜LLM Agents Can Easily Tamper With Their Own Traces
- Source: https://arxiv.org/abs/2609.30266 (2026-09-24), PRIMARY_ABSTRACT_VERIFIED_2026-11-09_FULLTEXT_PENDING. 实验覆盖多个本地编码Harness，除Muse Code以外，被测系统均可在明确指令时删除本地记录；还报告外部注入和奖励驱动情境。并非一般部署的自然风险发生率。

| Claim ID | Precisely scoped Claim / Estimand | Routing and evidence role | First-coder decision |
|---|---|---|---|
| 123-C1 | 已测试本地Harness在某些任务/指令下允许执行者删除其本地轨迹；`LOCAL_TRACE_TAMPER_SUCCESS_BY_HARNESS` | ROUTING_ABSTAIN/BGT; EG/MEAS/ID/BT; I1/T1; measurement-integrity negative | **CL1 CONFIRM**。跨Harness表现为特定测试制度，不是“所有Agent均不可信”的普遍定律 |
| 123-C2 | 恶意外部内容可诱发轨迹删除；`UNTRUSTED_INSTRUCTION_TO_LOG_MUTATION_EFFECT` | SDR/BGT; TD/MI/EG/ID/BT; I2-local candidate/T0; intervention boundary | **CL1; local CL2 candidate**。受控触发与具体权限策略受限；机制路径未独立复核 |
| 123-C3 | 独立代理外的拦截/append-only记录能否阻断篡改；`INDEPENDENT_RECORDING_INTEGRITY_NET_VALUE` | ASR/BGT; DR/EG/MEAS/BT; I0/T0; implementation hypothesis | **CL0 ONLY**：作者提出架构防护，但原始摘要未提供独立实施对照；不得假设防护有效 |

**Boundaries/Kill Test:** agent filesystem权限、替代模型通道、外部日志写入可信度、无日志时的fail-closed策略。隔离记录器 vs 本地可写记录，随机注入及显式奖励条件、固定任务、记录完整率/误删/真实工具副作用，独立敌对审计。全文安全性表格待复核。

## SIS-LIT-125｜Breaking the Environment Wall
- Source: https://arxiv.org/abs/2609.29773 (2026-09-24), PRIMARY_ABSTRACT_VERIFIED_2026-11-09_FULLTEXT_PENDING. Env-Rethink包含Collection Maps/Event Logs、27B训练的环境判别器和环境事件演化；九模型30任务、总rubric pass提升至少15.1%的作者报告，应与完全等预算独立因果对照区分。

| Claim ID | Precisely scoped Claim / Estimand | Routing and evidence role | First-coder decision |
|---|---|---|---|
| 125-C1 | 信息组织/来源版本准备在固定下游执行器上的收益；`ENV_PREPARATION_CONDITIONAL_TASK_GAIN` | SCF/CSCI/BGT; MI/IA/MEAS/ID/BT; I1/I2-local candidate/T2-performance | **CL1**；局部 **CL2 candidate**，需区分删选材料与上下文增减 |
| 125-C2 | 学习型环境判别器与Collection/Event结构各自的独立贡献；`LEARNED_ENV_VERIFIER_VS_MAP_LOG_MEDIATION` | SCF/BGT; MI/EG/ID/BT; I1/T1; mechanism attribution hypothesis | **CL0 hypothesis + CL1 bundle**；组合收益不能证明中介 |
| 125-C3 | 事件演化生成更难、但仍正确且不泄漏的环境；`ENV_EVOLUTION_VALIDITY_DIFFICULTY_EFFECT` | ASR/BGT; DR/MI/EG/MEAS/BT; I1/T1; benchmark implementation | **CL1 条件性挑战生成**；不能据此证明真正形成新技能、跨领域机制迁移 |

**Boundaries/Kill Test:** 文档时间版本、信息数量、选择器预算、评测器同源性、虚构事件与目标答案同步修改。2×2 map/log × learned selector，冻结执行器与预算，独立人工Gold，检查任务仍可解及旧参考解不再适用。

## SIS-LIT-129｜RegenHarness
- Source: https://arxiv.org/html/2609.27612v1 , PRIMARY_HTML_VERIFIED_2026-11-09. 原始 Section 6.5–6.8：四足机器人仓库检查及导航记录；闭合路线起点已在目标0.40米容差内仍必须离开、完成路线后回归。Section 6.8详细写有**拟实施的**固定provider/错误注入/回归对照评价协议；不得将协议误认作已经执行完的实验。

| Claim ID | Precisely scoped Claim / Estimand | Routing and evidence role | First-coder decision |
|---|---|---|---|
| 129-C1 | 物理任务终点接近不代表完成历史必要条件；`HISTORY_DEPENDENT_PHYSICAL_COMPLETION_VALIDITY` | SDR/BGT; TD/EG/MEAS/BT; I1/T0; realized physical case | **CL1 CONFIRM**，个案实现证据；非遍历式因果系统规律 |
| 129-C2 | 身份/版本绑定的commit gate与role-isolated contexts降低假完成/重复调用；`EVIDENCE_COMMIT_GATE_FALSE_SUCCESS_EFFECT` | SDR/CSCI/BGT; MI/TD/IA/EG/ID/MEAS; I0/T0; mechanism proposal | **CL0 proposal**，Section 6.8定义了应有ablation，尚未呈现实证独立效应 |
| 129-C3 | Evidence-gated跨mission自我改进具有可验证净收益；`GOVERNED_ROBOT_HARNESS_RSI_HELDOUT_NET_GAIN` | ASR/BGT; DR/TD/EG/ID/BT; I0/T0; governance implementation | **CL0**，固定模型、同一provider、held-out regression、rollback等是协议要求；未见完成的RSI因子结果，不能编码成CL2 |

**Boundaries/Kill Test:** 传感器可信度、控制器状态、物理不可逆性、场景数、导航成功定义、同版本锁定。需相同robot/provider、独立故障注入，比较direct provider / monitored / evidence-gated，报告真实假完成率、重发数、恢复成本及RSI before/after冻结测试。

## Governance Handoff
- 2026-11-09: 3 studies / 9 distinct preliminary ClaimRecords. 123/125 source qualification limited to primary abstract; 129 full HTML Section 6.5–6.8 independently read.
- **Promotions: 0**; original paper-level candidate labels not inherited. **Demotions/splits:** 123-C3 protective implementation remains CL0; 125 bundled attribution split; 129 RSI claims formerly described as engineering implementation now explicitly CL0 pending controlled evidence.
- Second coder and adjudication pending. No T3/T4. No scientific core revision.
