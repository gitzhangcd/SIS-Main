# SIS Daily Literature Update — 2026-10-26

**Authority:** SIS v0.3.1, scientific core frozen. **Discovery window:** since 2026-10-25 update; public arXiv cs.AI Friday 2026-10-23 is most recent at 2026-10-26 08:00 Asia/Shanghai. Peer-reviewed EMNLP 2026 proceedings appeared in October and are delayed discoveries, *not* October-26 publications. Preprints first posted October 19–21, not October 26.

**Dedup/lineage:** nine new provisional study identities, each matched by title and stable URL/identifier against 145 permanent Registry records and existing 2026-10-24/25 provisional sections. No duplicates found there; **2026-10-09–23 pending local candidate bundles not yet exhaustively reconciled**, so permanent SIS-LIT numbering deferred. Peer-reviewed ACL Anthology identity takes precedence over potential same-study arXiv version; no second record for it. No community analysis used to promote maturity. Three archival Findings EMNLP papers + six arXiv preprints. ARXIV-based claims bounded to available abstracts/HTML; numerical claims not independently replicated.

## Provisional entries

| Provisional ID | Study | Source/version | Primary | Cross cutting | Framework | Estimand | Claim | Identification/Transport | Role |
|---|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261026-01 | [TRACE: A Traceable Agentic Co-Optimizer for Experimental Optimization](https://aclanthology.org/2026.findings-emnlp.295/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | ASR | BGT | DR/EG/MEAS/ID/BT | `BO_CONSTRAINED_INTERVENTION_POLICY_VALUE` | CL1 | I1/T0 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-02 | [BID-SPO: Rethinking Multi-Agent Prompt Optimization as Information Contracting via Bidding-based Shapley Values](https://aclanthology.org/2026.findings-emnlp.239/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | SCF | CSCI/BGT | MI/IA/ID/MEAS/BT | `INTER_AGENT_INTERFACE_CONTRACT_ALIGNMENT_EFFECT` | CL1 | I1/T1 | INTERACTION_BOUNDARY |
| SIS-CAND-20261026-03 | [PaperScout: An Autonomous Agent for Academic Paper Search with Process-Aware Sequence-Level Policy Optimization](https://aclanthology.org/2026.findings-emnlp.1743/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | ASR | BGT | DR/TD/MEAS/ID/BT | `SEQUENCE_LEVEL_SEARCH_POLICY_VALUE` | CL1 | I1/T1 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-04 | [How Much Does the Harness Matter, and for Whom? A Multi-Model Study of Context in LLM-Driven Vulnerability Discovery](https://arxiv.org/abs/2610.28802) | arXiv v1 2026-10-20; delayed discovery | SCF | CSCI/BGT | MI/IA/ID/MEAS/BT | `MODEL_BY_PROMPT_CONTEXT_INTERACTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | CSCI_BOUNDARY |
| SIS-CAND-20261026-05 | [SpecMAGIC: Specification-Guided Multi-Task Generalization in Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2610.30443) | arXiv v1 2026-10-21; delayed discovery | SCF | BGT | MI/IA/EG/MEAS/BT | `TEMPORAL_SPEC_COMPOSITION_ZERO_SHOT_VALUE` | CL0 formal; CL1 empirical | I0/I1/T1 | FORMAL_BOUNDARY_FRAMEWORK |
| SIS-CAND-20261026-06 | [Soft Ontology Priors over Latent Concept Posteriors for Weakly Supervised Neuro-Symbolic Learning](https://arxiv.org/abs/2610.30391) | arXiv v1 2026-10-21; author marks NeSy 2026 oral, archival verification pending | SCF | BGT | MI/EG/ID/MEAS/BT | `ONTOLOGY_PRIOR_LATENT_CONCEPT_RECOVERY_EFFECT` | CL0 theoretical; CL1 empirical; local CL2 candidate | I1/I2-local/T0 | IDENTIFICATION_BOUNDARY |
| SIS-CAND-20261026-07 | [Route-and-Generate: KL-Regularized Router Improvement for Reasoning Routing in LLMs](https://arxiv.org/abs/2610.30351) | arXiv v1 2026-10-21; delayed discovery | ASR | BGT | DR/MEAS/MI/BT | `REASONING_FORMAT_ROUTING_COST_ADJUSTED_VALUE` | CL1 | I1/T1 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-08 | [Learning Who Talks to Whom: Role-Aware Communication Topology Scheduling for Efficient LLM Multi-Agent Collaboration](https://arxiv.org/abs/2610.25851) | arXiv v1 2026-10-19; delayed discovery | ASR | CSCI/BGT | DR/IA/ID/MEAS/BT | `ROLE_TOPOLOGY_CONDITIONAL_COMMUNICATION_VALUE` | CL1; local CL2 candidate | I1/I2-local/T1 | INTERACTION_BOUNDARY |
| SIS-CAND-20261026-09 | [Policy Search in Code Space for Multi-Agent Pathfinding](https://arxiv.org/abs/2610.25946) | arXiv v1 2026-10-19; delayed discovery | ASR | BGT | DR/MI/EG/MEAS/BT | `VERIFIED_CODE_POLICY_SEARCH_VALUE` | CL0 formal; CL1 empirical | I1/T2 performance only | REGULATION_IMPLEMENTATION |

## Claim-level first-pass qualification

### SIS-CAND-20261026-01: TRACE: A Traceable Agentic Co-Optimizer for Experimental Optimization
- Primary source: https://aclanthology.org/2026.findings-emnlp.295/; **Findings EMNLP 2026, Oct (archival; delayed discovery)**.
- Program: **ASR**; cross-cutting **BGT**; Framework **DR/EG/MEAS/ID/BT**; estimand `BO_CONSTRAINED_INTERVENTION_POLICY_VALUE`; claim **CL1**; identification **I1**, transport **T0**; role **REGULATION_IMPLEMENTATION**.
- Scientific finding / evidence qualification: Auditable, bounded interventions surrounding a Bayesian-optimization backbone improve low-budget reaction optimization against BO-only and other baselines. Component bundle and limited chemical domain prevent independent causal attribution; author abstract, exact table audit pending.
- Moderators and scope: chemical reaction task, experiment budget, external evidence quality, BO prior; no separate skill vs wrapper effect. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-02: BID-SPO: Rethinking Multi-Agent Prompt Optimization as Information Contracting via Bidding-based Shapley Values
- Primary source: https://aclanthology.org/2026.findings-emnlp.239/; **Findings EMNLP 2026, Oct (archival; delayed discovery)**.
- Program: **SCF**; cross-cutting **CSCI/BGT**; Framework **MI/IA/ID/MEAS/BT**; estimand `INTER_AGENT_INTERFACE_CONTRACT_ALIGNMENT_EFFECT`; claim **CL1**; identification **I1**, transport **T1**; role **INTERACTION_BOUNDARY**.
- Scientific finding / evidence qualification: Output Bid/Input Demand and conformance-constrained Shapley feedback address interface mismatch; seven benchmark comparisons report +2.93 and +4.38 points in named configurations. Attribution shares optimizer and bid constraints; Shapley allocations do not establish causal mediation.
- Moderators and scope: input/output formats, task and backbone, model compatibility, contract compliance. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-03: PaperScout: An Autonomous Agent for Academic Paper Search with Process-Aware Sequence-Level Policy Optimization
- Primary source: https://aclanthology.org/2026.findings-emnlp.1743/; **Findings EMNLP 2026, Oct (archival; delayed discovery)**.
- Program: **ASR**; cross-cutting **BGT**; Framework **DR/TD/MEAS/ID/BT**; estimand `SEQUENCE_LEVEL_SEARCH_POLICY_VALUE`; claim **CL1**; identification **I1**, transport **T1**; role **REGULATION_IMPLEMENTATION**.
- Scientific finding / evidence qualification: Sequential retrieval decisions and Proximal Sequence Policy Optimization (PSPO) report gains in retrieval recall/relevance vs workflow and RL baselines. Search environment, retriever and sequence-level training changed together; full measured cost and evidence validity require audit.
- Moderators and scope: complex research queries, corpus recall, retrieved-evidence independence, trajectory length. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-04: How Much Does the Harness Matter, and for Whom? A Multi-Model Study of Context in LLM-Driven Vulnerability Discovery
- Primary source: https://arxiv.org/abs/2610.28802; **arXiv v1 2026-10-20; delayed discovery**.
- Program: **SCF**; cross-cutting **CSCI/BGT**; Framework **MI/IA/ID/MEAS/BT**; estimand `MODEL_BY_PROMPT_CONTEXT_INTERACTION_EFFECT`; claim **CL1; local CL2 candidate**; identification **I2-local**, transport **T1**; role **CSCI_BOUNDARY**.
- Scientific finding / evidence qualification: 24 model-runner configurations, 265 independently confirmed security root causes; engineered prompts and CodeQL context yield model-conditional effects: context beyond engineered prompt helps only smallest model in four-model comparison. Initial combined contrast changes two factors and must not be attributed to call graph alone.
- Moderators and scope: model capability, prompt quality, call graph coverage, fixed production codebase, security-review quality. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-05: SpecMAGIC: Specification-Guided Multi-Task Generalization in Multi-Agent Reinforcement Learning
- Primary source: https://arxiv.org/abs/2610.30443; **arXiv v1 2026-10-21; delayed discovery**.
- Program: **SCF**; cross-cutting **BGT**; Framework **MI/IA/EG/MEAS/BT**; estimand `TEMPORAL_SPEC_COMPOSITION_ZERO_SHOT_VALUE`; claim **CL0 formal; CL1 empirical**; identification **I0/I1**, transport **T1**; role **FORMAL_BOUNDARY_FRAMEWORK**.
- Scientific finding / evidence qualification: Temporal-logic specification language plus compositional automaton planner reuses learned subtask policies on unseen specifications; soundness/probabilistic completeness conditional on planner assumptions. Navigation benchmark cannot establish deployment-level semantic safety or T3 transport.
- Moderators and scope: correct formal specifications, planner sampling, subtask policy quality, agent number. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-06: Soft Ontology Priors over Latent Concept Posteriors for Weakly Supervised Neuro-Symbolic Learning
- Primary source: https://arxiv.org/abs/2610.30391; **arXiv v1 2026-10-21; author marks NeSy 2026 oral, archival verification pending**.
- Program: **SCF**; cross-cutting **BGT**; Framework **MI/EG/ID/MEAS/BT**; estimand `ONTOLOGY_PRIOR_LATENT_CONCEPT_RECOVERY_EFFECT`; claim **CL0 theoretical; CL1 empirical; local CL2 candidate**; identification **I1/I2-local**, transport **T0**; role **IDENTIFICATION_BOUNDARY**.
- Scientific finding / evidence qualification: Soft rather than hard ontology priors constrain shortcut equivalence without deleting feasible support under noisy axioms. BDD-OIA six-concept F1 0.362±0.001 vs strongest non-Oracle 0.330; ten seeds; true task accuracy ~0.768 vs comparators similar, oracle gap persists. Ontology supplied can encode correct answer information; no universal concept identifiability.
- Moderators and scope: ontology noise, class ordering, finite concept scope, accuracy vs latent construct validity. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-07: Route-and-Generate: KL-Regularized Router Improvement for Reasoning Routing in LLMs
- Primary source: https://arxiv.org/abs/2610.30351; **arXiv v1 2026-10-21; delayed discovery**.
- Program: **ASR**; cross-cutting **BGT**; Framework **DR/MEAS/MI/BT**; estimand `REASONING_FORMAT_ROUTING_COST_ADJUSTED_VALUE`; claim **CL1**; identification **I1**, transport **T1**; role **REGULATION_IMPLEMENTATION**.
- Scientific finding / evidence qualification: KL-regularized routing distributes fixed candidate-generation budget across direct/short-CoT/code/long-CoT formats, jointly trains response generator. Reported accuracy-efficiency improvements; router benefit versus generator co-training is not independently identified.
- Moderators and scope: four defined formats, per-format token cost variation, task difficulty calibration, verifier correctness. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-08: Learning Who Talks to Whom: Role-Aware Communication Topology Scheduling for Efficient LLM Multi-Agent Collaboration
- Primary source: https://arxiv.org/abs/2610.25851; **arXiv v1 2026-10-19; delayed discovery**.
- Program: **ASR**; cross-cutting **CSCI/BGT**; Framework **DR/IA/ID/MEAS/BT**; estimand `ROLE_TOPOLOGY_CONDITIONAL_COMMUNICATION_VALUE`; claim **CL1; local CL2 candidate**; identification **I1/I2-local**, transport **T1**; role **INTERACTION_BOUNDARY**.
- Scientific finding / evidence qualification: Nine benchmarks; role-conditioned partner selection and topology-aware value mixing improve accuracy up to 6.19 points, >15% token reduction. Local ablation: replace mixer 75.01→71.83 macro accuracy on GPT-OSS-120B, but training/value mixer/policy changes remain coupled.
- Moderators and scope: role labels, graph sparsity, task and backbone, communication cost, information gain estimation. **First-coder provisional**; no paper-level CL2/CL3 finalization.

### SIS-CAND-20261026-09: Policy Search in Code Space for Multi-Agent Pathfinding
- Primary source: https://arxiv.org/abs/2610.25946; **arXiv v1 2026-10-19; delayed discovery**.
- Program: **ASR**; cross-cutting **BGT**; Framework **DR/MI/EG/MEAS/BT**; estimand `VERIFIED_CODE_POLICY_SEARCH_VALUE`; claim **CL0 formal; CL1 empirical**; identification **I1**, transport **T2 performance only**; role **REGULATION_IMPLEMENTATION**.
- Scientific finding / evidence qualification: Human-guided code-policy search with simulation and exact checks finds algorithms exceeding locally reproduced contest baseline by 35.0% on a dense map and proprietary warehouse baseline throughput by 58.9%. Conditional collision-freedom/completion proof applies only to new algorithm under stated assumptions. Two application families, days-long search, no causal operator ablation.
- Moderators and scope: warehouse topology, simulation validity, finite-time goal assumptions, search time/computational resources. **First-coder provisional**; no paper-level CL2/CL3 finalization.


## P0 audit backlog progression

First-coder re-audit of **SIS-LIT-033, SIS-LIT-034, SIS-LIT-038** produced **9 independently scoped ClaimRecords**, with interventions, measurement, boundary restrictions and causal ceilings in [same-date audit](../evidence-map/audits/SIS_P0_Reaudit_2026-10-26.md). No inheritance of prior paper-level CL2 labels. Second-coder and adjudication **PENDING**, prior final decisions preserved.

## Priority actionable experiments

1. **Interface Contract × Backbone Capability × Routing**: independently randomize schema/communication contracts, evaluate error localization, downstream failures and token budget (BID-SPO/ACTS).
2. **Soft Ontology × Noise × Concept Oracle**: hold task-label accuracy fixed, audit latent-concept F1 and inferred concept validity against independent Gold; include hard-prior null/perturbed axioms.
3. **Probing × Curation Instruction**: 2×2 across read-only environment access and probe prompts; compare *full pipeline* costs, drift conditions and error-memory propagation (SIS-LIT-034).
4. **Reasoning Format Router × Backbone Training**: separate router selection effects from co-trained generator, fixed candidate and total dollar budget.
5. **Temporal DSL Composition × Spec Incompleteness**: executable specification conformance vs intended-goal satisfaction, new task specifications and agents, realistic intervention and transfer.
6. **Skill Bandit × Population Evolution**: frozen candidate pool and evaluation budget, factor separation, model/harness changes; cost breakdown by target vs teaching tokens.
7. **Research Search × Evidence Sufficiency**: PaperScout high recall vs source uniqueness, claim entailment and independent citation verification.

## Formal SIS Impact Decision

**PRIMARY: `BENCHMARK_DELTA`**; secondary scientific pressure: **MEASUREMENT_IDENTIFICATION_DELTA** (identification designs to test). Today the newly found studies **mostly fill extant programs/frameworks**, particularly CSCI (interface and model-conditioned mechanisms), ASR (routing, search, resource allocation), SCF (specification and ontology externalization), BGT (cost and transfer). No uncovered estimand, nonreplaceable scientific capability or fourth program. `ScientificCoreDelta=0`; **SPEC_REVISION_CANDIDATE=NO**. No new confirmed T3 causal transport or T4 invariance. Today's practical improvement is a narrowed benchmark backlog and three claim splits, not a core revision.

## Evidence governance

Peer review is not claim-level causal identification; theoretical soundness under assumptions is not real-world performance proof. I0/I1/I2 and T0/T1/T2 are registry aids. Community technical writeups and project pages remain discovery-only absent independent replication; PDF full-text tables of the three new Findings papers were not directly audited in this first-pass update. No noise-only code/schema change.
