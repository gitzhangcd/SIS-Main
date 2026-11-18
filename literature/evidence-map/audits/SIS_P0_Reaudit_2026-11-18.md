# SIS P0 Claim-Level Re-Audit｜2026-11-18

**Authority:** SIS v0.3.1 Scientific Master; SIS-LEM-P0; ClaimRecord v0.1. **Unit:** 3 EXISTING StudyVersionRecords → 9 different scientific claims. **Status:** FIRST_CODER_ONLY; second coder and adjudication PENDING.
**Sources:** official Anthology proceedings for 109,110, primary author institutional article for 111, and original author arXiv HTML including result tables and ablations. None is newly published today; this is historical P0 backlog advancement.
**Guard:** Old paper-level candidate CL2/CL3 and T2 are triage only. No final ClaimLevel promotions, no CL3 or T3/T4.

## SIS-LIT-109｜BayesFlow
**Version lineage:** EACL Findings March 2026 / arXiv 2601.22305v1
**Primary provenance:** https://aclanthology.org/2026.findings-eacl.165/ ; https://arxiv.org/html/2601.22305
| Claim | Primary estimand / program / framework | First coder ceiling, identification and transfer | Evidence / limitation / kill test |
|---|---|---|---|
| 109-C1 | `SIX_DATASET_BAYESIAN_WORKFLOW_SEARCH_VS_AFLOW_TEST_ACCURACY` · SCF/BGT · MI/DR/MEAS/ID/BT | CL1 package; local I1 / T1 | Author Table 1: Claude executor six-task mean 80.8±0.8 vs AFlow 76.2±3.1; Qwen executor 63.4 vs 59.9; 3 search seeds and repeated test execution. Different search mechanics and evaluation cost; no single mechanism established. **KILL:** Equal optimizer tokens/FLOPs × identical search and test sets × fixed executor × blinded evaluation. |
| 109-C2 | `UNREFINED_SMC_POSTERIOR_CONVERGENCE_UNDER_ASSUMPTIONS` · ROUTING_ABSTAIN/BGT · ID/MEAS/BT | CL0 theorem / I0 / T0 | Section 4.4 Theorem 1 assumes refiner absent, N→infinity and standard SMC assumptions. Does not certify finite-N output, chosen highest-validation-score workflow, or empirical refiner variant. **KILL:** Finite N × invalid proposal density × biased reward × refiner on/off × true posterior coverage. |
| 109-C3 | `REFINER_IMPORTANCE_WEIGHTING_INDEPENDENT_VALUE` · ASR/BGT · DR/MI/ID/MEAS/BT | CL1 local intervention candidate / I1 / T0 | Look-ahead importance weighting and in-loop refinement coupled; theorem not applicable to refinement; repeated validation selection induces optimizer's curse. **KILL:** 2×2 lookahead weighting × refiner × fixed total eval calls × hidden test. |
**Decision:** Maintain no automatic promotion. Separate package result, subcomponent or mathematical guarantee, and transfer into distinct claims. Second coder PENDING.

## SIS-LIT-110｜Learning to Evolve / TPGO
**Version lineage:** ACL Findings July 2026 / arXiv 2604.20714v1
**Primary provenance:** https://aclanthology.org/2026.findings-acl.1534/ ; https://arxiv.org/html/2604.20714
| Claim | Primary estimand / program / framework | First coder ceiling, identification and transfer | Evidence / limitation / kill test |
|---|---|---|---|
| 110-C1 | `TPGO_GRAPH_OPTIMIZER_PACKAGE_HELDOUT_TASK_NET_GAIN` · ASR/CSCI/BGT · MI/DR/IA/MEAS/ID/BT | CL1 package, local CL2 candidate / I1 / T1 | Original Table 2: GAIA 73.8→81.6 pass@1, wall clock 4014→1765s; graph, textual gradient, clustering, memory all bundled, offline optimization cost 19.9M tokens. **KILL:** Matched total optimization+deployment cost × hidden task Gold × update on/off. |
| 110-C2 | `TEXT_GRAPH_STRUCTURAL_EDIT_CLUSTERING_COMPONENT_EFFECT` · ASR/CSCI/BGT · MI/DR/ID/MEAS/BT | CL1 / local ablation candidate I1-I2 / T0 | Table 3 Browser Automation: full 28.03, w/o graph 25.13, w/o structural edit 24.90, w/o clustering 26.52, random clustering 19.97; edits affect search and instruction length. **KILL:** Factorial graph representation × edit freedom × clustering × equal candidate pool and token budget. |
| 110-C3 | `OPTIMIZER_HISTORY_STABILITY_VS_CAUSAL_TRANSFER` · ASR/BGT · DR/EG/MEAS/ID/BT | CL1 / T2 performance-only; CL3 not supported | Figure 3 with GRAO rises 26.41→33.74 then stable, no-GRAO peaks 30.03 then 14.55; Browser-trained update gives Web +1.82, Repo +2.73, 3D +3.13. Non-independent settings, no causal mechanism-invariance. **KILL:** Freeze archive × sham history × matched seed × multi-domain hidden tasks × loss of previous ability. |
**Decision:** Maintain no automatic promotion. Separate package result, subcomponent or mathematical guarantee, and transfer into distinct claims. Second coder PENDING.

