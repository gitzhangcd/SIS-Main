# SIS Daily Literature Update｜2026-11-27
Base 1600d7d833626ae05ff20afc9a74dfab2ae9797a. Master, complete registry (identifier/title scan), P0 queue, evidence-map and schema consulted. arXiv cs.AI Nov 26 announcement 248 entries; screened first 50 selectively; targeted searches OpenReview, ACL/EMNLP, NeurIPS/ICML/ICLR, journals and technical indices; not exhaustive. Nine new Nov 25 preprints, one delayed EMNLP VOR paired with July preprint. No duplicate IDs/titles found in registry. Full HTML selected for skill audit, EvoLink and temporal graph; others abstract-level. Crucible, FWSP and AutoDNA (Nov 4 online, Nov 26 issue) deferred for later intake, not counted. No independent replication by SIS. Community analyses discovery-only. No padding.

### SIS-CAND-20261127-01｜GRASP: GRanularity-Aware Search Policy for Agentic RAG
- **StudyVersionRecord:** https://aclanthology.org/2026.findings-emnlp.1226/; Gandhi et al.; EMNLP Findings October 2026; arXiv:2607.10463 (July 11), same study; abstract; delayed discovery.
- **SIS:** ASR; BGT; DR/MI/EG/MEAS/ID/BT; POLICY_VALUE; RETRIEVAL_ACTION_GRANULARITY_POLICY_NET_VALUE; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/implementation: reinforcement learning chooses semantic, lexical and paragraph reading actions, improving retrieval and QA on multi-hop tasks for 3B/7B models. Reward and action space co-vary; no isolated mediator.
- **Boundary / kill test:** Fixed action space and query budget, compare fixed or random routing, independent answer and evidence gold; task and corpus distribution. SHARPENS. Worth Skimming.

### SIS-CAND-20261127-02｜What Does Skill Lift Actually Measure? A Source-Code-Level Audit and Noise-Aware Reanalysis of SkillsBench
- **StudyVersionRecord:** https://arxiv.org/abs/2611.33943v1; Zhang & Long; HTML §§III–V; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** DESCRIPTIVE_ONLY for measurement audit; BGT; CSCI hypothesis; MEAS/ID/BT/EG; operational SKILL_LIFT_MEASUREMENT_AND_GATE_SELECTION_LEAKAGE; separate ASR POLICY_VALUE candidate; CL1/I2-local/T1; provisional first coder, no final promotion.
- **Evidence:** LIMIT/NULL/INSTRUMENT: 7554 trials, 1421 paired cells; two grader-dependent cases and one operational gap; 58% cells cannot show decrease; no corrected task-level significant reduction; shuffled labels produce apparent gate gain 4–7 pp; held-out runs no significant improvement. Task-held-out risk forest AUC .52 among nonzero baseline cells. Not proof of no skill harm.
- **Boundary / kill test:** Run count, task clustering, grader contracts, built-in skills, reused outcomes; independent gate fitting and evaluation, sham labels and exact environment inventory. SHARPENS/CHALLENGES. Must Read.

### SIS-CAND-20261127-03｜EvoLink-Bench: A Benchmark for Evaluating Self-Evolving Agents in Long-Horizon Interdependent Task Streams
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34400v1; Chen et al.; HTML §§4–5.1 checked; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** SDR; BGT; CSCI hypothesis; TD/DR/EG/MEAS/ID/BT; LONG_HORIZON_EFFECT; PERSISTENT_STATE_VS_LATER_PROBE_PERFORMANCE; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** LIMIT/INSTRUMENT: five frameworks, three backbones, three persistence conditions, 19635 scored slots in selected cohorts. L1 factual revision vs L2 capability, retry vs persistent update vs later probe. No uniform winner; retained state not necessarily beneficial. Some framework cells backbone-specific.
- **Boundary / kill test:** Dependent tasks, missing configuration cells, prior task success, persistence content, evaluator; clone state with/without update, independent later probes, stream-clustered inference. SHARPENS. Must Read.

