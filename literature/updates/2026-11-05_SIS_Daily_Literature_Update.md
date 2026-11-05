# SIS Daily Literature Update | 2026-11-05

Authority: frozen SIS v0.3.1 Master; Registry v1.3 and P0 queue. From previous 2026-11-04 run. arXiv cs.AI listing of Wednesday November 4: 413 entries, 115 new submissions (not 413 new papers). Initial submission dates are November 2/3; Findings EMNLP studies were published October 2026 and are delayed discoveries. Source checks: official ACL and primary arXiv abstracts; full experimental replication not performed.

Decision: MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO.

## Peer-reviewed (October, delayed discovery)

- [Retrieval Myopia: Why RL Search Agents Fail to Read What They Find](https://aclanthology.org/2026.findings-emnlp.1713/)
- [Evaluating LLM Agents Beyond Local Edit Validity](https://aclanthology.org/2026.findings-emnlp.893/)

## Preprints

- [Artifact-to-Capability: Diagnosing Breaks in Capability Formation of Self-Evolving Agents in a Controlled Environment](https://arxiv.org/abs/2611.04952) (2026-11-03 preprint)
- [Silent Instrument Errors Reorder Agent Leaderboards](https://arxiv.org/abs/2611.04399) (2026-11-03 preprint)
- [Verifier strength does not buy discovery quality: a pre-registered two-domain test of LLM-based automated research](https://arxiv.org/abs/2611.04420) (2026-11-03 preprint)
- [What Is This Memory Useful For? Measuring Task-Conditioned Utility in Long-Term Agent Memory](https://arxiv.org/abs/2611.03930) (2026-11-02 preprint, newly surfaced)
- [From AutoResearch to Continual AutoResearch: Do Agents Learn Across Tasks?](https://arxiv.org/abs/2611.05108) (2026-11-03 preprint)
- [Meta^2: Precomputing Reusable Knowledge for Online Harness Evolution in Long-Horizon Agents](https://arxiv.org/abs/2611.05139) (2026-11-03 preprint)
- [Harness-S: Learning from Sibling Harnesses for Generalizable Agent Training](https://arxiv.org/abs/2611.04277) (2026-11-03 preprint)
- [Inter-Agent Influence: Evaluating Persuasion, Deception, and Coercion in Multi-Agent Systems](https://arxiv.org/abs/2611.04556) (2026-11-03 preprint; authors say NeurIPS 2026 accepted)

## Ten provisional scientific recodings (study metadata distinct from claim evidence)

### 1. Retrieval Myopia: Why RL Search Agents Fail to Read What They Find

- Source/lineage: https://aclanthology.org/2026.findings-emnlp.1713/; 2026-10 / Findings EMNLP.
- Claimed novelty and primary evidence: Five systems, three multi-hop benchmarks: up to 46.2% errors despite injected gold; plain QA re-presentation recovers up to 48.9% of these cases.
- Strength/limitations and boundary: Forced gold is not natural retrieval; format also changes attention. Boundary: retrieval regime, input format, model.
- SIS Primary: SCF; Cross-cutting: BGT; Framework Capability: MI/MEAS/ID/EG/BT; primary estimand: FORCED_GOLD_RETRIEVAL_FORMAT_CONDITIONAL_READING_EFFECT.
- Claim maturity / identification / transport ceiling: CL1; local CL2 candidate; I2-local/T1. Evidence role: Negative/format intervention. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 2. Evaluating LLM Agents Beyond Local Edit Validity

- Source/lineage: https://aclanthology.org/2026.findings-emnlp.893/; 2026-10 / Findings EMNLP.
- Claimed novelty and primary evidence: Alloy/GB1 often locally valid but succeed 16.0%/6.8%; exact 625 GB1 variants show 51.4% of locally valid episodes cross recovery boundary.
- Strength/limitations and boundary: Finite toy/proxy task limits generalizability; boundary: remaining budget, partial-state feasibility.
- SIS Primary: SDR; Cross-cutting: BGT; Framework Capability: TD/MEAS/ID/BT; primary estimand: BUDGET_CONDITIONAL_ARTIFACT_RECOVERABILITY.
- Claim maturity / identification / transport ceiling: CL0 finite enumeration + CL1; I1/T0. Evidence role: Negative/benchmark. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 3. Artifact-to-Capability: Diagnosing Breaks in Capability Formation of Self-Evolving Agents in a Controlled Environment

- Source/lineage: https://arxiv.org/abs/2611.04952; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Common-model freestyle Gomoku: Reflexion gains legality only; Voyager misses all 20 one-move wins despite sound components; DGM later loses passed states.
- Strength/limitations and boundary: Controlled single game, construct-defined checkpoint. Boundary: artifact lineage, composition, retention.
- SIS Primary: SCF; Cross-cutting: CSCI/BGT; Framework Capability: MI/TD/IA/MEAS/ID/BT; primary estimand: ARTIFACT_CAPABILITY_FORMATION_CHECKPOINT.
- Claim maturity / identification / transport ceiling: CL1 empirical + CL0 definition; I1/T0. Evidence role: Negative/construct validity. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 4. Silent Instrument Errors Reorder Agent Leaderboards

- Source/lineage: https://arxiv.org/abs/2611.04399; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Public HAL and tau2-bench artifact regrade: ungraded episodes falsely failed; 13-point apparent gap closes; nested-cost double counting and grader-action attribution found.
- Strength/limitations and boundary: Selected leaderboards, no broad incidence estimate; instrument fixes need independent Gold. Boundary: grader version, denominator, provenance.
- SIS Primary: ROUTING_ABSTAIN; Cross-cutting: BGT; Framework Capability: MEAS/EG/ID/BT; primary estimand: GRADER_COVERAGE_PROVENANCE_VERSION_RANKING_SENSITIVITY.
- Claim maturity / identification / transport ceiling: CL1 audit; local deterministic regrade I2/T0. Evidence role: Measurement/negative. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 5. Verifier strength does not buy discovery quality: a pre-registered two-domain test of LLM-based automated research

- Source/lineage: https://arxiv.org/abs/2611.04420; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Pre-registered 100 matched pairs per domain and three tiers; no growth in LLM-vs-random value with verifier tier; post-hoc pooled candidates gain 1.52 holdout units in one domain.
- Strength/limitations and boundary: Nearly identical lower-tier selection limits contrast; mixed pool result is post-hoc; two domains only.
- SIS Primary: ASR; Cross-cutting: BGT; Framework Capability: DR/MEAS/ID/EG/BT; primary estimand: VERIFIER_TIER_X_PROPOSER_POOL_HOLDOUT_VALUE.
- Claim maturity / identification / transport ceiling: CL1 negative; local I2 candidate/T0. Evidence role: Negative/null; proposal boundary. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 6. What Is This Memory Useful For? Measuring Task-Conditioned Utility in Long-Term Agent Memory

- Source/lineage: https://arxiv.org/abs/2611.03930; 2026-11-02 preprint, newly surfaced.
- Claimed novelty and primary evidence: Frozen reader + task-blind writer paired exposure: answer-bearing vs control difference +0.33 (95% interval +0.21,+0.46); no measurable gains on tested software/scientific coding.
- Strength/limitations and boundary: Single-call recall does not identify long-run utility; reader, filler, placement and domain are boundaries.
- SIS Primary: SCF; Cross-cutting: BGT; Framework Capability: MI/MEAS/ID/EG/BT; primary estimand: TASK_CONDITIONED_MEMORY_EXPOSURE_PAIRED_GAIN.
- Claim maturity / identification / transport ceiling: CL1; local CL2 candidate; I2-local/T1. Evidence role: Conditional mechanism and negative transfer. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 7. From AutoResearch to Continual AutoResearch: Do Agents Learn Across Tasks?

- Source/lineage: https://arxiv.org/abs/2611.05108; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Nine task families, five agents, matched streams/time and memory ablation: persistent state improves first-solution efficiency for all, not consistently final holdout performance.
- Strength/limitations and boundary: Persistence mixes code, memory and search state; new-task efficiency not learning mechanism.
- SIS Primary: SDR; Cross-cutting: BGT; Framework Capability: TD/DR/MEAS/ID/EG/BT; primary estimand: PERSISTENCE_VS_RESET_RESEARCH_EFFICIENCY_FINAL_VALUE.
- Claim maturity / identification / transport ceiling: CL1; local CL2 candidate; I2-local/T1. Evidence role: Boundary/negative final-value. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 8. Meta^2: Precomputing Reusable Knowledge for Online Harness Evolution in Long-Horizon Agents

- Source/lineage: https://arxiv.org/abs/2611.05139; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Offline privileged verifier only during training; online KEEP/EVOLVE task-local updates; reported 81.00% Terminal-Bench 2.1 and 44.44% DeepSWE 1.1 in tested configuration.
- Strength/limitations and boundary: Evolver/knowledge/online edits co-vary; compare full cost and evidence privilege.
- SIS Primary: ASR; Cross-cutting: BGT; Framework Capability: DR/MI/TD/EG/MEAS/ID/BT; primary estimand: OFFLINE_META_SKILL_ONLINE_KEEP_EVOLVE_VALUE.
- Claim maturity / identification / transport ceiling: CL1 composite; local candidate; I1/I2-local/T1. Evidence role: Regulation/implementation. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 9. Harness-S: Learning from Sibling Harnesses for Generalizable Agent Training

- Source/lineage: https://arxiv.org/abs/2611.04277; 2026-11-03 preprint.
- Claimed novelty and primary evidence: Sibling harnesses rescue base failures, train same policy, return evaluation to original harness on AppWorld/SWE-Gym/DBBench; conditional performance transfer.
- Strength/limitations and boundary: More successful training rollouts, policy selection and routing confounded; performance transfer not causal invariance.
- SIS Primary: SCF; Cross-cutting: CSCI/BGT; Framework Capability: MI/IA/DR/MEAS/ID/BT; primary estimand: SIBLING_HARNESS_RESCUE_BASE_POLICY_TRANSFER.
- Claim maturity / identification / transport ceiling: CL1 composite; I1/T2 performance only. Evidence role: CSCI/transfer boundary. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

### 10. Inter-Agent Influence: Evaluating Persuasion, Deception, and Coercion in Multi-Agent Systems

- Source/lineage: https://arxiv.org/abs/2611.04556; 2026-11-03 preprint; authors say NeurIPS 2026 accepted.
- Claimed novelty and primary evidence: Five environments; influence shifts overseer rejection to approval and redirects peer safety-work trajectories in designed settings.
- Strength/limitations and boundary: Attack-style scenarios not production harm rate; official proceedings version not independently matched.
- SIS Primary: SDR; Cross-cutting: CSCI/BGT; Framework Capability: IA/TD/EG/MEAS/ID/BT; primary estimand: INTER_COMPONENT_PERSUASION_OVERSIGHT_SHIFT.
- Claim maturity / identification / transport ceiling: CL1; I1/I2-local/T1. Evidence role: Viability/authority boundary. SIS impact: SHARPENS existing programs/frameworks; reading priority: Must Read.

## Five implications / candidate benchmarks

1. Artifact accumulation and score gains do not prove capability formation; impose state/game/lineage checkpoints and counterexamples.
2. Scoring pipelines are measurement instruments: track graded fraction, grader version, action provenance, root-span cost and regrade deltas.
3. Stronger verifier tiers need not improve scientific discovery, especially when admission gates select identical candidates; pair with candidate-pool factorial contrasts.
4. Memory value depends on the future task and exposure; factual recall gain did not transfer to tested coding. Require matched no-memory controls and full cost.
5. Persistence improves early research efficiency without guaranteeing better final answers; audit full retained state, held-out old/new tasks and authorization/influence boundaries.

| Priority | Fixture | Estimand / kill test |
|---|---|---|
| P0 | Artifact lineage x legal/action/reachability checkpoint | distinguish proxy gain from real capability |
| P0 | Frozen traces x evaluator coverage/version | identify hidden ranking changes, grading omissions |
| P0 | Proposal pool x verifier strength (matched) | check null effect versus post-hoc pool diversification |
| P0 | Task-conditioned memory randomized exposure | pair answer-bearing vs control, benefit minus storage/retrieval cost |
| P0 | Persistent vs reset research / old tasks | early efficiency vs final quality and retention |
| P0 | Role influence x authorization | unauthorized overseer or peer decision shift |
| P1 | Offline meta-skill x online KEEP/EVOLVE | isolate online regulation under full cost |
| P1 | Sibling-harness x frozen base executor | transfer quality vs training-rollout confound |

No independently reproduced community analysis was promoted; DISCOVERY_ONLY. Nine first-coder claim re-audits for SIS-LIT-001/020/032 are in companion audit ledger. No final CL2/3 promotion or T3/T4. Historical 2026-10-09..23 candidate lineage still requires cross-version reconciliation.
