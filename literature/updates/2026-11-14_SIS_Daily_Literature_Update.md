# SIS Daily Literature Update｜2026-11-14

**Source of truth:** SIS v0.3.1 Master, Registry v1.3, P0 Audit Queue. **Scientific Core remains FROZEN.**
**Discovery date:** 2026-11-14 (Asia/Shanghai). Latest official arXiv cs.AI `new` Friday 2026-11-13: **537 entries total (including cross-lists/replacements), 113 new submissions**. Never mistake listing date for first preprint submission date.

## Qualification, deduplication and source lineage
- 10 distinct studies first submitted Nov 10–12, not already present in the current Registry by exact arXiv ID; all source identity and first-submission date verified at official arXiv abstract. They are **temporary SIS-CAND** entries, not permanent SIS-LIT IDs nor CL2 adjudications. All ten are preprints; author workshop acceptance alone does not count as verified proceedings. No peer-reviewed first-publication candidate strong enough to displace these ten in this run.
- Scanned official arXiv new list/cross-lists and targeted OpenReview, ACL Anthology, NeurIPS proceedings/project sources and selected technical/community discussions. Community analyses DISCOVERY_ONLY, no independent replication eligible for claim-level promotion.
- Existing 006 (arXiv → EMNLP 2026) and 062 (arXiv 2609.15779 v1 → v2 on Nov 2) are same-study lineages, not new studies. Existing 066 retains its original Study ID.
- No global one-study/one-paper total inferred from 145 permanent baseline + daily candidates; historical 2026-10-09–23 candidate ledger remains in reconciliation backlog.

## Peer-reviewed papers newly qualifying today
No newly independently archived, nonduplicate peer-reviewed item admitted in the top ten. **P0 re-audit** includes an existing officially archived EMNLP study, not counted as a new study.

## Preprints — selected 10, primary-source verified
### 01. Cleaning an Agent's History Hurts When the World Still Holds the Error — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.14654, v1 2026-11-10; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 同一正确值以真实备注写入历史，使恢复率51%→66%；伪装已执行动作则50%→44%；AppWorld错误成功回执在世界状态未实际改变时令成功率45%→28%。
- **Evidence quality, limitations:** 冻结状态后编辑历史/世界带来较强局部因果对照，但接收模型、写入操作、回执真实性、随机流位置与任务分布均限制迁移。
- **SIS primary:** `SDR`; cross-cutting `BGT`; Framework `TD/MI/EG/ID/MEAS/BT`; **primary estimand** `HISTORY_WORLD_STATE_CONSISTENCY_RECOVERY_INTERACTION`.
- **Claim maturity:** CL1; local CL2 candidate (history × world intervention), no CL3; identification I2-local; transport T1; **evidence role** NEGATIVE_BOUNDARY / EXECUTED_STATE_INTERVENTION; nature NEGATIVE / BOUNDARY.
- **Key boundaries:** world mutation; receipt truthfulness; history edit framing; receiver; tool side effects; replay fidelity.
- **Effect on SIS:** SHARPENS SDR/ID：历史语义与真实世界状态的交互，不是仅把错误从文本中删除；补充真实状态条件的恢复实验。

### 02. When Should Semantic Priors Enter Partially-Identified Causal Discovery? — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.14736, v1 2026-11-10; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 将语义先验拆为边查询分配、提议准入和DAG集合保留；不稳定边优先没有证实胜过随机分配；准入证书在当前校准样本下无法实现有用准入；学习参考集仅3/80包含真DAG。
- **Evidence quality, limitations:** 基准网络允许已知真图，能检验错误纳入与排除；但校准样本不足、参考集合覆盖缺失、总体不可识别与有限样本不稳定必须区分。
- **SIS primary:** `ASR`; cross-cutting `BGT`; Framework `DR/ID/EG/MEAS/BT`; **primary estimand** `SEMANTIC_CAUSAL_EDGE_QUERY_ADMISSION_GRAPH_RETENTION_VALUE`.
- **Claim maturity:** CL0 formal / CL1 controlled simulations; no CL2 confirmed; identification I1 / I2-local allocation controls; transport T0; **evidence role** NEGATIVE_IDENTIFICATION / CALIBRATION_BOUNDARY; nature NEGATIVE / MEASUREMENT.
- **Key boundaries:** causal identifiability; calibration support; reference DAG coverage; semantic prior error; graph Markov equivalence.
- **Effect on SIS:** SHARPENS ID/ASR：语义提议有信息量不代表其入场决策可认证。强调识别支持集和选择器准入。

