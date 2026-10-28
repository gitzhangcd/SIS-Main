# SIS Daily Literature Update | 2026-10-29

**Authority:** `System_Intelligence_Science_v0.3.1.md` (Core frozen), Registry v1.3, SIS-LEM-P0 and ClaimRecord v0.1. **Sources checked:** arXiv new cs.AI listing for 2026-10-28 (407 listings; 95 new submissions), relevant cs.CR cross-list, ACL Anthology, OpenReview/NeurIPS venue status, official author/project sources. Discovery window since 2026-10-28 prior run; some first submitted 2026-10-23/26 but newly indexed or newly surfaced. **No accepted paper's formal proceedings were independently authenticated for this selection**: all ten listed below are preprints for evidence purposes; NeurIPS workshop/track acceptance author claims are preserved as metadata only.

**Governance:** 10 date-scoped provisional candidates; no permanent SIS-LIT ID before resolving unsynced 2026-10-09–23 and preprint/conference lineages. IDs checked against all canonical registry/arXiv IDs and Oct 24–28 provisional records; zero direct ID matches. No whole-paper CL2/CL3. Community/technical discussion discovery-only. No new T3/T4.

**Formal SIS Impact Decision:** `MEASUREMENT_IDENTIFICATION_DELTA`; secondary `BENCHMARK_DELTA`. Real pressure is on audit noninterference, evidence supersession, scientific specification sufficiency and net cost/defect metrics. **ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO**: covered by existing SCF/SDR/ASR, BGT and MI/TD/DR/IA/BT/MEAS/ID/EG.

## Provisional studies and claim-bounded coding