## SIS-LIT-111｜Learning to Orchestrate / Conductor
**Version lineage:** ICLR 2026 author confirmation / arXiv v5 May 2026; OpenReview browser challenge
**Primary provenance:** https://sakana.ai/learning-to-orchestrate/ ; https://arxiv.org/html/2512.04388v5 ; https://openreview.net/forum?id=U23A2BUKYt
| Claim | Primary estimand / program / framework | First coder ceiling, identification and transfer | Evidence / limitation / kill test |
|---|---|---|---|
| 111-C1 | `RL_CONDUCTOR_POOL_CONDITIONAL_WORKER_SYSTEM_PERFORMANCE` · SCF/CSCI/BGT · MI/IA/DR/MEAS/ID/BT | CL1 package, local controlled comparison candidate / I1 / T1 | Table 7: controlled worker pool with Conductor higher scores than worker and alternative multi-agent baselines. Selection, topology, instructions and model budget jointly vary. **KILL:** Equal total worker calls/token budget × fixed model pool × randomized task order × topology placebo. |
| 111-C2 | `CONDUCTOR_TARGETED_SUBTASK_VS_TOPOLOGY_SELECTION_EFFECT` · SCF/CSCI/BGT · IA/MI/ID/MEAS/BT | CL1, local ablation candidate / I1 / T0 | Appendix B.7 removes task-specific instructions but retrains the Conductor; drop especially on code tasks, confounded by retraining and instructions. Scale effects of 3B vs 7B do not uniquely reveal mechanism. **KILL:** Fixed trained Conductor × topology fixed/shuffled × prompt matching × equal model pool. |
| 111-C3 | `DYNAMIC_WORKER_POOL_RECURSION_BUDGETED_TRANSFER` · ASR/CSCI/BGT · DR/IA/BT/ID/MEAS | CL1 / T2 performance-only; no T3 causal transport | Open-pool finetune and self-reference recursion are distinct; Table 2 recursive mean 61.93→63.00 with extra calls (<2×) and BigCodeBench 37.8→40.0. Not a free improvement, and model ID is not mechanism-invariance evidence. **KILL:** Fixed budget recursion × random worker substitution × unseen tools/domain × hidden benchmark. |
**Decision:** Maintain no automatic promotion. Separate package result, subcomponent or mathematical guarantee, and transfer into distinct claims. Second coder PENDING.

## Claim-level audit register
- IDs: 109-C1, 109-C2, 109-C3, 110-C1, 110-C2, 110-C3, 111-C1, 111-C2, 111-C3.
- **Evidence role:** 109 performance vs conditional formal theorem; 110 graph edit/optimizer feedback and retention; 111 component coordination vs information and recursive budget effects.
- **P0 changes:** 3 studies screened to HTML-matched first-coder status; source and version links refreshed. **Final CL promotions 0**; **new confirmed T3/T4 0**.
- **Kill-test decision:** All 9 claims require matching budgets, independent outcomes, and the intervention contrasts described above before formal CL2/CL3 promotion.
- **Core pressure:** WATCH on component–system interaction and optimization selection confounding; ScientificCoreDelta=0.