### 03. Leaderboard Hacking: Preference-Based Model Evaluations are Vulnerable to Manipulation — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.14769, v1 2026-11-10; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 公开偏好排名在战略投票、挑选提示及插入无关模型后可被操纵；作者报告单一手段改变15–20名、联合手段最多45名。
- **Evidence quality, limitations:** 排名敏感性重评分不等于实际平台攻击发生率，Bradley–Terry假设、投票分布和允许的参与规则决定外推范围。
- **SIS primary:** `ROUTING_ABSTAIN`; cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; **primary estimand** `BRADLEY_TERRY_RANK_SENSITIVITY_TO_VOTE_PROMPT_NOMINATION`.
- **Claim maturity:** CL1 instrument audit; local deterministic re-ranking; identification I2-local (controlled manipulation); transport T0; **evidence role** MEASUREMENT_NEGATIVE / RANKING_INSTRUMENT; nature NEGATIVE / MEASUREMENT.
- **Key boundaries:** pairwise sampling; voting access; prompt selection; nomination rights; BT model assumptions.
- **Effect on SIS:** SHARPENS MEAS/EG：公开排行榜是可被参与机制影响的测量器，而不必然是系统能力变化。

### 04. When Is Proof-Step Verification Worth Its Cost? Operating Requirements of Certify-or-Decline Verification for Open-Weight Mathematical Reasoning — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.14794, v1 2026-11-10; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 对GPQA、AIME、MATH的分步认证提高被接纳回答的答案匹配精度，但仅覆盖35%或21%；等输出token的自一致基线精度差+4.8pp，95% CI [-8.2,18.5]；88个样本中52个构建证明前已失败。
- **Evidence quality, limitations:** 论文报告NeurIPS MATH-AI Workshop接收但未独立确认论文集；答案匹配、外部LLM接纳、形式证明真值不同；没有独立人类或形式内核真值。
- **SIS primary:** `ASR`; cross-cutting `BGT`; Framework `DR/EG/MEAS/ID/BT`; **primary estimand** `PROOF_STEP_CERTIFY_OR_DECLINE_PRECISION_COVERAGE_NET_VALUE`.
- **Claim maturity:** CL1; no independently verified proof-truth CL2; identification I1/I2-local comparative gate; transport T1 performance only; **evidence role** NEGATIVE / SELECTIVE_VERIFICATION_BOUNDARY; nature NEGATIVE / POLICY.
- **Key boundaries:** coverage; solver strength; proof parser failures; verifier budget; proof truth; task saturation.
- **Effect on SIS:** SHARPENS ASR/MEAS：验证的净收益应同时计入覆盖损失、前置执行失败与独立证明真值。

### 05. AutoAssumption: Searching over Assumptions Discovers ML-Systems Algorithms — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.14844, v1 2026-11-10; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 把89个ML系统算法映射为显式假设与Lean证明图，再放松某项假设、重推导、重证明并生成代码；作者在KV缓存淘汰与剪枝中报告较好结果，等预算与OpenEvolve相近。
- **Evidence quality, limitations:** 证明只保证给定形式假设与实现的相容性，算法选择、代码优化、基础设施和评测覆盖共同变化，不能独立识别‘假设放松’中介。
- **SIS primary:** `ASR`; cross-cutting `BGT`; Framework `MI/DR/EG/ID/MEAS/BT`; **primary estimand** `ASSUMPTION_RELAXATION_PROOF_CHECKED_ALGORITHM_DISCOVERY_VALUE`.
- **Claim maturity:** CL0 conditional proof validity / CL1 empirical package; identification I1; local matched budget; transport T1 performance only; **evidence role** IMPLEMENTATION / SCIENTIFIC_DISCOVERY_CANDIDATE; nature IMPLEMENTATION / MECHANISM_CANDIDATE.
- **Key boundaries:** formalization fidelity; assumption coverage; proof checker; code synthesis; equal compute; holdout.
- **Effect on SIS:** SHARPENS ASR/MI：假设本身可成为受约束的优化变量，但非新的科学纲领。

### 06. Verify by Doing: Co-Evolving Agent Execution and Evaluation without External Feedback — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.15276, v1 2026-11-11; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 固定权重、同任务演化Actor和Evaluator，后者主动检查工具及环境证据；在AutomationBench、τ³ Banking、GDPval上相较强基线分别报告+3.3、+4.1、+2.3个百分点。
- **Evidence quality, limitations:** 执行者与评价者协同演化造成互相适应、选择偏差和共同盲点；自生成评价不能替代外部独立Gold。
- **SIS primary:** `ASR`; cross-cutting `CSCI/BGT`; Framework `DR/MI/EG/ID/MEAS/BT`; **primary estimand** `CO_EVOLVED_ACTOR_EVALUATOR_FROZEN_MODEL_BUDGETED_VALUE`.
- **Claim maturity:** CL1; local CL2 candidate for ablation only; identification I1/I2-local; transport T1; **evidence role** MECHANISM_CANDIDATE / EVALUATOR_INDEPENDENCE_BOUNDARY; nature MECHANISM_CANDIDATE / POLICY.
- **Key boundaries:** shared failure modes; evaluator evolution; tool observability; fixed candidate pool; budget; independent Gold.
- **Effect on SIS:** SHARPENS ASR/EG：评价器进化应独立校准，不能让自评反馈自动授权更新。

