# SIS Daily Literature Update｜2026-11-26
Authority: [Master](../../specs/System_Intelligence_Science_v0.3.1.md), [Registry](../SIS_v0.3.1_Literature_Re-Coding_Registry.md), [P0 Queue](../evidence-map/SIS_P0_Audit_Queue.csv). Base 816c7b56334bc263dc30bdabb7cdb635f5c27807; includes 2026-11-25 manual DeepEvidence intake. Search: arXiv cs.AI recent list 25 Nov (300 entries), targeted first-page screening; targeted OpenReview, ACL Anthology, NeurIPS/ICLR/ICML/ACL/EMNLP, journals and technical/project searches; not exhaustive. Nine v1 preprints submitted Nov 24; one delayed EMNLP VOR reconciled with March preprint. Title and identifier checks against complete registry; no duplicates identified. No padding. Most evidence abstract-level; selected HTML/table anchors below; no independent replication. Other discovered candidates HUB-J and Delegent not prioritized today; December-dated IBM General Agent Evaluation not treated as already published. Community technical reporting discovery only (e.g. Architect Labs CPU presilicon claims; no independent validation).

### SIS-CAND-20261126-01｜AgentCollab: A Self-Evaluation-Driven Collaboration Paradigm for Efficient LLM Agents — Worth Skimming
- **StudyVersionRecord:** https://aclanthology.org/2026.emnlp-main.2400/; Gao et al.; EMNLP October 2026 VOR; arXiv:2603.26034 (2026-03-27) same Study; delayed discovery; VOR abstract verified; full version delta pending.
- **SIS:** ASR; BGT; CSCI hypothesis only; DR/IA/TD/MEAS/ID/BT; POLICY_VALUE; SELF_EVALUATION_CONDITIONAL_ESCALATION_NET_VALUE; CL1/I1/T1; provisional only, independent coding pending.
- **Evidence:** Performance/implementation: small-large model control escalates based on self-evaluation and recent failures; reported accuracy-efficiency frontier gains. No independently identified trigger validity or component interaction.
- **Boundary / kill test:** Model pair, task difficulty, trigger calibration, escalation costs; random trigger, fixed routing, equal total budget and independent Gold. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-02｜Can LLM Judges Catch Unsafe Clinical Actions? A Fault-Injection Study — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33012v1; Ghafouri; preprint; 2026-11-24, announced 25; HTML §§IV–VII, Table IV/V checked.
- **SIS:** No forced primary route for measurement claim (DESCRIPTIVE_ONLY pending full audit); BGT; EG/MEAS/ID/BT; operational EHR_EVIDENCE_ACCESS_BY_FAULT_PAIRED_DISCRIMINATION; separate SCF mechanism contrast candidate; CL1/I2-local/T1; provisional only, independent coding pending.
- **Evidence:** Controlled measurement and negative boundary: 416 injected traces, eight faults, six judges; full trace paired discrimination Δ=.75 [.70,.80], EHR responses +.39 vs actions alone; rationale does not improve overall; original grader misses all 38 skipped checks; combined checker detects 97% injected faults. Not clinical safety or patient benefit.
- **Boundary / kill test:** Fault representativeness, clean parent clustering, severity scarcity, EHR access, reviewer dependence; blind real-fault Gold, harmless edit control, sensitivity/specificity and severity. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-03｜RecurSciBench: Benchmarking Recursive Self-Improvement in Data-Driven Scientific Research — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32508v1; Xu et al.; preprint technical report; 2026-11-24, announced 25; HTML §§4–5, Tables 2–3 checked.
- **SIS:** ASR; BGT; CSCI hypothesis; DR/TD/MEAS/ID/EG/BT; POLICY_VALUE; FROZEN_EVOLVED_STATE_VS_INITIAL_HELDOUT_SCIENTIFIC_TASK_GAIN; CL1/I1/T2 performance only; provisional only, independent coding pending.
- **Evidence:** Negative/boundary: four systems, fixed GLM-5.3-Flash, 20 disjoint test tasks; 24 evolved states gain -3.34% to +2.62%, half negative; all regress on >=8 tasks; positive average can coexist with 12 regressions. A learned safeguard can select wrong estimator in target task. No causal transport.
- **Boundary / kill test:** Evolution seed, source and target structure, relative-score aggregation, compute cost, only one backbone; independent evolution seeds, matched no-update and sham-update controls, per-task non-inferiority. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-04｜ShellBench: What Matters More for AI Agents, Models, or Harness for Everyday Tasks — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32946v1; Koc et al.; preprint; 2026-11-24, announced 25; abstract and HTML design/limitations headings checked.
- **SIS:** SCF; BGT; CSCI hypothesis; MI/IA/MEAS/ID/BT; MECHANISM_INTERACTION_EFFECT (candidate question); MODEL_HARNESS_EFFORT_BY_REALISTIC_TASK_PASS; CL1/I1/T1; provisional only, independent coding pending.
- **Evidence:** Performance/boundary: 100 tasks, 12 models, five harnesses, three reasoning levels, 53,100 rollouts; marginal harness pass@1 42.9–45.2; model choice larger overall in tested configurations. Not equivalence or proof of no interactions.
- **Boundary / kill test:** Compatibility missing cells, reasoning effort, estimated token cost, private tasks, judge validity; balanced factorial common support, task clustered uncertainty, prespecified equivalence margin. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-05｜Lazy Agents Answer Against Their Own Beliefs: Reinforcement Learning with Verifiable Beliefs Teaches Them to Act on What They Believe — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32884v1; Sin Jing Xuan et al.; preprint; 2026-11-24, announced 25; abstract.
- **SIS:** ASR; BGT; DR/TD/EG/MEAS/ID/BT; POLICY_VALUE; EXACT_POSTERIOR_GATED_CONTINUE_COMMIT_TRAINING; CL1/I1/T2 performance only; provisional only, independent coding pending.
- **Evidence:** Controlled training candidate/negative baseline: exact simulator posterior supplies process reward without reading stated beliefs. Three models × three benchmarks; reported mean +17.1% vs base, outcome-reward PPO/GRPO below base on average; two held-out benchmarks. Stated belief not established mediator.
- **Boundary / kill test:** Oracle posterior validity, simulator support, train/test split, reward shaping and compute; compare matched reward/compute, perturb posterior calibration, measure premature and unnecessary continuation. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-06｜RecordRoute: Auditing Agent Failures with Localization-Guided Diagnosis — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33022v1; Duan et al.; preprint; 2026-11-24, announced 25; HTML §5.4.2 Table 3 checked.
- **SIS:** SDR candidate for failure attribution; BGT; TD/MI/MEAS/ID/BT; PROPAGATION_EFFECT is future causal target not identified; operational LOCAL_RECORD_VS_FULL_TRACE_MODE_DIAGNOSIS; CL1/I2-local/T1; provisional only, independent coding pending.
- **Evidence:** Measurement/controlled evidence contrast: fixed actor and step predictions, same classifier design; 77.47% pooled joint accuracy vs 69.28% full trace, selected record median 19.77% trace tokens. Natural failure datasets support localization, not repair causality.
- **Boundary / kill test:** Injected shortcuts, annotation, error propagation, multiple causes; blind matched fault removal/replay and downstream recovery validation. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-07｜Measurement Artifacts in Trustworthiness Evaluations of Quantized Small Language Models — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32848v1; Abbas et al.; preprint; 2026-11-24, announced 25; abstract and HTML section map.
- **SIS:** DESCRIPTIVE_ONLY/no forced primary for measurement audit; BGT; MEAS/ID/BT; operational QUANTIZATION_BY_MEASUREMENT_INSTRUMENT_INTERACTION; CL1/I2-local/T1; provisional only, independent coding pending.
- **Evidence:** Measurement boundary: eight sub-2B models, three precisions, identical items and two annotators; human-rated harmful compliance rise only half to two-thirds keyword non-refusal rise; two scoring protocols correlate .10 vs noise ceiling ~.77; int8 batch/padding dependence reported.
- **Boundary / kill test:** Annotator scope, implementation, batch composition, precision, hardware, score construct; randomize instruments and batch composition, independent human Gold, report sign reversals. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-08｜MetaFORGE: A Meta-Learning Framework for Harness Optimization in Automated Code Generation for Parallel Computing — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33119v1; Piersall et al.; preprint; 2026-11-24, announced 25; abstract.
- **SIS:** ASR; BGT; CSCI hypothesis; DR/MI/TD/EG/MEAS/ID/BT; POLICY_VALUE; EXECUTION_GROUNDED_TEXTUAL_GRADIENT_SKILL_AND_MEMORY_TRANSFER; CL1/I1/T2 performance only; provisional only, independent coding pending.
- **Evidence:** Implementation and transfer: six MPI tasks × three workloads, correctness/compiler/runtime/load imbalance reward; model-matched refiner and retrieval ablation; held-out and zero-update tests support persistent skill and memory value.
- **Boundary / kill test:** Hardware/workload, reward weights, test leakage, optimization budget; 2x2 skill/memory frozen transfer, same optimizer budget, quality-constrained runtime. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-09｜VISE: Verifier-Independent Skill Self-Evolution with Feedback from Tool Implementations — Must Read
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32480v1; Liu et al.; preprint; 2026-11-24, announced 25; abstract.
- **SIS:** ASR; BGT; DR/MI/EG/MEAS/ID/BT; VALUE_OF_INFORMATION (candidate); IMPLEMENTATION_GROUNDED_REVISION_VS_NO_VERIFIER_POLICY; CL1/I1/T1; provisional only, independent coding pending.
- **Evidence:** Implementation/controlled candidate: source-code tool contract feedback plus traces used to revise skills; four evolution methods, two benchmarks; +9.14–13.35 pp average success vs no-verifier, +12.36–18.29 pp tasks solved in all three runs. Task verifier absent during optimization, not validation-free.
- **Boundary / kill test:** Tool implementation access and version, code comprehension, extra context/compute; matched irrelevant code/placebo, independent held-out outcome, tool-version perturbation. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

