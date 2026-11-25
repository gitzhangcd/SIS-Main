# SIS Daily Literature Update｜2026-11-25
Authority: [Master](../../specs/System_Intelligence_Science_v0.3.1.md), [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md), [P0 Queue](../evidence-map/SIS_P0_Audit_Queue.csv); parent 900d3b1265cf437f5bf005bc0cb15f8649e1416c.
Search: arXiv cs.AI Nov 24 list 485 entries, targeted screening of first page; targeted ACL Anthology/OpenReview/conference/journal/project and technical searches, not exhaustive all listings. Eight preprints submitted Nov 23; two journal delayed discoveries Nov 19–20. MOFGen preprint→VOR reconciled with four vs five synthesized count discrepancy. No identified duplicate by title/IDs/known lineage against full Registry; RhoAgent earlier version unresolved. Primary abstracts verified; selected HTML checks on uncertainty, Tail-CRC and P0-070; no claim-level independent replication. Community roundup discovery only: https://nhip.verai.vn/en/papers/2026-11-24. Future dated December conference pages not treated as published. No padding.

### SIS-CAND-20261125-01｜System of agentic AI for the discovery of metal–organic frameworks — Must Read
- **StudyVersionRecord:** https://www.nature.com/articles/s43588-026-01058-x; Jaffrelot Inizan et al.; Nature Computational Science 2026-11-20; PEER_REVIEWED; arXiv:2504.14110 (2025-04-18) → DOI 10.1038/s43588-026-01058-x; one Study. Version discrepancy: preprint reports five synthesized MOFs, VOR four; use VOR four.
- **SIS:** Primary SCF; cross-cutting BGT; CSCI hypothesis; Framework MI/IA/EG/MEAS/ID/BT; canonical estimand CAPABILITY_FRONTIER_SHIFT; operational estimand PROPOSAL_STRUCTURE_FILTER_SYNTHESIS_VERIFIED_OUTPUT; provisional CL1/I1/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Physical verification/implementation; hundreds of thousands of candidates and four synthesized MOFs in VOR; not component causal effect.
- **Boundary / kill test:** Candidate selection, synthesizability, expert rules, experiment budget; compare equal-budget non-LLM proposal and independent blinded synthesis.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-02｜Programmable functional RNA design with a virtual scientist — Must Read
- **StudyVersionRecord:** https://www.nature.com/articles/s41587-026-03362-3; Huang et al.; Nature Biotechnology 2026-11-19; PEER_REVIEWED; DOI 10.1038/s41587-026-03362-3; earlier version not independently identified.
- **SIS:** Primary SCF; cross-cutting BGT; CSCI hypothesis; Framework MI/DR/EG/MEAS/ID/BT; canonical estimand CAPABILITY_FRONTIER_SHIFT; operational estimand RNA_DESIGN_EXPERIMENT_FEEDBACK_FUNCTIONAL_OUTPUT; provisional CL1/I1/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Physical validation/implementation: experimental feedback with RDiff; active ribozymes, up to sixfold cleavage relative to expert truncated construct, fluorescence +230% relative to wild type; not AI-specific causal contribution.
- **Boundary / kill test:** Assay, candidate selection, human baseline, wet-lab costs; freeze candidates and match number of synthesis attempts across ablations.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-03｜Language Models Steer on Injected Uncertainty Tokens, but Fail to Self-Monitor In Situ — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31228v1; Theron; PREPRINT; submitted 2026-11-23, announced 2026-11-24; HTML §§3,6 Table 5 checked.
- **SIS:** Primary SDR; cross-cutting BGT; Framework TD/MI/DR/MEAS/ID/BT; canonical estimand RECOVERY_EFFECT; operational estimand ERROR_VS_CLEAN_PREFIX_UNCERTAINTY_INJECTION_RECOVERY_RETENTION; provisional CL1; local CL2 candidate/I2-local/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Negative boundary + controlled recovery: 15,200 attempts, 2,017 error prefixes, 27,568 continuations; AUROC 0.500–0.561; low tag +3.7–22.5 pp correction vs high; correct-prefix disruption up to 22.8 pp. Separate ASR POLICY_VALUE for monitor-triggered intervention; not established by oracle prefixes.
- **Boundary / kill test:** Process judge validity, depth, model, tag semantics, intervention timing, compute; compare true/false trigger and placebo, cluster by task.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-04｜Seeking in Space: Benchmarking Purposeful Active Exploration of Vision-Language Models for Spatial Reasoning — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31215v1; Liu et al.; PREPRINT; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary ASR; cross-cutting BGT; CSCI hypothesis; Framework DR/TD/MI/MEAS/EG/ID/BT; canonical estimand ACTION_SELECTION_EFFECT; operational estimand FIXED_REASONER_OWN_VS_RANDOM_VS_ORACLE_EXPLORATION; provisional CL1/I2-local candidate/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Controlled benchmark: 994 questions, 234 episodes, 72 scanned scenes, 23 VLMs; strongest purposeful, memory loss; weaker may not outperform random. Oracle route is diagnostic ceiling not matched policy.
- **Boundary / kill test:** Scene, horizon, observation budget, memory, navigation cost, masked evidence; randomize routes and memory under fixed reasoner.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-05｜Reducing Order Sensitivity in Decision Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31174v1; Liu et al.; PREPRINT; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary SCF; cross-cutting BGT; Framework MI/MEAS/ID/BT; canonical estimand CAUSAL_MECHANISM_EFFECT; operational estimand OPTION_PERMUTATION_TREE_ATTENTION_DECISION_STABILITY; provisional CL1; local CL2 candidate/I2-local/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Boundary + implementation: ten models, eight mitigations; tree attention branches over shared context; no-retraining accuracy -1.1 pp while removing order sensitivity in tested setting.
- **Boundary / kill test:** Option count, semantics, tie behavior, training, latency; same options random permutations and positional-bias controls; preserve valid order-dependent tasks.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-06｜When Does Overriding the Majority Vote Help? — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31165v1; Ma and Zhang; PREPRINT; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary ASR; cross-cutting BGT; CSCI hypothesis; Framework DR/IA/MEAS/ID/BT; canonical estimand SELECTIVE_ACTION_UTILITY; operational estimand MAJORITY_OVERRIDE_CORRECTED_MINUS_INTRODUCED_ERRORS; provisional CL1/I1/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Negative/boundary: 150 math tasks, three models, 16 responses; executed programs correct more than harm at tested thresholds; cross-model override not established better than stronger standalone model; rare strict overrides.
- **Boundary / kill test:** Candidate availability, agreement, correlation, execution cost, sparse events; paired same-budget holdout and confidence intervals.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-07｜Tradeoffs between objective outcomes and human enjoyment of work in human-AI task allocation — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31095v1; Collins et al.; PREPRINT; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary ASR; cross-cutting BGT; Framework DR/IA/MEAS/ID/BT; canonical estimand ACTION_SELECTION_EFFECT; operational estimand HUMAN_ENJOYMENT_FRAMING_STAKES_ALLOCATION_CHOICE; provisional CL1/I1/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Behavioral evidence N=800; participants balance expected performance and enjoyment, particularly aversion; LLM heterogeneity. Actual welfare/policy value untested.
- **Boundary / kill test:** Stakes, framing, task type, actual experience vs stated choice, human preference; randomize work assignments with independent welfare and quality outcomes.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-08｜Decoupling Solving from Abstention: Single-Rollout Conformal Risk Control for Hard-Budget LLM Reasoning — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31065v1; Chen and Li; PREPRINT; submitted 2026-11-23 announced 2026-11-24; HTML §3.4 and Appendix A.1 checked.
- **SIS:** Primary ASR; cross-cutting BGT; Framework DR/MEAS/ID/EG/BT; canonical estimand SELECTIVE_ACTION_UTILITY; operational estimand FIXED_BUDGET_SOLVER_SUBMISSION_POLICY_WRONG_SUBMISSION_RISK; provisional CL0 theory; CL1 empirical/I1–I2-local/T2 performance only; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Conditional guarantee + experiment: fixed solver, tail token surprise; under exchangeability controls marginal expected wrong-submission probability (not accepted-case conditional risk); 8B Omni-MATH target calibration 30.3→5.8% at 4K, 41.8→6.5% at 8K.
- **Boundary / kill test:** Fixed kernel, exchangeability, family split, calibration, grader, budget; compare coverage and cost at fixed risk; stress OOD without recalibration.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-09｜ComputeWise: Measuring and Fixing GPU Waste by AI Research Agents — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31027v1; Pakhomov et al.; PREPRINT preliminary; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary ASR; cross-cutting BGT; CSCI hypothesis; Framework DR/TD/MEAS/ID/BT; canonical estimand REGULATION_NET_VALUE; operational estimand ANSWER_NECESSARY_GPU_TIME_VS_BUSY_TIME_SCHEDULING_POLICY; provisional CL1/I1/T1; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Resource measurement and implementation: replay simulator reports 52% necessary, 22% unnecessary work, 26% idle; prompt + code removes >80% excess time across five models.
- **Boundary / kill test:** Replay validity, hindsight definition of necessity, exploration value, parallelism, simulator fidelity, offline optimization costs; prospective real GPU trial and quality-matched baseline.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

