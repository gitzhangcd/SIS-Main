# SIS P0 Claim-Level Re-Audit｜2026-11-20

**Authority:** SIS v0.3.1 Master and current P0 Audit Queue; claim records are not inherited from study-level candidate labels.
**Status:** FIRST_CODER_ONLY / SECOND_CODER_PENDING / ADJUDICATION_PENDING. 3 studies, 9 scoped claims; no formal CL2/CL3 promotions or causal T3/T4. Date reflects audit, not study publication.

## SIS-LIT-005｜LLM-as-a-Judge Is Not an Oracle
**Primary provenance:** https://arxiv.org/html/2609.02246; original field report with retrospective real-world cases.
**Record:** PRIMARY_ARXIV_HTML_FIELD_CASES_REAUDITED_2026-11-20.

| Claim | Primary estimand; program / Framework | Identification limit; maturity / transport | Required kill test |
|---|---|---|---|
| 005-C1 | `EVALUATOR_HARNESS_GOLD_FAILURE_TAXONOMY`; ROUTING_ABSTAIN/BGT; `MEAS/EG/ID/BT` | 11类现场失效（judge bias、解析/指标、Gold错误、reward hacking）作为CL1案例；生产数据不是事先定义的完整随机抽样; **CL1/I1/T0** | 事先冻结系统日志与故障标签×双人盲分类×独立语义Gold |
| 005-C2 | `BROKEN_SCORE_OPTIMIZATION_CAPABILITY_REGRESSION`; ASR/BGT; `DR/EG/MEAS/ID/BT` | 缓存答案或解析回退使指标提升但能力退化；观察性轨迹说明选择压力会利用缺陷，未随机化评估器错误; **CL1; mechanism hypothesis CL0/I1/T0** | 植入等幅评分器缺陷×冻结候选×盲任务Gold×随机选择与优化选择 |
| 005-C3 | `DETERMINISTIC_GUARDRAIL_AUTHORITY_SEPARATION_SAFETY_NET_VALUE`; ASR/CSCI/BGT; `DR/IA/EG/ID/MEAS/BT` | PROCTOR五层约束的现场经验与阻断实例；未完成完整2×…正交部署消融，且工具权限、模板改变同时变化; **CL1 implementation; local CL2 candidate only/I1/T1** | 等任务下角色权限×隔离×pre-apply验证×canary分层随机并以真实越权行为评分 |

**First-coder determination:** split three non-equivalent scientific claims; no package-to-mediator inflation; preserve source provenance, confounders and negative/absence findings; no normative CL promotion.

## SIS-LIT-046｜Why Prompt Optimization Works, and Why It Sometimes Doesn't
**Primary provenance:** https://arxiv.org/html/2605.26655; primary HTML observational study with IPTW and FDR claims.
**Record:** PRIMARY_ARXIV_HTML_IPTW_FDR_AND_LIMITS_REAUDITED_2026-11-20.

| Claim | Primary estimand; program / Framework | Identification limit; maturity / transport | Required kill test |
|---|---|---|---|
| 046-C1 | `PROMPT_EDIT_FAMILY_BY_TASK_PERFORMANCE_ASSOCIATION`; SCF/BGT; `MI/ID/MEAS/BT` | 约2万优化轨迹单位、IPTW按任务分层，部分多重检验BH-FDR后仍显著；作者明确称为associational，不是do(edit); **CL1/I1/T1** | 冻结上游prompt状态×随机指定编辑算子×多任务交叉×等token×事后盲评分 |
| 046-C2 | `COMPLEXITY_META_INSTRUCTION_MATH_MULTIHOP_NEGATIVE_BOUNDARY`; ASR/BGT; `DR/MEAS/ID/BT` | 复杂度与meta instruction在数学/多跳任务中的负相关为条件性信号；隐含文本变化与优化器选择未完全消除; **CL1 negative boundary/I1/T1** | 控制总长度/示例数×随机meta vs无meta×难度分层×跨模型留出 |
| 046-C3 | `CROSS_FRAMEWORK_EDIT_MOTIF_TRANSFER_VS_CAUSAL_INVARIANCE`; SCF/CSCI/BGT; `MI/IA/ID/BT` | 跨框架/多个编辑表示方向复核提升可重复性，不是T3因果机制运输；motif测量和未测混杂限制; **CL1/T2 performance pattern, no T3/I1** | 同一编辑操作跨框架盲置换×原任务与新任务×模型能力梯度×等预算 |

**First-coder determination:** split three non-equivalent scientific claims; no package-to-mediator inflation; preserve source provenance, confounders and negative/absence findings; no normative CL promotion.

## SIS-LIT-063｜REALM: Retrieval-Driven Memory Reconsolidation
**Primary provenance:** https://arxiv.org/abs/2609.16053; primary arXiv original research (source text/method/result sections reviewed).
**Record:** PRIMARY_ARXIV_FULLTEXT_EXTRACTED_METHOD_RESULTS_REAUDITED_2026-11-20.

| Claim | Primary estimand; program / Framework | Identification limit; maturity / transport | Required kill test |
|---|---|---|---|
| 063-C1 | `RETRIEVAL_DRIVEN_RECONSOLIDATION_MEMORY_QA_EFFECT`; SCF/BGT; `MI/TD/EG/MEAS/ID/BT` | LoCoMo 75.97%与LongMemEval 65.11%，超过最佳对照7.17/1.31分；组件及预算未完全正交; **CL1; local ablation CL2 candidate/I1/T1** | 冻结检索输出×允许/禁止图重整×同模型×跨会话独立题×计入维护费用 |
| 063-C2 | `ADAPTIVE_GRAPH_RETRIEVAL_VS_RECONSOLIDATION_COMPONENT_EFFECT`; ASR/CSCI/BGT; `DR/MI/IA/ID/MEAS` | 自主建图、可组合搜索与retrieval-feedback同时存在；消融支持模块必要性候选，未识别唯一中介; **CL1/I1/T1, CL3 not supported** | 2×2因子：静态/动态搜索×关闭/打开重整×图固定×同查询预算 |
| 063-C3 | `MEMORY_TOPOLOGY_CHANGE_FUTURE_APPLIED_DECISION_AND_REGRESSION`; SDR/BGT; `TD/EG/ID/MEAS/BT` | 结构更一致与QA分数改善不等于未来行动净效用；缺少真实后续操作或负记忆退化的充分观测; **CL0 mechanism + CL1 descriptive/I0-I1/T0** | 记录每次图变动×后续实际行动Gold×反事实撤回×时效失效任务×保留集 |

**First-coder determination:** split three non-equivalent scientific claims; no package-to-mediator inflation; preserve source provenance, confounders and negative/absence findings; no normative CL promotion.

## Audit governance & disagreements to resolve
- **005:** deterministic verifier rejects syntactic/authority violations but cannot prove semantic task truth; field anecdotes are not randomized policy-value estimates.
- **046:** propensity-weighted **observational association** and BH-corrected patterns are not randomized edit effects; T2 pattern replication != T3 transport.
- **063:** reconsolidation may improve benchmark answers, but memory topology changes and realized future-action causal contribution remain separate outcomes.
- **Pending independent second coder:** check source tables, repeated runs/selection, scenario eligibility and claim-level estimand consistency. On disagreement perform adjudication. Keep Queue final fields PENDING_CLAIM_LEVEL_AUDIT.
- **Impact decision:** MEASUREMENT_IDENTIFICATION_DELTA; CorePressure WATCH; ScientificCoreDelta=0; no new Scientific Core primitive.