### SIS-CAND-20261029-01 — Blindfold: Keeping the Audit Coin Secret from LLM Agents
- **Primary source / StudyVersionRecord:** [arXiv:2610.37055](https://arxiv.org/abs/2610.37055) (v1 preprint; first submitted 2026-10-27; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **ROUTING_ABSTAIN**; cross-cutting **BGT**; Framework **MEAS/ID/EG/BT**. Primary estimand: `PRECOMMIT_AUDIT_COIN_NONINTERFERENCE_CERTIFICATE_VALIDITY`.
- **Claim maturity / identification / transport:** CL0 formal + CL1 empirical; local controlled attack only; **I0/I2-local/T0**. Evidence role: **FORMAL_IDENTIFICATION_LIMIT_AND_NEGATIVE_CONTROL**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** Pre-commit noninterference (PNI) is needed for unbiased auditing against adaptive agents; worst-case certification bias (1-epsilon)*D_A. A timestamp-visible silent audit leaks the coin even without output changes; fresh per-call randomization closes the tested timing channel.
- **Identification, construct and transport limits:** The theorem depends on its audit/observation model. Prototype monitor and injection demonstrations are not universal field prevalence; production noninterference and side channels remain unverified.
- **SIS influence:** Real identification pressure: random audit sampling is insufficient without observation-channel independence; already expressible through SIS ID/MEAS/EG.

### SIS-CAND-20261029-02 — M4Bench: Evaluating Procedural Specification for Clinical EHR Derivation Agents
- **Primary source / StudyVersionRecord:** [arXiv:2610.37459](https://arxiv.org/abs/2610.37459) (v1 preprint; first submitted 2026-10-27; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **SCF**; cross-cutting **BGT; CSCI exploratory**; Framework **MI/MEAS/ID/EG/BT**. Primary estimand: `OPERATIONAL_SPECIFICATION_VS_SKILL_DELIVERY_INCREMENTAL_VALUE`.
- **Claim maturity / identification / transport:** CL1 performance; local CL2 candidate for controlled specification contrast; **I2-local/T2-performance-only**. Evidence role: **CONTROLLED_SPECIFICATION_MEASUREMENT_AND_NULL_BOUNDARY**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** 28 clinical derivation tasks on MIMIC-IV/eICU. Skill vs no-skill reward +0.136; operational specification alone +0.162 on eight-task subset, skills +0.024 beyond specification, statistically indistinguishable from zero. Only 25/280 with-skill and 13/280 without-skill executions passed every strict check.
- **Identification, construct and transport limits:** Small 8/10-task mechanism subgroups, incomplete strict correctness, reference SQL and clinical-source validity constraints; zero-significance on +0.024 is not proof of equivalence. NeurIPS 2026 E&D acceptance author-declared, official proceedings identity not independently verified.
- **SIS influence:** Spec completeness appears more important than packaged skill surface; high relevance to expert clinical evidence workflows and capability representation; no new primitive.

### SIS-CAND-20261029-03 — When Retrieval Is Not Enough: Obsolete Facts in Agent Memory
- **Primary source / StudyVersionRecord:** [arXiv:2610.36308](https://arxiv.org/abs/2610.36308) (v1 preprint; first submitted 2026-10-26; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **SDR**; cross-cutting **BGT**; Framework **TD/EG/ID/MEAS/BT**. Primary estimand: `OBSOLETE_COMPETING_EVIDENCE_SUPERSESSION_FAILURE_EFFECT`.
- **Claim maturity / identification / transport:** CL1 overall; local CL2 candidate for frozen-prompt stale-statement substitution; **I2-local/T1**. Evidence role: **NEGATIVE_MEMORY_SUPERSESSION_BOUNDARY**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** 6K-history BM25: Qwen2.5 accuracy 45% at 64 tokens versus 32% at 512 although latest fact was present. Equal-size four-statement replacement: irrelevant statement -> stale competing version drops 100% to 44.6% for Qwen2.5 and 87.8% for Qwen3-14B.
- **Identification, construct and transport limits:** Single-hop FactConsolidation benchmark, limited model/task regimes, gold-assisted evidence audit; workshop acceptance author-declared and not archival proof.
- **SIS influence:** Correct retrieval is distinct from applying the temporally authoritative update; supports explicit obsolete-versus-current evidence governance.

### SIS-CAND-20261029-04 — Don't Pick a Winner: Knowledge Conflicts Need a Prior, Not a Rule
- **Primary source / StudyVersionRecord:** [arXiv:2610.36169](https://arxiv.org/abs/2610.36169) (v1 preprint; first submitted 2026-10-26; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **ASR**; cross-cutting **BGT**; Framework **DR/EG/ID/MEAS/BT**. Primary estimand: `SOURCE_RELIABILITY_PRIOR_CONDITIONAL_SELECTION_NET_VALUE`.
- **Claim maturity / identification / transport:** CL0 decision-theory + CL1 results; local controlled context interventions; **I1/I2-local/T1**. Evidence role: **BOUNDARY_AND_ADAPTIVE_SOURCE_SELECTION_MEASUREMENT**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** Controlled GRACE context interventions separately assess model knowledge, context correctness and truth; calibrated prior-conditioned selection reports scores 45.3/35.0 vs 29.4/27.5 for best comparison on two backbones, and outperforms on pre-registered ClashEval.
- **Identification, construct and transport limits:** Strongest GRACE mixture comparison supplies the true proportion of correct contexts (oracle prior). Need prior-estimation error and shift tests before deployment/net-value claims; relative source confidence may be miscalibrated.
- **SIS influence:** Supports ASR selective trust/abstention conditioned on source reliability and explicit prior; generic source-following rules cannot be treated as universal.

### SIS-CAND-20261029-05 — Counting the Bandages: On measuring the time that AI saves
- **Primary source / StudyVersionRecord:** [arXiv:2610.35942](https://arxiv.org/abs/2610.35942) (v1 preprint; first submitted 2026-10-23; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **ROUTING_ABSTAIN**; cross-cutting **BGT**; Framework **MEAS/ID/EG/BT**. Primary estimand: `COUNTERFACTUAL_TIME_SAVED_VS_ESCAPED_DEFECT_BREAK_EVEN_COST`.
- **Claim maturity / identification / transport:** CL0 theoretical/estimand + CL1 secondary data; local controlled reviewer experiment; **I1/I2-local/T0**. Evidence role: **MEASUREMENT_IDENTIFICATION_AND_NEGATIVE_BOUNDARY**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** Reanalysis of the 246-issue METR developer trial shows alternative slowdown estimands around 19% or 24% (34% without imbalance adjustment); an additional small pre-specified reviewer experiment reports reduced checking and 22.5% of briefs allowing a wrong figure through when told error rate was ten times smaller.
- **Identification, construct and transport limits:** Reanalysis relies on public data/design choices and small new experimental scale; subjective escaped-defect cost not known from stopwatch alone; trade-offs conditional on risk and reviewer policy.
- **SIS influence:** Strengthens full-system cost, unobserved defect burden and estimand alignment; speed alone not system net benefit.

### SIS-CAND-20261029-06 — How Stable Are LLM-Generated Proofs Under Program Refactoring? A Stress Test for Verifiable Code Generation
- **Primary source / StudyVersionRecord:** [arXiv:2610.36328](https://arxiv.org/abs/2610.36328) (v1 preprint; first submitted 2026-10-26; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **SCF**; cross-cutting **BGT**; Framework **MI/MEAS/ID/BT**. Primary estimand: `BEHAVIOR_PRESERVING_REFACTOR_UNCHANGED_PROOF_SURVIVAL_EFFECT`.
- **Claim maturity / identification / transport:** CL1 robustness measurement; local controlled program transformation; **I2-local/T1**. Evidence role: **NEGATIVE_REPRESENTATION_BOUNDARY_AND_MEASUREMENT_INSTRUMENT**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** RefactorProof builds 458 Lean-certified variants from 185 compilable VERINA tasks; structural proof survival 4.3% for supplied references and 13.3–26.8% for specialized provers. Many failed proofs are easy to repair (51/54 reference and 58/85 prover structural failures via a one-identifier edit).
- **Identification, construct and transport limits:** Matched model-vs-reference subset only 21–25 tasks; unchanged-proof survival is not repair cost or semantic invalidity. Workshop acceptance author-declared, not independently archival.
- **SIS influence:** Separates formal program behavior equivalence, certificate survival, and repair cost. Valuable BGT/MEAS non-regression fixture.

### SIS-CAND-20261029-07 — InfraDev: Can Coding Agents Develop AI Infrastructure, and How Can We Tell?
- **Primary source / StudyVersionRecord:** [arXiv:2610.36589](https://arxiv.org/abs/2610.36589) (v1 preprint; first submitted 2026-10-27; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **ROUTING_ABSTAIN**; cross-cutting **BGT**; Framework **MEAS/EG/ID/BT**. Primary estimand: `HIDDEN_INFRASTRUCTURE_PROBE_INCREMENTAL_CONFORMANCE_VALIDITY`.
- **Claim maturity / identification / transport:** CL1 benchmark measurement; no mechanism promotion; **I1/T0**. Evidence role: **NEGATIVE_BENCHMARK_CONSTRUCT_VALIDITY**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** 36 real PR-derived multi-file, multi-GPU tasks from Megatron-LM/vLLM/verl; best of six frontier models resolves only 38.9%; new hidden probes reject 32% of submissions that pass all original tests. Original PR descriptions alone yield zero resolutions.
- **Identification, construct and transport limits:** Probe correctness, specification leakage, 36-task sample and shared infrastructure are boundaries; original-test pass does not prove intended behavior, but new hidden probes also require validation.
- **SIS influence:** Raises SIS scientific test/evaluator independence and hidden-state/runtime conformance measurement.

### SIS-CAND-20261029-08 — Concordat: Typed Sessions for LLM Agents
- **Primary source / StudyVersionRecord:** [arXiv:2610.37461](https://arxiv.org/abs/2610.37461) (v1 preprint; first submitted 2026-10-27; discovered/reviewed 2026-10-29); **Reading:** Worth Skimming.
- **Routing:** Primary **SCF**; cross-cutting **BGT**; Framework **MI/EG/ID/MEAS/BT**. Primary estimand: `TYPED_SESSION_PROTOCOL_AUTHORIZATION_VIOLATION_EFFECT`.
- **Claim maturity / identification / transport:** CL1; local CL2 candidate under controlled protocol enforcement; **I2-local/T0**. Evidence role: **VIABILITY_CONSTRAINT_IMPLEMENTATION_AND_BOUNDARY**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** Finite-state typed interfaces prohibit disallowed tool calls before side effects. In 50 tau-bench airline tasks, baseline produced 13/50 unauthorized changes with GPT-4.1 and 29/128 runs with Claude Haiku 5.5, while tested Concordat agent produced zero; no significant success difference.
- **Identification, construct and transport limits:** Small airline-task scope, encoded confirmation policy only; zero observed violations is not general guarantee for unmodeled effects, semantics or deployment. Tool availability and prompts may change together.
- **SIS influence:** Separates semantic user authorization, formal protocol coverage and endpoint reward; supports viable-region enforcement, not a new SIS primitive.

### SIS-CAND-20261029-09 — CohortFlow: A Steerable Clinical Cohort Curation Agent with Localized Semantic Correction
- **Primary source / StudyVersionRecord:** [arXiv:2610.36100](https://arxiv.org/abs/2610.36100) (v1 preprint; first submitted 2026-10-26; discovered/reviewed 2026-10-29); **Reading:** Must Read.
- **Routing:** Primary **ASR**; cross-cutting **BGT**; Framework **DR/TD/MI/MEAS/ID/BT**. Primary estimand: `DEPENDENCY_SCOPED_CORRECTION_COST_ADJUSTED_REQUIREMENT_FIDELITY`.
- **Claim maturity / identification / transport:** CL1; local CL2 candidate for controlled recomputation policy; **I2-local/T0**. Evidence role: **CONDITIONAL_SEMANTIC_REPAIR_EFFICIENCY_AND_NULL**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** 100 clinical-trial-criteria scenarios, 126 correction turns: 77.0% requirement micro-F1 versus 76.4% full regeneration, p=0.493; correction latency -64.8% after completion / -44.3% in flight, model calls -38.1%. Proof of concept: 13 MIMIC cohort states execute.
- **Identification, construct and transport limits:** No significant accuracy gain; not equivalence proof. Small executable clinical demonstration does not validate real cohorts or downstream clinical claims; frozen 8B model and scenario semantics bound transport.
- **SIS influence:** Strong candidate for scoped semantic invalidation/recompute fixture in scientific workbench, preserving unaffected evidence and requirements.

### SIS-CAND-20261029-10 — The Trinity: Capability-Driven Recursive Self-Improvement for Multimodal Agents
- **Primary source / StudyVersionRecord:** [arXiv:2610.36077](https://arxiv.org/abs/2610.36077) (v1 preprint; first submitted 2026-10-26; discovered/reviewed 2026-10-29); **Reading:** Worth Skimming.
- **Routing:** Primary **SCF**; cross-cutting **BGT**; Framework **MI/DR/EG/MEAS/BT**. Primary estimand: `CAPABILITY_HIERARCHY_ROUTED_HARNESS_EVOLUTION_HELDOUT_VALUE`.
- **Claim maturity / identification / transport:** CL1 composition/performance; no mechanism CL2 from bundled system; **I1/T2-performance-only**. Evidence role: **IMPLEMENTATION_AND_CROSS_TASK_PERFORMANCE_TRANSFER**. Paper-level metadata must not be inherited as final scientific claim.
- **Author-reported finding:** Creator/Explorer/Evolver combine verifiable simplified worlds, capability-tree routing and harness evolution. Authors report +34 points over 28 training benchmarks, +26 points across 18 unseen benchmarks including two real-world embodied tasks.
- **Identification, construct and transport limits:** World synthesis, capability grouping, inherited modules, routing and budget co-vary. Held-out task performance does not prove causal transfer or mechanism invariance; embodied subgroup small.
- **SIS influence:** Reinforces representation externalization and capability-conditional system design; no new first-principles program.

## Synthesis / benchmark delta

1. **Independent audit observability:** Blindfold demonstrates an audit-sampling scheme can be invalidated by pre-commit timing leakage; add randomized-audit PNI and visibility-control fixture, including adaptive auditor interactions.
2. **Scientific contract and expert validity:** M4Bench and InfraDev show operational task specifications and hidden executable oracles matter more than superficial skill/test pass; separate spec completeness, delivery surface, actual strict outcomes and schema/repository shifts.
3. **Evidence version and source reliability:** Obsolete Facts and Don't Pick a Winner demand dated source supersession and calibrated prior-conditioned use; correct retrieval is not correct evidence application.
4. **System net-value measurement:** Counting the Bandages requires cost of escaped defects, verification effort and counterfactual speed in same estimand; CohortFlow adds latency–quality non-inferiority caution.
5. **Conditional system capability:** RefactorProof, Concordat and Trinity give implementation-relevant tests of proof stability, stateful authorization, and task-condition capability routing, with narrow validated boundaries rather than transportable causal law.

**Recommended P0 fixtures:** AUDIT_COIN_PNI; EHR_SPEC_COMPLETE_VS_SKILL_FORMAT; STALE_VS_CURRENT_FACT_PAIRED; SOURCE_PRIOR_SHIFT; TIME_SAVED_ESCAPED_DEFECT_LEDGER; REFACTOR_PROOF_SURVIVAL_VS_REPAIR; HIDDEN_INFRA_EXECUTION_ORACLE; TYPED_SESSION_AUTHORITY; SCOPED_SEMANTIC_RECOMPUTATION. All require independent Gold, fixed budget/information or explicit budget accounting, and provenance.

## Claim-level re-audit actions

3 studies and 9 claims first-coder re-audited. Full source-level breakdown: [SIS_P0_Reaudit_2026-10-29.md](../evidence-map/audits/SIS_P0_Reaudit_2026-10-29.md). Source provenance retained. No second coder/adjudication yet, no final CL2/CL3 elevation.

**Repository commit policy:** substantive new studies and claim splits warrant a dated commit. This note must remain provisional until source/version lineage reconciliation; no scientific mother-spec changes.
