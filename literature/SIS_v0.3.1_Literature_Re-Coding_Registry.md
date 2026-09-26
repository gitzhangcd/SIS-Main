# SIS v0.3.1 Literature Re-Coding Registry

## System Intelligence Science Evidence Map｜ARSO Research Stream Re-Coding

**Registry version:** `v1.2`  
**SIS authority:** `System Intelligence Science v0.3.1`  
**Date:** `2026-09-26`  
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

- **Total coded items:** `121`
- **Primary Program:** SCF `47` · SDR `25` · ASR `48` · Routing Abstain `1`
- **Framework capability occurrences:** DR `64` · MI `54` · ID `31` · TD `27` · MEAS `31` · EG `26` · IA `21` · BT `22`
- **Transport coding:** T0 `48` · T1 `58` · T2 `15` · **T3 `0` · T4 `0`**

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
| SIS-LIT-004 | DCFA: Dual-view Causal-inspired Attribution for Failure Reasoning in LLM-based Multi-agent Systems | arXiv:2609.04749 (preprint) | `P2/SDR` | `ASR` | `ID; IA` | `PROPAGATION_EFFECT` | `CL1→CL2 candidate` | `I1/I2` / `T0` | Attribution mechanism — Supports dependency-aware attribution; causal language should remain bounded by intervention evidence. |
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
| SIS-LIT-077 | Chronicle: Cut-Point Replay for Regression Testing of LLM Agents | 2026 preprint | `P2/SDR` | `ASR` | `TD; ID; EG` | `RECOVERY_EFFECT` | `CL2` | `I2` / `T0` | Counterfactual replay instrument — Controlled cut-point intervention with immutable boundary envelopes. |
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

## 9. Version decision

**Registry conclusion:** the current corpus supports continued use of SIS v0.3.1 without a Scientific Core revision. The immediate priority is to expand benchmark fixtures, causal identification, component-capability interaction experiments, and transportability tests rather than to create additional first-principles objects or Programs.

```math
SIS\ v0.3.1\ Core\Delta = 0
```

```math
Benchmark\ /\ Experiment\ Portfolio\Delta > 0
```