### 07. Where Autonomy Belongs: A Separation of Powers for Agentic Program Evolution — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.15309, v1 2026-11-11; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** EvoTrias分离Govern、Propose、Judge的权限与Typed Contract；作者报告治理—提议分离降低64% token，扩展到68万行代码仓库，并主张保护独立Judge。
- **Evidence quality, limitations:** 治理、提议、评价权限、类型契约与工程实现可能共同变化；‘Protected Judge’的独立性需盲评及污染测试而非仅系统自述。
- **SIS primary:** `ASR`; cross-cutting `CSCI/BGT`; Framework `IA/DR/EG/MEAS/ID/BT`; **primary estimand** `GOVERN_PROPOSE_JUDGE_AUTHORITY_SEPARATION_NET_VALUE`.
- **Claim maturity:** CL1 package; no isolated authority mediation confirmed; identification I1/I2-local component comparison; transport T1; **evidence role** IMPLEMENTATION / AUTHORITY_BOUNDARY; nature IMPLEMENTATION / MECHANISM_CANDIDATE.
- **Key boundaries:** judge ownership; information leakage; candidate search budget; role capability; contract enforceability.
- **Effect on SIS:** SHARPENS ASR/CSCI：制度权威是因果干预变量，不是‘Multi-Agent’新原语。

### 08. CapLite: Prompt-Injection Defense for Small Language Model Agents without Model-Written Security Artifacts — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.17115, v1 2026-11-12; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 不让弱模型编写授权策略，基于工具schema和用户请求预先约束写操作；作者报告在13,935次AgentDojo受攻击执行中未成功越权，受攻击效用29.0%对CaMeL 27.2%。
- **Evidence quality, limitations:** 零次攻击成功不意味着任意工具/权限/用户请求都安全；写完整性保证依赖用户意图可明确定义、无隐藏副作用与固定威胁模型。
- **SIS primary:** `SDR`; cross-cutting `CSCI/BGT`; Framework `TD/IA/EG/MEAS/ID/BT`; **primary estimand** `SCHEMA_DERIVED_WRITE_AUTHORITY_INTEGRITY_AND_BENIGN_UTILITY`.
- **Claim maturity:** CL0 conditional integrity property / CL1 controlled episodes; identification I2-local under specified threat model; transport T1; **evidence role** NEGATIVE_BOUNDARY / CONDITIONAL_SAFETY_INSTRUMENT; nature NEGATIVE / BOUNDARY.
- **Key boundaries:** schema correctness; explicit user authorization; write-vs-read; hidden side effects; adversary powers; small model.
- **Effect on SIS:** SHARPENS SDR/EG：系统安全依赖可验证的权限边界，不能依赖较弱模型自证其安全策略。

### 09. Cited but Unused: Parametric Provenance in Retrieval-Augmented Generation — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.17161, v1 2026-11-12; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 通过替换检索段落中事实再提问，观察引用与模型内部知识的分离；所测配置中1.2%–15.7%可引用结论更像来自参数记忆，普通NLI校验接近随机，归因探针也不足以可靠触发干预。
- **Evidence quality, limitations:** 反事实替换会引入不自然内容和分布变化；能测模型已有知识，不必然识别当时实际使用的来源，故不能把检测输出视为科学证据溯源真值。
- **SIS primary:** `SCF`; cross-cutting `BGT`; Framework `MI/EG/ID/MEAS/BT`; **primary estimand** `CITATION_SUPPORT_VS_ACTUAL_RETRIEVED_EVIDENCE_USE`.
- **Claim maturity:** CL1; local I2 substitutions not mechanism identification; identification I2-local contrast, I1 provenance interpretation; transport T1; **evidence role** NEGATIVE_IDENTIFICATION / EVIDENCE_PROVENANCE; nature NEGATIVE / MEASUREMENT.
- **Key boundaries:** substitution distance; model scale; retrieved evidence conflict; NLI verifier; causal use vs availability.
- **Effect on SIS:** SHARPENS EG/ID：‘有引用’不等于‘使用了该证据’，也不等于证据对结论的因果贡献。