### SIS-CAND-20261126-10｜From Memory Access to Evidence Sufficiency: Diagnosing and Addressing Demand--Evidence Misalignment — Worth Skimming
- **StudyVersionRecord:** https://arxiv.org/abs/2611.32088v1; Liu et al.; preprint; 2026-11-24, announced 25; abstract.
- **SIS:** SCF; BGT; MI/EG/MEAS/ID/BT; CAUSAL_MECHANISM_EFFECT (package candidate); TYPED_DEMAND_COVERAGE_EVIDENCE_PRESENTATION_ANSWER_VALUE; CL1/I1/T1; provisional only, independent coding pending.
- **Evidence:** Measurement/implementation: separate access, demand coverage and utilization; +6.23 pp vs Mnemis LoCoMo; 91.80% LongMemEval. Compact implementation uses organized evidence and reader guidance, not separate four-state verifier.
- **Boundary / kill test:** Question taxonomy, reader, retrieval budget, judge, evidence necessity; fixed record pool, typed-demand placebo, strict subset removal and independent Gold. Impact SHARPENS (implementation fills existing capabilities); no formal promotion.

## P0 re-audit
[037/044/051 audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-26.md): nine provisional claims, no final promotions; official ACL sources verified. 
## Synthesis / proposed tests
1. Frozen-state independent scientific transfer: measure relative gain, negative task count, worst-domain non-inferiority and lifecycle compute; reject promotion if mean improvement hides critical regressions.
2. Clinical judge evidence and measurement instrument interaction: paired fault and harmless edit, real independent gold, sensitivity/false alarms by severity, no clinical deployment inference.
3. Local diagnosis vs causal repair: hold locator fixed, then independently remove cause and replay.
4. Exact posterior vs self-report for stopping; compare false commit/extra steps and target shift.
5. Model/harness and code-grounded optimization: balanced factorial, matched budget, frozen transfer assets.
Formal decision MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; CorePressure WATCH; ScientificCoreDelta 0; SPEC_REVISION_CANDIDATE NO. Master §§9, 33–38, 40–44, 54–68, 69–73 and 91–94 cover these estimands; no missing first-principles object or capability identified. 