### SIS-CAND-20261127-04｜Did the Model Forecast It, or Already Know It? Evaluating Large Language Models for Novel Drug-Target Prioritisation with a Temporal Knowledge-Graph Oracle
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34247v1; Siu et al.; HTML §3 Table 1; workshop acceptance author-reported only; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** DESCRIPTIVE_ONLY measurement claim; BGT; EG/MEAS/ID/BT; operational DECISION_TIME_GRAPH_VS_FUTURE_GRAPH_FORECAST_VALIDITY; SCF CAUSAL_MECHANISM_EFFECT candidate for retrieval contrast; CL1/I2-local/T1; provisional first coder, no final promotion.
- **Evidence:** LIMIT/NULL: six models; decision-time dated evidence has no significant AUROC gain after model cutoff; latest graph often includes future trial. Qwen3-32B post-cutoff AUROC .768/.773/.942 without/dated/latest graph; trial-history overall .754. First trial is not efficacy or biological novelty.
- **Boundary / kill test:** Approximate cutoff, time stamps, candidate sampling, clinical trial selection; as-of snapshots, predecision features, postdecision outcomes and trial-history baseline. SHARPENS/CHALLENGES. Must Read.

### SIS-CAND-20261127-05｜What Is a Theory Worth to an LLM Solver? Measuring, Inducing, and Merging Theories in Context
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34751v1; Gao & Bi; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** SCF; BGT; CSCI hypothesis; MI/IA/MEAS/ID/BT; CAUSAL_MECHANISM_EFFECT; LENGTH_MATCHED_THEORY_CONTEXT_BY_SOLVER_BUDGET; CL1/I2-local candidate/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT: Qwen3-14B pass@1 .37→.83, median correct tokens 10.2k→6.3k; length-matched examples do not help; gain shrinks with solver/budget; induced unpublished theories recover 60%,48%, near zero on three families. Completion explains long-budget advantage, not identified mediation.
- **Boundary / kill test:** Oracle theory access, task family, solver, budget, induced-note selection; factorial theory/example/placebo × budget, independent planted families, censoring-aware outcome. SHARPENS. Must Read.

### SIS-CAND-20261127-06｜REE: A Scientific Research Entrance Exam for AI Agents
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34646v1; Zhou et al.; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** DESCRIPTIVE_ONLY measurement claim; BGT; MI/TD/MEAS/EG/ID/BT; operational STARTER_TO_EXPERT_SOLUTION_SCORE_UNDER_TIME_BUDGET; SCF CAPABILITY_FRONTIER_SHIFT candidate; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** INSTRUMENT: 100 open-ended tasks across 23 domains; 12-hour improvement budget; two evaluated systems outperform expert reference solutions on 86% and 81% tasks. Expert reference is not the limit of human researchers; benchmark score not scientific novelty.
- **Boundary / kill test:** Starter quality, public solution exposure, matched budget, expert reference age, evaluator; hidden prospective problems, equal-resource humans and independent scientific verification. SHARPENS. Must Read.

### SIS-CAND-20261127-07｜HoMe: Toward Practical Harness Optimization of Memory Systems for AI Assistants
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34624v1; Xu et al.; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** ASR; BGT; DR/TD/MI/EG/MEAS/ID/BT; POLICY_VALUE; VERSIONED_TRACE_GUIDED_MEMORY_HARNESS_SEARCH; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/implementation: session versions + traces, structural candidate exploration, smoke tests/adaptive sampling/reuse; six formal candidate evaluations after initial evaluation on each of LongMemEval-S and BEAM; reported better end-task performance and lower query tokens. Diagnosis not causal attribution.
- **Boundary / kill test:** Candidate selection, reused memory compatibility, total build/search cost, held-out cases; equal budget random edits, cold rebuild and blind validation. SHARPENS. Worth Skimming.

