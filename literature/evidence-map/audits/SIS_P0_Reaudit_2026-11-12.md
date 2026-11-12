# SIS P0 Claim-Level Re-Audit｜2026-11-12

Authority: SIS v0.3.1 Master, Literature Registry v1.3, P0 Audit Queue. FIRST CODER ONLY. No automatic inheritance of paper-level CL2/CL3 candidate tags. Second coder and adjudication PENDING.

## SIS-LIT-016｜Meta^n

Primary source: https://arxiv.org/abs/2608.24735
Qualification: PRIMARY_HTML_ABLATION_REAUDITED_2026-11-12

| Claim | Primary estimand | Routing/Framework/Identification/Transport | First-coder disposition |
|---|---|---|---|
| 016-C1 | META_LAYER_DEPTH_CONDITIONAL_HELDOUT_TASK_GAIN | ASR/BGT; DR/MI/MEAS/ID/BT; I1 T1 | CL1 confirmed; local CL2 candidate pending budget-matched test. Multiple meta levels and available context vary together. |
| 016-C2 | INTERLAYER_CONDITIONING_VS_ARCHIVE_SELECTION_VALUE | SCF/CSCI/BGT; MI/IA/ID/BT; I1 T0 | CL1 ablation; CL3 mediation not established. Archive, depth and context covary. |
| 016-C3 | DEPTH_ONE_VALIDATION_SCORE_EQUALS_INDEPENDENT_TEST_GAIN | ROUTING_ABSTAIN/BGT; MEAS/EG/ID/BT; I0 T0 | CL0 measurement caution: depth-one best-archive validation scores are not independent held-out test scores; no depth-one held-out test pass. |

Boundaries: 模型、Archive大小、层间信息、API/token成本、训练与留出数据隔离
Kill test: n=1/2/3相同预算+Archive on/off+隐藏测试集+多随机种子

## SIS-LIT-017｜Recuris

Primary source: https://arxiv.org/abs/2608.24876
Qualification: PRIMARY_HTML_METHOD_AND_TABLES_REAUDITED_2026-11-12

| Claim | Primary estimand | Routing/Framework/Identification/Transport | First-coder disposition |
|---|---|---|---|
| 017-C1 | VERIFIED_WORKING_EXPERIENTIAL_MEMORY_COUPLING_LONG_HORIZON_EXECUTION_GAIN | SDR/BGT; TD/MI/EG/MEAS/BT; I1/I2-local T1 | CL1, local CL2 candidate for combination; memory and execution gate are not separated. |
| 017-C2 | KNOWN_COMPONENT_FAULT_STRUCTURED_TRACE_LOCALIZATION_EFFECT | SDR/BGT; TD/ID/EG/MEAS/BT; I2-local T0 | CL1, local CL2 candidate. Known-fault macro localization outcome-only 13.0%, raw trace 37.0%, structured 64.8%; not executed causal repair. |
| 017-C3 | EVOLVED_MEMORY_HELDOUT_REPAIR_TRANSFER_AND_GATE_NECESSITY | ASR/CSCI/BGT; DR/IA/MI/EG/ID/BT; I1/I2-local T2-performance | CL1, 86 held-out tasks +9.01–17.44 pp reported. No-gate comparison did NOT show the rejected patches' predicted held-out harm; gate necessity not validated. |

Boundaries: 任务长度、精确receipt、工具权限、86个保留任务、模型、不同记忆层
Kill test: 2×2记忆开关×检查器开关+注入故障重跑+独立Gate安全测试

## SIS-LIT-021｜SE-GoS

Primary source: https://arxiv.org/abs/2609.08228
Qualification: PRIMARY_ABSTRACT_REAUDITED_2026-11-12_FULLTEXT_PENDING

| Claim | Primary estimand | Routing/Framework/Identification/Transport | First-coder disposition |
|---|---|---|---|
| 021-C1 | EXECUTION_TRACE_EVOLVED_SKILL_GRAPH_OVER_STATIC_RETRIEVAL | ASR/BGT; DR/MI/MEAS/BT; I1 T1 | CL1; summary reports 52.4% to 59.4% reward, mechanism not isolated. |
| 021-C2 | TOPOLOGY_EDGE_WEIGHT_DESCRIPTION_COMPONENT_INCREMENTAL_EFFECTS | SCF/CSCI/BGT; MI/IA/ID/BT; I0/I1 T0 | CL0 mechanism hypothesis: topology, weights and description change together. |
| 021-C3 | HELDOUT_GRAPH_TRANSFER_TO_UNSEEN_TASKS | SCF/BGT; MI/BT/MEAS/EG; I1 T2-performance-only | CL1 only: reported +5.4 pp held-out versus static GoS, no T3 causal transport. |

Boundaries: 技能库、拓扑、技能检索、token与延迟、测试模型、任务族
Kill test: Topology×weight×description 2×2×2、固定预算多次执行和跨执行器

## Governance

3 studies, 9 atomic first-coder claims, 0 confirmed promotions, 0 verified T3/T4. 016/017 original HTML audited, 021 abstract only (fulltext pending). All final claim levels PENDING_CLAIM_LEVEL_AUDIT, second coder PENDING, adjudication PENDING. No Scientific Core change.