### 10. CoReMem: Cost-Internalizing Memory for Successive Coding Tasks with Prospective Valuation — **Must Read**
- **Paper version/provenance:** https://arxiv.org/abs/2611.17316, v1 2026-11-12; first discovered 2026-11-14. SOURCE=PREPRINT, claim screening only.
- **Novelty/findings:** 对同一继承代码仓库状态比较下一任务有无轨迹片段，结合记忆锚点和读写成本；ChainSWE上27B模型解决率21.0%→25.7%，步数减少17%，总缓存计费token减少11%。
- **Evidence quality, limitations:** 未来任务分布、片段筛选偏倚、actor再训练与锚点门控共同作用；相同继承仓库和配对控制只支持局部效应，不自动成立跨执行器迁移。
- **SIS primary:** `SCF`; cross-cutting `CSCI/BGT`; Framework `MI/DR/EG/ID/MEAS/BT`; **primary estimand** `PROSPECTIVE_MEMORY_SEGMENT_INTERVENTION_UTILITY_NET_COST`.
- **Claim maturity:** CL1; local CL2 candidate for next-task paired exposure; identification I2-local / package I1; transport T1; **evidence role** MECHANISM_CANDIDATE / COST_BOUNDARY; nature MECHANISM_CANDIDATE / POLICY.
- **Key boundaries:** future task distribution; inherited repo state; memory read-write cost; anchor use; actor policy; nonstationarity.
- **Effect on SIS:** SHARPENS SCF/CSCI/ASR：记忆价值应包含未见任务的真实增量及读写成本。

## Technical / community analyses
Discovery-only; no independently reproduced new claim eligible for maturity promotion. No padding.

## P0 claim-level re-audit
See [audit file](../evidence-map/audits/SIS_P0_Reaudit_2026-11-14.md): existing SIS-LIT-006, 062, 066; 9 atomic claims with source anchors, estimands, evidence roles, I/T, confirm/split/candidate ceilings and kill tests. **0 final promotions**, **0 T3/T4**, second coder pending. Queue source qualifications and stage updated. Source-version reconciled for 062.

## Scientific synthesis and proposed P0 fixtures
1. **History × actual world state**: truthful note vs falsely completed action across frozen-world and executed-world conditions; measure real executed recovery and replay fidelity.
2. **Semantic causal priors admission**: randomized query target vs edge uncertainty, independently calibrated admission plus reference DAG set coverage; distinguish population unidentifiability from finite sample variance.
3. **Evaluation institution validity**: blinded leaderboard voting/prompt/nomination interventions; proof precision–coverage curve; judge authority and grading independence, with independent Gold.
4. **Evidence causal use**: citation availability vs randomized evidence substitution/exposure vs final answers; require use-dependent counterfactual effects, not NLI citation consistency alone.
5. **Self-improvement governance**: independent Actor/Evaluator, govern/propose/judge separation and memory prospective value, with common candidate pool, fixed budgets and tests of regressions / information leakage.

| P0 Fixture | Primary estimand | Kill condition |
|---|---|---|
| HISTORY × WORLD × RECEIPT | `HISTORY_WORLD_STATE_CONSISTENCY_RECOVERY_INTERACTION` | Claim vanishes when real state/replay controlled |
| SEMANTIC_PRIOR × ADMISSION_SUPPORT | `SEMANTIC_CAUSAL_EDGE_QUERY_ADMISSION_GRAPH_RETENTION_VALUE` | False DAG exclusion under calibrated gates |
| JUDGE_ROLE × RANKING_PROTOCOL | `BRADLEY_TERRY_RANK_SENSITIVITY_TO_VOTE_PROMPT_NOMINATION` | Rank reversal under unchanged model capability |
| EVIDENCE_EXPOSURE × VALUE_SWAP | `CITATION_SUPPORT_VS_ACTUAL_RETRIEVED_EVIDENCE_USE` | Citations persist without causal dependence on evidence |
| MEMORY × FUTURE_TASK × COST | `PROSPECTIVE_MEMORY_SEGMENT_INTERVENTION_UTILITY_NET_COST` | No net value once read/write/steps included |
| UPDATE × INDEPENDENT_EVALUATOR | `CO_EVOLVED_ACTOR_EVALUATOR_FROZEN_MODEL_BUDGETED_VALUE` | Co-adapted evaluator accepts degraded true Gold |

## Formal SIS Impact Decision
**PRIMARY: MEASUREMENT_IDENTIFICATION_DELTA.** Secondary **BENCHMARK_DELTA**.
**CorePressure: WATCH**, but **SPEC_REVISION_CANDIDATE=NO** and **ScientificCoreDelta=0**.
All currently grounded phenomena fit SCF/SDR/ASR with CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG. Real pressure is on measurement identification and boundary operationalization, not a missing first-principles primitive or irreplaceable Framework Capability.
