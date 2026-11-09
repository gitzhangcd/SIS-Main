# SIS v0.3.1 Literature Re-Coding Registry

## System Intelligence Science Evidence Map｜ARSO Research Stream Re-Coding

**Registry version:** `v1.3`  
**SIS authority:** `System Intelligence Science v0.3.1`  
**Date:** `2026-10-08`  
**Corpus:** papers and analyses previously surfaced in the ARSO research briefs, plus explicitly referenced delayed-indexing items re-verified during registry construction  
**Status:** `ACTIVE / GROWING REGISTRY`  

> This registry does **not** treat Agent, Multi-Agent, RAG, Workflow, Planner, Verifier, Memory, Tool Use, Harness, or Prompt Optimizer as first-principles SIS primitives. Each item is re-coded by its primary scientific question, estimand, identification strength, boundary conditions, and claim maturity.

---

## 1. Governing SIS v0.3.1 semantics

### Primary Scientific Programs

- `SCF` — **P1 System Capability Formation**: how mechanisms, organization, state, and context generate system properties.
- `SDR` — **P2 System Dynamics, Failure & Recovery**: how state, perturbation, failure, propagation, containment, recovery, and long-horizon behavior evolve over time.
- `ASR` — **P3 Adaptive System Regulation**: when, why, where, and how a system should act or change given available evidence.

### Cross-cutting programs

- `CSCI` — Component–System Capability Interaction: how component capability modifies a system mechanism effect.
- `BGT` — Boundary / Generalization / Transportability: replication, performance transfer, causal transportability, and mechanism invariance must remain distinct.

### Framework Capability Profile

| Code | SIS v0.3.1 Framework Capability |
|---|---|
| `MI` | `MECHANISM_INTERVENTION` |
| `TD` | `TRAJECTORY_DYNAMICS` |
| `DR` | `DECISION_REGULATION` |
| `IA` | `INTERACTION_ANALYSIS` |
| `BT` | `BOUNDARY_TRANSPORT` |
| `MEAS` | `MEASUREMENT` |
| `ID` | `IDENTIFICATION` |
| `EG` | `EVIDENCE_GOVERNANCE` |

### Claim maturity

- `CL0`: descriptive claim.
- `CL1`: associational / performance claim.
- `CL2`: controlled causal effect (`do(M) → Y`).
- `CL3`: mechanistic causality (`do(M) → Z → Y`).
- `CL4`: boundary-aware mechanism.
- `CL5`: replicated cross-context effect.
- `CL6`: transportable causal relation.
- `CL7`: candidate system law.

`CL1→CL2 candidate`, `CL2 candidate`, and `CL2→CL3 candidate` are **registry review labels**, not SIS normative claim levels. They indicate that the study contains some intervention/identification evidence but still needs a stricter claim-level audit before promotion.

### Registry-only identification tiers

- `I0`: descriptive / architectural demonstration; no controlled intervention.
- `I1`: matched baseline, ablation, or controlled comparison, but causal identification remains limited.
- `I2`: explicit manipulation, randomization, fault injection, replay, branch intervention, or otherwise strong controlled contrast.
- `I3`: intervention plus mediator/pathway-relevant evidence or unusually strong mechanistic identification within the study setting.

### Registry-only transport tiers

- `T0`: no meaningful cross-context evidence.
- `T1`: replication or multi-task/model/context performance evidence.
- `T2`: explicit cross-executor, cross-domain, cross-scale, or asset performance transfer.
- `T3`: causal transportability evidence.
- `T4`: mechanism-invariance evidence.

These `I*` and `T*` tiers are maintenance aids for this registry; they are **not** additions to SIS v0.3.1 Core.

---

## 2. Corpus-level snapshot

- **Total coded items:** `145`
- **Primary Program:** SCF `53` · SDR `32` · ASR `56` · ROUTING_ABSTAIN `4`
- **Framework capability occurrences:** MI `65` · TD `37` · DR `76` · IA `23` · BT `43` · MEAS `47` · ID `40` · EG `38`
- **Transport coding:** T0 `49` · T1 `71` · T2 `25` · T3 `0` · T4 `0`

### Immediate interpretation

1. The corpus strongly populates all three Primary Programs; no fourth Primary Program is required by the reviewed literature.
2. `ASR` is the largest and fastest-expanding cluster, especially for stopping, routing, evidence acquisition, influence strength, budget allocation, readiness, and selective intervention.
3. `CSCI` has substantial empirical motivation, but most studies still compare model IDs rather than explicitly estimating a component-capability × mechanism interaction.
4. The dominant evidence maturity remains around `CL1`; controlled-intervention studies exist, but mature transportable mechanism claims are rare.
5. The sharpest evidence gap is transportability: **no item in this registry is currently coded T3/T4**.

---

## 3. Master re-coding table