### SIS-CAND-20261127-08｜vSFT: Learning to Verbally Tune Agents at Test Time
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34440v1; Wen et al.; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** ASR; BGT; CSCI hypothesis; DR/MI/TD/MEAS/ID/BT; POLICY_VALUE; VERBAL_FEEDBACK_TO_LOW_RANK_UPDATE_TEST_TIME_VALUE; CL1/I1/T1; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/implementation: supervisor interprets failed trajectories; hypernetwork maps text to low-rank weight edits; Qwen3-4B authors report ALFWorld success improvement 8.7% vs GRPO and 13.9% vs Reflexion, WebShop 4.8% and 18.2% (as reported, unit not rederived). No evidence of indefinite improvement.
- **Boundary / kill test:** Supervisor/hypernetwork training, rollout budgets, failure information, parameter update retention; text-only/weight-only/sham feedback and equal total costs, frozen blind test. SHARPENS. Must Read.

### SIS-CAND-20261127-09｜MedSkill-E²: Evaluating and Evolving Skills for Medical Agents
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34250v1; Hua et al.; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** SCF; BGT; CSCI hypothesis; MI/IA/DR/EG/MEAS/ID/BT; MECHANISM_INTERACTION_EFFECT candidate; AUTONOMOUS_VS_GUIDED_SKILL_USE_BY_MODEL_HARNESS; CL1/I1/T2 performance-only; provisional first coder, no final promotion.
- **Evidence:** LIMIT/SUPPORT: 12 medical task groups; mean enable-but-underuse gap 43.94 pp; same model differs up to 38.96 pp across harnesses; revised skills +33.33–55.17 pp and cross-configuration gains. Opening skill insufficient; guided condition adds direction, not pure availability. Not clinical safety.
- **Boundary / kill test:** Skill/task identity, guidance information, harness exposure, evaluation gold; factorial access × guidance × model/harness, no extra hints, external clinical gold, retention. SHARPENS. Must Read.

### SIS-CAND-20261127-10｜Knowledge-Base Gradient Descent: Self-Structuring Learning through Question Answering
- **StudyVersionRecord:** https://arxiv.org/abs/2611.34841v1; Kato; abstract; preprint v1 submitted 2026-11-25, announced Nov 26.
- **SIS:** ASR; BGT; DR/MI/EG/MEAS/ID/BT; POLICY_VALUE; QUESTION_CONDITIONED_STRUCTURAL_EDIT_HELDOUT_VALUE; CL1/I1/T1; separate CL0 mathematical formulation; provisional first coder, no final promotion.
- **Evidence:** SUPPORT/LIMIT: evaluate proposed structural edits and retain loss-reducing ones; derivative wrt randomized edit-selection probability, not a gradient over arbitrary text. Generated held-out question F1 improves for cards/schema; human-question F1 rises for schema but falls for cards.
- **Boundary / kill test:** Same source documents, generated vs human question distribution, evaluation cost, coupled edits; independent human questions and new sources, factorial joint edits, frozen acceptance split. SHARPENS/CHALLENGES. Must Read.

## Synthesis
1. Gate selection on noisy baseline and evaluation on the same outcomes can manufacture gains; enforce independent run split and sham-label null.
2. Evaluate persistent updates on independent later probes, not immediate retries; capability acquisition, retention and recovery are separate.
3. Decision-time evidence requires temporal lineage and leakage checks; trial entry is not biological efficacy.
4. Theory/skill/schema value is conditional on executor, information, budget and question distribution. Test CSCI interaction, not marginal averages.
5. Compare text and weight interventions with equal lifecycle budget and independent retention tests.
## Impact
MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; core pressure WATCH (operational measurement/identification, not uncovered primitive). ScientificCoreDelta=0; no SPEC_REVISION_CANDIDATE. Existing §§9,20,33–38,53–54,66,82 and canonical estimands suffice. Suggested fixtures: independent gate-fit/test and shuffled-label negative control; temporal as-of snapshot; cloned persistent state and blind probes; factorial representation × executor × budget; text/weight/sham update.
## P0
[First-coder re-audit](../evidence-map/audits/SIS_P0_Reaudit_2026-11-27.md): 052,072,073; nine claims, zero final promotions, no T3/T4. Source qualifications upgraded, no permanent IDs allocated.
