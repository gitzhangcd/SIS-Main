# SIS Daily Literature Update｜2026-11-28
Base d5a5210f2a307695b16de9c809d149fcb70a5932. Master, full registry, P0 queue, evidence map/schema and previous note read. arXiv recent/new both show Nov 26 (different counts 248 and 398); no verified Nov 27 announcement. Targeted cross-source searches, not exhaustive. Ten delayed-discovery candidates: two VORs paired with preprints, eight preprints. No claim of new Nov 28 publication. 2611.33160 and 2611.33161 August submission vs November identifier quarantined; AutoDNA journal access failed. Full identifier/title scan; no duplicates found. Community discovery only. Selected HTML sections for Certify, Jacobian and FWSP; others abstract-level unless specified. No independent replication.

### SIS-CAND-20261128-01｜Evolving Agents in the Dark: Retrospective Harness Optimization via Self-Preference
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-emnlp.2439/ ; Pan et al.; EMNLP Findings October 2026; arXiv:2606.05922 v1 June 4, v3 August 29, same study; delayed discovery; abstracts.
- **SIS:** ASR; BGT; DR/TD/EG/MEAS/ID/BT; POLICY_VALUE; RETROSPECTIVE_SELF_PREFERENCE_HARNESS_UPDATE; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/implementation: replay difficult past tasks, self-consistency, candidate updates and self-preference. Reported SWE-Bench Pro 59% to 78% after one round; no external grading in optimization, not absence of independent evaluation.
- **Boundary / kill test:** Selection/validation separation, rerun budget, self-judge bias; freeze candidates, equal search cost, fresh gold and shuffled preference. SHARPENS. Must Read.

### SIS-CAND-20261128-02｜The Hard Part Comes After Search: Benchmarking Web Agents on Synthesizing, Organizing, and Displaying Knowledge
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-emnlp.2127/ ; Gill et al.; October 2026; arXiv:2609.30604 Sep 24 same study; delayed discovery; abstracts.
- **SIS:** DESCRIPTIVE_ONLY measurement; BGT; MEAS/EG/TD/ID/BT; operational JOINT_ARTIFACT_COMPLETION_VS_PARTIAL_STEP_SCORE; SCF CAPABILITY_FRONTIER_SHIFT candidate; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** INSTRUMENT/LIMIT: KNOWS browser tasks culminate in artifacts; deterministic checks plus judge; best full completion below 3%, visual failures can invalidate artifacts despite more than half other steps completed.
- **Boundary / kill test:** Rubric, visual usability, task difficulty, judge calibration; independent human artifact audit and fixed retrieval oracle. SHARPENS. Must Read.

### SIS-CAND-20261128-03｜Certify What You Plant: Shortcut-Free Proof Depth in Logical Reasoning Data
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33303v1 ; Juran et al.; Nov 24 2026; delayed discovery; HTML sections 3,4,7.
- **SIS:** DESCRIPTIVE_ONLY measurement; BGT; MEAS/ID/EG/BT; PLANTED_VS_REQUIRED_PROOF_DEPTH; separate SCF CAUSAL_MECHANISM_EFFECT candidate for training; MI/MEAS/ID; CL1/I2-local/T1; provisional first coder, no final promotion.
- **Evidence:** INSTRUMENT/LIMIT/NULL: audits eight datasets; mandatory rules and certificates relative to calculus. Balancing negation cue, fourteen Qwen3-0.6B seeds show no clear accuracy difference from certified depth alone; varied problem mixtures outperform narrow derivation data.
- **Boundary / kill test:** Calculus, shortcut cues, label balance, premise count, training mix; matched datasets and independent certificate checker. SHARPENS/CHALLENGES. Must Read.

### SIS-CAND-20261128-04｜The Platonic Representation Hypothesis in Jacobian-Space: Language and Vision Models Agree Approximately Up to a Rotation
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33304v1 ; Murphy & Brostow; Nov 24 2026; delayed discovery; HTML sections 3,5.4.
- **SIS:** SCF; BGT; MI/MEAS/ID/BT; CAUSAL_MECHANISM_EFFECT; ROTATED_JACOBIAN_STEERING_RESPONSE_TRANSFER; CL1/I2-local/T2 performance/intervention-response only; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT mechanism candidate: rotation fitted on subset of words; target activation interventions transfer to text, vision and image generation. Randomizing ViT blocks reduces steering; self-supervised vision without semantic readout lacks J-space alignment despite activation alignment. Not universal invariance.
- **Boundary / kill test:** Semantic head, layer, vocabulary, vector magnitude; held-out concepts, random rotation, matched norm and head swap, off-target tests. SHARPENS/WATCH. Must Read.

### SIS-CAND-20261128-05｜General-Purpose Decision Models for AI Configuration Tuning
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33190v1 ; Gong & Zhang; page states Nov 15 2026; delayed discovery Nov 26 listing; chronology not independently confirmed; abstract.
- **SIS:** ASR; BGT; DR/MEAS/ID/BT; POLICY_VALUE; DECISION_MODEL_ROLE_BY_TUNING_NET_VALUE; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** LIMIT/SUPPORT: eight tuning tasks, conventional optimizer ranks first in six, established predictor beats Jev in seven; region guidance can find lower perplexity at extra cost.
- **Boundary / kill test:** Role, search landscape, fees, latency; same tuner with/without guidance and matched budget. CHALLENGES. Must Read.