### SIS-CAND-20261125-10｜Know When to Abstain: Conformal Confidence Estimation for Text-to-SQL — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.31190v1; Singh et al.; PREPRINT; submitted 2026-11-23 announced 2026-11-24; abstract.
- **SIS:** Primary ASR; cross-cutting BGT; Framework DR/MEAS/ID/EG/BT; canonical estimand SELECTIVE_ACTION_UTILITY; operational estimand SQL_ACCEPTANCE_CONDITIONAL_RISK_COVERAGE_AND_TRANSFER; provisional CL0 theory; CL1 empirical/I1/T2 performance only; no final promotion. CSCI only where explicitly stated as hypothesis.
- **Evidence:** Boundary/measurement: Spider 15% risk target δ=.1; 52.4% accepted and 9.1% observed accepted error, 10 resampled splits; BIRD AUROC .72 vs .79 Spider but risk guarantee does not transfer.
- **Boundary / kill test:** Schema shift, gold query equivalence, critic dependency, calibration set independence; target recalibration and accepted-case risk with coverage.; Impact SHARPENS (implementation results fill existing framework); independent coding pending.

## Synthesis / Formal decision
MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; CorePressure WATCH, ScientificCoreDelta 0, no SPEC_REVISION_CANDIDATE. Monitoring vs correction (SDR/ASR), conditional vs marginal risk and exchangeability (MEAS/ID), permutation invariance vs correctness (SCF), physical outcome vs attributable mechanism and complete resource costs (SCF/ASR), human experience vs objective outcomes (ASR). Existing §§9,15,54–56,58–62,71–73 and reopen conditions express these distinctions.
P0 fixtures: true/false error trigger × correction policy; risk denominator × target drift × calibration; option permutation × tree attention × valid order control; matched physical candidate budgets × blinded experimental Gold; replay GPU accounting × prospective actual GPU and hidden outcome; human assignment × welfare and quality.
P0 re-audit: [070/055/034 nine claims](../evidence-map/audits/SIS_P0_Reaudit_2026-11-25.md). No new permanent IDs.