| ID | Study | Source / status | Primary | Cross-cutting | Capability | Primary estimand | Claim | ID / Transport | Evidence role & SIS interpretation |
|---:|---|---|---|---|---|---|---|---|---|
| SIS-LIT-001 | WHALE: A Simple Recipe for Joint Harness-Weight Optimization | arXiv:2609.00196 (preprint) | `SCF` | `CSCI` | `MI; BT` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T1` | Mechanism support — Joint harness/model optimization; supports system–component interaction; no Core change. |
| SIS-LIT-002 | JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution | arXiv:2608.25593 (preprint) | `ASR` | `SCF` | `DR; MI` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Framework/mechanism support — Adaptive runtime harness selection; supports endogenous regulation. |
| SIS-LIT-003 | AutoSaddler: Automatic Harness Optimization with Durable Updates from Agent Execution Traces | arXiv:2608.23041 (preprint) | `P2/SDR` | `ASR` | `TD; MI; EG` | `RECOVERY_EFFECT` | `CL1→CL2 candidate` | `I1` / `T1` | Recovery mechanism — Trace diagnosis→durable repair→validation; useful recovery fixture. |
| SIS-LIT-004 | DCFA: Dual-view Causal-inspired Attribution for Failure Reasoning in LLM-based Multi-agent Systems | arXiv:2609.04749 → EMNLP 2026 Main: 2026.emnlp-main.1887 (same study; version linked 2026-11-09) | `P2/SDR` | `ASR` | `ID; IA` | `PROPAGATION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Attribution mechanism — Supports dependency-aware attribution; causal language should remain bounded by intervention evidence. |
| SIS-LIT-005 | LLM-as-a-Judge Is Not an Oracle: Why Self-Improving Agents Need Deterministic Guardrails | arXiv:2609.02246 (preprint) | `SCF` | `—` | `MEAS; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Negative/boundary evidence — Evaluator reliability is a system mechanism; supports evidence-independence and deterministic guardrails. |
| SIS-LIT-006 | From Rollouts to Recipes: Self-Contained Post-Training for LLMs | arXiv:2609.01422; EMNLP 2026 | `ASR` | `CSCI` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Regulation mechanism — Routes among training operators; supports policy-selection framing. |
| SIS-LIT-007 | Adaptive Influence Graphs for Failure Attribution in Multi-Agent Systems | arXiv:2608.24361 (preprint) | `P2/SDR` | `—` | `TD; ID; IA` | `PROPAGATION_EFFECT` | `CL1` | `I1` / `T0` | Attribution instrument — Influence-graph representation for dynamic attribution. |
| SIS-LIT-008 | MAPRO: Recasting Multi-Agent Prompt Optimization as Maximum a Posteriori Inference | Findings EACL 2026 | `SCF` | `—` | `MI; IA` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T0` | Mechanism support — Coupled prompt optimization; supports interaction-aware optimization rather than isolated edits. |
| SIS-LIT-009 | Don’t Generate, Classify! Low-Latency Prompt Optimization with Structured Complementary Prompt | EACL 2026 Long | `SCF` | `—` | `MI` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Representation mechanism — Structured prompt fields as intervention representation; implementation evidence. |
| SIS-LIT-010 | Control-Data Flow Separation: Stable Prompt Optimization in Multi-Agent LLMs | EMNLP 2026 Findings / preprint | `SCF` | `—` | `MI; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1` / `T0` | Mechanism support — Typed control vs mutable data flow; strong externalization hypothesis for SCF. |
| SIS-LIT-011 | Polished but Unresolved: Identifying Late-Stage Pressure States in Long-Horizon Tool-Use Agents | EMNLP 2026 / preprint | `P2/SDR` | `—` | `TD; MEAS` | `LONG_HORIZON_EFFECT` | `CL1` | `I1` / `T0` | Failure-state measurement — Premature termination/unresolved constraints; supports terminal-state dynamics. |
| SIS-LIT-012 | τ^τ-Bench: An Environment for End-To-End, Realistic Agent Construction | 2026 benchmark preprint | `SCF` | `BGT` | `MEAS; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL0→CL1` | `I0/I1` / `T1` | Benchmark instrument — Deployment/artifact-level evaluation; useful Tier-2/3 fixture, not mechanism evidence. |
| SIS-LIT-013 | Bilevel Coordinated Reflection: A Game-Theoretic Approach to Multi-Agent LLM Systems | 2026 preprint | `ASR` | `P2/SDR` | `DR; EG` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Regulation/guarding mechanism — Grounded-gated reflective update; reflection should not self-authorize. |
| SIS-LIT-014 | Where Reliability Lives: Experimental Localisation of Behavioural Properties in an Agent System | 2026 preprint | `SCF` | `P2/SDR` | `MI; IA` | `ORGANIZATION_EFFECT` | `CL1→CL2 candidate` | `I2` / `T0` | Mechanism/boundary evidence — Reliability can reside in boundaries/institutions/world rather than model cognition. |
| SIS-LIT-015 | TruthInsightBench: Evidence-Grounded Benchmark for Automated Evaluation of Open-Ended Scientific Discovery Agents | 2026 benchmark preprint | `SCF` | `—` | `MEAS; EG` | `CAPABILITY_FRONTIER_SHIFT` | `CL0→CL1` | `I0` / `T0` | Benchmark instrument — Evidence/robustness/falsifiability dimensions for open-ended outcomes. |
| SIS-LIT-016 | Meta^n: Recursive Self-Improvement through Emergent Depth | 2026 preprint | `ASR` | `P2/SDR` | `DR; TD` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Adaptation mechanism — Recursive meta-state growth; useful recursive-regulation fixture. |
| SIS-LIT-017 | Recuris: Recursive Experiential-Working Memory Evolution for Long-Horizon Agent Harnesses | 2026 preprint | `P2/SDR` | `ASR` | `TD; EG; DR` | `LONG_HORIZON_EFFECT` | `CL1` | `I1` / `T0` | Memory/recovery mechanism — Working/skill memory and validation-gated updates; implementation evidence. |
| SIS-LIT-018 | AgentGrad: Intervention-guided Prompt Optimization for Multi Agent Systems | arXiv:2609.08572 (preprint) | `ASR` | `P2/SDR` | `MI; ID; DR` | `INTERVENTION_LOCUS_SELECTION_EFFECT` | `CL2` | `I2` / `T1` | Causal attribution→repair evidence — Important intervention-based locus verification; strong SIS fixture. |
| SIS-LIT-019 | Procedural Graphs: Self-Evolving Execution Structures for LLM Agents | arXiv:2609.09153 (preprint) | `SCF` | `ASR` | `MI; TD` | `ORGANIZATION_EFFECT` | `CL1` | `I1` / `T1` | Representation mechanism — Procedural execution structures as reusable system mechanism. |
| SIS-LIT-020 | Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Models Catch Up Where Imitation Fails | arXiv:2609.09134 (preprint) | `SCF` | `CSCI` | `MI; BT` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T2` | Boundary/interaction evidence — Harness–executor compatibility and co-adaptation; strong CSCI motivation. |
| SIS-LIT-021 | SE-GoS: Self-Evolving Graph-of-Skills for Skill Library at Scale | arXiv:2609.08228 (preprint) | `ASR` | `SCF` | `DR; IA` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Regulation mechanism — Skill-graph routing/topology optimization. |
| SIS-LIT-022 | MemForest: Efficient Agent Memory Management via EventTree Partitioning and Progressive Merging | arXiv:2609.08273 (preprint) | `SCF` | `P2/SDR` | `MI; TD` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Representation mechanism — Memory compaction/structure mechanism; not a new SIS primitive. |
| SIS-LIT-023 | Does Your Agent's Memory Survive a Model Upgrade? A Controlled Study of Memory Portability | arXiv:2609.05339 (preprint) | `SCF` | `CSCI; BGT` | `BT; MI` | `MECHANISM_INTERACTION_EFFECT` | `CL1→CL2 candidate` | `I1` / `T2` | Boundary evidence — Structured memory more portable than free-text notes; performance transfer, not causal transport. |
| SIS-LIT-024 | MA-Evolve / At Equal Inference Cost, Multi-Agent Structure Does Not Beat a Single Frozen Agent | arXiv:2609.04217 (preprint) | `SCF` | `CSCI` | `IA; MEAS` | `ORGANIZATION_EFFECT` | `CL2 candidate` | `I2` / `T1` | Negative evidence — Iso-compute result challenges complexity/multi-agent superiority assumptions. |
| SIS-LIT-025 | ARISE-RL: Agentic Rubric-Grounded Iterative Self-Evolution with Reinforcement Learning | arXiv:2609.01058 (preprint) | `ASR` | `—` | `DR; EG` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Regulation framework — Rubric/task generation and reward-gated updates; evaluator co-adaptation risk. |
| SIS-LIT-026 | ExecCritic: Learn to Test, Test to Improve for Coding Agents | arXiv:2609.09133 (preprint) | `P2/SDR` | `ASR` | `EG; ID; MI` | `RECOVERY_EFFECT` | `CL2 candidate` | `I2` / `T0` | Negative + recovery evidence — Poor tests can be worse than no tests; supports independent evaluator authority. |
| SIS-LIT-027 | EDGE: Error Dependency Graph-Guided Multi-Error Attribution in Multi-Agent LLM Systems | EMNLP 2026 / arXiv:2609.01360 | `P2/SDR` | `—` | `TD; ID; IA` | `PROPAGATION_EFFECT` | `CL2 candidate` | `I2` / `T0` | Dynamic attribution — Error dependency + counterfactual rollout; strong P2 fixture. |
| SIS-LIT-028 | MASkills: Continual Skills Optimization for Multi-Agent LLM Systems | arXiv:2609.02094 (preprint) | `SCF` | `ASR` | `MI; DR` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T1` | Mechanism support — Experience→skill consolidation/pruning; mechanism promotion implementation. |
| SIS-LIT-029 | How Fast Do Agents Rot? An Empirical Study of Long-Horizon Degradation in LLM Agents | arXiv:2609.01660 (preprint) | `P2/SDR` | `BGT` | `TD; MEAS; BT` | `LONG_HORIZON_EFFECT` | `CL1` | `I1` / `T1` | Dynamics/boundary evidence — Horizon-dependent reliability decay; supports trajectory-first evaluation. |
| SIS-LIT-030 | What LLM Trading Agents Actually Do in Production | arXiv:2609.05663 (preprint) | `SCF` | `CSCI` | `MEAS; IA` | `ORGANIZATION_EFFECT` | `CL1` | `I0/I1` / `T0` | Real-world associational evidence — Operating-layer effects motivate system ≠ model; causal claims remain limited. |
| SIS-LIT-031 | Artic: Natural-Language Workflows Are Not Software Yet | arXiv:2608.21341 (preprint) | `SCF` | `—` | `MI` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1` / `T0` | Representation mechanism — Typed artifact workflow externalization; useful SCF manipulation. |
| SIS-LIT-032 | Ecdysis: Efficient and Effective Training of Runtime Harnesses for LLM Agents | 2026 preprint | `P2/SDR` | `ASR` | `TD; ID; DR` | `RECOVERY_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Failure generality mechanism — Distinguishes local model errors from systematic harness defects. |
| SIS-LIT-033 | COBRA-Skills: Contextual Bandit-Guided Evolution for Agent Skill Optimization | 2026 preprint | `ASR` | `—` | `DR` | `VALUE_OF_INFORMATION` | `CL1` | `I1` / `T1` | Budget regulation — Allocates evaluation budget among candidate skills. |
| SIS-LIT-034 | Grounding Agent Memory: Environment-Probing Curation for Enterprise Agents | 2026 preprint | `ASR` | `SCF` | `EG; DR; ID` | `VALUE_OF_INFORMATION` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Evidence-governance mechanism — Probe before memory promotion; strong evidence-governance example. |
| SIS-LIT-035 | Decoupling Readiness from Release for Tail-Aware Scheduling of Agentic LLM Workflows | 2026 preprint | `ASR` | `—` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Regulation mechanism — Readiness vs release as scheduling policy state. |
| SIS-LIT-036 | JTPRO: A Joint Tool–Prompt Reflective Optimization Framework for Language Agents | Findings ACL 2026 | `SCF` | `—` | `MI` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T1` | Mechanism interaction — Joint prompt/tool-schema optimization; interface is part of system. |
| SIS-LIT-037 | PROTEA: Offline Evaluation and Iterative Refinement for Multi-Agent LLM Workflows | ACL 2026 Demo | `P2/SDR` | `ASR` | `TD; ID; MI` | `RECOVERY_EFFECT` | `CL1` | `I1` / `T0` | Diagnosis→repair instrument — Intermediate localization and targeted patching. |
| SIS-LIT-038 | Do We Always Need Query-Level Workflows? Rethinking Agentic Workflow Generation for Multi-Agent Systems / SCALE | Findings ACL 2026 | `ASR` | `SCF` | `DR; MI` | `SELECTIVE_ACTION_UTILITY` | `CL1` | `I1` / `T1` | Granularity/boundary evidence — Shared/coarse workflows can retain quality at lower cost. |
| SIS-LIT-039 | Accelerating Language Model Workflows with Prompt Choreography | TACL 2026 | `SCF` | `—` | `MI; MEAS` | `CAPABILITY_FRONTIER_SHIFT` | `CL1` | `I1` / `T0` | Runtime mechanism — Context/cache/runtime scheduling shifts performance–cost frontier. |
| SIS-LIT-040 | Agent-GWO: Collaborative Agents for Dynamic Prompt Optimization in Large Language Models | Findings ACL 2026 | `ASR` | `—` | `DR` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Optimization regime — Population search over prompt/configuration; needs iso-compute interpretation. |
| SIS-LIT-041 | Reflective RAG: Self-Evaluation Driven Strategy Optimization in Agentic Retrieval-Augmented Generation | Findings ACL 2026 | `ASR` | `—` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Regulation mechanism — Reflection tags guide strategy; reflection is signal, not authority. |
| SIS-LIT-042 | HFlow: Evolving Agentic Workflow Driven by Human-Agent Collaboration | Findings ACL 2026 | `SCF` | `ASR` | `MI; DR; IA` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T1` | Joint optimization — Workflow/prompts/backbones co-evolve; attribution of contribution remains open. |
| SIS-LIT-043 | Learning from Contrastive Prompts: An Automated Prompt Optimization Framework | Findings ACL 2026 | `ASR` | `—` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Evidence-use mechanism — Contrastive success/failure evidence informs edits. |
| SIS-LIT-044 | Failure Makes the Agent Stronger: Enhancing Accuracy through Structured Reflection for Reliable Tool Interactions | Findings ACL 2026 | `P2/SDR` | `ASR` | `TD; MI` | `RECOVERY_EFFECT` | `CL1` | `I1` / `T0` | Recovery mechanism — Structured erroneous-call diagnosis→corrected-call recovery. |
| SIS-LIT-045 | Prompt Optimization Is a Coin Flip: Diagnosing When It Helps in Compound AI Systems | 2026 paper/preprint | `ASR` | `CSCI` | `DR; MEAS` | `SELECTIVE_ACTION_UTILITY` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Negative/boundary evidence — Headroom/coupling tests motivate optimization eligibility and NoOp. |
| SIS-LIT-046 | Why Prompt Optimization Works, and Why It Sometimes Doesn't: A Causal-Inspired Edit-Level Analysis | 2026 paper/preprint | `SCF` | `ASR; BGT` | `MI; ID` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Mechanism/boundary evidence — Edit family × task type heterogeneity; operator effects are conditional. |
| SIS-LIT-047 | Agentic Harness Engineering: The Operating System for Machine Intelligence | Technical/community analysis | `SCF` | `—` | `—` | `—` | `CL0` | `I0` / `T0` | Technical synthesis — Engineering ontology/discovery only; not scientific evidence. |
| SIS-LIT-048 | Verified Critical Step Optimization for LLM Agents | Findings ACL 2026 | `P2/SDR` | `ASR` | `ID; TD; MI` | `RECOVERY_EFFECT` | `CL2` | `I2` / `T1` | Counterfactual verification — Outcome-flip + target-policy reachability; strong causal repair fixture. |
| SIS-LIT-049 | Attribution-Based Analysis and Optimization of Modular Agentic Workflows / ShapleyFlow | Findings ACL 2026 | `SCF` | `—` | `IA; ID` | `MECHANISM_INTERACTION_EFFECT` | `CL2 candidate` | `I2` / `T1` | Contribution attribution — Marginal component value differs from failure causation. |
| SIS-LIT-050 | Seeing the Whole Elephant: A Benchmark for Failure Attribution in LLM-based Multi-Agent Systems / TraceElephant | ACL 2026 Long | `P2/SDR` | `—` | `MEAS; ID` | `TRAJECTORY_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Observability evidence — Full vs partial trace changes attribution quality; supports observability experiments. |
| SIS-LIT-051 | Reflection in the Dark: Exposing and Escaping the Black Box in Reflective Prompt Optimization / VISTA | ACL 2026 SRW | `ASR` | `P2/SDR` | `DR; ID` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Negative/boundary evidence — Defective-seed reflection can degrade; verify hypotheses before rewrite. |
| SIS-LIT-052 | FAMA: Failure-Aware Meta-Agentic Framework for Open-Source LLMs in Interactive Tool Use Environments | Findings ACL 2026 | `ASR` | `—` | `DR` | `SELECTIVE_ACTION_UTILITY` | `CL1` | `I1` / `T1` | Selective regulation — Activates minimal specialist subset by failure mode. |
| SIS-LIT-053 | Do LLMs Catch Their Own Mistakes? A Comprehensive Benchmark for Reflective Tool Use LLMs | Findings ACL 2026 | `P2/SDR` | `CSCI` | `MEAS; ID` | `TRAJECTORY_EFFECT` | `CL1` | `I1` / `T1` | Negative evidence — Self-error recognition lags external-error recognition; supports independent diagnosis. |
| SIS-LIT-054 | TRAJDEBUG: Tracing Error Lifecycle to Identify Critical Failures in Long-Horizon Agent Trajectories | arXiv:2608.06346 (preprint) | `P2/SDR` | `—` | `TD; ID` | `PROPAGATION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Dynamics mechanism — Active/resolved/masked/propagated status + terminal impact. |
| SIS-LIT-055 | When Agents Slow Down: Understanding LLM Agents' Test-Time Strategies via Elo-per-token Analysis | arXiv:2609.15309 (preprint) | `ASR` | `BGT` | `DR; MEAS` | `REGULATION_NET_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Resource-regulation evidence — Performance–compute curves and inflection points motivate stop/restart policy. |
| SIS-LIT-056 | The Router Within: Eliciting Native Skill Routing from a Frozen LLM | arXiv:2609.15982 (preprint) | `ASR` | `CSCI` | `DR; MEAS` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T2` | Routing mechanism — Executor-native latent routing signal; router implementation should remain replaceable. |
| SIS-LIT-057 | RSIAgent: Autonomous Exploration for Recursive Self-improvement in New Environments | arXiv:2609.15364 (preprint) | `ASR` | `P2/SDR` | `DR; EG; TD` | `VALUE_OF_INFORMATION` | `CL1` | `I1` / `T1` | Exploration mechanism — Proactive environment exploration→reusable knowledge; compute confounding remains. |
| SIS-LIT-058 | LIMBO: Lifelong Inference-Time Memory and Budget Optimization for LLM Agents | ICTAI 2026 / preprint | `ASR` | `CSCI` | `DR; BT` | `REGULATION_NET_VALUE` | `CL1` | `I1` / `T2` | Resource regulation — Memory use as controllable inference-time resource. |
| SIS-LIT-059 | Asclepius: An Adaptive Harness for Long-Horizon Clinical Agents | EMNLP 2026 Findings | `P2/SDR` | `SCF` | `TD; MI; IA` | `RECOVERY_EFFECT` | `CL2 candidate` | `I2` / `T1` | Coupled bottleneck evidence — Multiple failure modes may require joint intervention. |
| SIS-LIT-060 | Recursive Self-Improvement LLM Agents for Inverter Dynamic Model Identification | 2026 position/proof-of-concept preprint | `SCF` | `ASR` | `MI; DR` | `CAUSAL_MECHANISM_EFFECT` | `CL0→CL1` | `I0/I1` / `T0` | Cross-domain implementation — Typed vocabulary + grammar-constrained program search; proof-of-concept only. |
| SIS-LIT-061 | ScienceBuddy: Recursive-in-Recursive Self-Improvement for Interactive Scientific Agents | 2026 preprint | `SCF` | `CSCI` | `MI; BT; DR` | `MECHANISM_INTERACTION_EFFECT` | `CL1` | `I1` / `T1` | Co-evolution hypothesis — Harness evolution + model learning; interaction effect needs factorial validation. |
| SIS-LIT-062 | EvoOntology: A Self-Evolving Ontology Layer for Data Agents | 2026 preprint | `SCF` | `ASR` | `MI; DR; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T1` | Typed semantic mechanism — Ontology as mutable typed artifact with paired evaluation. |
| SIS-LIT-063 | REALM: Retrieval-Driven Memory Reconsolidation for Long-Term LLM Agents | 2026 preprint | `P2/SDR` | `ASR` | `TD; DR` | `RECONFIGURATION_TRAJECTORY_EFFECT` | `CL1` | `I1` / `T1` | Memory dynamics — Retrieval feedback changes future memory organization. |
| SIS-LIT-064 | Emergence World: Adversarial Stress-Testing of Long-Horizon Multi-Agent Systems | 2026 preprint | `P2/SDR` | `BGT` | `TD; IA; MEAS` | `LONG_HORIZON_EFFECT` | `CL0→CL1` | `I0/I1` / `T1` | Stress-test benchmark — Failure can propagate through memory/environment/agent network over long horizons. |
| SIS-LIT-065 | Assembling the CREW: A Collaborative Multi-Agent Reinforcement Learning Framework for Automated Related Work Generation | 2026 preprint | `ASR` | `SCF` | `DR; IA` | `POLICY_VALUE` | `CL1` | `I1` / `T0` | Regulation mechanism — Learned collaboration policy; single-domain evidence. |
| SIS-LIT-066 | Symbolic Separation: Grounding Deep Agents in Knowledge Graphs for Trustworthy Operational Data Analytics | 2026 preprint | `SCF` | `—` | `MI; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Execution-boundary mechanism — Ontology-constrained data access; semantic layer as control boundary. |
| SIS-LIT-067 | Blueprint First, Model Second: A Framework for Deterministic LLM Workflow | ICSME 2026 Research Track | `SCF` | `—` | `MI` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Compiler mechanism — Deterministic blueprint separates control from probabilistic reasoning. |
| SIS-LIT-068 | Dream-RSI: Recursive Self-Improvement through Evolving Worlds | arXiv:2609.14858 (preprint) | `ASR` | `P2/SDR` | `DR; TD; BT` | `POLICY_VALUE` | `CL2 candidate` | `I2` / `T1` | Replay/regulation mechanism — Historical exploration trees act as replay environments; online generalization remains bounded. |
| SIS-LIT-069 | Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in Mathematics and Theoretical Computer Science | arXiv:2609.15983 (preprint) | `ASR` | `P2/SDR` | `DR; TD` | `SELECTIVE_ACTION_UTILITY` | `CL1` | `I1` / `T0` | Readiness regulation — Readiness gate before expensive decomposition/execution. |
| SIS-LIT-070 | Large Language Models Develop Belief State Geometry In-Context | arXiv:2609.17376 (preprint) | `SCF` | `—` | `MEAS; ID` | `MEDIATED_MECHANISM_EFFECT` | `CL2→CL3 candidate` | `I2/I3` / `T0` | Representation/mechanistic evidence — Latent belief state is probeable and interventionally relevant in controlled HMM setting. |
| SIS-LIT-071 | SVMemAgent: A Streaming Video Memory Agent for Query-Agnostic Online Frame Selection | 2026 preprint | `ASR` | `—` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Curation policy — Keep/replace/discard evidence under fixed memory budget. |
| SIS-LIT-072 | Think Earlier, Not Longer: Prompt Optimization via Reducing Unhealthy Exploration | Findings ACL 2026 | `SCF` | `ASR` | `MI; DR` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T1` | Search-dynamics mechanism — Prompt intervention changes reasoning trajectory distribution. |
| SIS-LIT-073 | LLM Prompt Duel Optimizer: Efficient Label-Free Prompt Optimization | Findings ACL 2026 | `ASR` | `—` | `DR; MEAS` | `VALUE_OF_INFORMATION` | `CL1` | `I1` / `T0` | Evaluation-budget regulation — Dueling-bandit allocation of judge budget. |
| SIS-LIT-074 | Historical Reflection-Guided Prompt Optimization | Findings ACL 2026 | `ASR` | `—` | `DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Optimizer-memory mechanism — Positive+negative optimization history guides next action; semantic compression may lose diversity. |
| SIS-LIT-075 | Knowledge-Based Zero-Replay Debugging of Multi-Agent LLM Traces | 2026 preprint | `ASR` | `P2/SDR` | `ID; DR; TD` | `VALUE_OF_INFORMATION` | `CL2 candidate` | `I2` / `T1` | Hierarchical debugging instrument — Predict which trace branches deserve replay budget. |
| SIS-LIT-076 | SoL-Pi: Recursively Scaling Auto-Research Loops for Efficient Agent Harness | 2026 preprint | `SCF` | `ASR; BGT` | `MI; BT; DR` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Mechanism promotion evidence — Reusable harness mechanisms selected across tasks/executors; causal invariance not shown. |
| SIS-LIT-077 | Chronicle: Cut-Point Replay for Regression Testing of LLM Agents | REALM 2026 Workshop / arXiv:2609.20625 | `P2/SDR` | `ASR` | `TD; ID; EG` | `RECOVERY_EFFECT` | `CL2` | `I2` / `T0` | Counterfactual replay instrument — Controlled cut-point intervention with immutable boundary envelopes. |
| SIS-LIT-078 | Failure-Guided Co-Evolution of Prompts and Training Data / FORGE | 2026 preprint | `ASR` | `SCF` | `DR; EG` | `VALUE_OF_INFORMATION` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Evidence-generation mechanism — Failure modes generate new diagnostic/training cases; confirmation-loop risk. |
| SIS-LIT-079 | Designing Agentic AI Workflow Portfolios under Imperfect Selection and Compute Cost | 2026 preprint | `ASR` | `SCF` | `DR; IA` | `POLICY_VALUE` | `CL1` | `I1` / `T1` | Portfolio regulation — Workflow portfolio + selector; more candidates can hurt under imperfect selection. |
| SIS-LIT-080 | Semantic Layer Induction from Raw Telemetry via Hierarchical LLM and RAG Abstraction | 2026 preprint | `SCF` | `—` | `MI; MEAS` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Representation mechanism — Induced semantic layer from raw traces; judge dependence limits causal interpretation. |
| SIS-LIT-081 | SAGE: Governed Artifact Generation from Enterprise Guidelines | 2026 preprint | `SCF` | `—` | `MI; EG; MEAS` | `CAUSAL_MECHANISM_EFFECT` | `CL2 candidate` | `I2` / `T0` | Contract/governance evidence — No-governance ablation suggests measurable reliability effect. |
| SIS-LIT-082 | Dual-Axis Policy Optimization for LLM Agents: Bayesian Feedback Attribution and Trajectory Mass Normalization / BATON | arXiv:2609.19830 (preprint) | `ASR` | `P2/SDR` | `DR; ID` | `POLICY_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Signal decomposition — Separates intra-trajectory attribution from inter-trajectory aggregation. |
| SIS-LIT-083 | Self-Evolving Search Index | arXiv:2609.19656 (WIP preprint) | `SCF` | `ASR` | `MI; DR; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T1` | Infrastructure mechanism — Index keys as selective intervention surface; WIP evidence. |
| SIS-LIT-084 | Symbolic Temporal Supervision of LLM Agents Using Contracts / ContrAgent | arXiv:2609.18128 (preprint) | `SCF` | `—` | `MI; MEAS; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL2 candidate` | `I2` / `T1` | Executable-spec mechanism — Same formal contract compiles to runtime gate and offline evaluator. |
| SIS-LIT-085 | AutoData: Agentic Search for Pre-training Data Selection | arXiv:2609.19754 (preprint) | `SCF` | `ASR` | `MI; DR; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL1` | `I1` / `T2` | Program-search mechanism — Data-selection program as optimizable mechanism; proxy→scale transfer. |
| SIS-LIT-086 | Flag Game: A Toy Model for Mechanistic Swarm Interpretability | arXiv:2609.19124 (preprint) | `P2/SDR` | `CSCI; BGT` | `IA; ID; TD` | `PROPAGATION_EFFECT` | `CL2→CL3 candidate` | `I3` / `T1` | Mechanistic boundary evidence — Population scale changes attribution/intervention efficacy; local cause≠local repair. |
| SIS-LIT-087 | Coding Agents with an Obstacle-Aware Harness for Safe Robot Manipulation | arXiv:2609.20822 (preprint) | `P2/SDR` | `SCF` | `ID; MI` | `RECOVERY_EFFECT` | `CL2 candidate` | `I2` / `T0` | Cross-layer fault evidence — Requirement understood but absent from planning objective; targeted harness repair. |
| SIS-LIT-088 | What Prompts Don’t Say: Understanding and Managing Underspecification in LLM Prompts | Findings ACL 2026 | `SCF` | `BGT` | `MEAS; MI` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Boundary/robustness evidence — Observed success can hide inferred requirements and silent regression. |
| SIS-LIT-089 | ARCHITECT: Uncertainty-Aware Dynamic Tool Learning via Causal Intervention for Open-World Agents | ACL 2026 Long | `P2/SDR` | `ASR` | `ID; MI; EG` | `RECOVERY_EFFECT` | `CL2→CL3 candidate` | `I3` / `T1` | Causal attribution→repair evidence — SCM + sandbox intervention + targeted repair downstream utility. |
| SIS-LIT-090 | AT²PO: Agentic Turn-based Policy Optimization via Tree Search | ACL 2026 Long | `ASR` | `—` | `DR` | `POLICY_VALUE` | `CL1` | `I1` / `T1` | Granularity mechanism — Turn-level optimization as policy granularity; effect modest/conditional. |
| SIS-LIT-091 | Beyond Prompts: Measuring and Optimizing LLM Tool-Agent Harnesses / PRISM | 2026 preprint | `ASR` | `SCF` | `DR; ID; MI` | `INTERVENTION_LOCUS_SELECTION_EFFECT` | `CL2 candidate` | `I2` / `T1` | Locus-routing evidence — Failure clusters route repair to prompt/tool/joint edit; selected-repair reliability matters. |
| SIS-LIT-092 | GUIDE: Designer-in-the-loop Authoring of Conformant Generative User Interfaces | 2026 preprint | `ASR` | `SCF` | `EG; DR; MEAS` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Human-edit evidence — Edit-derived feedback is richer than scalar rating; small expert study. |
| SIS-LIT-093 | Ontology-to-tools Compilation for Executable Semantic Constraint Enforcement in LLM Agents | 2026 preprint | `SCF` | `—` | `MI; EG` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T0` | Compiler mechanism — Ontology→executable interface; proof-of-principle domain evidence. |
| SIS-LIT-094 | SelfOp: An Optimization Algorithm for Self-Improving Security Agents | 2026 preprint | `ASR` | `SCF; BGT` | `DR; BT` | `REGULATION_NET_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Stopping/promotion evidence — Cross-instance textual-gradient consensus and diagnostic convergence stopping. |
| SIS-LIT-095 | EDGEGEN: Improving Tool-Calling Agents Beyond Happy Paths with Synthetic Edge Case Generation | 2026 preprint | `ASR` | `SCF` | `EG; DR` | `VALUE_OF_INFORMATION` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Proactive evidence generation — Specification-conditioned edge-case generation; strong benchmark-factory relevance. |
| SIS-LIT-096 | MemCalib: Benchmarking and Optimizing Memory Use in LLM Agents | 2026 preprint | `ASR` | `CSCI` | `DR; ID; MEAS` | `ACTION_SELECTION_EFFECT` | `CL2 candidate` | `I2` / `T1` | Influence-calibration evidence — Over-use and under-use of memory; counterfactual credit assignment. |
| SIS-LIT-097 | Emergent Collusion in Long-Horizon LLM Agent Interaction | 2026 preprint | `P2/SDR` | `BGT` | `TD; IA; ID` | `LONG_HORIZON_EFFECT` | `CL2 candidate` | `I2` / `T1` | History-mediated failure — Peer/history/reward interactions causally influence collusion in constructed setting. |
| SIS-LIT-098 | onPanda: Efficient Annotation of On-Policy Alignment Data for LLMs and Agents via Token-Level Correction | 2026 preprint | `ASR` | `—` | `EG; DR` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T0` | Human-intervention instrument — First-divergence correction as efficient human escalation primitive. |
| SIS-LIT-099 | RAFT: A Stateful Retrieval-Augmented Framework for Troubleshooting Agents | EMNLP 2026 Industry Track | `SCF` | `ASR` | `MI; DR; BT` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T1` | State-conditioned retrieval — Retrieve by current troubleshooting state rather than whole-case similarity. |
| SIS-LIT-100 | Data Agents: Agentic Data Systems | IEEE TKDE 2026 | `SCF` | `ASR` | `MI; DR; EG` | `ORGANIZATION_EFFECT` | `CL1` | `I1` / `T1` | Architecture synthesis — Semantic operators/pipeline/feedback/memory as system implementation; not a new SIS primitive. |
| SIS-LIT-101 | Recursive Self-Improvement of AI Research Agents / AIDE² | 2026 preprint | `ASR` | `SCF; BGT` | `DR; BT; EG` | `POLICY_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Recursive adaptation evidence — Self-modification with hidden evaluation and held-out transfer; optimization plasticity remains open. |
| SIS-LIT-102 | Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Specialist Agents | 2026 preprint | `SCF` | `P2/SDR; BGT` | `MI; TD; BT` | `CAUSAL_MECHANISM_EFFECT` | `CL2 candidate` | `I2` / `T2` | Representation-promotion evidence — Recurring semantic control crystallizes into executable code with rollback gates. |
| SIS-LIT-103 | CausalLoss-Fin: Attributing Financial-Agent Loss to Decisions and Infrastructure Faults | 2026 preprint | `P2/SDR` | `—` | `ID; IA; TD` | `PROPAGATION_EFFECT` | `CL2→CL3 candidate` | `I3` / `T0` | Causal-variable coverage evidence — Agent-only causal model necessarily misattributes infrastructure failures. |
| SIS-LIT-104 | How Strongly Should Task State Influence an LLM Agent? | 2026 preprint | `ASR` | `CSCI` | `DR; MEAS` | `ACTION_SELECTION_EFFECT` | `CL2 candidate` | `I2` / `T1` | Influence-policy evidence — Observe/checklist/directive/enforcement effects depend on state correctness and executor obedience. |
| SIS-LIT-105 | ToolCompass: Guiding Tool Trialing, Not Suppressing It | 2026 preprint | `ASR` | `CSCI; BGT` | `DR; BT` | `ACTION_SELECTION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Functional-transfer evidence — Function-based tool representation improves OOD trialing; supports functional rather than domain similarity. |
| SIS-LIT-106 | FIRE: Failure-Informed Runtime Engineering for Reliable Language-Model Agents | 2026 preprint | `ASR` | `P2/SDR` | `DR; ID` | `SELECTIVE_ACTION_UTILITY` | `CL2` | `I2` / `T1` | Reliability-regulation evidence — Randomized controls show runtime policies improve repeated reliability more than capability ceiling. |
| SIS-LIT-107 | Passes Alone, Fails Together: Benchmarking Semantic Coordination in Parallel LLM-Agent Development | 2026 preprint | `P2/SDR` | `SCF; BGT` | `IA; TD; MEAS` | `MECHANISM_INTERACTION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Composition-interference evidence — Independent component success does not guarantee joint success; real prevalence is context-dependent. |
| SIS-LIT-108 | Reasoning as Gradient: Scaling MLE Agents Beyond Tree Search | Findings ACL 2026 (2026.findings-acl.438) | `SCF` | `CSCI; BGT` | `MI; ID; BT` | `CAUSAL_MECHANISM_EFFECT` | `CL2 candidate` | `I2` / `T1` | Regime-transition evidence — Tree-search vs directed diagnostic-gradient optimization crosses over with component capability; strong CSCI fixture. |
| SIS-LIT-109 | BayesFlow: A Probability Inference Framework for Meta-Agent Assisted Workflow Generation | Findings EACL 2026 (2026.findings-eacl.165) | `SCF` | `ASR` | `MI; DR` | `ORGANIZATION_EFFECT` | `CL1` | `I1` / `T1` | Workflow-generation mechanism — Bayesian posterior over workflows; useful framework, not evidence of universal workflow superiority. |
| SIS-LIT-110 | Learning to Evolve: A Self-Improving Framework for Multi-Agent Systems via Textual Parameter Graph Optimization (TPGO) | Findings ACL 2026 (2026.findings-acl.1534; arXiv:2604.20714) | `ASR` | `SCF` | `DR; MI; IA` | `INTERVENTION_LOCUS_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Meta-optimization framework — Textual parameter graph + trace gradients + learned optimization experience; maps to regulation over structured intervention surfaces. |
| SIS-LIT-111 | Learning to Orchestrate Agents in Natural Language with the Conductor | ICLR 2026; arXiv:2512.04388 | `ASR` | `SCF; CSCI` | `DR; IA; BT` | `POLICY_VALUE` | `CL1` | `I1` / `T2` | Coordination-policy evidence — RL-learned communication topology/instructions across worker pools; strong ASR/CSCI implementation evidence. |
| SIS-LIT-112 | Agentic TCAD Calibration Workflow for Oxide Semiconductor Transistors | arXiv:2609.12184 (preprint) | `SCF` | `ASR; BGT` | `MI; ID; BT` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Scientific-domain mechanism — Residuals+sensitivity tests guide bounded parameter/model changes under simulator authority; domain-specific transfer across bias/geometry. |
| SIS-LIT-113 | HIPO: A Hierarchical Prompt Optimization Framework with Task Awareness and Fine-Grained Debugging | Findings ACL 2026 (2026.findings-acl.996) | `ASR` | `CSCI` | `DR; MEAS` | `ACTION_SELECTION_EFFECT` | `CL1` | `I1` / `T1` | Sample-conditioned regulation — Router selects prompt-complexity tier by sample difficulty; supports endogenous granularity/complexity regulation. |

| SIS-LIT-114 | STEVE: Stabilizing Textual Gradient-Based Prompt Optimization via Error-Driven Refinement and Regularized Verification | arXiv:2609.23716 (preprint) | `ASR` | `SCF` | `DR; EG; MI` | `SELECTIVE_ACTION_UTILITY` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Regulation + preservation evidence — Error-only gradients plus regression-gated verification; supports selective update and non-regression rather than unrestricted textual-gradient descent. |
| SIS-LIT-115 | RRSI: Regularized Recursive Self-Improvement of Agent Harnesses | arXiv:2609.24972 (preprint) | `ASR` | `SCF; BGT` | `DR; BT; EG; MI` | `REGULATION_NET_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Boundary/negative evidence — Unregularized recursive harness evolution can overfit evolve tasks; regularized proposal/selection improves OOD retention and efficiency. |
| SIS-LIT-116 | Agensh: Scaling Organizational Intelligence to 1,024 Agents | arXiv:2609.26781 (preprint) | `SCF` | `CSCI` | `IA; MI; MEAS` | `ORGANIZATION_EFFECT` | `CL1` | `I1` / `T1` | Organization/scaling evidence — Decentralized self-organization scales to large worker counts, but agent-count intervention is entangled with compute and task-parallelism; not evidence of a universal agent-count law. |
| SIS-LIT-117 | When Does Execution Provenance Help Agent Memory Retrieval? | arXiv:2609.25913 (preprint) | `SCF` | `—` | `MI; MEAS; ID` | `CAUSAL_MECHANISM_EFFECT` | `CL2 candidate` | `I2` / `T0` | Representation/identification evidence — Source-aligned provenance units and held-candidate graph propagation improve budgeted evidence completion, with controls isolating topology/relation contributions. |
| SIS-LIT-118 | CliffCompaction: Cost-Efficient Compaction for Long-Horizon Coding Agents | arXiv:2609.26779 (preprint) | `SCF` | `CSCI; BGT` | `MI; DR; MEAS; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Efficiency/boundary evidence — Faithful non-rewriting compaction shifts performance–cost frontier across coding agents; supports information-state management as a system mechanism. |
| SIS-LIT-119 | Jev-Mem: System-One-Controlled Agentic Memory for Efficient AI Agents | arXiv:2609.23986 (preprint) | `ASR` | `SCF` | `DR; MI; MEAS` | `POLICY_VALUE` | `CL1` | `I1` / `T1` | Regulation mechanism — Lightweight controller selects routing, retrieval budget, traversal and stopping while reserving generative reasoning for harder cases; useful control-plane fixture. |
| SIS-LIT-120 | Testing-Driven Reliability Audit of Trajectory-Based Early Outcome Prediction for LLM Agents | arXiv:2609.25647 (preprint) | `ROUTING_ABSTAIN` | `BGT` | `MEAS; BT; ID` | `—` | `CL1` | `I1` / `T1` | Measurement-transport boundary evidence — Target-specific calibration transfer failures persist within one benchmark but do not replicate cross-benchmark; best treated as cross-cutting measurement/BGT evidence rather than forced SCF/SDR/ASR routing. |
| SIS-LIT-121 | DolphinBench: Mapping the Pareto Frontier of Agent Memory | arXiv:2609.24971 (preprint) | `SCF` | `BGT` | `MEAS; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL0→CL1` | `I0/I1` / `T1` | Benchmark instrument — Verifies task dependence on history and requires accuracy–cost–latency reporting; strong Tier-2 memory fixture, not mechanism validation by itself. |
| SIS-LIT-122 | Where Does Exactly-Once Live? Model, Harness, and Tool-Contract Effects on Duplicate Side Effects in LLM Agents | arXiv:2609.29095 (preprint) | `P2/SDR` | `CSCI; BGT` | `TD; ID; MEAS; BT` | `RECOVERY_EFFECT` | `CL2 candidate` | `I2` / `T1` | Fault-regime evidence — 25,930 controlled episodes separate model, harness, contract and recovery-condition effects; exactly-once behavior shifts from model-dominated to contract-dominated across fault regimes. |
| SIS-LIT-123 | LLM Agents Can Easily Tamper With Their Own Traces | arXiv:2609.30266 (preprint) | `ROUTING_ABSTAIN` | `—` | `MEAS; ID; EG` | `—` | `CL1` | `I1` / `T1` | Measurement-integrity warning — most tested local-agent harnesses permit trace deletion; execution traces are not automatically trustworthy observations when the acting system controls the logging surface. |
| SIS-LIT-124 | Who Holds the Pen? Let Specifications, Not Agents, Sign Off | arXiv:2609.29921 (preprint) | `SCF` | `ASR` | `MI; MEAS; EG; DR` | `CAUSAL_MECHANISM_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Authority-boundary evidence — independent specification-governed state separates agent proposals/completion claims from admissible evidence and authoritative commitment. |
| SIS-LIT-125 | Breaking the Environment Wall: Evolving LLM Agent Environments for Recursive Self-Improvement | arXiv:2609.29773 (preprint) | `SCF` | `ASR; BGT` | `MI; DR; EG; BT` | `CAUSAL_MECHANISM_EFFECT` | `CL1` | `I1` / `T2` | Environment-representation package evidence — collection maps, event logs, noise detection and environment evolution improve downstream performance across nine models, but bundled mechanisms prevent clean attribution. |
| SIS-LIT-126 | Demystifying Agent Skills for Smart Contract Auditing: Design, Effectiveness, Behavioral Impact | arXiv:2609.29454 (preprint) | `SCF` | `CSCI; BGT` | `MI; TD; MEAS; BT` | `MECHANISM_INTERACTION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T1` | Component–system interaction evidence — 83 skills across seven agent-model configurations show skill benefit is strongly model-dependent and skill triggering is a bottleneck. |
| SIS-LIT-127 | A Wrong Turn Does Not Ruin the Journey: Deviation-Guided Skill Self-Evolution for LLM Agents | arXiv:2609.29154 (preprint) | `ASR` | `SCF; BGT` | `DR; TD; MI; BT` | `INTERVENTION_LOCUS_SELECTION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Localized-repair evidence — deviation-point detection identifies where a useful prefix becomes an erroneous suffix and constrains skill updates to that locus. |
| SIS-LIT-128 | Canopy: Exploiting Piecewise Smooth Tree Priors for Multi-Fidelity Bandits | arXiv:2609.30017 (preprint) | `ASR` | `SCF; BGT` | `DR; MEAS; BT` | `VALUE_OF_INFORMATION` | `CL2 candidate` | `I2` / `T2` | Budgeted-regulation evidence — online bias certificates determine where expensive evaluations are worth spending under matched budgets, with theory and cross-application tests. |
| SIS-LIT-129 | RegenHarness: A Robot Agent Harness with Evidence-Gated Recursive Self-Improvement | arXiv:2609.27612 (preprint; indexed after prior run) | `P2/SDR` | `ASR; BGT` | `TD; DR; MI; EG; BT` | `RECOVERY_EFFECT` | `CL1` | `I1` / `T1` | Embodied history/authority evidence — verified completion, versioned state, bounded recovery and rollback are integrated in a real quadruped deployment; mechanism effects are not isolated. |
| SIS-LIT-130 | Reflection in the Dark: Exposing and Escaping the Black Box in Reflective Prompt Optimization | ACL 2026 SRW; arXiv:2603.18388 (delayed-indexing discovery) | `ASR` | `SCF; BGT` | `DR; MI; ID; BT` | `POLICY_VALUE` | `CL2 candidate` | `I2` / `T1` | Negative/repair evidence — GEPA can degrade under defective seeds while explicit hypothesis search, verification and exploration recover performance under matched budget. |
| SIS-LIT-131 | Gradient-Guided Multi-Judge Prompt Optimization | ACL 2026 Long | `ASR` | `SCF; BGT` | `DR; ID; MEAS; BT` | `ACTION_SELECTION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Attribution/evaluator-governance evidence — first-order segment scoring lowers attribution cost and multi-judge selection reduces single-evaluator dependence across domains/models. |
| SIS-LIT-132 | Serving a Revisable World: Versioned Execution for Interruptible Agents | arXiv:2610.01160 | `SDR` | `ASR; BGT` | `TD; EG; MI; MEAS; BT` | `RECONFIGURATION_TRAJECTORY_EFFECT` | `CL2 candidate` | `I2` / `T1` | Version revocation and certified state inheritance; controlled systems evidence. |
| SIS-LIT-133 | Threat-Preserving Representation Sensitivity in Agent-Security Benchmarks | arXiv:2610.03585 | `ROUTING_ABSTAIN` | `BGT` | `MEAS; ID; BT` | `MEASUREMENT_REPRESENTATION_SENSITIVITY` | `CL2 candidate` | `I2` / `T1` | Measurement representation changes security outcomes without changing underlying threat. |
| SIS-LIT-134 | Sentry: Learning to Recover from LLM Agent Failures at Test Time | arXiv:2610.02994 | `SDR` | `ASR; BGT` | `TD; DR; EG; MEAS; BT` | `RECOVERY_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Conditional failure knowledge exposure and recovery; bundled policy. |
| SIS-LIT-135 | Mistake Notebook Learning: Batch-Clustered Failures for Training-Free Agent Adaptation | Findings ACL 2026; 2026.findings-acl.719 | `ASR` | `SDR; BGT` | `DR; EG; TD; BT` | `POLICY_VALUE` | `CL1` | `I1` / `T2` | Failure-pattern abstraction and validation-gated memory promotion. |
| SIS-LIT-136 | Remember Me, Refine Me: A Dynamic Procedural Memory Framework for Experience-Driven Agent Evolution | Findings ACL 2026; 2026.findings-acl.829 | `ASR` | `SCF; BGT` | `DR; MI; EG; BT` | `POLICY_VALUE` | `CL1` | `I1` / `T2` | Distill-reuse-refine package; no standalone memory primitive. |
| SIS-LIT-137 | Seeing the Whole Elephant: A Benchmark for Failure Attribution in LLM-based Multi-Agent Systems | ACL 2026 Long; 2026.acl-long.912 | `SDR` | `BGT` | `TD; MEAS; ID; BT` | `DIAGNOSTIC_OBSERVABILITY_EFFECT` | `CL1` | `I1` / `T1` | Full-trace attribution measurement; observability not causal propagation. |
| SIS-LIT-138 | SILO-BENCH: A Scalable Environment for Evaluating Distributed Coordination in Multi-Agent LLM Systems | ACL 2026 Long; 2026.acl-long.1354 | `SCF` | `CSCI; BGT` | `IA; MEAS; BT` | `ORGANIZATION_EFFECT` | `CL1` | `I1` / `T1` | Negative/boundary communication-reasoning gap across information silos. |
| SIS-LIT-139 | Identifying Collective Intelligence Factor in LLM Agent Groups for Generalizable Multi-Agent System Design | Findings ACL 2026; 2026.findings-acl.624 | `SCF` | `CSCI; BGT` | `MEAS; IA; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL1` | `I1` / `T2` | Predictive latent group factor; not identified causal mechanism. |
| SIS-LIT-140 | Towards Self-Improving Error Diagnosis in Multi-Agent Systems | Findings ACL 2026; 2026.findings-acl.98 | `SDR` | `ASR; BGT` | `TD; ID; EG; MEAS; BT` | `PROPAGATION_EFFECT` | `CL1` | `I1` / `T2` | Tool-grounded ErrorProbe diagnostic evidence; no isolated causal intervention. |
| SIS-LIT-141 | Beyond Corrected Memory: Execution Consistency in Multi-Agent Systems | arXiv:2610.08101 | `SDR` | `ASR; BGT` | `TD; EG; MEAS; ID; BT` | `EXECUTION_CONSISTENCY_IDENTIFIABILITY` | `CL1→CL2 candidate` | `I2` / `T1` | Evidence-removal/restoration contrasts show correct records can hide duty violations. |
| SIS-LIT-142 | CheckerBench: Can Long-Horizon Agents Synthesize Static-Analysis Checkers? | arXiv:2610.07557 | `SCF` | `CSCI; BGT` | `MEAS; MI; BT` | `CAPABILITY_FRONTIER_SHIFT` | `CL1` | `I1` / `T1` | Independent executable verifier benchmark, 300 tasks and repeated model-harness trials. |
| SIS-LIT-143 | DAEDALUS: Bootstrapping Agent Memory from Self-Generated Tasks | arXiv:2610.08048 | `ASR` | `SCF; BGT` | `DR; EG; MI; BT` | `POLICY_VALUE` | `CL1→CL2 candidate` | `I1/I2` / `T2` | Self-generated practice and heuristic qualification; package effect. |
| SIS-LIT-144 | EIO-Agents: The Missing Semantic Layer for AI Agent Evaluation | arXiv:2610.07675 | `ROUTING_ABSTAIN` | `BGT` | `EG; MEAS; ID` | `EVALUATION_SEMANTIC_CONTRACT` | `CL0` | `I0` / `T0` | Semantic evaluation specification; implementation-only until independently tested. |
| SIS-LIT-145 | OOPMAS: Object-Oriented Multi-Agent Systems for Query-Level Workflow Generation | arXiv:2610.07787 | `ASR` | `SCF; BGT` | `DR; MI; BT` | `POLICY_VALUE` | `CL1` | `I1` / `T1` | Query-level workflow package; granularity mechanism not isolated. |
---

## 4. High-pressure evidence set for SIS theory

The following items are not simply high-performing systems; they exert unusually strong pressure on SIS scientific assumptions or benchmark design:

- **Flag Game** — local attribution/intervention efficacy changes with population scale; motivates intervention-scope transition experiments.
- **CausalLoss-Fin** — causal attribution is upper-bounded by causal-variable coverage; infrastructure causes cannot be found if the causal universe excludes them.
- **ARCHITECT** — controlled intervention links causal attribution to targeted repair utility.
- **How Strongly Should Task State Influence an LLM Agent?** — separates state correctness from optimal influence strength; stronger enforcement can harm when state/matcher quality is wrong.
- **FIRE** — randomized controls separate reachable capability from repeated delivery reliability.
- **Prompt Optimization Is a Coin Flip** — optimization eligibility/headroom is itself a regulation variable.
- **Reasoning as Gradient** — system optimization regime exhibits a component-capability crossover, directly motivating CSCI.
- **MA-Evolve** — iso-compute negative evidence against assuming multi-agent structure is inherently better.
- **When Agents Slow Down** — regulation should be studied over performance–compute trajectories rather than endpoint score alone.
- **TraceElephant** — diagnosis depends on observability conditions; missing trace channels can change attribution.

---

## 5. Registry-level scientific conclusions

### 5.1 No SIS Core expansion is justified

The reviewed corpus is naturally expressible through `SCF`, `SDR`, `ASR`, `CSCI`, and `BGT`. Concepts that previously appeared as ARSO schema candidates—such as replayable experience, influence policy, representation promotion, diagnostic convergence, intervention readiness, mechanism promotion, or specification-conditioned evidence generation—should remain **framework/experiment constructs** unless future evidence shows that they define a new first-principles estimand that cannot be represented by current SIS semantics.

### 5.2 ASR is the highest-density near-term opportunity

The corpus repeatedly studies endogenous action choice under information: `NO_CHANGE`, probe, verification, retry, escalation, reconfiguration, intervention, memory use, routing, budget allocation, and stop/restart decisions. This provides a dense evidence base for a dedicated SIS ASR experimental program.

### 5.3 CSCI subsumes the core EI-SMCT question

Studies such as NPO, Reasoning as Gradient, The Router Within, Co-Evolving Harnesses and Models, Memory Portability, MA-Evolve, ToolCompass, and ScienceBuddy motivate an explicit effect-modification program:

```math
Effect(M)=f(ComponentCapability)
```

EI-SMCT should therefore be maintained as a **CSCI research line**, not as a parallel mother theory.

### 5.4 Transportability is the major evidence deficit

Many papers show multi-model or cross-task performance transfer (`T1/T2`), but the registry currently contains **no T3 causal-transportability or T4 mechanism-invariance evidence**. SIS should treat source→target causal preservation as an open scientific problem rather than an established advantage.

### 5.5 Thin, replaceable Framework semantics are validated by coverage

The eight SIS Framework Capability Profile dimensions are sufficient to operationally describe the reviewed corpus without creating new program identities for memory, harnesses, replay, prompt optimization, workflow optimization, or multi-agent systems.

---

## 6. Benchmark / experiment backlog derived from the registry

1. **Regime Transition Fixtures** — test search vs directed-gradient vs structured intervention across component-capability regimes.
2. **Intervention-Scope Transition Fixtures** — local → component-set → subgraph → system-level repair as interaction density/scale changes.
3. **Screen → Replay → Execute Fixtures** — cheap attribution screening → counterfactual verification → real intervention under matched budget.
4. **Influence Regulation Fixtures** — ignore / observe / advise / direct / enforce as a function of state reliability, executor obedience, risk, and decision criticality.
5. **Representation Externalization Fixtures** — text → schema → executable control under both stable and shifted environments; measure reliability–plasticity trade-off.
6. **Recursive Adaptation / Plasticity Fixtures** — determine whether an accepted optimization improves or harms the system's future ability to adapt.
7. **Causal-Variable Coverage Fixtures** — test attribution when the true cause lies in agent, tool, memory, workflow, environment, infrastructure, or contract layers.
8. **Transportability Fixtures** — explicitly distinguish replication, performance transfer, causal transportability, and mechanism invariance.

---

## 7. Maintenance protocol

Every new study added to this registry should receive:

```text
SIS-LIT ID
bibliographic/source status
PrimaryProgram
CrossCuttingProgram(s)
FrameworkCapabilityProfile
PrimaryEstimand
ClaimMaturity
IdentificationTier
TransportTier
EvidenceRole
BoundaryVariables
SISImpact
```

Maintenance rules:

1. **Primary estimand determines Primary Program.** Keywords such as agent, memory, workflow, RAG, replay, prompt, or harness never determine program identity.
2. **One identified claim has one Primary Program.** A framework may support multiple capabilities, but a scientific claim must be routed by its estimand.
3. **Do not inflate claim maturity because a framework is sophisticated or high-performing.**
4. **Performance transfer is not causal transportability.** Cross-model reuse is normally `T2` at most unless an intervention relation is shown to transport.
5. **Negative results are first-class evidence.** Equal-compute null results, degradation, interference, failed local repairs, and over-/under-influence findings should remain in the registry.
6. **Community/industry analyses remain discovery or engineering evidence unless independent scientific validation is available.**
7. **New ontology/schema additions require evidence of a missing scientific estimand, not merely a newly named implementation mechanism.**

---

## 8. Provenance and verification note

This v1.0 registry re-codes the corpus already reviewed in the ARSO research-brief stream. The primary-source factual review for most entries was performed during those briefs. During registry construction, the following delayed-indexing / synthesis-referenced items were explicitly re-verified against primary sources: **Reasoning as Gradient**, **BayesFlow**, **TPGO**, **Learning to Orchestrate Agents in Natural Language with the Conductor**, **Agentic TCAD Calibration Workflow for Oxide Semiconductor Transistors**, and **HIPO**.

The `Claim`, `I*`, `T*`, `Evidence role`, and `SIS interpretation` fields are **SIS v0.3.1 re-codings**, not claims made by the paper authors.

---

### 8.1 Daily increment — 2026-09-24

Registry v1.1 adds SIS-LIT-114–121 from the 2026-09-24 daily intelligence run. One item (SIS-LIT-120) is deliberately coded as `ROUTING_ABSTAIN`: its primary scientific contribution is calibration-transfer auditing of a measurement instrument, not a direct SCF/SDR/ASR estimand. This is an application of SIS routing-abstention semantics, not a new Primary Program.

The daily increment does **not** change SIS v0.3.1 Core. It strengthens three evidence gaps: recursive-improvement generalization, measurement-transfer calibration, and performance–cost frontier measurement.

### 8.2 Daily increment — 2026-09-26

Registry v1.2 adds SIS-LIT-122–131. Eight records are new/recent primary-source items from the post-2026-09-24 window or indexing delay; two ACL 2026 papers (VISTA and GMPO) are delayed-indexing discoveries added because they materially strengthen SIS evidence around optimizer failure, diagnostic search, evaluator independence and budgeted optimization.

This increment also sharpens a measurement-governance distinction: execution traces and completion claims are not automatically authoritative observations. Trace integrity and authority boundaries must be independently governed when the acting system can alter its own evidence surface.

No record in this increment establishes T3 causal transportability or T4 mechanism invariance.

### 8.3 Daily reconciliation — 2026-10-08

Registry v1.3 reconciles SIS-LIT-132–137 from the 2026-10-06 daily update and qualifies SIS-LIT-138–145 from 2026-10-08. Paper-level CL labels remain provisional until P0 claim-level audit; no T3/T4. See the 2026-10-08 daily update for primary source links and boundaries.

## 9. Version decision

**Registry conclusion:** the current corpus supports continued use of SIS v0.3.1 without a Scientific Core revision. The immediate priority is to expand benchmark fixtures, causal identification, component-capability interaction experiments, and transportability tests rather than to create additional first-principles objects or Programs.

```math
SIS\ v0.3.1\ Core\Delta = 0
```

```math
Benchmark\ /\ Experiment\ Portfolio\Delta > 0
```

## 10｜2026-10-24 source-verified provisional candidates (NOT permanent SIS-LIT IDs)

**Scope:** 10 preprints newly discovered from the 2026-10-23 arXiv listing (originally submitted 2026-10-21/22 UTC); these are version/lineage candidates awaiting reconciliation with the unmerged 2026-10-09–23 daily batches. **Canonical count stays 145** pending permanent-ID adjudication. Paper-level columns are discovery metadata; any claim-level labels are provisional and **not** final Gold. Detailed evidence and limits: [daily update](updates/2026-10-24_SIS_Daily_Literature_Update.md).

| Temp ID | Study / primary source | Primary | Cross-cutting | Capability Profile | Primary estimand | Claim-level ceiling / I/T | Evidence role |
|---|---|---|---|---|---|---|---|
| SIS-CAND-20261024-01 | [ARATest](https://arxiv.org/abs/2610.30495) | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | CLAIM_PROPERTY_EXECUTION_VALIDITY | CL1; I1/T0 | measurement |
| SIS-CAND-20261024-02 | [ARC-AGI-3 controlled harness self-improvement](https://arxiv.org/abs/2610.30499) | SCF | CSCI/BGT | MI/TD/ID/MEAS/BT | HELDOUT_HARNESS_REVISION_VALUE | CL1; I1/T1 | negative/boundary |
| SIS-CAND-20261024-03 | [RoleFlow (SECPO)](https://arxiv.org/abs/2610.30429) | ASR | CSCI/BGT | DR/IA/ID/MI/MEAS/BT | SINGLE_EDIT_STRUCTURAL_REGULATION_VALUE | CL1; local CL2 candidate; I2/T2-performance | local intervention |
| SIS-CAND-20261024-04 | [BELT](https://arxiv.org/abs/2610.30450) | ASR | BGT | DR/ID/MEAS/BT | PRICE_CONDITIONAL_TERMINATION_POLICY_VALUE | CL1; I1/T2-performance | regulation/boundary |
| SIS-CAND-20261024-05 | [MemPABench](https://arxiv.org/abs/2610.30485) | ROUTING_ABSTAIN | BGT | EG/DR/MEAS/BT | PREFERENCE_CONDITIONAL_ACTION_VALIDITY | CL1; I1/T0 | negative/measurement |
| SIS-CAND-20261024-06 | [Multi-Actor Event Worlds](https://arxiv.org/abs/2610.30488) | SDR | CSCI/BGT | TD/ID/MEAS/BT | OTHER_ACTOR_UNOBSERVABILITY_EFFECT | CL1; I1/T1 | negative/boundary |
| SIS-CAND-20261024-07 | [What the Trace Shows and What the Label Says](https://arxiv.org/abs/2610.30491) | ROUTING_ABSTAIN | BGT | TD/ID/MEAS/EG/BT | TRACE_LABEL_CONSTRUCT_VALIDITY | CL1; I1/T0 | measurement/null |
| SIS-CAND-20261024-08 | [AgentTriage](https://arxiv.org/abs/2610.30738) | ROUTING_ABSTAIN | BGT | TD/ID/EG/MEAS/BT | REPLAYABLE_GROUNDED_DIAGNOSIS_VALIDITY | CL1; I1/T1 | measurement/instrument |
| SIS-CAND-20261024-09 | [Externalise the Memory](https://arxiv.org/abs/2610.30478) | SCF | CSCI/BGT | MI/EG/MEAS/BT | EXTERNAL_RETRIEVAL_VS_WEIGHT_DISTILLATION_EFFECT | CL1; local CL2 candidate; I2/T0 | negative/boundary |
| SIS-CAND-20261024-10 | [Feedback That Backfires in Games](https://arxiv.org/abs/2610.30205) | SDR | CSCI/BGT | TD/ID/EG/MEAS/BT | FAILED_ACTION_REEXPOSURE_EFFECT | CL1; local CL2 candidate; I2/T1 | negative/boundary |

**Non-inflation:** no CL3 or T3/T4; not an SIS v0.3.1 core revision. Existing permanent IDs and prior final audit outcomes remain unchanged. First-coder P0 re-audit is in [2026-10-24 audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-24.md).

## 11｜2026-10-25 source-verified provisional candidates (NOT permanent SIS-LIT IDs)

**Scope:** 10 arXiv studies screened against 145 permanent records and the 2026-10-24 provisional section. Friday 2026-10-23 source listing; **2026-10-25 is audit date, not a publication date**. Previous 2026-10-09–23 staged files still await batch lineage reconciliation; do not increment canonical count 145 or reuse their potential permanent IDs. Primary-source abstracts support first-pass screen; **CL2 candidate ≠ final CL2**, no automatic CL3/T3/T4.

Detailed [daily evidence note](updates/2026-10-25_SIS_Daily_Literature_Update.md) and [three-study re-audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-25.md).

| Temp ID | Primary source | Program | Cross-cutting | Capability | Primary estimand | Claim ceiling / I/T | Evidence role |
|---|---|---|---|---|---|---|---|
| SIS-CAND-20261025-01 | [EpiSEM-Bench: Evaluating Safety and Evidence Recovery in LLM Agents under Missing Evidence](https://arxiv.org/abs/2610.31650) | SDR | BGT | TD/ID/MEAS/EG/BT | `CRITICAL_EVIDENCE_OMISSION_FAILURE_EFFECT` | CL1; local CL2 candidate; I2(local)/T1 | MEASUREMENT_NEGATIVE |
| SIS-CAND-20261025-02 | [Post-Audit Mirage: Identifiability Limits of Offline Agent Verification](https://arxiv.org/abs/2610.31130) | ROUTING_ABSTAIN | BGT | ID/MEAS/EG/BT | `OFFLINE_VERIFIER_IDENTIFIABILITY_BOUND` | CL0 theoretical; CL1 empirical; I0/I1/T0 | IDENTIFICATION_LIMIT |
| SIS-CAND-20261025-03 | [Simulated Control Evals](https://arxiv.org/abs/2610.31593) | ROUTING_ABSTAIN | BGT | MEAS/ID/BT/EG | `SIMULATED_CONTROL_EVAL_PREDICTIVE_VALIDITY` | CL1; I1/T2 performance only | MEASUREMENT_INSTRUMENT |
| SIS-CAND-20261025-04 | [RIDAR: Safeguarding Research Integrity in Autonomous Research Agents](https://arxiv.org/abs/2610.31372) | ASR | BGT | DR/TD/EG/ID/MEAS/BT | `RUNTIME_RESEARCH_INTEGRITY_REGULATION_EFFECT` | CL1; local intervention candidate pending full audit; I1/I2(local)/T0 | INTEGRITY_MEASUREMENT_INTERVENTION |
| SIS-CAND-20261025-05 | [Conservative Meta-Agent Search: Architecture Adaptation under Non-Stationarity](https://arxiv.org/abs/2610.31436) | ASR | CSCI/BGT | DR/IA/ID/MEAS/BT | `SHADOW_REPLAY_ARCHITECTURE_PROMOTION_NET_VALUE` | CL1; local CL2 candidate; I2(local)/T0 | REGULATION_BOUNDARY |
| SIS-CAND-20261025-06 | [Certified Execution Harness for Agentic AI](https://arxiv.org/abs/2610.31376) | ASR | BGT | DR/MI/EG/ID/MEAS/BT | `SAFE_SUPERVISOR_LEAST_INTRUSIVE_POLICY_VALUE` | CL0 formal; CL1 example; I0/I1/T0 | FORMAL_BOUNDARY |
| SIS-CAND-20261025-07 | [ADAPT for Science: A Multi-Agent System for Self-Evolving Scientific Optimization](https://arxiv.org/abs/2610.30851) | ASR | CSCI/BGT | DR/MI/MEAS/BT | `CONSTRAINED_SCIENTIFIC_SEARCH_POLICY_VALUE` | CL1; I1/T2 performance only | IMPLEMENTATION_BOUNDARY |
| SIS-CAND-20261025-08 | [LLM Multi-Agent Systems Are Vulnerable to Herding and Runaway Cascades](https://arxiv.org/abs/2610.30769) | SDR | CSCI/BGT | TD/IA/ID/MEAS/BT | `CUMULATIVE_SOCIAL_SIGNAL_CASCADE_EFFECT` | CL1; local CL2 candidate; I2(local)/T1 | NEGATIVE_BOUNDARY |
| SIS-CAND-20261025-09 | [SCOPE: Compiling Natural-Language Policies into Neurosymbolic Predicate Programs](https://arxiv.org/abs/2610.31062) | SCF | BGT | MI/EG/ID/MEAS/BT | `NEUROSYMBOLIC_POLICY_COMPILATION_EFFECT` | CL1; I1/T2 performance only | FRAMEWORK_IMPLEMENTATION |
| SIS-CAND-20261025-10 | [Adaptive Skill Granularity for Coding Agents](https://arxiv.org/abs/2610.31461) | ASR | BGT | DR/TD/MI/ID/MEAS/BT | `ACTION_GRANULARITY_ROUTING_RECOVERY_VALUE` | CL1; controlled recovery candidate pending full audit; I1/I2(local)/T0 | RECOVERY_BOUNDARY |

**Non-inflation:** Scientific Core remains frozen; per-paper screening cannot settle causal or mechanistic claim level. Older pending batches unchanged.


---

## 2026-10-26 daily provisional candidates (not part of 145 permanent-ID corpus)

Source window: latest Friday arXiv list (2026-10-23; first submissions Oct 19–21) plus October 2026 archival EMNLP Findings delayed discoveries. The nine items below remain **provisional**, pending retrospective 2026-10-09–23 candidate de-duplication and preprint→proceedings lineage audit. Claim levels are first-pass *claim-specific ceilings*, not whole-paper final levels.

| SIS-CAND-20261026-01 | [TRACE: A Traceable Agentic Co-Optimizer for Experimental Optimization](https://aclanthology.org/2026.findings-emnlp.295/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | ASR | BGT | DR/EG/MEAS/ID/BT | `BO_CONSTRAINED_INTERVENTION_POLICY_VALUE` | CL1 | I1/T0 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-02 | [BID-SPO: Rethinking Multi-Agent Prompt Optimization as Information Contracting via Bidding-based Shapley Values](https://aclanthology.org/2026.findings-emnlp.239/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | SCF | CSCI/BGT | MI/IA/ID/MEAS/BT | `INTER_AGENT_INTERFACE_CONTRACT_ALIGNMENT_EFFECT` | CL1 | I1/T1 | INTERACTION_BOUNDARY |
| SIS-CAND-20261026-03 | [PaperScout: An Autonomous Agent for Academic Paper Search with Process-Aware Sequence-Level Policy Optimization](https://aclanthology.org/2026.findings-emnlp.1743/) | Findings EMNLP 2026, Oct (archival; delayed discovery) | ASR | BGT | DR/TD/MEAS/ID/BT | `SEQUENCE_LEVEL_SEARCH_POLICY_VALUE` | CL1 | I1/T1 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-04 | [How Much Does the Harness Matter, and for Whom? A Multi-Model Study of Context in LLM-Driven Vulnerability Discovery](https://arxiv.org/abs/2610.28802) | arXiv v1 2026-10-20; delayed discovery | SCF | CSCI/BGT | MI/IA/ID/MEAS/BT | `MODEL_BY_PROMPT_CONTEXT_INTERACTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | CSCI_BOUNDARY |
| SIS-CAND-20261026-05 | [SpecMAGIC: Specification-Guided Multi-Task Generalization in Multi-Agent Reinforcement Learning](https://arxiv.org/abs/2610.30443) | arXiv v1 2026-10-21; delayed discovery | SCF | BGT | MI/IA/EG/MEAS/BT | `TEMPORAL_SPEC_COMPOSITION_ZERO_SHOT_VALUE` | CL0 formal; CL1 empirical | I0/I1/T1 | FORMAL_BOUNDARY_FRAMEWORK |
| SIS-CAND-20261026-06 | [Soft Ontology Priors over Latent Concept Posteriors for Weakly Supervised Neuro-Symbolic Learning](https://arxiv.org/abs/2610.30391) | arXiv v1 2026-10-21; author marks NeSy 2026 oral, archival verification pending | SCF | BGT | MI/EG/ID/MEAS/BT | `ONTOLOGY_PRIOR_LATENT_CONCEPT_RECOVERY_EFFECT` | CL0 theoretical; CL1 empirical; local CL2 candidate | I1/I2-local/T0 | IDENTIFICATION_BOUNDARY |
| SIS-CAND-20261026-07 | [Route-and-Generate: KL-Regularized Router Improvement for Reasoning Routing in LLMs](https://arxiv.org/abs/2610.30351) | arXiv v1 2026-10-21; delayed discovery | ASR | BGT | DR/MEAS/MI/BT | `REASONING_FORMAT_ROUTING_COST_ADJUSTED_VALUE` | CL1 | I1/T1 | REGULATION_IMPLEMENTATION |
| SIS-CAND-20261026-08 | [Learning Who Talks to Whom: Role-Aware Communication Topology Scheduling for Efficient LLM Multi-Agent Collaboration](https://arxiv.org/abs/2610.25851) | arXiv v1 2026-10-19; delayed discovery | ASR | CSCI/BGT | DR/IA/ID/MEAS/BT | `ROLE_TOPOLOGY_CONDITIONAL_COMMUNICATION_VALUE` | CL1; local CL2 candidate | I1/I2-local/T1 | INTERACTION_BOUNDARY |
| SIS-CAND-20261026-09 | [Policy Search in Code Space for Multi-Agent Pathfinding](https://arxiv.org/abs/2610.25946) | arXiv v1 2026-10-19; delayed discovery | ASR | BGT | DR/MI/EG/MEAS/BT | `VERIFIED_CODE_POLICY_SEARCH_VALUE` | CL0 formal; CL1 empirical | I1/T2 performance only | REGULATION_IMPLEMENTATION |

- [Daily evidence notes](updates/2026-10-26_SIS_Daily_Literature_Update.md) contain full provenance, boundary and classification detail.
- [P0 audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-26.md) contains 9 distinct claim decisions for SIS-LIT-033/034/038. Permanent corpus totals and pre-existing final labels **unchanged**; second coder pending.

---

## 2026-10-27 daily provisional candidates (NOT permanent SIS-LIT IDs)

**Window:** arXiv cs.AI 2026-10-26 announcement (79 new of 321 total listings), studies initially submitted 2026-10-22 or 2026-10-23 UTC; none first submitted 2026-10-27. Cross-check with 145 permanent Registry IDs and provisional Oct 24–26 (29 items), older Oct 9–23 bundles not exhaustively available. No confirmed independent peer-reviewed study in selected fresh batch; one author-described nonarchival workshop poster is categorized as preprint. No independent community replication. Detailed [daily source update](updates/2026-10-27_SIS_Daily_Literature_Update.md) and [P0 re-audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-27.md).

| Temporary ID | Primary paper / version | Primary | Cross-cutting | Framework | Claim-level primary estimand | First-coder claim ceiling | I / T | Evidence role |

|---|---|---|---|---|---|---|---|---|

| SIS-CAND-20261027-01 | [SWE-Shift: Evaluating Coding Agents in Evolving Workspaces](https://arxiv.org/abs/2610.32196), arXiv v1 2026-10-23 | SDR | BGT | TD/ID/MEAS/EG/BT | `MID_EXECUTION_CHANGE_RECOVERY_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | CONTROLLED_BOUNDARY_NEGATIVE |

| SIS-CAND-20261027-02 | [The Helpful Agent Problem: When Emergent Cooperation Among LLM Agents Bypasses Intended Workflows](https://arxiv.org/abs/2610.31985), arXiv v1 2026-10-22 | SDR | CSCI/BGT | TD/IA/EG/ID/MEAS/BT | `BENIGN_CROSS_OWNER_COOPERATION_OVERSIGHT_BYPASS_EFFECT` | CL1; local intervention candidate | I1/I2-local/T0 | NEGATIVE_BOUNDARY |

| SIS-CAND-20261027-03 | [Permission to Retry: A Study of Authorization and Recovery in AI Agent Workflows](https://arxiv.org/abs/2610.31916), arXiv v1 2026-10-22 | SDR | BGT | TD/DR/EG/ID/MEAS/BT | `AUTHORITY_CONDITIONAL_RETRY_RECOVERY_CONFORMANCE` | CL1; local CL2 candidate | I2-local/T0 | CONTROLLED_RECOVERY_BOUNDARY |

| SIS-CAND-20261027-04 | [Not All Information Is Worth Asking For: Decision-Informed Information Seeking with LLMs](https://arxiv.org/abs/2610.32181), arXiv v1 2026-10-23 | ASR | BGT | DR/ID/MEAS/EG/BT | `DECISION_CONDITIONAL_VALUE_OF_INFORMATION_NET_REGRET` | CL1; local controlled comparison | I1/I2-local/T1 | REGULATION_MEASUREMENT |

| SIS-CAND-20261027-05 | [Async-RBench: Benchmarking Asynchronous Task Execution in LLM Agents](https://arxiv.org/abs/2610.32429), arXiv v1 2026-10-23 | SDR | BGT | TD/DR/ID/MEAS/BT | `ASYNCHRONOUS_EVENT_RESPONSE_CONFORMANCE_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | DYNAMIC_MEASUREMENT_NEGATIVE |

| SIS-CAND-20261027-06 | [Don't Forget What You Just Learned: Self-Directed Repair Turns Agent Mistakes Into Lasting Lessons](https://arxiv.org/abs/2610.31846), arXiv v1 2026-10-22 | SCF | CSCI/BGT | MI/DR/EG/MEAS/BT | `PERSISTENT_LOCAL_ADAPTER_REPAIR_RETENTION_EFFECT` | CL1; mechanism not independently identified | I1/T2-performance-only | CAPABILITY_RETENTION_IMPLEMENTATION |

| SIS-CAND-20261027-07 | [Beyond On-Policy vs. Off-Policy: At What Level Should LLM Agent Distillation Follow the Student?](https://arxiv.org/abs/2610.31918), arXiv v1 2026-10-22 | SCF | CSCI/BGT | MI/TD/ID/MEAS/BT | `HISTORY_POLICY_BY_ACTION_PREFIX_SOURCE_INTERACTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | TRAINING_MECHANISM_INTERACTION |

| SIS-CAND-20261027-08 | [Do AI-for-Science Agents Preserve Model Safety?](https://arxiv.org/abs/2610.32045), arXiv v1 2026-10-23 | SCF | CSCI/BGT | IA/EG/ID/MEAS/BT | `SCIENCE_HARNESS_BY_MODEL_SAFETY_RETENTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | NEGATIVE_SAFETY_BOUNDARY |

| SIS-CAND-20261027-09 | [CEMIR vs. FISER: a comparative study of reasoning-based and enrichment-based approaches to pragmatic intent recognition](https://arxiv.org/abs/2610.32022), arXiv v1 2026-10-23 | SCF | CSCI/BGT | MI/ID/MEAS/BT | `SYNTHETIC_MULTIMODAL_ENRICHMENT_INCREMENTAL_INTENT_VALUE` | CL1 conditional null | I2-local/T1 | NEGATIVE_BOUNDARY |

| SIS-CAND-20261027-10 | [Who Verifies the Tools? How Warped Formatters Mislead Agents and Their Verifiers](https://arxiv.org/abs/2610.32110), arXiv v1 2026-10-23 | ROUTING_ABSTAIN | BGT | MI/EG/ID/MEAS/BT | `TOOL_FORMATTER_OMISSION_EVALUATOR_CONSTRUCT_EFFECT` | CL1; local CL2 candidate | I2-local/T0 | MEASUREMENT_INSTRUMENT_BOUNDARY |

**Evidence status:** Provisional; no CL3, T3 or T4 admitted. The old 2026-10-09–23 unmerged candidate corpus has not been exhaustively reconciled. Prevent permanent-ID collision; do not alter final Gold without second coder/adjudication.


---

## 2026-10-28 daily provisional candidates (NOT permanent SIS-LIT IDs)

**Window:** official arXiv cs.AI 2026-10-27 announcement (172 new / 711 total including cross-lists and replacements), initial arXiv submissions Oct 12/23/24/25; two verified EMNLP archival identities; NeurIPS author-declared acceptance remains preprint. Cross-check against 145 permanent IDs and 39 synced Oct 24–27 provisional studies, unsynced Oct 9–23 not globally reconciled.

| Temporary ID | Primary paper/version | Primary | Cross-cutting | Framework | Primary estimand | First-coder ceiling | I/T | Evidence role |
|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261028-01 | [SkillShift-Bench: Benchmarking Skill Learning under Environment Evolution for Web Agents](https://aclanthology.org/2026.emnlp-main.1952/), EMNLP 2026 Main, ACL Anthology 2026.emnlp-main.1952, 2026-10-24 | SDR | BGT | TD/DR/MI/MEAS/ID/BT | `SHIFT_CONDITIONAL_SKILL_EXECUTABILITY_AND_RECOVERY` | CL1; local CL2 candidate | I2-local/T1 | CONTROLLED_DYNAMIC_BOUNDARY |
| SIS-CAND-20261028-02 | [Scoped Semantic Invariance as a Foundation for LLM Reliability](https://aclanthology.org/2026.emnlp-main.2545/), EMNLP 2026 Main, ACL Anthology 2026.emnlp-main.2545, 2026-10-23 | SCF | BGT | MI/EG/MEAS/ID/BT | `SCOPED_SEMANTIC_INVARIANCE_GROUNDING_EFFECT` | CL0 formal + CL1 empiric; local CL2 candidate | I1/I2-local/T2-performance | MEASUREMENT_CONSTRUCT_NEGATIVE_BOUNDARY |
| SIS-CAND-20261028-03 | [Task Success Is Not Enough: Side-effect-Aware Evaluation of Tool-Using Language Model Agents (SABench)](https://arxiv.org/abs/2610.34167), arXiv v1; author states NeurIPS 2026 Evaluations and Datasets Track accepted, final proceedings not verified, 2026-10-25 | SDR | BGT | TD/EG/ID/MEAS/BT | `GOAL_SUCCESS_CONDITIONAL_UNAUTHORIZED_SIDE_EFFECT_RISK` | CL1; paired oracle measurement | I1/T1 | NEGATIVE_CONSTRAINT_MEASUREMENT |
| SIS-CAND-20261028-04 | [AOS-Bench: Can LLM Agents Manage Dynamic Workloads?](https://arxiv.org/abs/2610.33178), arXiv v1 preprint, 2026-10-23 | SDR | CSCI/BGT | TD/DR/IA/MEAS/ID/BT | `DYNAMIC_WORKLOAD_DELIVERY_RETENTION_UNDER_RESOURCE_CONSTRAINT` | CL1; local CL2 candidate | I2-local/T1 | DYNAMIC_SYSTEM_CAPABILITY_BOUNDARY_NEGATIVE |
| SIS-CAND-20261028-05 | [Lessons from Luck: Do LLM-Written Lessons Carry Chance into an Agent's Next Decision?](https://arxiv.org/abs/2610.33029), arXiv v1 preprint; cross-listed to cs.AI in 2026-10-27 listing (delayed discovery), 2026-10-12 | SDR | BGT | TD/EG/ID/MEAS/BT | `STOCHASTIC_OUTCOME_CONTAMINATION_OF_PERSISTED_LESSON_EFFECT` | CL1; local preregistered CL2 candidate | I2-local/T1 | REGISTERED_NEGATIVE_MECHANISM_BOUNDARY |
| SIS-CAND-20261028-06 | [Can LLMs Trust Appropriately? Evaluating Calibrated Reliance on Imperfect Partners](https://arxiv.org/abs/2610.34107), arXiv v1 preprint, 2026-10-25 | ASR | CSCI/BGT | DR/IA/ID/MEAS/BT | `EVIDENCE_CONDITIONAL_PARTNER_RELIANCE_POLICY_NET_VALUE` | CL1; local controlled-policy candidate | I2-local/T0 | REGULATION_MEASUREMENT_NEGATIVE |
| SIS-CAND-20261028-07 | [Estimation of Propagated Risk in LLM-based Multi-Agent Systems (IE-Prop)](https://arxiv.org/abs/2610.33282), arXiv v1 preprint, 2026-10-23 | SDR | CSCI/BGT | TD/IA/ID/MEAS/BT | `INTERACTION_CONDITIONED_ERROR_RISK_PREDICTION_INCREMENT` | CL1 (predictive, not causal) | I1/T1 | DYNAMIC_RISK_MEASUREMENT_IMPLEMENTATION |
| SIS-CAND-20261028-08 | [AdaPRA: Process Reward Agents with Adaptive Rubrics for Data Science](https://arxiv.org/abs/2610.33245), arXiv v1 preprint, 2026-10-23 | ASR | CSCI/BGT | DR/EG/MEAS/ID/BT | `TASK_ADAPTIVE_RUBRIC_PROCESS_REGULATION_NET_VALUE` | CL1; local ablation candidate | I1/T2-performance | REGULATION_IMPLEMENTATION_AND_EVIDENCE_GOVERNANCE |
| SIS-CAND-20261028-09 | [Optimal Correction Sets for Provable Redress of Contestable Causal Discovery](https://arxiv.org/abs/2610.33138), arXiv v1 preprint, 2026-10-23 | ROUTING_ABSTAIN | BGT | ID/EG/MEAS/BT | `MINIMUM_COST_CONTESTABLE_CAUSAL_FACT_REPAIR_CONFORMANCE` | CL0 formal + CL1 benchmark | I0/I1/T0 | FORMAL_IDENTIFICATION_BOUNDARY |
| SIS-CAND-20261028-10 | [Distilling Expert Judgment at Scale](https://arxiv.org/abs/2610.33233), arXiv v1 preprint, 2026-10-23 | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | `EXPERT_CALIBRATED_AUTOMATED_EVALUATOR_CONSTRUCT_VALIDITY` | CL1; evaluator agreement | I1/T0 | EXPERT_GOLD_MEASUREMENT_INSTRUMENT |

- [Daily note](updates/2026-10-28_SIS_Daily_Literature_Update.md) carries author results, boundaries, evidence roles and source/version links.
- [P0 audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-28.md) splits 014/026/027 into nine ClaimRecords. All second-coder/adjudication fields remain PENDING; no inherited whole-paper CL2/CL3, no new T3/T4.


## 19｜2026-10-29 source-verified provisional candidate update (NOT permanent SIS-LIT IDs)

**Scope:** 10 arXiv preprints found in 2026-10-28 listing including cross-lists (first submitted Oct 23/26/27); source IDs and names checked against 145 permanent studies and 49 synced Oct 24–28 candidates. **Canonical permanent count remains 145.** Earlier Oct 9–23 unsynced batches require a full reconciliation before assigning permanent IDs. No new CL2/CL3 finalized or T3/T4.

| Temporary ID | Primary source / version | Primary | Cross | Framework | Estimand | Provisional claim ceiling | I/T | Evidence role |
|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261029-01 | [Blindfold: Keeping the Audit Coin Secret from LLM Agents](https://arxiv.org/abs/2610.37055), v1 2026-10-27 | ROUTING_ABSTAIN | BGT | MEAS/ID/EG/BT | `PRECOMMIT_AUDIT_COIN_NONINTERFERENCE_CERTIFICATE_VALIDITY` | CL0 formal + CL1 empirical; local controlled attack only | I0/I2-local/T0 | FORMAL_IDENTIFICATION_LIMIT_AND_NEGATIVE_CONTROL |
| SIS-CAND-20261029-02 | [M4Bench: Evaluating Procedural Specification for Clinical EHR Derivation Agents](https://arxiv.org/abs/2610.37459), v1 2026-10-27 | SCF | BGT; CSCI exploratory | MI/MEAS/ID/EG/BT | `OPERATIONAL_SPECIFICATION_VS_SKILL_DELIVERY_INCREMENTAL_VALUE` | CL1 performance; local CL2 candidate for controlled specification contrast | I2-local/T2-performance-only | CONTROLLED_SPECIFICATION_MEASUREMENT_AND_NULL_BOUNDARY |
| SIS-CAND-20261029-03 | [When Retrieval Is Not Enough: Obsolete Facts in Agent Memory](https://arxiv.org/abs/2610.36308), v1 2026-10-26 | SDR | BGT | TD/EG/ID/MEAS/BT | `OBSOLETE_COMPETING_EVIDENCE_SUPERSESSION_FAILURE_EFFECT` | CL1 overall; local CL2 candidate for frozen-prompt stale-statement substitution | I2-local/T1 | NEGATIVE_MEMORY_SUPERSESSION_BOUNDARY |
| SIS-CAND-20261029-04 | [Don't Pick a Winner: Knowledge Conflicts Need a Prior, Not a Rule](https://arxiv.org/abs/2610.36169), v1 2026-10-26 | ASR | BGT | DR/EG/ID/MEAS/BT | `SOURCE_RELIABILITY_PRIOR_CONDITIONAL_SELECTION_NET_VALUE` | CL0 decision-theory + CL1 results; local controlled context interventions | I1/I2-local/T1 | BOUNDARY_AND_ADAPTIVE_SOURCE_SELECTION_MEASUREMENT |
| SIS-CAND-20261029-05 | [Counting the Bandages: On measuring the time that AI saves](https://arxiv.org/abs/2610.35942), v1 2026-10-23 | ROUTING_ABSTAIN | BGT | MEAS/ID/EG/BT | `COUNTERFACTUAL_TIME_SAVED_VS_ESCAPED_DEFECT_BREAK_EVEN_COST` | CL0 theoretical/estimand + CL1 secondary data; local controlled reviewer experiment | I1/I2-local/T0 | MEASUREMENT_IDENTIFICATION_AND_NEGATIVE_BOUNDARY |
| SIS-CAND-20261029-06 | [How Stable Are LLM-Generated Proofs Under Program Refactoring? A Stress Test for Verifiable Code Generation](https://arxiv.org/abs/2610.36328), v1 2026-10-26 | SCF | BGT | MI/MEAS/ID/BT | `BEHAVIOR_PRESERVING_REFACTOR_UNCHANGED_PROOF_SURVIVAL_EFFECT` | CL1 robustness measurement; local controlled program transformation | I2-local/T1 | NEGATIVE_REPRESENTATION_BOUNDARY_AND_MEASUREMENT_INSTRUMENT |
| SIS-CAND-20261029-07 | [InfraDev: Can Coding Agents Develop AI Infrastructure, and How Can We Tell?](https://arxiv.org/abs/2610.36589), v1 2026-10-27 | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | `HIDDEN_INFRASTRUCTURE_PROBE_INCREMENTAL_CONFORMANCE_VALIDITY` | CL1 benchmark measurement; no mechanism promotion | I1/T0 | NEGATIVE_BENCHMARK_CONSTRUCT_VALIDITY |
| SIS-CAND-20261029-08 | [Concordat: Typed Sessions for LLM Agents](https://arxiv.org/abs/2610.37461), v1 2026-10-27 | SCF | BGT | MI/EG/ID/MEAS/BT | `TYPED_SESSION_PROTOCOL_AUTHORIZATION_VIOLATION_EFFECT` | CL1; local CL2 candidate under controlled protocol enforcement | I2-local/T0 | VIABILITY_CONSTRAINT_IMPLEMENTATION_AND_BOUNDARY |
| SIS-CAND-20261029-09 | [CohortFlow: A Steerable Clinical Cohort Curation Agent with Localized Semantic Correction](https://arxiv.org/abs/2610.36100), v1 2026-10-26 | ASR | BGT | DR/TD/MI/MEAS/ID/BT | `DEPENDENCY_SCOPED_CORRECTION_COST_ADJUSTED_REQUIREMENT_FIDELITY` | CL1; local CL2 candidate for controlled recomputation policy | I2-local/T0 | CONDITIONAL_SEMANTIC_REPAIR_EFFICIENCY_AND_NULL |
| SIS-CAND-20261029-10 | [The Trinity: Capability-Driven Recursive Self-Improvement for Multimodal Agents](https://arxiv.org/abs/2610.36077), v1 2026-10-26 | SCF | BGT | MI/DR/EG/MEAS/BT | `CAPABILITY_HIERARCHY_ROUTED_HARNESS_EVOLUTION_HELDOUT_VALUE` | CL1 composition/performance; no mechanism CL2 from bundled system | I1/T2-performance-only | IMPLEMENTATION_AND_CROSS_TASK_PERFORMANCE_TRANSFER |

**Primary evidence, quantitative results, identification limits, boundary conditions and novelty assessment:** [2026-10-29 Daily Update](updates/2026-10-29_SIS_Daily_Literature_Update.md). **P0 claim re-audit:** [2026-10-29 audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-29.md) (003,004,103; 9 claims). M4Bench NeurIPS E&D, Obsolete Facts / RefactorProof workshop acceptance are author-declared metadata, not independently verified archival identities; do not count as peer-reviewed paper editions yet.


---

## 20｜2026-10-30 delayed archival and recent preprint source-verified candidates (NOT permanent SIS-LIT IDs)

**Scope:** 5 independently verified EMNLP 2026 archival study identities (published October, discovered/re-coded now) + 5 recent Oct 26–27 preprints. Latest accessible arXiv new-list: 2026-10-28. Cross-checked 145 permanent records and 59 synced Oct 24–29 provisionals; unsynced Oct 9–23 candidates remain to reconcile; no second coder promotions or T3/T4.

| Temporary ID | StudyVersionRecord | Primary | Cross | Framework | Estimand | First-coder ceiling | I/T | Evidence role |
|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261030-01 | [Beneath the Diff: Diagnosing and Mitigating Algorithmic Mode Collapse in Code-Level Autonomous Research Loops](https://aclanthology.org/2026.emnlp-main.1029/) — EMNLP 2026 Main (October; delayed archival discovery) | ASR | BGT | DR/MI/MEAS/ID/EG/BT | `SEMANTIC_PROPOSAL_DIVERSITY_HELDOUT_OPTIMIZATION_EFFECT` | CL1; local CL2 candidate | I1/I2-local/T1 | NEGATIVE_OPTIMIZER_DYNAMICS |
| SIS-CAND-20261030-02 | [Gaming the Judge: How Unfaithful Chain-of-Thought Can Undermine Agent Evaluation](https://aclanthology.org/2026.findings-emnlp.1636/) — Findings EMNLP 2026 (October; delayed archival discovery) | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | `COT_REWRITE_JUDGE_FALSE_POSITIVE_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | NEGATIVE_MEASUREMENT_CONSTRUCT |
| SIS-CAND-20261030-03 | [Who is the Agent to Blame? Localizing Faithfulness and Citation Mistakes in Agentic Deep Research](https://aclanthology.org/2026.emnlp-main.1681/) — EMNLP 2026 Main (October; delayed archival discovery) | SDR | CSCI/BGT | TD/IA/EG/ID/MEAS/BT | `LOCAL_CITATION_ERROR_PROPAGATION_AND_REPAIR` | CL1; local repair candidate | I1/I2-local/T0 | TRACE_FAITHFULNESS_BOUNDARY |
| SIS-CAND-20261030-04 | [AgentRx: Diagnosing AI Agent Failures from Execution Trajectories](https://aclanthology.org/2026.findings-emnlp.598/) — Findings EMNLP 2026 (October; delayed archival discovery) | SDR | BGT | TD/ID/EG/MEAS/BT | `AUDITABLE_CONSTRAINT_FAILURE_LOCALIZATION_ACCURACY` | CL1; local label comparison | I1/T1 | DIAGNOSTIC_MEASUREMENT_INSTRUMENT |
| SIS-CAND-20261030-05 | [The Cold-Start Safety Gap in LLM Agents](https://aclanthology.org/2026.emnlp-main.1973/) — EMNLP 2026 Main (October; delayed archival discovery) | SDR | BGT | TD/EG/MEAS/ID/BT | `PRECEDING_TASK_DEPTH_CONDITIONAL_SAFETY_EFFECT` | CL1; local session-depth candidate | I2-local/T1 | DYNAMIC_VIABILITY_BOUNDARY |
| SIS-CAND-20261030-06 | [Evolving Agent Teams](https://arxiv.org/abs/2610.36848) — arXiv:2610.36848 v1, 2026-10-27 (preprint) | ASR | CSCI/BGT | DR/IA/MI/MEAS/ID/BT | `TEAM_RESTRUCTURING_LOCAL_OPTIMUM_POLICY_NET_VALUE` | CL1; local ablation candidate | I1/I2-local/T2-performance | IMPLEMENTATION_AND_CAPABILITY_INTERACTION |
| SIS-CAND-20261030-07 | [MARQ: A Modular, LLM-Agnostic Requirement Quality Assessor Infused with Systems Engineering Knowledge](https://arxiv.org/abs/2610.36234) — arXiv:2610.36234 v1, 2026-10-26 (preprint) | SCF | CSCI/BGT | MI/EG/MEAS/ID/BT | `CRITERION_KNOWLEDGE_INFUSION_REQUIREMENT_DEFECT_F1_EFFECT` | CL1; local knowledge contrast candidate | I1/I2-local/T1 | MEASUREMENT_INSTRUMENT |
| SIS-CAND-20261030-08 | [Grounding LLM Agents in Business Processes: Process-Aware Knowledge Graphs for Reliable Multi-Step Service Invocation](https://arxiv.org/abs/2610.37242) — arXiv:2610.37242 v1, 2026-10-27 (preprint) | SCF | BGT | MI/TD/EG/MEAS/ID/BT | `TYPED_PROCESS_GRAPH_CONTEXT_API_CONFORMANCE_EFFECT` | CL1; local schema contrast candidate | I1/I2-local/T0 | REPRESENTATION_EXTERNALIZATION_BOUNDARY |
| SIS-CAND-20261030-09 | [From Structural Feedback to Prompt Policies: Learning Faithful Text-to-Image Prompt Editors](https://arxiv.org/abs/2610.36146) — arXiv:2610.36146 v1, 2026-10-26 (preprint) | ASR | BGT | DR/MI/EG/MEAS/ID/BT | `GRAPH_CONDITIONED_PROMPT_EDIT_RELATIONAL_FIDELITY_EFFECT` | CL1; local ablation candidate | I1/I2-local/T1 | SEMANTIC_INVARIANT_OPTIMIZER |
| SIS-CAND-20261030-10 | [Agentic Distributional Regression: Conditional Density Estimation through Agent-Written Programs](https://arxiv.org/abs/2610.37611) — arXiv:2610.37611 v1, 2026-10-27 (preprint) | ASR | BGT | MI/DR/EG/MEAS/ID/BT | `EXPLICIT_DENSITY_PROGRAM_SEARCH_VALIDATED_VALUE` | CL0 theorem + CL1 empirical | I0/I1/T1 | FORMAL_PROGRAM_SEARCH |

- [2026-10-30 scientific update](updates/2026-10-30_SIS_Daily_Literature_Update.md)
- [2026-10-30 nine-claim P0 source-level re-audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-30.md)

---

## 21｜2026-10-31 source-verified provisional discoveries (NOT permanent SIS-LIT IDs)

**Scope:** one independently verified October EMNLP 2026 archival study + nine arXiv v1 preprints (first submitted Oct 27–29, indexed by Fri Oct 30). 145 permanent studies + 69 synced Oct 24–30 provisional IDs cross-checked. Unmerged Oct 9–23 candidates remain pending global dedup. No paper-level CL2/CL3 promotion.

| Temporary ID | StudyVersionRecord | Primary | Cross | Framework | Estimand | First-coder ceiling | I/T | Evidence Role |
|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261031-01 | [LogicInception: Discourse-Level Indirect Prompt Injection via Causal Chain Construction](https://aclanthology.org/2026.emnlp-main.1831/) — EMNLP 2026 Main; archival October 2026, delayed discovery | SDR | CSCI/BGT | TD/IA/EG/ID/MEAS/BT | `DISCOURSE_CAUSAL_CHAIN_UNAUTHORIZED_ACTION_EFFECT` | CL1; local CL2 candidate (not adjudicated) | I1/I2-local/T1 | NEGATIVE_VIABILITY_BOUNDARY |
| SIS-CAND-20261031-02 | [What Does an Ontology Catch? Curated, LLM-Generated and Data-Derived Ontologies as Checkers of LLM Agents over Knowledge Graphs](https://arxiv.org/abs/2610.37809) — arXiv:2610.37809v1; first submitted 2026-10-27; preprint under review | ROUTING_ABSTAIN | BGT | EG/MEAS/ID/BT | `ONTOLOGY_CHECKER_FALSE_FLAG_DECISION_VALIDITY` | CL1; no causal mechanism promotion | I1/T1 | NEGATIVE_MEASUREMENT_BOUNDARY |
| SIS-CAND-20261031-03 | [Measuring Where Intent Gets Lost in Agentic Smart Contract Synthesis](https://arxiv.org/abs/2610.37830) — arXiv:2610.37830v1; first submitted 2026-10-27; preprint (2027 conference note not peer review) | SCF | BGT | MI/EG/MEAS/ID/BT | `PREGENERATION_ELICITATION_VS_POSTHOC_REPAIR_INTENT_CONFORMANCE` | CL1; local CL2 candidate | I2-local/T1 | SPECIFICATION_BOUNDARY_AND_MECHANISM_CANDIDATE |
| SIS-CAND-20261031-04 | [OpenFrontiers: A Collection of Open Research Problems and a Benchmark for Scientific Rediscovery](https://arxiv.org/abs/2610.37739) — arXiv:2610.37739v1; first submitted 2026-10-27; preprint | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | `CLOSED_BOOK_REDISCOVERY_VS_SOLUTION_RETRIEVAL_VALIDITY` | CL1 measurement; no mechanism CL2 | I1/T0 | MEASUREMENT_INSTRUMENT_AND_LEAKAGE_BOUNDARY |
| SIS-CAND-20261031-05 | [SciGame: Let Agents Play the Scientific Discovery Games in the Real and Counterfactual World](https://arxiv.org/abs/2610.37919) — arXiv:2610.37919v1; first submitted 2026-10-27; preprint | ASR | BGT | DR/ID/MEAS/BT | `COUNTERFACTUAL_LAW_DISCOVERY_ADAPTIVE_EXPERIMENT_NET_VALUE` | CL1; intervention candidate subject to full controls | I1/I2-local/T1 | COUNTERFACTUAL_BOUNDARY_AND_NEGATIVE_RESULT |
| SIS-CAND-20261031-06 | [Prefix Executability: Evaluating Tool-Using Agents Beyond Final Success](https://arxiv.org/abs/2610.40444) — arXiv:2610.40444v1; first submitted 2026-10-29; NeurIPS acceptance author-declared; archive not independently linked | SDR | BGT | TD/MEAS/ID/BT | `PREFIX_EXECUTABILITY_CONDITIONAL_TERMINAL_SUCCESS_GAP` | CL1; local plan-checking contrast CL2 candidate | I1/I2-local/T1 | TRAJECTORY_MEASUREMENT_AND_RECOVERY_BOUNDARY |
| SIS-CAND-20261031-07 | [Efficient Scalable Oversight via Rewinding](https://arxiv.org/abs/2610.40535) — arXiv:2610.40535v1; first submitted 2026-10-29; preprint | ROUTING_ABSTAIN | BGT | EG/ID/MEAS/BT | `REWINDABLE_VERIFICATION_SOUNDNESS_AND_COST_UNDER_ORACLE_ROBUSTNESS` | CL0 conditional theorem; CL1 preliminary prototype | I0/I1/T0 | FORMAL_IDENTIFICATION_INSTRUMENT |
| SIS-CAND-20261031-08 | [PCM: A Proof-Carrying Message Protocol for Verifiable Multi-Agent Communication](https://arxiv.org/abs/2610.39109) — arXiv:2610.39109v1; first submitted 2026-10-29; preprint cross-listed cs.AI | ROUTING_ABSTAIN | BGT | EG/MI/ID/MEAS/BT | `SIGNED_INDEPENDENT_EVIDENCE_MESSAGE_AUTHORITY_VALIDITY` | CL0 conditional security proof + CL1 benchmark | I0/I1/T0 | EVIDENCE_GOVERNANCE_IMPLEMENTATION_AND_NEGATIVE_BOUNDARY |
| SIS-CAND-20261031-09 | [Disparity Laundering: Consensus Without Fairness in Clinical Multi-Agent Systems](https://arxiv.org/abs/2610.38215) — arXiv:2610.38215v1; first submitted 2026-10-28; preprint; EACL 2027 noted but not peer reviewed archive | SCF | CSCI/BGT | IA/ID/MEAS/BT | `TOPOLOGY_BY_MODEL_COMMITTED_CLINICAL_DECISION_DISPARITY` | CL1; local demographic-swap and pooling CL2 candidate | I2-local/T1 | NEGATIVE_CSCI_VIABILITY_BOUNDARY |
| SIS-CAND-20261031-10 | [Beyond fabrication: Misattributed numbers in papers written by AI research agents](https://arxiv.org/abs/2610.38691) — arXiv:2610.38691v1; first submitted 2026-10-28; preprint | ROUTING_ABSTAIN | BGT | EG/MEAS/ID/BT | `NUMERIC_CLAIM_TO_EXPERIMENT_METRIC_RUN_PROVENANCE_VALIDITY` | CL1 measurement; no causal promotion | I1/T0 | NEGATIVE_CLAIM_PROVENANCE_AND_MEASUREMENT_INSTRUMENT |

**Detailed evidence / boundaries / impact:** [2026-10-31 literature update](updates/2026-10-31_SIS_Daily_Literature_Update.md). **P0 re-audit:** [2026-10-31 audit](evidence-map/audits/SIS_P0_Reaudit_2026-10-31.md) (SIS-LIT-048/049/050). `ROUTING_ABSTAIN` is scientific primary-routing abstention, not a fourth Primary Program.

---

## 22｜2026-11-01 verified late-October discoveries (provisional, not permanent SIS-LIT IDs)

**Date semantics:** latest regular cs.AI batch was 2026-10-30; papers first submitted 2026-10-27–29, and three archival EMNLP items published October 2026. Discovered/verified on 2026-11-01. 145 permanent + 79 Oct 24–31 provisional checked by source ID; Oct 9–23 backlog incomplete. **No automatic CL2/CL3 promotion, no T3/T4 established.**

| Temporary ID | StudyVersionRecord | Primary | Cross | Framework | Estimand | First-coder ceiling | I/T | Evidence role |
|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261101-01 | [TraceProbe: An Execution-Based Benchmark for Diagnosing Safety Failures in LLM Agents](https://aclanthology.org/2026.emnlp-main.1233/) — EMNLP 2026 Main, October 2026, delayed discovery | SDR | BGT | TD/ID/EG/MEAS/BT | `EXECUTABLE_TRACE_LATENT_VIOLATION_LOCALIZATION_VALIDITY` | CL1; local replay-based CL2 candidate only for executed substitutions | I1/I2-local/T1 | NEGATIVE_DYNAMIC_VIABILITY_AND_MEASUREMENT |
| SIS-CAND-20261101-02 | [Trust Cascade through Provenance Erasure: How Multi-Agent Delegation Breaks Single-Agent Safety](https://aclanthology.org/2026.emnlp-main.1005/) — EMNLP 2026 Main, October 2026, delayed discovery | SDR | CSCI/BGT | TD/IA/EG/ID/MEAS/BT | `DELEGATION_PROVENANCE_ERASURE_AUTHORITY_ESCALATION_EFFECT` | CL1; local controlled delegation/channel candidate CL2 | I2-local/T1 | MECHANISM_CANDIDATE_AND_NEGATIVE_BOUNDARY |
| SIS-CAND-20261101-03 | [Tracing Error Propagation in Reasoning Language Models](https://aclanthology.org/2026.emnlp-main.1559/) — EMNLP 2026 Main, October 2026, delayed discovery | SDR | BGT | TD/ID/MEAS/BT | `PERSISTENT_REASONING_ERROR_RECOVERABILITY_SIGNAL_VALIDITY` | CL1; counterfactual resampling local CL2 candidate | I1/I2-local/T0 | RECOVERY_BOUNDARY_AND_MEASUREMENT |
| SIS-CAND-20261101-04 | [Masked Erosion: How Acceptance Gates Lose Redundant Safeguards in Self-Improving Agents](https://arxiv.org/abs/2610.38392) — arXiv:2610.38392v1, first submitted 2026-10-28, preprint | ASR | CSCI/BGT | DR/TD/EG/ID/MEAS/BT | `REDUNDANT_SAFEGUARD_DELETION_ACCEPTANCE_GATE_MASKING_EFFECT` | CL1; controlled safeguard deletion CL2 candidate | I2-local/T1 | NEGATIVE_REGULATION_BOUNDARY_AND_MECHANISM_CANDIDATE |
| SIS-CAND-20261101-05 | [DynaRev: Benchmarking Web Agents under Dynamic Goal Revision](https://arxiv.org/abs/2610.40133) — arXiv:2610.40133v1, first submitted 2026-10-29, preprint | SDR | BGT | TD/DR/MI/ID/MEAS/BT | `SEMANTIC_MILESTONE_GOAL_REVISION_ADAPTATION_EFFECT` | CL1; local revision/reset ablations need audit | I1/I2-local/T1 | DYNAMIC_GOAL_BOUNDARY_AND_BENCHMARK |
| SIS-CAND-20261101-06 | [MemSteer: Turning User Histories into Supervision for Agent Memory Optimization](https://arxiv.org/abs/2610.39276) — arXiv:2610.39276v1, first submitted 2026-10-29, preprint | ASR | CSCI/BGT | DR/MI/EG/ID/MEAS/BT | `EVIDENCE_GROUNDED_SYNTHETIC_MEMORY_SUPERVISION_OPTIMIZATION_VALUE` | CL1; local supervision-policy contrast candidate | I1/T1 (new-user results exploratory T2 performance) | OPTIMIZER_POLICY_AND_EVIDENCE_GOVERNANCE |
| SIS-CAND-20261101-07 | [Detecting Covert Collusion between AI Agents through Partner-Outsider Positive Listening](https://arxiv.org/abs/2610.37849) — arXiv:2610.37849v1, first submitted 2026-10-27, work in progress preprint | SDR | CSCI/BGT | IA/TD/ID/MEAS/BT | `PARTNER_OUTSIDER_PARAPHRASE_DIFFERENTIAL_CHANNEL_USE` | CL1; local controlled wording perturbation candidate | I2-local/T0 | MEASUREMENT_INSTRUMENT_AND_NEGATIVE_BOUNDARY |
| SIS-CAND-20261101-08 | [Evaluating and improving AI agents for sequencing protocol understanding / LibStructBench](https://arxiv.org/abs/2610.37851) — arXiv:2610.37851v1, first submitted 2026-10-27, preprint | SCF | CSCI/BGT | MI/TD/ID/MEAS/BT | `BIOPROTOCOL_EXACT_MOLECULAR_STATE_WORKFLOW_RECONSTRUCTION` | CL1; controlled model/harness contrasts need full audit | I1/I2-local/T1 | NEGATIVE_SCIENTIFIC_CAPABILITY_AND_BENCHMARK |
| SIS-CAND-20261101-09 | [ThinkJev: One Thought, Every Budget for Calibrated Typed Decisions](https://arxiv.org/abs/2610.37732) — arXiv:2610.37732v1, first submitted 2026-10-27, preprint | ASR | BGT | DR/ID/MEAS/BT | `CONFIDENCE_CONDITIONAL_REASONING_ESCALATION_AND_STOPPING_NET_VALUE` | CL1; local budget contrast candidate | I1/I2-local/T1 | ADAPTIVE_REGULATION_BOUNDARY |
| SIS-CAND-20261101-10 | [WebAnything: From the Wild Web to Scalable Agent Environments](https://arxiv.org/abs/2610.37786) — arXiv:2610.37786v1, first submitted 2026-10-27, preprint | SCF | BGT | MI/TD/EG/ID/MEAS/BT | `SOURCE_GROUNDED_RECONSTRUCTED_WEB_ENVIRONMENT_FIDELITY_AND_TRAINING_VALUE` | CL1; local independent verifier contrast candidate | I1/T2-performance-only | REPLACEABLE_BENCHMARK_ENVIRONMENT_IMPLEMENTATION |

**Full first-coder evidence, boundaries, program effects:** [2026-11-01 daily update](updates/2026-11-01_SIS_Daily_Literature_Update.md). **Nine-claim P0 audit:** [2026-11-01 claim-level re-audit](evidence-map/audits/SIS_P0_Reaudit_2026-11-01.md). `ROUTING_ABSTAIN` denotes primary routing abstention, not a new program.


---

## Provisional New Literature / Delayed Official Proceedings Discovery | 2026-11-02

**Not yet canonical SIS-LIT:** 10 official October EMNLP publications newly discovered in this daily workflow on Nov 2; no permanent identifiers. Original paper-level sources are distinct from claim-level evidence. Verify against historical unsynced backlog before formal accession.

### SIS-CAND-20261102-01 — Messier: A High-Resolution Corpus for Cross-Benchmark Agent Evaluation

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.1398/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 统一不同 Benchmark 的任务、执行器和验证器记录，并研究评分规则如何改变系统排序。
- **Reported evidence:** 957,611 条记录、30 个 Benchmarks、745 个 Agents、11,891 个 Tasks、74,263 个 Verifiers；不同多验证器规则的反事实重评分可改变排序，能力评分与 Epoch 指数 Spearman ρ=0.84。
- **Limitations/confounders:** 异质历史数据和验证器质量不同；重评分不是对系统实施新的因果干预；相关性不能证明能力测量的独立 Gold 有效。
- **Scientific routing:** Primary `ROUTING_ABSTAIN`; Cross-cutting `BGT`; Framework `MEAS/EG/ID/BT`; primary estimand `VERIFIER_SCORING_RULE_CONDITIONAL_AGENT_RANKING_VALIDITY`.
- **Evidence maturity:** CL1; counterfactual rescoring local measurement contrast (not mechanism); identification I1/I2-local measurement; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Measurement instrument; negative ranking-boundary evidence. **Boundary variables:** 验证器组合、all-pass 规则、任务领域、模型版本、执行预算.
- **SIS impact:** SHARPENS：强迫将 System Capability Frontier 与评分语义/验证器有效性分开；归入 BGT/MEAS，不构成第四 Primary。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-02 — STAGE: Diagnosing Semantic Transfer at Grounded Execution in Embodied Agents

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1148/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 固定视觉观察与系统状态，改变指令语义，直接测量语义已被解析时是否传递至连续动作控制。
- **Reported evidence:** LIBERO 目标和关系交换中语义恢复分别 100.0%、95.8%，OpenVLA 动作敏感性只有 6.8%、7.7%；另有 1,000 个组合和时序反事实，动作敏感性 6.1%。
- **Limitations/confounders:** 语义恢复与连续动作的匹配测量依赖阈值及物理仿真；低敏感性不自动意味着真实任务全部失败；未识别内部因果中介。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/ID/MEAS/BT`; primary estimand `FIXED_OBSERVATION_SEMANTIC_INTERVENTION_ACTION_SENSITIVITY`.
- **Evidence maturity:** CL1; local CL2 candidate for instruction-swap intervention only; identification I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Negative/boundary; semantic-to-action measurement. **Boundary variables:** 视觉状态、语义替换、连续动作幅度、控制器与物理任务.
- **SIS impact:** SHARPENS：语义理解与可执行能力分离；Representation Construct Validity 新 Fixture，不修订 Core。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-03 — SkillAlign: Aligning Skill Interfaces for LLM-based Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.2565/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 固定任务、执行器和候选技能，只切换完整说明、提示、摘要、工作流或不暴露等技能接口形式。
- **Reported evidence:** 在 ALFWorld 与 SkillsBench 上发现接口形式显著改变任务成功与上下文成本；紧凑 top-k 可能优于完整技能库注入，重放式学习显示自适应选择仍远离 Oracle。
- **Limitations/confounders:** 暴露形式会改变有效输入预算及信息密度；有限任务/技能分布；不应将接口作用归因于 Skill 内容本身或跨执行器机制不变性。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/ID/MEAS/BT`; primary estimand `FIXED_SKILL_CONTENT_EXPOSURE_INTERFACE_CAUSAL_EFFECT`.
- **Evidence maturity:** CL1; local CL2 candidate; identification I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Mechanism candidate; interface boundary. **Boundary variables:** 技能长度、接口压缩损失、模型上下文预算、技能适用性.
- **SIS impact:** SUPPORTS：SCF 中的 Representational Interface Effect；精细化 Skill Packaging 与能力之间的识别。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-04 — LegalWorld: A Life-Cycle Interactive Environment for Legal Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.390/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 将法律诉讼五阶段建成共享状态的因果连接过程，不再在每个子任务重置到独立真值。
- **Reported evidence:** 使用 75,309 对判决作为来源，五阶段七子场景；217 名法律背景评估者贡献 18,992 条评分；整体评分差距 4 分内的模型在单阶段可相差 15 个归一化点。
- **Limitations/confounders:** 法律模拟环境中的因果连锁由生成器定义；评估者程序忠实性不直接代表现实法律结果；反思 Skill 与环境作用组合。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/EG/MEAS/BT`; primary estimand `CROSS_STAGE_STATE_DEPENDENCE_LONG_HORIZON_CAPABILITY_GAP`.
- **Evidence maturity:** CL1 descriptive; no independent mechanism promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Benchmark instrument; state-history boundary. **Boundary variables:** 跨阶段历史、案件制度、时间跨度、前期错误不可逆性.
- **SIS impact:** SHARPENS：SDR 历史依赖与跨阶段后果；现实部署迁移未证明。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-05 — Asuka-Bench: Benchmarking Code Agents on Underspecified User Intent and Multi-Round Refinement

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1548/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 让欠完整用户需求经过网页生成—实际浏览器测试—自然语言反馈—多轮修订的闭环展开。
- **Reported evidence:** 50 个网站任务、784 项评价准则、2,402 个期望结果；8 个模型和 2 个执行框架；加权通过率跨模型相差 38 个百分点，最强模型三轮后只完成 52%。
- **Limitations/confounders:** 用户反馈来自 User LLM，可能偏离真实用户意图；不同轮次项目状态、算力和反馈同时改变；真实主观满意度未被证明。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/DR/MEAS/EG/BT`; primary estimand `UNDERSPECIFIED_INTENT_FEEDBACK_CONDITIONAL_REFINEMENT_EFFECT`.
- **Evidence maturity:** CL1; no CL2 promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Measurement and dynamic user-feedback boundary. **Boundary variables:** 规范欠完整程度、反馈质量、浏览器验证有效性、轮次预算.
- **SIS impact:** SHARPENS：用户意图动态演化和系统恢复；现有 SDR + MEAS 充分表达。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-06 — CoEmbod: A Long-Horizon Benchmark for Multi-Agent Embodied Cooperation with Diverse Inter-Agent Dependencies

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.2247/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 在长时程具身模拟中分别构造空间分配、并行约束与失败恢复三类组件依赖，并联合测量任务成功、合作忠实性及资源效率。
- **Reported evidence:** 155 项人工设计任务、40 个场景、10,845 个对象；作者称最强被测多模态执行流程成功率仅 20.23%。
- **Limitations/confounders:** 模拟任务和人工依赖设计限制外推；低成功率不单独识别某类协作机制的因果贡献；缺少正交任务/组织对照。
- **Scientific routing:** Primary `SDR`; Cross-cutting `CSCI/BGT`; Framework `TD/IA/MEAS/BT`; primary estimand `INTER_AGENT_DEPENDENCY_CONDITIONAL_COOPERATIVE_RECOVERY_VALUE`.
- **Evidence maturity:** CL1; identification I1; transport T0; no automatic whole-paper CL2/CL3.
- **Evidence role:** Benchmark instrument; dependency and failure boundary. **Boundary variables:** 组件间前置约束、时间协调、可观察性、恢复资源.
- **SIS impact:** SUPPORTS：SDR/CSCI 的多组件依赖测量；不是 Multi-Agent primitive。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-07 — CUADebug: Diagnosing and Repairing Computer-Use Agent Failures

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.530/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 联合低层 GUI 动作、前后截图和人工根因标签，定位故障再重新执行，避免将最终失败位置等同于根因。
- **Reported evidence:** 204 条 OSWorld 失败轨迹、30 个故障子类型；Gemini 2.5 Pro 的 Tag+Step exact 从 11.1% 到 19.4%；单次重新执行恢复率从 13.89% 到 29.86%。
- **Limitations/confounders:** 人工标签不等于可干预因果真值；某些重跑比较由人工标注固定重启点，诊断器与重试流程的独立效应仍需拆分。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/ID/EG/MEAS/BT`; primary estimand `TRAJECTORY_DIAGNOSIS_GUIDED_REEXECUTION_RECOVERY_EFFECT`.
- **Evidence maturity:** CL1; local CL2 candidate conditional on matched rerollout; identification I1/I2-local; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Failure recovery; local intervention candidate. **Boundary variables:** 界面状态、截图粒度、恢复起点、重试次数、模型版本.
- **SIS impact:** SHARPENS：故障定位和修复净收益可拆分；建议反事实重启点冻结 Fixture。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-08 — TopoCurate: Modeling Interaction Topology for Tool-Use Agent Training

- **Primary source & StudyVersionRecord:** [Findings EMNLP 2026 (Oct 2026, delayed discovery)](https://aclanthology.org/2026.findings-emnlp.1969/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Must Read. **Core novelty:** 不用最终成功/失败筛选训练样本，而是从多次尝试形成的执行交互拓扑中选择含恢复路径、多样策略和高错误分支的示例。
- **Reported evidence:** 在 BFCLv3、Tau2 Bench 作者报告 SFT +4.2%、RL +6.9% 的收益（原文未在摘要澄清是绝对点还是相对幅度，此处仅按报告数值记）。
- **Limitations/confounders:** 样本选择会改变难度、token、训练分布及奖励信噪比；拓扑指标与真实训练机制的中介作用未单独识别。
- **Scientific routing:** Primary `ASR`; Cross-cutting `BGT`; Framework `DR/TD/MI/ID/MEAS/BT`; primary estimand `INTERACTION_TOPOLOGY_CONDITIONAL_TRAINING_EXAMPLE_SELECTION_VALUE`.
- **Evidence maturity:** CL1; no causal mediation promotion; identification I1; transport T1; no automatic whole-paper CL2/CL3.
- **Evidence role:** Regulation/operator selection; mechanism candidate. **Boundary variables:** 任务分支比、失败与恢复密度、训练预算、模型能力、评估域.
- **SIS impact:** SHARPENS：ASR 训练数据/任务选择策略与最终收益的独立对照。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-09 — OpenResearcher: A Fully Open Pipeline for Long-Horizon Deep Research Trajectory Synthesis

- **Primary source & StudyVersionRecord:** [EMNLP 2026 Main (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-main.42/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 将文献语料初始化和多轮 search/open/find 轨迹生成分离，在可记录、可复现的离线环境生成长轨迹。
- **Reported evidence:** 1,500 万文档，超过 97,000 条训练轨迹；30B-A3B 模型在 BrowseComp-Plus 达 54.8%，相较基础模型提高 34.0 个百分点。
- **Limitations/confounders:** 语料中答案存在性、检索质量和训练分布均影响成绩；离线文献与真实网络的时效、来源权威及引证充分性不同；多组件共同改变。
- **Scientific routing:** Primary `SCF`; Cross-cutting `BGT`; Framework `MI/TD/EG/MEAS/BT`; primary estimand `OFFLINE_RESEARCH_TRAJECTORY_SYNTHESIS_HELDOUT_CAPABILITY_EFFECT`.
- **Evidence maturity:** CL1; performance transfer only; identification I1; transport T2-performance-only; no automatic whole-paper CL2/CL3.
- **Evidence role:** Implementation plus training/measurement instrument. **Boundary variables:** 文献覆盖、检索工具、答案泄漏、训练量、评估独立性.
- **SIS impact:** SUPPORTS：SCF 科研系统的训练环境机制；实际科学 Claim 证据治理仍须独立评价。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.

### SIS-CAND-20261102-10 — AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents

- **Primary source & StudyVersionRecord:** [EMNLP 2026 System Demonstrations (Oct 2026, delayed discovery)](https://aclanthology.org/2026.emnlp-demos.52/); EMNLP 2026 official ACL Anthology record. October 2026 publication; **discovered 2026-11-02**, not newly published today.
- **Reading:** Worth Skimming. **Core novelty:** 提供 Detect–Attribute–Recover–Rerun 可重放诊断闭环和可选的去敏故障记忆库。
- **Reported evidence:** Who When 的严格 agent+step 定位准确率 28.8% vs 21.7% 单次分析基线；GAIA 73 次失败中单次重跑修复 13 项，对照为 4–6 项；总体准确率 55.8% 至 63.6%。
- **Limitations/confounders:** 系统演示论文不等于多中心机制验证；诊断器、重试策略和先验记忆共同变化；受控复制集有限。
- **Scientific routing:** Primary `SDR`; Cross-cutting `BGT`; Framework `TD/DR/ID/EG/MEAS/BT`; primary estimand `MULTI_TURN_ROOT_CAUSE_DEBUGGING_GUIDED_RERUN_RECOVERY_VALUE`.
- **Evidence maturity:** CL1; demo evidence ceiling; identification I1; transport T0; no automatic whole-paper CL2/CL3.
- **Evidence role:** Implementation + initial recovery comparison. **Boundary variables:** 故障分类质量、诊断深度、重启点、重试预算、日志脱敏与遗忘.
- **SIS impact:** IMPLEMENTATION：已有 SDR/EG 能承载；建议作为多步诊断与真实重跑实施基准。
- **Paper/Claim separation:** study-level publication and benchmark metadata do not confer causality, calibration, or transport status on individual claims.



---

## Daily provisional intake — 2026-11-03

Ten independently sourced arXiv v1 records (first submitted 2026-10-29–30 UTC, posted 2026-11-02; PREPRINT); not new Nov 3 submissions. No exact arXiv-ID duplicate in the existing permanent/provisional registry; pending October 9–23 full lineage reconciliation. Claim ceilings are initial paper-level source checks; no whole-paper promotion.

## Claim-level preliminary evidence coding

### SIS-CAND-20261103-01 — Does Recursive Knowledge Construction Help Agents Verify Consensus Claims in Science?

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40906 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 外部结构化证据状态与停止 Judge 分离测试，718 条由五个专家数据库标注的科学共识 Claim；外部状态优于纯上下文积累，独立训练 Judge 在五个子集中的三个达到最优或并列水平。
- Limitations and confounders: 专家共识不是普遍真值；检索覆盖、时间新鲜度、数据集独立性限制跨域因果推断。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/DR/EG/ID/MEAS/BT; primary estimand EXTERNAL_EVIDENCE_STATE_AND_STOP_JUDGE_CLAIM_VERIFICATION.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T1.
- Evidence role: Measurement / evidence externalization. Boundary variables: 证据结构、停止预算、Gold 独立性、领域、时效.
- SIS Impact: SHARPENS：既有 SCF 表示能力与 ASR 停止应拆为独立 Claim。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-02 — ReplayRCA: Measuring Post-hoc Diagnosis and Live Oversight of Agent Failures by Counterfactual Replay

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41025 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 同状态替换行动并配对原动作 placebo 重放，比较事后故障诊断和不知道最终结局的在线监督；62 个校准失败任务最佳事后修复 +51.3 点；87 次在线监督有系统反而 -14.5 点。
- Limitations and confounders: 生成式确定性 OpsWorld 不能代表真实系统；选择失败轨迹带来选择性，模型名次差异不全显著。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/ID/MEAS/BT; primary estimand PAIRED_REPLAY_POSTHOC_VS_LIVE_CAUSAL_REPAIR_EFFECT.
- Claim ceiling: CL1; local CL2 candidate; identification I2-local; transport T0.
- Evidence role: Controlled recovery / negative transport. Boundary variables: 已知失败、介入时间、不可逆性、重复执行、预算.
- SIS Impact: CHALLENGES：后验归因分数不能替代在线监督净收益。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-03 — More Rules, Longer Lists? Benchmarking Self-Evolving Agents on a Hidden-Rule Curriculum

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40758 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: CLR-Bench 测试从反馈中抽象未明示规则而非累积例外；20 条链、10 领域、六种自演化方法；部分模型收益不超过 5 点，不如保留原始历史，较强模型部分方法达到 78% 准确率。
- Limitations and confounders: 规则来自公开群体名称，预训练已知知识和模型识别性是关键混杂；不能证明自演化一般无效。
- Scientific routing: Primary SCF; Cross-cutting CSCI/BGT; Framework MI/ID/MEAS/BT; primary estimand HIDDEN_RULE_INDUCTION_VS_EXCEPTION_MEMORIZATION.
- Claim ceiling: CL1; identification I1; transport T1.
- Evidence role: Negative/boundary + capability interaction. Boundary variables: 组件能力、规则可识别性、历史记录、反馈量.
- SIS Impact: SHARPENS：能力形成区别于例外记忆；CSCI 是核心调节变量。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-04 — BABA-Bench: Evaluating Long-Horizon Patient-Advocacy Agents

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41076 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 47 个由去标识患者倡导案例改写的交互世界、14 模型和 1,974 次执行；921 次达成最终结果，其中 254 次（约 28%）走了不被允许的过程；提供经过验证的计划明显改善严格通过率。
- Limitations and confounders: 模拟场景不代表患者结局；路线提供的规范信息和规划能力提升耦合。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/EG/MEAS/BT; primary estimand GOAL_COMPLETION_CONDITIONAL_PROCEDURAL_AUTHORIZATION.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Clinical viability measurement. Boundary variables: 许可、证据、禁止动作、长时程协调、人类 Gold.
- SIS Impact: SUPPORTS：最终任务成功不等于系统 Viability。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-05 — Beyond Plausible Prediction: Safety Sufficiency in Web World Models

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40798 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 十个冻结模型的 3,000 个预测中 86.1% 被认为语义合理，却不能稳定支持 EXECUTE/ASK/BLOCK；安全微调可提高证据保留却降低授权判断。
- Limitations and confounders: 人类主观合理性不是安全授权 Gold；校准效果受基础模型与类别分布影响。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/DR/ID/MEAS/EG/BT; primary estimand PREDICTIVE_PLAUSIBILITY_VS_AUTHORIZATION_SUFFICIENCY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Negative construct-validity boundary. Boundary variables: 授权条件、ASK 召回、读出校准、证据缺失.
- SIS Impact: SHARPENS：预测合理和决策充分性应分开测量。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-06 — Agentic World Modeling for Agent Test-time Scaling without Environment Replica

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40927 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 以安全只读查询和可执行计算预测假设动作的后继观察，避免共享不可复位环境被多个轨迹修改；在 τ-bench、AppWorld、OfficeBench 相对单次模拟和训练世界模型有报告收益。
- Limitations and confounders: 隐藏写入副作用及不可见环境状态可能未被只读接口捕获；仿真提升不代表部署安全保证。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/TD/EG/MEAS/BT; primary estimand READ_GROUNDED_SIMULATION_NONRESETTABLE_STATE_VALUE.
- Claim ceiling: CL1; identification I1; transport T1.
- Evidence role: Implementation and observability boundary. Boundary variables: 可观察性、工具只读能力、状态更新、资源.
- SIS Impact: SUPPORTS：作为外部化状态估计的 Framework 实现。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-07 — Evidence-Guided Recovery for AI Agents with Ambiguous Tool Outcomes and Partial Execution

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41453 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 对超时、已提交与仍执行等未知结果做状态可行集和权限检查；预注册 58 个配对单元中指导接口认证完成 30 次、对照 9 次，差 36.2 个百分点，116 条轨迹独立重放通过。
- Limitations and confounders: 检验的是共同安全约束下的 Advice 接口，不是搜索算法独立收益；提供者契约、合成任务限制外推。
- Scientific routing: Primary SDR; Cross-cutting BGT; Framework TD/DR/EG/ID/MEAS/BT; primary estimand ADVICE_INTERFACE_CONDITIONAL_CERTIFIED_RECOVERY_EFFECT.
- Claim ceiling: CL1; local CL2 candidate; identification I2-local; transport T0.
- Evidence role: Controlled recovery / boundary. Boundary variables: 授权时效、未知效果、幂等性、残留效果.
- SIS Impact: SUPPORTS：受限状态下的证据引导恢复，不是普适 Exactly-Once。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-08 — When Should AI Agents Ask? Clarification Requests Under Limited Human Attention

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41129 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 把提问、检索和继续独立工作作为多任务共享人类注意力的动态策略；PCP 在至多两项未决要求时理论最优；864 合成实例平均距离最优成本 0.07%，比简单规则节约 18–31%。
- Limitations and confounders: 模型是理想化人类答复与任务耗时；小型 LLM 案例不能证明真实临床专家负担。
- Scientific routing: Primary ASR; Cross-cutting CSCI/BGT; Framework DR/IA/ID/MEAS/BT; primary estimand SHARED_HUMAN_ATTENTION_CLARIFICATION_NET_COST.
- Claim ceiling: CL0 theoretical + CL1 empirical; identification I0/I1; transport T0.
- Evidence role: Shared-resource regulation. Boundary variables: 注意力容量、任务关联、等待时间、询问成本.
- SIS Impact: SHARPENS：ASR 交互调节需要联合优化，而不是单任务贪心。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-09 — Can Personal Requirements Become Supervision for Planning?

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.40992 (v1 preprint; first submitted 2026-10-29 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: Noura 利用可执行个人营养约束同时验证多日计划并生成训练目标；4,993 名保留参与者上同一执行闭环 Qwen3-14B 完整合规率 24.0% 至 72.5%，与模型生成目标相比执行目标在匹配比较中减少违规 41%。
- Limitations and confounders: 合规与营养质量是模拟计划指标，不能推广为临床疗效；指南约束、食品数据库和训练同时变化。
- Scientific routing: Primary SCF; Cross-cutting BGT; Framework MI/EG/ID/MEAS/BT; primary estimand EXECUTABLE_PERSONAL_SPECIFICATION_SUPERVISION_PLAN_VALIDITY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T1.
- Evidence role: Clinical scientific specification. Boundary variables: 多疾病条件、用药冲突、专家 Gold、指南更新.
- SIS Impact: SUPPORTS：可执行科学规范作为数据构建、训练和评价桥梁。 Reading priority: Must Read.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.

### SIS-CAND-20261103-10 — Counterfactual Pairwise Augmentation Improves Small Pointwise LLM Judges

- Source / StudyVersionRecord: https://arxiv.org/abs/2610.41149 (v1 preprint; first submitted 2026-10-30 UTC; posted in Monday 2026-11-02 issue).
- Novelty and evidence: 对同一查询构造并审核反向标签的配对样本训练判定器；六种二分类标准 Qwen3-8B 宏平均 F1 比点标注单独训练高 2.5 点。
- Limitations and confounders: 生成式反事实可能改变多项语义属性；Workshop 接收为作者自述，不作已正式归档会议论文证据。
- Scientific routing: Primary ROUTING_ABSTAIN; Cross-cutting BGT; Framework MEAS/EG/ID/BT; primary estimand COUNTERFACTUAL_PAIR_JUDGE_BOUNDARY_VALIDITY.
- Claim ceiling: CL1; local CL2 candidate; identification I1/I2-local; transport T0.
- Evidence role: Measurement instrument. Boundary variables: 反事实最小性、Gold 可靠性、标准分布.
- SIS Impact: SHARPENS：判定器准确率和独立科学真值需要分离。 Reading priority: Worth Skimming.
- Paper/claim separation: this is provisional paper-level intake plus candidate evidence; local effects require independently verified ClaimRecords and second-coder adjudication.


Formal decision: MEASUREMENT_IDENTIFICATION_DELTA, secondary BENCHMARK_DELTA, SPEC_REVISION_CANDIDATE=NO. See [daily note](updates/2026-11-03_SIS_Daily_Literature_Update.md) and [P0 Claim audit](evidence-map/audits/SIS_P0_Reaudit_2026-11-03.md).

---

## 2026-11-04 | dated provisional study-version intake

Source window: arXiv public 2026-11-03 cs.AI listing, 816 total records / 222 new submissions. Original submission dates preserved. Ten preprints, no independently verified archival status; global October history lineage unresolved. Paper-level intake is not adjudicated Claim evidence.

| ID | Paper | Primary | Cross | Framework | Claim | Priority |
|---|---|---|---|---|---|---|
| SIS-CAND-20261104-01 | [Top-k Retrieval Leaves Memory Value Undetermined](https://arxiv.org/abs/2611.03289) | ROUTING_ABSTAIN | BGT | ID/MEAS/EG/BT | CL0 theory + CL1 empirical | Must Read |
| SIS-CAND-20261104-02 | [Can Coding Agents Sustain Continual Evolution without Forgetting?](https://arxiv.org/abs/2611.03219) | SDR | CSCI/BGT | TD/DR/ID/MEAS/BT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261104-03 | [SelfImprove-Bench: Evaluating Generalization in Self-Improving Agents](https://arxiv.org/abs/2611.02797) | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | CL1 benchmark | Must Read |
| SIS-CAND-20261104-04 | [Delivered, Not Used: Evaluating Agent Memory at Its Point of Use](https://arxiv.org/abs/2611.01718) | ROUTING_ABSTAIN | BGT | TD/MEAS/EG/ID/BT | CL1 | Must Read |
| SIS-CAND-20261104-05 | [Accessed, never disclosed: Silent access to protected health information by medical artificial intelligence agents](https://arxiv.org/abs/2611.02319) | SDR | BGT | TD/EG/ID/MEAS/BT | CL1; local CL2 candidate | Must Read |
| SIS-CAND-20261104-06 | [LEANGUARD: Lean-Verified Guardrails for Tool-Using Agents](https://arxiv.org/abs/2611.02332) | ASR | BGT | MI/DR/EG/ID/MEAS/BT | CL0 conditional formal + CL1 empirical | Must Read |
| SIS-CAND-20261104-07 | [CARE: Grounded Recursive Self-Improvement for Production Customer-Service Agents](https://arxiv.org/abs/2611.02839) | ASR | CSCI/BGT | DR/TD/EG/ID/MEAS/BT | CL1 composite | Must Read |
| SIS-CAND-20261104-08 | [Early Stopping in Large Reasoning Models: A Survey and Empirical Audit of Efficiency and Reliability](https://arxiv.org/abs/2611.00166) | ASR | BGT | DR/ID/MEAS/BT | CL1 audit | Worth Skimming |
| SIS-CAND-20261104-09 | [Exo: An Architecture for Self-Improving Systems at Runtime](https://arxiv.org/abs/2611.00463) | ASR | CSCI/BGT | DR/MI/TD/EG/MEAS/BT | CL1 composite; local candidate | Must Read |
| SIS-CAND-20261104-10 | [ScienceCUA: Resource-to-Skill Construction and Execution-Guided Skill Evolution for Scientific Computer Use Agents](https://arxiv.org/abs/2611.03238) | SCF | BGT | MI/TD/EG/ID/MEAS/BT | CL1; local candidate | Must Read |

### SIS-CAND-20261104-01 — Top-k Retrieval Leaves Memory Value Undetermined

- StudyVersionRecord: https://arxiv.org/abs/2611.03289 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 证明 top-k 共检索日志无法识别单条记忆价值；14 基准、55 配置均无单项识别；LEDGER 经主动检索使 HotpotQA 可识别比例约 0.001→0.797。
- Identification limits: 研究依赖特定 Shapley 价值定义及支持集设计；HotpotQA 准确率损失 2.6 点，可识别不等于有净收益。
- Mapping: Primary ROUTING_ABSTAIN; Cross BGT; Framework ID/MEAS/EG/BT; estimand TOPK_MEMORY_VALUE_IDENTIFIABILITY_FROM_RETRIEVAL_DESIGN.
- Evidence role: Identification limit / negative; Claim ceiling CL0 theory + CL1 empirical; I0/I1; T0.
- Boundary variables: 检索支持集、共同曝光、探索成本. Impact: SHARPENS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-02 — Can Coding Agents Sustain Continual Evolution without Forgetting?

- StudyVersionRecord: https://arxiv.org/abs/2611.03219 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 三数据集六演化顺序比较；一个模型配置的 SWE-Bench 94%→32%，下降 62 个百分点，后续优化破坏原能力。
- Identification limits: 需验证顺序、模型、预算和保留集独立性；不能泛化为所有模型必然遗忘。
- Mapping: Primary SDR; Cross CSCI/BGT; Framework TD/DR/ID/MEAS/BT; estimand SEQUENTIAL_HARNESS_EVOLUTION_BACKWARD_RETENTION_EFFECT.
- Evidence role: Negative / retention boundary; Claim ceiling CL1; local CL2 candidate; I1/I2-local; T1.
- Boundary variables: 任务顺序、执行器、版本、非回归门控. Impact: CHALLENGES. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-03 — SelfImprove-Bench: Evaluating Generalization in Self-Improving Agents

- StudyVersionRecord: https://arxiv.org/abs/2611.02797 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 游戏可控任务及 G0–G4 泛化阶梯评估自我优化是否超出训练场景；不同方法各阶梯收益不一致。
- Identification limits: 作者 G0–G4 不等于 SIS T0–T4，游戏成绩不能证明 T3 因果传输。
- Mapping: Primary ROUTING_ABSTAIN; Cross BGT; Framework MEAS/EG/ID/BT; estimand RSI_GAIN_GENERALIZATION_LADDER_CONSTRUCT_VALIDITY.
- Evidence role: Measurement / transport boundary; Claim ceiling CL1 benchmark; I1; T1.
- Boundary variables: 难度、训练/测试隔离、系统变化. Impact: SHARPENS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-04 — Delivered, Not Used: Evaluating Agent Memory at Its Point of Use

- StudyVersionRecord: https://arxiv.org/abs/2611.01718 (preprint v1; original 2026-11-01).
- Scientific novelty/evidence: MemUse 分别审查记忆交付、内容新颖性、使用与后果；8000 条 SWE-bench 执行中三种记忆系统成功率与无记忆差距均在 0.4 百分点以内。
- Identification limits: 影响标注依赖轨迹 Judge；没有随机记忆替换，不能把观察到的影响作为单条记忆因果效应。
- Mapping: Primary ROUTING_ABSTAIN; Cross BGT; Framework TD/MEAS/EG/ID/BT; estimand DELIVERED_MEMORY_OBSERVED_USAGE_AND_EFFECT_VALIDITY.
- Evidence role: Measurement / conditional null; Claim ceiling CL1; I1; T0.
- Boundary variables: 记忆冗余、交付时机、Judge 独立性. Impact: SHARPENS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-05 — Accessed, never disclosed: Silent access to protected health information by medical artificial intelligence agents

- StudyVersionRecord: https://arxiv.org/abs/2611.02319 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 合成患者 Canary 与工具调用日志识别隐藏 PHI 读取；五模型四级权限七类攻击条件，三模型发生不必要读取，执行前门控接近消除。
- Identification limits: 合成数据及构造攻击不是真实临床事故率；输出不泄漏不能证明访问合规。
- Mapping: Primary SDR; Cross BGT; Framework TD/EG/ID/MEAS/BT; estimand UNNECESSARY_PHI_TOOL_ACCESS_CONDITIONAL_POLICY_GATE_EFFECT.
- Evidence role: Viability / controlled boundary; Claim ceiling CL1; local CL2 candidate; I1/I2-local; T1.
- Boundary variables: 访问必要性、工具权限、声称授权、审计. Impact: SUPPORTS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-06 — LEANGUARD: Lean-Verified Guardrails for Tool-Using Agents

- StudyVersionRecord: https://arxiv.org/abs/2611.02332 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: Lean4 前置动作审查及可证明修复；Tau-Bench 未防护至少 33 条违规调用，防护 0 条；DTap 注入成功 57.9%→5.9%。
- Identification limits: 形式证明只覆盖已编码规则；不能证明规范完整或真实用户意图正确。
- Mapping: Primary ASR; Cross BGT; Framework MI/DR/EG/ID/MEAS/BT; estimand FORMAL_TOOL_CALL_ADMISSION_AND_PROOF_GUIDED_REPAIR_EFFECT.
- Evidence role: Formal constraints / implementation; Claim ceiling CL0 conditional formal + CL1 empirical; I0/I2-local; T1.
- Boundary variables: 规范覆盖、Fail-closed、状态、工具副作用. Impact: SUPPORTS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-07 — CARE: Grounded Recursive Self-Improvement for Production Customer-Service Agents

- StudyVersionRecord: https://arxiv.org/abs/2611.02839 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 生产自改进依据当时 SOP 版本独立盲审，分离模型与工具/技能故障，冻结模拟+离线评价+在线比较+人类批准完成准入。
- Identification limits: 多个更新机制及策略变化共同作用；摘要没有足够随机效应数字支持单独因果晋升。
- Mapping: Primary ASR; Cross CSCI/BGT; Framework DR/TD/EG/ID/MEAS/BT; estimand VERSION_CONDITIONED_GOVERNED_RSI_UPDATE_ADMISSION_VALUE.
- Evidence role: Deployment governance / implementation; Claim ceiling CL1 composite; I1; T1.
- Boundary variables: SOP 版本、历史评估、更新准入、人类审查. Impact: SHARPENS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-08 — Early Stopping in Large Reasoning Models: A Survey and Empirical Audit of Efficiency and Reliability

- StudyVersionRecord: https://arxiv.org/abs/2611.00166 (preprint v1; original 2026-10-30; 2026-11-03 listed).
- Scientific novelty/evidence: 五推理模型的共同重放协议、TITE 指标；较晚出口不保证更正确，部分提前终止后支持理由更弱。
- Identification limits: 重放不等于在线干预，成本需含停止判定与校准；同时含综述性内容。
- Mapping: Primary ASR; Cross BGT; Framework DR/ID/MEAS/BT; estimand EARLY_STOP_TOKEN_EFFICIENCY_JUSTIFICATION_VALIDITY.
- Evidence role: Measurement / stopping boundary; Claim ceiling CL1 audit; I1; T1.
- Boundary variables: 目标正确率、退出点、证据质量、预算. Impact: SHARPENS. Priority: Worth Skimming.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-09 — Exo: An Architecture for Self-Improving Systems at Runtime

- StudyVersionRecord: https://arxiv.org/abs/2611.00463 (preprint v1; original 2026-10-30; 2026-11-03 listed).
- Scientific novelty/evidence: 固定受保护的执行历史与策略激活层，允许实时修改执行政策；AppWorld/SREGym 相近正确率时模型费用下降约 35–61%。
- Identification limits: 模型费用不等于全系统成本；多个实现因素同步变化且旧能力保持未充分识别。
- Mapping: Primary ASR; Cross CSCI/BGT; Framework DR/MI/TD/EG/MEAS/BT; estimand PROTECTED_RUNTIME_POLICY_EVOLUTION_COST_ADJUSTED_VALUE.
- Evidence role: Framework / performance transfer; Claim ceiling CL1 composite; local candidate; I1/I2-local; T2-performance-only.
- Boundary variables: 保护层、工作负载、成本账、更新准入. Impact: SHARPENS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

### SIS-CAND-20261104-10 — ScienceCUA: Resource-to-Skill Construction and Execution-Guided Skill Evolution for Scientific Computer Use Agents

- StudyVersionRecord: https://arxiv.org/abs/2611.03238 (preprint v1; original 2026-11-02).
- Scientific novelty/evidence: 科学软件文档转为可执行技能与动态参考，并按成败轨迹验证更新；初始收益最多 7.23 点，演化后总收益最多 17.12 点。
- Identification limits: 文档版本、执行条件和更新预算混杂；需独立测试严格正确性。
- Mapping: Primary SCF; Cross BGT; Framework MI/TD/EG/ID/MEAS/BT; estimand SCIENTIFIC_DOCUMENTATION_TO_EXECUTABLE_SKILL_VALIDATED_VALUE.
- Evidence role: Scientific capability / implementation; Claim ceiling CL1; local candidate; I1; T1.
- Boundary variables: 文档版本、任务隔离、软件状态、规范完整性. Impact: SUPPORTS. Priority: Must Read.
- Paper-level provisional only; no CL2/CL3 promotion without second-coder evidence audit.

Formal SIS Impact Decision: MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; SPEC_REVISION_CANDIDATE=NO. Existing SCF/SDR/ASR, CSCI/BGT and thin Frameworks suffice. 115/118/127 first-coder claim re-audit in separate ledger.


---

## Provisional daily intake — 2026-11-05 (10 study-version candidates)

The study date and intake date are different. These are provisional IDs, *not* permanent SIS-LIT assignments; second coder/adjudication pending. ROUTING_ABSTAIN is a governance routing outcome, not a fourth Primary Program.

### SIS-CAND-20261105-01 — Retrieval Myopia: Why RL Search Agents Fail to Read What They Find

- StudyVersionRecord: [primary](https://aclanthology.org/2026.findings-emnlp.1713/); 2026-10 (Findings EMNLP; delayed discovery). Study identity checked against current registry.
- Novelty / evidence: 5 RL-search systems; up to 46.2% errors despite injected gold; reformatting restores up to 48.9% of those errors.
- Identification limitation and key boundary variables: Forced gold and format/attention coupling; task, model and input format.
- Primary Program: `SCF`; cross-cutting: `BGT`; Framework Capability Profile: `MI/MEAS/ID/EG/BT`.
- Primary estimand: `FORCED_GOLD_RETRIEVAL_FORMAT_CONDITIONAL_READING_EFFECT`; Claim ceiling and identification/transport: CL1; local CL2 candidate; I2-local/T1; Evidence role: Negative/boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-02 — Evaluating LLM Agents Beyond Local Edit Validity

- StudyVersionRecord: [primary](https://aclanthology.org/2026.findings-emnlp.893/); 2026-10 (Findings EMNLP; delayed discovery). Study identity checked against current registry.
- Novelty / evidence: Local-valid alloy/GB1 success 16.0%/6.8%; exhaustive 625 GB1 variants find 51.4% locally valid episodes exceed recoverability boundary.
- Identification limitation and key boundary variables: Toy/proxy landscapes; remaining budget and future action reachability.
- Primary Program: `SDR`; cross-cutting: `BGT`; Framework Capability Profile: `TD/MEAS/ID/BT`.
- Primary estimand: `BUDGET_CONDITIONAL_ARTIFACT_RECOVERABILITY`; Claim ceiling and identification/transport: CL0 finite property + CL1; I1/T0; Evidence role: Negative/boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-03 — Artifact-to-Capability: Diagnosing Breaks in Capability Formation of Self-Evolving Agents in a Controlled Environment

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.04952); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: Controlled freestyle Gomoku shows legality-only gain, 20 missed one-move wins, and later regression.
- Identification limitation and key boundary variables: Single controlled task, selected systems, checkpoint construct.
- Primary Program: `SCF`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `MI/TD/IA/MEAS/ID/BT`.
- Primary estimand: `ARTIFACT_CAPABILITY_FORMATION_CHECKPOINT`; Claim ceiling and identification/transport: CL0 definitions + CL1; I1/T0; Evidence role: Negative/construct validity.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-04 — Silent Instrument Errors Reorder Agent Leaderboards

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.04399); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: HAL and tau2 artifacts: ungraded counted failure, 13-point comparison gap closes after regrading, misattributed grader actions and duplicate cost.
- Identification limitation and key boundary variables: Selected evaluations, grader-version and coverage dependence, independent Gold required.
- Primary Program: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `MEAS/EG/ID/BT`.
- Primary estimand: `GRADER_COVERAGE_PROVENANCE_VERSION_RANKING_SENSITIVITY`; Claim ceiling and identification/transport: CL1 measurement audit; local deterministic I2/T0; Evidence role: Measurement/negative.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-05 — Verifier strength does not buy discovery quality: a pre-registered two-domain test of LLM-based automated research

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.04420); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: Prespecified two-domain 100 matched pairs each; stronger gates do not improve relative heldout discovery; posthoc pool mix +1.52 one domain.
- Identification limitation and key boundary variables: Lower tiers select near-identical candidates; mixed pool post-hoc; two domains.
- Primary Program: `ASR`; cross-cutting: `BGT`; Framework Capability Profile: `DR/MEAS/ID/EG/BT`.
- Primary estimand: `VERIFIER_TIER_X_PROPOSER_POOL_HOLDOUT_VALUE`; Claim ceiling and identification/transport: CL1 negative; local I2 candidate/T0; Evidence role: Negative/null, optimization boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-06 — What Is This Memory Useful For? Measuring Task-Conditioned Utility in Long-Term Agent Memory

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.03930); 2026-11-02 v1, newly surfaced. Study identity checked against current registry.
- Novelty / evidence: Paired exposure answer-bearing vs matched control +0.33 (95% interval +0.21,+0.46); tested scientific/software coding shows null detectable gain.
- Identification limitation and key boundary variables: Single-call recall, frozen reader, task distribution, format and placement.
- Primary Program: `SCF`; cross-cutting: `BGT`; Framework Capability Profile: `MI/MEAS/ID/EG/BT`.
- Primary estimand: `TASK_CONDITIONED_MEMORY_EXPOSURE_PAIRED_GAIN`; Claim ceiling and identification/transport: CL1; local CL2 candidate; I2-local/T1; Evidence role: Conditional mechanism/boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-07 — From AutoResearch to Continual AutoResearch: Do Agents Learn Across Tasks?

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.05108); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: Nine task families, five agents; persistent execution improves early efficiency but not consistently final held-out value.
- Identification limitation and key boundary variables: Session state, code and memory co-vary; finite task streams.
- Primary Program: `SDR`; cross-cutting: `BGT`; Framework Capability Profile: `TD/DR/MEAS/ID/EG/BT`.
- Primary estimand: `PERSISTENCE_VS_RESET_RESEARCH_EFFICIENCY_FINAL_VALUE`; Claim ceiling and identification/transport: CL1; local CL2 candidate; I2-local/T1; Evidence role: Conditional positive/negative.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-08 — Meta^2: Precomputing Reusable Knowledge for Online Harness Evolution in Long-Horizon Agents

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.05139); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: Offline precomputation and online KEEP/EVOLVE; reported Terminal-Bench 2.1 81.00%, DeepSWE 1.1 44.44% in configurations.
- Identification limitation and key boundary variables: Meta-knowledge, editing and compute coupled; train-only verifier privilege requires audit.
- Primary Program: `ASR`; cross-cutting: `BGT`; Framework Capability Profile: `DR/MI/TD/EG/MEAS/ID/BT`.
- Primary estimand: `OFFLINE_META_SKILL_ONLINE_KEEP_EVOLVE_VALUE`; Claim ceiling and identification/transport: CL1 composite; local candidate; I1/I2-local/T1; Evidence role: Regulation/implementation.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-09 — Harness-S: Learning from Sibling Harnesses for Generalizable Agent Training

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.04277); 2026-11-03 v1. Study identity checked against current registry.
- Novelty / evidence: Sibling harness rollout rescue trains shared policy then evaluates with original harness on AppWorld/SWE-Gym/DBBench.
- Identification limitation and key boundary variables: Training volume, sibling quality and switching policy confounded; T2 not T3.
- Primary Program: `SCF`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `MI/IA/DR/MEAS/ID/BT`.
- Primary estimand: `SIBLING_HARNESS_RESCUE_BASE_POLICY_TRANSFER`; Claim ceiling and identification/transport: CL1; I1/T2-performance-only; Evidence role: CSCI/transport boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.

### SIS-CAND-20261105-10 — Inter-Agent Influence: Evaluating Persuasion, Deception, and Coercion in Multi-Agent Systems

- StudyVersionRecord: [primary](https://arxiv.org/abs/2611.04556); 2026-11-03 preprint; author states NeurIPS acceptance unverified. Study identity checked against current registry.
- Novelty / evidence: Five environments; persuasion modifies overseer reject-to-approve and peer trajectories.
- Identification limitation and key boundary variables: Designed settings not deployment incidence; proceedings version unverified.
- Primary Program: `SDR`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `IA/TD/EG/MEAS/ID/BT`.
- Primary estimand: `INTER_COMPONENT_PERSUASION_OVERSIGHT_SHIFT`; Claim ceiling and identification/transport: CL1; I1/I2-local/T1; Evidence role: Viability/authority boundary.
- SIS impact: SHARPENS existing Framework and identification tests (no core revision); Priority: Must Read. The study-level metadata cannot be promoted to claim-level CL2 without a second-coder review.


## 2026-11-06 daily intake — 10 source-verified provisional candidates (first-coder screening only)

> arXiv cs.AI 2026-11-05 listing: 359 records, of which 93 new submissions; submission history and indexing/curation date are distinct. First two studies were submitted in September yet surfaced here only now; classify as delayed-indexing rather than freshly authored. Unique arXiv IDs were checked against this registry, no permanent SIS-LIT assignment. These are StudyVersionRecords, not adjudicated ClaimRecords.

### SIS-CAND-20261106-01 — Who May Overrule the Agent? Evidence-Gated Authority in LLM Review Institutions

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.05390; 2026-09-12 v1; surfaced 2026-11-05 as delayed-indexing cs.AI listing. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: 96 spatial policy + 96 transfer tasks; gate reduces corruption of already-correct proposals but keeps many valid repairs; prospective retain/replace/escalate differs sharply between Qwen and Mistral.
- Key boundaries / confounds: Author-designed binding constraint and gate predefine part of effect; two models, proposal-state and jurisdiction dependence; not general institutional safety.
- Primary routing: `ASR`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `DR/IA/EG/ID/MEAS/BT`.
- Primary estimand: `EVIDENCE_GATED_REVIEW_AUTHORITY_CORRUPTION_REPAIR_TRADEOFF`; provisional claim ceiling / identification / transport: CL1; local intervention candidate only / I2-local / T1 performance. Evidence role: Boundary, conditional intervention.
- SIS relevance: SHARPENS ASR regulation and CSCI authority; no new primitive. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-02 — Agent Harness Awareness: Turning Verified Telemetry into Operational Control for Tool-Using Agents

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.05391; 2026-09-13 v1; surfaced 2026-11-05 as delayed-indexing cs.AI listing. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: 216 matched decisions across three models: observable policy regret 4252→131 ms and single dispatch 69.4→95.8%; live fault-injection 27 decisions: 9/9 vs 5/9 success.
- Key boundaries / confounds: Tool/network health is narrow operational domain; not direct evidence for authorization, memory, economics or general workload scheduling; host telemetry remains privileged.
- Primary routing: `ASR`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `DR/TD/EG/ID/MEAS/BT`.
- Primary estimand: `VERIFIED_HOST_TELEMETRY_PRE_DISPATCH_POLICY_REGRET_EFFECT`; provisional claim ceiling / identification / transport: CL1; local CL2 candidate / I2-local / T1 limited models. Evidence role: Local mechanism/boundary.
- SIS relevance: SUPPORTS ASR condition-sensitive regulation; requires independent host-state measurements. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-03 — Verified but Vacuous: Three Failure Surfaces of LLM-Driven Verified Code Generation

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.05590; 2026-11-03 v1; newly listed 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: 99.1% verifier acceptance vs 1.9% binding certificate on HumanEval in one pipeline; structurally verified Rust outputs still fail hidden tests in 11.48% and 14.82%.
- Key boundaries / confounds: Two different pipelines/languages demonstrate distinct surfaces, not a jointly matched full causal mediation; benchmark and repair budget differ.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `MI/EG/MEAS/ID/BT`.
- Primary estimand: `VERIFIER_ACCEPTANCE_SPEC_BINDING_SEMANTIC_FIDELITY_GAP`; provisional claim ceiling / identification / transport: CL1 measurement; local formally defined predicates CL0 / I1 / T0. Evidence role: Measurement construct negative/boundary.
- SIS relevance: SHARPENS MEAS and EG specification-grounding; no novel science primitive. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-04 — Attributing Agent Failures to Their History Needs an Executed Counterfactual: Toward a Reporting Standard

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.05650; 2026-11-03 v1; surfaced 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: Proposes measured replay certificates; 24/24 same-snapshot restores agree with one another yet 9 or 20 of 24 disagree with live continuation; capturing random-stream position restores agreement.
- Key boundaries / confounds: Paper does not itself apply full proposed standard to validate substantive history-effect claims; demonstration is narrow and model/simulator specific.
- Primary routing: `SDR`; cross-cutting: `BGT`; Framework Capability Profile: `TD/ID/EG/MEAS/BT`.
- Primary estimand: `EXECUTED_HISTORY_COUNTERFACTUAL_REPLAY_CERTIFICATE_IDENTIFICATION`; provisional claim ceiling / identification / transport: CL0 reporting proposal; CL1 measured replay failure / I1-I2-local / T0. Evidence role: Identification requirement and negative control.
- SIS relevance: SHARPENS existing SDR counterfactual replay and evidence governance. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-05 — Grounded but Not Immune: Confirmation Bias in Agent-as-a-judge

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.05662; 2026-11-03 v1; surfaced 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: Across four tool-using judges and five datasets, irrelevant false prescreening note flips up to 40% of previously correct decisions; two Claude judges' harmful flips 67–75% over-trust type.
- Key boundaries / confounds: Designed authority cue and five datasets cannot estimate natural prevalence; failure-mode categories are diagnostic, not mechanistic mediation tests.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `EG/MEAS/ID/BT`.
- Primary estimand: `NONPROBATIVE_AUTHORITY_CUE_TOOL_JUDGE_VERDICT_FLIP_EFFECT`; provisional claim ceiling / identification / transport: CL1; local cue intervention CL2 candidate / I2-local / T1. Evidence role: Negative evaluator-independence boundary.
- SIS relevance: CHALLENGES naive belief that gathering decisive evidence immunizes a judge. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-06 — One Scale, Four Texts: Gaps, Overlaps and Silent Repairs in Published Grading Schemes

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.06569; 2026-11-04 v1; newly listed 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: Four retinopathy grading texts compiled to 24-variable rules; enumerated 1,425,807,360 profiles plus SMT cross-check; 927 images, one DDR conditional referral disagreement 26.8%; preregistered classifier/LLM tests.
- Key boundaries / confounds: Thickening not observed on photos, so many comparisons are undecidable; assumption-dependent precisification, specific guidelines/datasets; not clinical outcome effect.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `MI/EG/MEAS/ID/BT`.
- Primary estimand: `VERSIONED_CLINICAL_RULE_TEXT_DECISION_NON_EQUIVALENCE`; provisional claim ceiling / identification / transport: Formal conditional CL0; empirical CL1; I1-I2-local / T1 datasets. Evidence role: Negative schema/version equivalence and measurement.
- SIS relevance: SHARPENS specification completeness and versioned clinical evidence validity. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-07 — Signed, Sealed, Leaked: Trust Beyond Signature for MCP Toolchains

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.06585; 2026-11-04 v1; cross-listed cs.AI 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: Authenticated tool can leak through allowed destination; germline isolated invocation: zero observed unauthorized disclosures in 153 attacks vs 5.9–74.5% for tested baselines; formal result under isolation assumptions.
- Key boundaries / confounds: No claim about all information-flow channels; proof assumes confined copy and data-free germline; crafted attacks and baseline selection limit transport.
- Primary routing: `SDR`; cross-cutting: `CSCI/BGT`; Framework Capability Profile: `TD/IA/EG/ID/MEAS/BT`.
- Primary estimand: `DATA_ISOLATED_SIGNED_TOOL_SINK_NONINTERFERENCE_EFFECT`; provisional claim ceiling / identification / transport: Conditional formal CL0; empirical CL1/local CL2 candidate / I2-local/T0. Evidence role: Security mechanism/boundary.
- SIS relevance: SUPPORTS action-level viability; signatures do not establish behavioral safety. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-08 — Task-Efficient Agent Evaluation Using Cached Traces

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.06803; 2026-11-04 v1; newly listed 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: One task observed: trace-informed mean absolute prediction error 0.13→0.08 on SWE-bench Verified and 0.14→0.12 on Terminal-Bench 2.0, with significant Wilcoxon tests.
- Key boundaries / confounds: Predictive error on held-out system does not certify construct validity or ranking stability under unfamiliar model/harness; LLM summary features and reference pool may leak identity.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `TD/MEAS/ID/EG/BT`.
- Primary estimand: `REFERENCE_TRACE_GEOMETRY_LOW_SAMPLE_SCORE_PREDICTION_ERROR`; provisional claim ceiling / identification / transport: CL1 measurement prediction / I1 / T1 two benchmarks. Evidence role: Measurement implementation and efficiency.
- SIS relevance: FILLS MEAS instrumentation; not causal identification. Reading priority: Worth Skimming. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-09 — FrontierPhysics: Evaluating Agents for End-to-End Physics Research

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.06910; 2026-11-04 v1; newly listed 2026-11-05. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: 56 tasks authored by 42 physicists across nine domains, 22 models/26 configurations; best configuration passes at most 46 of 168 rollouts; deterministic checks + expert-authored rubrics.
- Key boundaries / confounds: Expert publication-worthiness subject to rubric differences and task selection; benchmark success not a general scientific discovery law or transport claim.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `MI/TD/EG/MEAS/ID/BT`.
- Primary estimand: `END_TO_END_SCIENTIFIC_RESEARCH_CORRECTNESS_VS_PUBLISHABILITY`; provisional claim ceiling / identification / transport: CL1 benchmark / I1 / T1 cross-domain performance only. Evidence role: Scientific capability measurement.
- SIS relevance: SHARPENS SCI research measurement, fits existing MEAS/EG. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**

### SIS-CAND-20261106-10 — BEAKER: An Expert-Curated Benchmark for Embodied Brains in Self-Driving Chemical Laboratories

- StudyVersionRecord / primary source: https://arxiv.org/abs/2611.06911; 2026-11-04 v1; newly listed 2026-11-05; author reports NeurIPS 2026 E&D Spotlight, archival version not independently matched. Source class: PREPRINT; reviewed-proceedings lineage unconfirmed where claimed.
- Core novelty / paper-level evidence: 1000 expert-created and reviewed questions across 11 image/video task types; 28 MLLMs offline single-turn; coarse procedure understanding stronger than apparatus, trajectory and action-region grounding.
- Key boundaries / confounds: Offline questions do not demonstrate safe robotic actuation, physical lab execution, or scientific discovery outcomes; peer-review listing author claim only.
- Primary routing: `ROUTING_ABSTAIN`; cross-cutting: `BGT`; Framework Capability Profile: `MI/TD/MEAS/EG/ID/BT`.
- Primary estimand: `CHEMICAL_LAB_ACTION_GROUNDING_PROCEDURAL_FEASIBILITY_CONSTRUCT`; provisional claim ceiling / identification / transport: CL1 instrument/diagnostic / I1 / T1 model families. Evidence role: Scientific/embodied measurement boundary.
- SIS relevance: SHARPENS SCF executable laboratory capability construct, no core change. Reading priority: Must Read. **No paper-level CL2/CL3 inherited; separate claim-level adjudication required.**


---

## 2026-11-07｜新文献日期限定候选（首次提交 11-04—05；11-06 列表公开）

本轮选取原始 arXiv 研究十项；对应研究版本和 Claim 证据分开，临时 ID 未分配永久编号。全部均按 PREPRINT 标记，正式同行评审版未独立核实。源页面核验、与现有 Registry arXiv ID 精确去重完成。历史 10 月 9–23 日候选仍有全局谱系欠账。

### SIS-CAND-20261107-01 — Benchmarks as Software: Terminal-Bench and the Case for Continuous Benchmarks

- StudyVersionRecord: https://arxiv.org/abs/2611.08417（v1 首次 2026-11-05，2026-11-06 公开列表，PREPRINT）。
- Primary ROUTING_ABSTAIN; cross-cutting BGT; Framework MEAS/EG/ID/BT; primary estimand `BENCHMARK_VERSION_BUDGET_CONDITIONAL_RANKING`.
- Claim ceiling / identification / transport: CL1/I1-I2local/T0; evidence role INSTRUMENT+NEGATIVE; reading priority Must Read.
- Original result/novelty: 审计Terminal-Bench 2.0发现约30%任务存在问题；2.1修订后准确率变化超过10个百分点、排名最大变化三位，时间预算改变Harness差距。
- Scientific boundary / identification: 人工门控修订有选择偏差；新评价器并非独立绝对Gold，任务修复和资源预算需正交控制。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-02 — When Verification Is Not Agreement: Cross-Agent LLM-to-Dafny Formalization

- StudyVersionRecord: https://arxiv.org/abs/2611.07073（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary SCF; cross-cutting CSCI/BGT; Framework MI/EG/MEAS/ID/BT; primary estimand `ROLE_SWAP_FORMAL_SPECIFIER_IMPLEMENTER_AGREEMENT`.
- Claim ceiling / identification / transport: CL1/I2local/T1; evidence role NEGATIVE+BOUNDARY; reading priority Must Read.
- Original result/novelty: 96份临床试验文档；同模型独立抽取仅59.3%一致；强模型担任实施者或规范者时一致率分别53.0%与14.3%，且发现直接调用谓词的验证捷径。
- Scientific boundary / identification: 形式正确不意味着独立重建或真实临床意图；角色对调改变组件能力；Workshop接收为作者声明，非正式存档。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-03 — BabyTheorist: A Benchmark for Learning to Theorize the World from Observation Alone

- StudyVersionRecord: https://arxiv.org/abs/2611.08177（v1 首次 2026-11-05，2026-11-06 公开列表，PREPRINT）。
- Primary SCF; cross-cutting BGT; Framework MI/TD/MEAS/ID/BT; primary estimand `CONTINUAL_OBSERVATIONAL_COMPOSITIONAL_THEORY_INDUCTION`.
- Claim ceiling / identification / transport: CL1/I1/T0; evidence role INSTRUMENT+NEGATIVE; reading priority Must Read.
- Original result/novelty: 隐藏组合程序连续生成状态转移，训练时不暴露规则标签、任务身份及支持集；七种基线随课程复杂度升高持续落后。
- Scientific boundary / identification: 合成DSL及课程先验限定构念；不能当作真实科学发现或跨域机制迁移。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-04 — Trust Responsive Runtime Authorization for Agentic AI with Empirical Characterization of Policy Behavior and Parameter Sensitivity

- StudyVersionRecord: https://arxiv.org/abs/2611.06996（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary ASR; cross-cutting CSCI/BGT; Framework DR/TD/MEAS/ID/BT; primary estimand `ABRUPT_VS_GRADUAL_RISK_AUTHORITY_GATE_EFFECT`.
- Claim ceiling / identification / transport: CL1/I2local/T0; evidence role NEGATIVE_BOUNDARY+POLICY; reading priority Must Read.
- Original result/novelty: 100条匹配Monte Carlo轨迹下非对称门控对突发退化迅速收紧；渐进退化下多数轨迹没有及时收权，20段中的15.9–18.9段处于过高权限。
- Scientific boundary / identification: 后者为探索性事后试验； readiness人为构造，不是独立的真实信任Gold。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-05 — Formalizing inverse problems in the age of AI: possibilities, pitfalls, and an invitation

- StudyVersionRecord: https://arxiv.org/abs/2611.06962（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary ROUTING_ABSTAIN; cross-cutting BGT; Framework MI/EG/MEAS/ID/BT; primary estimand `FORMAL_THEOREM_NATURAL_INTENT_FIDELITY`.
- Claim ceiling / identification / transport: CL0-CL1/I0-I1/T0; evidence role CONSTRUCT_WARNING; reading priority Must Read.
- Original result/novelty: AutoIP以Lean形式化逆问题与正则化理论；数学证明检查只保证形式陈述，对教科书条件过宽的案例展示规范核对必要性。
- Scientific boundary / identification: 方法论文及案例而非代表性失败率；证明有效和数学陈述符合原意须独立核查。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-06 — Autonomous AI Agents Systematically Diverge From Human Preferences in Proof Formalization

- StudyVersionRecord: https://arxiv.org/abs/2611.06995（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary SCF; cross-cutting CSCI/BGT; Framework IA/MI/MEAS/ID/BT; primary estimand `HUMAN_AGENT_PROOF_PATH_PREFERENCE_GAP`.
- Claim ceiling / identification / transport: CL1/I1/T1; evidence role INTERACTION_BOUNDARY; reading priority Worth Skimming.
- Original result/novelty: 研究九个Lean合作项目、470万定义和六千余次提交，模拟Agent与人类选择证明缺口、中心节点和复杂目标的偏好不同。
- Scientific boundary / identification: 历史人类行为不是最优Gold，模拟组件与人类资源不同；没有真实联合协作的因果效率试验。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-07 — Adapting the Process of Adaptation: Darwinian, Lamarckian, and Agent-Directed Evolution in AI

- StudyVersionRecord: https://arxiv.org/abs/2611.07048（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary ASR; cross-cutting BGT; Framework DR/MI/EG/ID/BT; primary estimand `SEARCH_EFFORT_WITH_MISSPECIFIED_OBJECTIVE_REGULATION_VALUE`.
- Claim ceiling / identification / transport: CL0/I0/T0; evidence role THEORY+NEGATIVE; reading priority Worth Skimming.
- Original result/novelty: 理论比较达尔文式、拉马克式与定向演化：当评价目标错设时，提高搜索强度可能更快收敛于错误目标。
- Scientific boundary / identification: 理论假设尚未实证推广为系统规律，须独立测量真实目标与代理指标。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-08 — KDASO: Knowledge-Data Dual-Driven Automated Skill Optimization for Liability Adjudication Tasks

- StudyVersionRecord: https://arxiv.org/abs/2611.06972（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary ASR; cross-cutting BGT; Framework DR/MI/TD/EG/ID/BT; primary estimand `SKILL_STALENESS_ALIGNMENT_ROUTING_COMPOSITE_VALUE`.
- Claim ceiling / identification / transport: CL1/I1/T2-performance; evidence role IMPLEMENTATION+TRANSFER; reading priority Worth Skimming.
- Original result/novelty: 最近裁决案例驱动技能更新，执行轨迹用于对齐改写，预算约束决定路由；作者报告相似概念转移改进8.96%。
- Scientific boundary / identification: 归纳、改写与路由共同变化，缺少独立机制中介；仅性能迁移不等于T3因果迁移。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-09 — BlockLock: Reproducible LLM Inference with Fixed Batch Geometry

- StudyVersionRecord: https://arxiv.org/abs/2611.06977（v1 首次 2026-11-04，2026-11-06 公开列表，PREPRINT）。
- Primary SCF; cross-cutting BGT; Framework MI/TD/MEAS/ID/BT; primary estimand `BATCH_COMPANION_INVARIANT_BITWISE_REPLAY_COST`.
- Claim ceiling / identification / transport: CL1/I2local/T1; evidence role REPLAY_INSTRUMENT; reading priority Must Read.
- Original result/novelty: 固定受保护请求的计算几何，保留批量prefill；五种模型、三种GPU报告在改变批次同伴后输出及Top20 logits位级一致，延迟相对基线下降约53.5%–55%。
- Scientific boundary / identification: 仅具体部署、精度与kernel合同下成立；推理数值可复现不代表完整工具/外部状态可重放。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

### SIS-CAND-20261107-10 — When Bigger Becomes Brittle: Why Compression Hurts More as Language Models Scale

- StudyVersionRecord: https://arxiv.org/abs/2611.07891（v1 首次 2026-11-05，2026-11-06 公开列表，PREPRINT）。
- Primary SCF; cross-cutting CSCI/BGT; Framework MI/IA/MEAS/ID/BT; primary estimand `MODEL_SCALE_COMPENSATION_RETRIEVAL_HEAD_DAMAGE`.
- Claim ceiling / identification / transport: CL1/I2local/T1; evidence role BOUNDARY+MECHANISM_CANDIDATE; reading priority Must Read.
- Original result/novelty: 对检索注意力头的消融损失进行被其他组件恢复与传至输出部分的分解；报告大模型补偿较弱，同等压缩伤害更明显。
- Scientific boundary / identification: 仅特定注意力头与检索任务，比较损伤和架构尺度存在边界；尚非通用系统机制。 此项主要填充现有 Framework，未触发新 Core 原语。Paper-level label 不自动成为 CL2/CL3 Claim。

---

## 2026-11-08｜Daily provisional candidate intake (6 arXiv Nov 4–5; 4 delayed archival EMNLP October)

All source IDs/titles exact-deduplicated against the preexisting Registry. These are temporary StudyVersionRecords, not permanent SIS-LIT IDs and not adjudicated ClaimRecords. Global preprint/conference lineage, Oct 9–23 backlog still unresolved.

### SIS-CAND-20261108-01 — EnvOpt: Automated Optimization for Agent Environments

- StudyVersionRecord: https://arxiv.org/abs/2611.07372; release 2026-11-05; source class PREPRINT. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 环境组织可优化；固定模型/Harness下Haiku成本-72.7%、成功率+14.34个百分点；向Opus迁移成本-68.1%、成功率+1.34个百分点
- Routing: Primary **SCF**, cross-cutting **CSCI/BGT**; Framework Capability **MI/DR/MEAS/ID/EG/BT**.
- Primary estimand: STATIONARY_ENVIRONMENT_INTERVENTION_COST_SUCCESS_EFFECT; provisional claim/identification/transport: CL1 / I2-local candidate / T2-performance-only. Evidence role: Mechanism candidate / environment representational intervention; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 环境内容、可见性与资源消耗共同变化；跨执行器表现并非T3机制因果迁移
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-02 — Who Should Know What? Empirical Information Design for Multi-Agent LLM Economies

- StudyVersionRecord: https://arxiv.org/abs/2611.07667; release 2026-11-05; source class PREPRINT. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 在固定模型与交互规则下改变信息披露，10个模型与三种市场；细化披露对不同模型的收益影响方向相反，交易收益示例98%→91%和72%→86%
- Routing: Primary **SCF**, cross-cutting **CSCI/BGT**; Framework Capability **MI/IA/DR/MEAS/ID/BT**.
- Primary estimand: DISCLOSURE_GRANULARITY_BY_COMPONENT_CAPABILITY_WELFARE_EFFECT; provisional claim/identification/transport: CL1 / I2-local candidate / T1. Evidence role: Negative boundary / CSCI; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 经济模拟的策略响应、信任与价格机制不能直接外推现实；需明确信息×模型交互
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-03 — PharmAgents2: Towards Autonomous End-to-End Drug Discovery

- StudyVersionRecord: https://arxiv.org/abs/2611.07653; release 2026-11-05; source class PREPRINT. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 121项科研决策任务、3项端到端任务；报告三个研究中的人类执行实验支持部分候选，包括LpxH抑制活性和JAK1候选活性
- Routing: Primary **SCF**, cross-cutting **CSCI/BGT**; Framework Capability **MI/TD/DR/EG/MEAS/ID/BT**.
- Primary estimand: AI_GUIDED_DRUG_DISCOVERY_HUMAN_EXPERIMENTAL_VALIDATION; provisional claim/identification/transport: CL1 system / I1 / T1; local chemical claim independently supported but not system CL2. Evidence role: Scientific capability / external physical evidence; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 人类实验支持特定化学事实，不代表系统科研决策链整体因果优越；缺候选选择偏倚与独立跨实验室复现控制
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-04 — MCPHallu: Benchmarking Reasoning, Execution, and Memory Hallucinations in MCP Agents

- StudyVersionRecord: https://arxiv.org/abs/2611.07689; release 2026-11-05; source class PREPRINT. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 358任务、36个生产MCP服务容器、14模型、5012轨迹；不可达目标类得分0.458，成功23.2%；故障子类型间排名不同
- Routing: Primary **SDR**, cross-cutting **BGT**; Framework Capability **TD/EG/MEAS/ID/BT**.
- Primary estimand: INFEASIBLE_GOAL_RECOGNITION_BY_STRUCTURAL_FAILURE_SUBTYPE; provisional claim/identification/transport: CL1 / I1 / T1. Evidence role: Failure measurement / negative stopping boundary; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 预构建触发器非自然事件发生率；不同子类得分不代表因果故障源或真实工作净收益
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-05 — PromptOps: Iterative Prompt Optimization for LLM-as-a-Judge Systems

- StudyVersionRecord: https://arxiv.org/abs/2611.07123; release 2026-11-04; source class PREPRINT; CONVERSATIONS author claim unconfirmed. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 将何时更新、选择哪种优化器、选择反馈和如何修改Judge Prompt分开；对五种优化路径报告受控评分分布漂移后的恢复，最优选择依赖环境
- Routing: Primary **ASR**, cross-cutting **BGT**; Framework Capability **DR/MEAS/ID/EG/BT**.
- Primary estimand: JUDGE_DRIFT_OPERATOR_TIMING_FEEDBACK_POLICY_VALUE; provisional claim/identification/transport: CL1 / I1 / T1. Evidence role: Adaptive regulation / operator selection implementation; reading priority **Worth Skimming**.
- Identification, key boundary variables and transport caution: 参考评分漂移不等于真实任务质量漂移；同源优化与评估循环潜在污染且预算未独立识别
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-06 — Goal Revelation as a Bridge Between Information-Theoretic Empowerment and Capability-Based Human Power

- StudyVersionRecord: https://arxiv.org/abs/2611.07247; release 2026-11-04; source class PREPRINT. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: Markov game中比较目标达成能力、目标识别互信息与行动通道容量；给出信息高但真实目标达成能力低的反例
- Routing: Primary **ASR**, cross-cutting **CSCI/BGT**; Framework Capability **DR/IA/MEAS/ID/BT**.
- Primary estimand: HUMAN_GOAL_REVELATION_VS_ATTAINMENT_POWER; provisional claim/identification/transport: CL0 theory / CL1 simulation / I0-I1 / T0. Evidence role: Theoretical boundary / human agency; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 理论界依赖目标分布、可观测性与策略空间；随机环境模拟不证明部署可行性
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-07 — ICE: Intervention-Consistent Explanation Evaluation with Statistical Grounding for LLMs

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.1055/; release 2026-10 delayed discovery; source class PEER_REVIEWED_FINDINGS_EMNLP_2026. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 7模型、4任务，删除与检索填补算子、同大小随机对照；28个比较中5个跨越正证据门槛，最大44个百分点差异
- Routing: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**; Framework Capability **MI/MEAS/ID/EG/BT**.
- Primary estimand: EXPLANATION_FAITHFULNESS_INTERVENTION_OPERATOR_RANDOM_BASELINE; provisional claim/identification/transport: CL1 / I1-I2-local / T1. Evidence role: Measurement identification / negative; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 干预算子改变输入分布；解释忠实性为operator-conditioned测量，不是普遍心理机制
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-08 — CausalPrism: Component-Level Evaluation of Intervention-Based Causal Reasoning in Large Language Models

- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.1294/; release 2026-10 delayed discovery; source class PEER_REVIEWED_FINDINGS_EMNLP_2026. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 14模型，分解因果先验、状态前推、信念更新和能动性敏感；信念更新最强模型正确率仅0.613
- Routing: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**; Framework Capability **MEAS/ID/BT**.
- Primary estimand: SCM_CAUSAL_PRIOR_FORWARD_TRACE_BELIEF_UPDATE_CAPABILITY; provisional claim/identification/transport: CL1 / I1 / T1. Evidence role: Component measurement / negative; reading priority **Worth Skimming**.
- Identification, key boundary variables and transport caution: 单模型推理能力子项不是SIS的复合系统第一性Primitive；叙事DAG场景与真实系统能力有差距
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-09 — PASTABench: Proactive Assessment of Sequential Trajectories for Agent Safety

- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.2281/; release 2026-10 delayed discovery; source class PEER_REVIEWED_EMNLP_2026. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 1139条多步轨迹、16模型，标注Earliest Signal与Trigger；最强模型最佳干预时机准确率40.74%，词汇中和后部分模型退化
- Routing: Primary **ASR**, cross-cutting **BGT**; Framework Capability **TD/DR/MEAS/ID/EG/BT**.
- Primary estimand: EARLIEST_SIGNAL_TRIGGER_INTERVENTION_TIMING_VALIDITY; provisional claim/identification/transport: CL1 / I1 / T1. Evidence role: Regulation timing / safety measurement; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 标注时间窗口不是唯一可干预时间；词汇中和可能改变语义；离线准确率不是在线干预净价值
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.

### SIS-CAND-20261108-10 — Lazy Grounding: Attacking Search Agents with Factual Evidence

- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.2600/; release 2026-10 delayed discovery; source class PEER_REVIEWED_EMNLP_2026. Exact study-lineage adjudication pending; October items are delayed discoveries, not new publication on Nov 8.
- Novelty and direct primary evidence: 将只对相邻改写问题正确的事实注入当前检索库；12组模型-任务平均准确率下降5.9个百分点，最多17.3点
- Routing: Primary **SDR**, cross-cutting **BGT**; Framework Capability **TD/MI/EG/MEAS/ID/BT**.
- Primary estimand: FACTUAL_NEIGHBOR_EVIDENCE_WRONG_QUERY_APPLICATION_EFFECT; provisional claim/identification/transport: CL1 / local CL2 candidate / I2-local / T1. Evidence role: Evidence applicability / negative boundary; reading priority **Must Read**.
- Identification, key boundary variables and transport caution: 攻击控制检索库/文本位置；可识别局部误用效应，不保证唯一注意力或证据绑定中介
- SIS impact: sharpens/fills existing SCF/SDR/ASR + CSCI/BGT and MEAS/ID/EG capabilities; source-level effect does not establish universal mechanism, T3 transport, or a new SIS primitive.




---

## 2026-11-09 daily intake｜Nine distinct delayed-indexing papers, one existing-version update

All peer-reviewed research below was published in **October 2026** and newly qualified for Registry on 2026-11-09; these are NOT 2026-11-09 newly published items. P0 first coder details under `literature/evidence-map/audits/SIS_P0_Reaudit_2026-11-09.md`. These candidate entries are paper-level only and cannot promote whole-study maturity.

### SIS-CAND-20261109-01 — Causal Decomposition of LLM Agent Failure via Oracle-State Intervention
- StudyVersionRecord: https://aclanthology.org/2026.realm-1.6/; October 2026; REALM_2026_WORKSHOP; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 420条WebArena失败轨迹、2模型；失败后替换真实结构化状态恢复率低于10%，持续oracle-state使成功率提升19–38%；58–74%故障在上下文与环境恢复后仍失败。
- Routing: Primary **SDR**, cross-cutting **BGT**, Framework **MI/TD/ID/MEAS/BT**; Estimand `POSTHOC_VS_CONTINUOUS_ORACLE_STATE_RECOVERY_EFFECT`.
- Provisional claim **CL1; local CL2 candidate**, ID **I2-local**, transport **T1**, role **Negative mechanism boundary / state-timing intervention**.
- Boundaries/identification: 失败后修复与从一开始持续给予真实状态是不同制度；oracle-state是不可自然获得的特权信息；条件效应不证明全部失败机制。
- Impact **SHARPENS SDR：后验修复价值与连续状态治理价值分离。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-02 — When Failures Propagate: Causal Failure Attribution in Agentic Retrieval-Augmented Generation
- StudyVersionRecord: https://aclanthology.org/2026.realm-1.46/; October 2026; REALM_2026_WORKSHOP; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 在多跳检索中注入已知故障并重执行后缀；覆盖率型诊断在首跳准确0.91、后二跳0.00，过度依赖首跳启发式。
- Routing: Primary **SDR**, cross-cutting **BGT**, Framework **MI/TD/ID/EG/MEAS/BT**; Estimand `INJECTED_FAULT_HOP_CONDITIONAL_LOCALIZATION_ACCURACY`.
- Provisional claim **CL1; local intervention target CL2 candidate**, ID **I2-local**, transport **T0**, role **Intervention benchmark / negative late-hop attribution**.
- Boundaries/identification: MuSiQue三跳与特定模型样本；已知注入位置是实验真值，但诊断正确率不是修复效应；后缀重执行会改变故障显现。
- Impact **SHARPENS SDR：注入位置、传播位置、故障被观察位置和实际修复收益分离。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-03 — Beyond Consensus: Downward Bias and Role Asymmetry in Multi-Agent LLM Judges for Subjective Evaluation
- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.243/; October 2026; FINDINGS_EMNLP_2026; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 六种Judge模型、两类主观评分任务；多人共识反而降低人类对齐；三种消融将主要退化指向严格/宽松角色不对称及严格立场主导。
- Routing: Primary **ROUTING_ABSTAIN**, cross-cutting **BGT**, Framework **IA/MEAS/ID/EG/BT**; Estimand `ASYMMETRIC_JUDGE_ROLE_CONSENSUS_HUMAN_ALIGNMENT_EFFECT`.
- Provisional claim **CL1; local CL2 candidate**, ID **I2-local**, transport **T1**, role **Negative evaluator-construct / role intervention**.
- Boundaries/identification: 人类评分自身有不确定性；角色、评分共享和讨论轮次均可改变分布；不能推断所有共识机制失效。
- Impact **SHARPENS MEAS/CSCI：共识一致性不等于独立人类真值。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-04 — The Autonomy Tax: Defense Training Breaks LLM Agents
- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.52/; October 2026; EMNLP_2026_MAIN; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 97项代理任务、1000次对抗提示；防御训练模型在干净任务上产生动作拒绝或无效调用，部分设置的超时99%而基线13%；作者称存在表面模式捷径学习。
- Routing: Primary **SDR**, cross-cutting **CSCI/BGT**, Framework **TD/IA/MEAS/ID/BT**; Estimand `DEFENSE_TRAINING_BENIGN_EXECUTION_AND_ATTACK_ROBUSTNESS_TRADEOFF`.
- Provisional claim **CL1; local intervention candidate**, ID **I1/I2-local**, transport **T1**, role **Negative viability / cascading failure boundary**.
- Boundaries/identification: 模型训练和推理配置不同，不能完全归因于单一训练信号；攻击集不代表自然风险；99%仅为指定测试条件。
- Impact **SHARPENS SDR/CSCI：安全性更新必须联合监测任务能力与长时程失效放大。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-05 — Leaving the Past Behind: Breaking Personalization Inertia in Long-Term LLM Agents
- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.1744/; October 2026; FINDINGS_EMNLP_2026; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: Pivot以轨迹独立证据判断既有偏好是否失效，并在局部回滚时保留可信前缀、重写后缀，报告个性化准确性和轨迹忠实度改善。
- Routing: Primary **SDR**, cross-cutting **BGT**, Framework **TD/DR/EG/ID/MEAS/BT**; Estimand `STALE_PREFERENCE_ROLLBACK_CURRENT_INTENT_CONFORMANCE_EFFECT`.
- Provisional claim **CL1; local CL2 candidate**, ID **I1/I2-local**, transport **T1**, role **Temporal evidence boundary / local recovery**.
- Boundaries/identification: 历史偏好标签和当前意图Gold存在时效歧义；回滚策略、外部证据、修复均同时改变；缺真实长时程决策净收益。
- Impact **SHARPENS SDR：历史记忆可成为当前意图的错误约束，需状态时效和纠偏价值测量。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-06 — Causal Episodic Memory for Feedback-Driven Agent Repair
- StudyVersionRecord: https://aclanthology.org/2026.realm-1.70/; October 2026; REALM_2026_WORKSHOP; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 仅检索先前已结束episode的正负修复记忆；Spider执行准确率66.34→69.79%，BIRD 47.35→48.44%；Spider配对证据较清楚，BIRD较弱。
- Routing: Primary **SCF**, cross-cutting **BGT**, Framework **MI/TD/EG/ID/MEAS/BT**; Estimand `PRIOR_FINALIZED_REPAIR_MEMORY_CONDITIONAL_SQL_EXECUTION_GAIN`.
- Provisional claim **CL1; local CL2 candidate**, ID **I1/I2-local**, transport **T1**, role **Conditional benefit / modest negative-null subtype evidence**.
- Boundaries/identification: Oracle辅助的真实答案反馈不一定生产可得；类型化检索与非类型检索未可靠区分；训练和运行成本应独立计。
- Impact **SHARPENS SCF：记忆效果是任务、Schema局部性与反馈制度条件性的。**; priority **Worth Skimming**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-07 — Aligning Progress and Feasibility: A Neuro-Symbolic Dual Memory Framework for Long-Horizon LLM Agents
- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.227/; October 2026; FINDINGS_EMNLP_2026; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 分别构造语义进度记忆与从失败转移合成的可执行可行性检查函数，在ALFWorld、WebShop、TextCraft报告组合改进。
- Routing: Primary **SDR**, cross-cutting **BGT**, Framework **MI/TD/DR/EG/ID/MEAS/BT**; Estimand `GLOBAL_PROGRESS_VS_LOCAL_FEASIBILITY_CONSTRAINT_EFFECT`.
- Provisional claim **CL1**, ID **I1**, transport **T1**, role **Composite implementation / failure-mode distinction**.
- Boundaries/identification: 同时增加上下文与逻辑检查，未独立证实各模块因果中介；检测到的可行性条件可能不完整。
- Impact **FILLS EXISTING FRAMEWORK：进度漂移与局部可行性违反应分别测量。**; priority **Worth Skimming**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-08 — Drift No More: Spectral Locking for Long-Horizon Open-Weight Multi-Agent AI
- StudyVersionRecord: https://aclanthology.org/2026.emnlp-main.1796/; October 2026; EMNLP_2026_MAIN; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 14,832标注轮次中三种漂移相关；联合task-role-state子空间的消融损失7.2分，等秩随机子空间损失0.8分；报告跨模型和扰动收益。
- Routing: Primary **SDR**, cross-cutting **CSCI/BGT**, Framework **MI/TD/IA/ID/MEAS/BT**; Estimand `TASK_ROLE_STATE_SUBSPACE_INTERVENTION_LONG_HORIZON_RETENTION`.
- Provisional claim **CL1; local CL2 candidate**, ID **I2-local**, transport **T2-performance-only**, role **Representation intervention / conditional mechanism candidate**.
- Boundaries/identification: 隐藏态相关与激活操纵不必然证明单一中介；只适用于可访问内部状态模型；迁移为性能级非T3。
- Impact **SHARPENS CSCI/SDR：可观测轨迹漂移与表示层控制作用需分开。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### SIS-CAND-20261109-09 — IterInject: Indirect Prompt Injection Against LLM Agents via Feedback-Guided Iterative Optimization
- StudyVersionRecord: https://aclanthology.org/2026.findings-emnlp.808/; October 2026; FINDINGS_EMNLP_2026; qualified 2026-11-09 (delayed discovery, not November publication).
- Evidence: 诊断反馈驱动的间接注入优化在AgentDojo/InjectAgent优于静态方法；在Claude Code 9个目标中5个完全成功，附带三项注意力层干预。
- Routing: Primary **SDR**, cross-cutting **BGT**, Framework **TD/DR/EG/ID/MEAS/BT**; Estimand `ADAPTIVE_UNTRUSTED_INPUT_ATTACK_SUCCESS_AND_ATTENTION_PATHWAY`.
- Provisional claim **CL1; local CL2 mechanism candidate pending**, ID **I1/I2-local**, transport **T1**, role **Adversarial boundary / mechanism candidate**.
- Boundaries/identification: 构造攻击成功率不能代表实际发生率；训练预算与攻击迭代次数可能不同；注意力通路证据需独立复核，不能直接晋升CL3。
- Impact **SHARPENS SDR/EG：不可信输入的自适应攻击与证据权限边界。**; priority **Must Read**; independently adjudicated ClaimRecord pending.

### StudyVersionRecord reconciliation: existing SIS-LIT-004 DCFA
- Legacy: https://arxiv.org/abs/2609.04749 ; peer-reviewed October 2026: https://aclanthology.org/2026.emnlp-main.1887/ ; same underlying study, NO NEW STUDY ID, no CL promotion from publication status alone. Official source abstract supports a step-level diagnostic metric; causal-inspired reasoning does NOT independently establish executed do(step) mechanism.