### SIS-CAND-20261128-06｜Confidence scores for gated automation of large language models
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33394v1 ; Alves & Vermeersch; Nov 24 2026; delayed discovery; abstract.
- **SIS:** ASR; BGT; DR/MEAS/ID/BT; SELECTIVE_ACTION_UTILITY; FROZEN_HIDDEN_STATE_CONFIDENCE_RISK_COVERAGE; CL1/I1/T2 performance only; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT: frozen 2B backbone linear confidence head beats text metamodels and prompted confidence; higher coverage at high accuracy; calibration can hide insufficient resolution, transfer modest. Data about 98% SQuAD.
- **Boundary / kill test:** Dataset, scorer, threshold, domain shift; fresh target calibration and independent risk-coverage gold. SHARPENS. Worth Skimming.

### SIS-CAND-20261128-07｜Crucible: Evaluating LLM Agents in Executable Chemistry Research Environments
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34254v1 ; Liu et al.; Nov 25 2026; deferred Nov 27 now screened; abstract.
- **SIS:** DESCRIPTIVE_ONLY measurement; BGT; MEAS/EG/TD/ID/BT; CHEMICAL_ARTIFACT_VALIDITY_VS_TOOL_EXIT_AND_OPTIMIZATION; SCF CAPABILITY_FRONTIER_SHIFT candidate; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** INSTRUMENT/LIMIT: 1078 tasks, 12 families, 18 datasets, 75 tools, seven environments, 14 models; best .545 overall; model 12th overall best closed-loop optimization. Tools can succeed while outputs chemically invalid; simulation/prior data not new wet lab.
- **Boundary / kill test:** Simulator fidelity, tool access, data overlap, grader validity; matched tool access and independent experimental gold. SHARPENS. Must Read.

### SIS-CAND-20261128-08｜TASK Memory: Beyond Text-Only Memory with Activation Steering and Knowledge Editing against Memory Hallucination
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34762v1 ; Zhao & Wu; Nov 25 2026; delayed discovery; abstract and method headings.
- **SIS:** SCF; BGT; CSCI hypothesis; MI/EG/MEAS/ID/BT; CAUSAL_MECHANISM_EFFECT; MEMORY_CONTENT_ADDRESS_USE_POLICY_EFFECT; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** LIMIT/SUPPORT: retrieved correct memory ignored up to 46%, misapplied up to 24%, 49% retrieval+editing; obsolete answer 53% with both versions. Text stores content, removable edit addresses entity, steering gates use; bundled.
- **Boundary / kill test:** Entity overlap, version, layer, access, unrelated knowledge retention; factorial text/address/steering and sham edits. SHARPENS. Must Read.

### SIS-CAND-20261128-09｜Do We Really Need an LLM for Weight-Space Programming? A Deterministic Forward-Only Paradigm and Its Capability Boundaries
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34612v1 ; Lin Yao; Nov 25 2026; deferred Nov 27 now screened; HTML section 4 dispatch table.
- **SIS:** ASR; BGT; DR/MI/MEAS/ID/BT; ACTION_SELECTION_EFFECT; STRUCTURED_FAULT_OPERATOR_DISPATCH_VALUE; CL1/I2-local candidate/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT: deterministic blind dispatch 15/18 vs 27B tool router 6/18; same library; exhaustive also 15/18, higher mean accuracy 67.0 vs 63.2 deterministic. Structured fault regime, not all optimization.
- **Boundary / kill test:** Fault generator, routing oracle, small n, probe costs, locality; held-out faults, equal library/budget, sham and abstention. CHALLENGES. Must Read.

### SIS-CAND-20261128-10｜A Failure-Driven Data Flywheel for Post-Training Vision-Language-Action Models
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34698v1 ; Luo et al.; Nov 25 2026; delayed discovery; abstract.
- **SIS:** ASR; BGT; DR/TD/MI/MEAS/ID/BT; POLICY_VALUE; FAILURE_CONDITIONED_DATA_ALLOCATION_HELDOUT_BEHAVIOR; CL1/I1/T2 performance only; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT: failure-map allocates synthetic data quotas. Five rounds sealed collision-free metric .261 to .579 AutoVLA and .390 to .765 ReCogDrive; vehicle pilot 4/5 vs 1/5. Anticipatory slowing improved more than reactive braking; no safety certification.
- **Boundary / kill test:** Simulator/physical shift, scenario diversity, compute, small pilot; random/static quota controls and independent safety tests. SHARPENS. Worth Skimming.

## P0
See literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-28.md. Nine first-coder claim splits, no promotion.

## Impact
MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; CorePressure WATCH; ScientificCoreDelta 0; no SPEC_REVISION_CANDIDATE. Master sections 36,54,58–62,66–68,82,91–94,165 and F4 cover targets. Benchmark certified proof difficulty vs planted labels; cross-modal intervention response vs static alignment; deterministic operator routing vs LLM; blinded clinical factorial with independent action gold. No new primitive.
