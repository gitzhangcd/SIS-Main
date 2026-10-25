# SIS Daily Literature Update — 2026-10-25

**Authority:** SIS v0.3.1 (Scientific Core frozen). **Discovery window:** since the 2026-10-24 brief; latest public arXiv cs.AI Friday 2026-10-23 batch, including previously unselected submissions from 2026-10-22/23; Sunday 2026-10-25 is the review date, not a paper publication date.

**Source classes:** ten arXiv preprints. Post-Audit Mirage states NeurIPS 2026 workshop acceptance but has not been promoted to an independently verified archival peer-reviewed publication. No other archival paper or community commentary was used to elevate claim level.

## Qualification and lineage

Canonical master register remains **145 permanent SIS-LIT records**; the 2026-10-24 section contains ten dated provisional candidates. Current ten identifiers are **provisional only**, matched against the permanent table and the 2026-10-24 candidates by normalized title/arXiv ID. Older 2026-10-09–23 local staged studies still require reconciliation before assigning permanent IDs. No same-ID preprint/conference duplicate created.

**Evidence boundary:** Friday arXiv abstract and available primary HTML used for first-pass metadata and claim screening; papers without full methods/table audit remain CL1 or CL2 candidate only. Formal and observed results are split. No final causal promotion without independent coding, provenance and adjudication.

## Ten primary-source discoveries

| Provisional ID | Primary study | Primary program | Cross-cutting | Framework profile | Primary estimand | Claim maturity | Identification | Transport | Evidence role |
|---|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261025-01 | [EpiSEM-Bench: Evaluating Safety and Evidence Recovery in LLM Agents under Missing Evidence](https://arxiv.org/abs/2610.31650) | SDR | BGT | TD/ID/MEAS/EG/BT | `CRITICAL_EVIDENCE_OMISSION_FAILURE_EFFECT` | CL1; local CL2 candidate | I2(local) | T1 | MEASUREMENT_NEGATIVE |
| SIS-CAND-20261025-02 | [Post-Audit Mirage: Identifiability Limits of Offline Agent Verification](https://arxiv.org/abs/2610.31130) | ROUTING_ABSTAIN | BGT | ID/MEAS/EG/BT | `OFFLINE_VERIFIER_IDENTIFIABILITY_BOUND` | CL0 theoretical; CL1 empirical | I0/I1 | T0 | IDENTIFICATION_LIMIT |
| SIS-CAND-20261025-03 | [Simulated Control Evals](https://arxiv.org/abs/2610.31593) | ROUTING_ABSTAIN | BGT | MEAS/ID/BT/EG | `SIMULATED_CONTROL_EVAL_PREDICTIVE_VALIDITY` | CL1 | I1 | T2 performance only | MEASUREMENT_INSTRUMENT |
| SIS-CAND-20261025-04 | [RIDAR: Safeguarding Research Integrity in Autonomous Research Agents](https://arxiv.org/abs/2610.31372) | ASR | BGT | DR/TD/EG/ID/MEAS/BT | `RUNTIME_RESEARCH_INTEGRITY_REGULATION_EFFECT` | CL1; local intervention candidate pending full audit | I1/I2(local) | T0 | INTEGRITY_MEASUREMENT_INTERVENTION |
| SIS-CAND-20261025-05 | [Conservative Meta-Agent Search: Architecture Adaptation under Non-Stationarity](https://arxiv.org/abs/2610.31436) | ASR | CSCI/BGT | DR/IA/ID/MEAS/BT | `SHADOW_REPLAY_ARCHITECTURE_PROMOTION_NET_VALUE` | CL1; local CL2 candidate | I2(local) | T0 | REGULATION_BOUNDARY |
| SIS-CAND-20261025-06 | [Certified Execution Harness for Agentic AI](https://arxiv.org/abs/2610.31376) | ASR | BGT | DR/MI/EG/ID/MEAS/BT | `SAFE_SUPERVISOR_LEAST_INTRUSIVE_POLICY_VALUE` | CL0 formal; CL1 example | I0/I1 | T0 | FORMAL_BOUNDARY |
| SIS-CAND-20261025-07 | [ADAPT for Science: A Multi-Agent System for Self-Evolving Scientific Optimization](https://arxiv.org/abs/2610.30851) | ASR | CSCI/BGT | DR/MI/MEAS/BT | `CONSTRAINED_SCIENTIFIC_SEARCH_POLICY_VALUE` | CL1 | I1 | T2 performance only | IMPLEMENTATION_BOUNDARY |
| SIS-CAND-20261025-08 | [LLM Multi-Agent Systems Are Vulnerable to Herding and Runaway Cascades](https://arxiv.org/abs/2610.30769) | SDR | CSCI/BGT | TD/IA/ID/MEAS/BT | `CUMULATIVE_SOCIAL_SIGNAL_CASCADE_EFFECT` | CL1; local CL2 candidate | I2(local) | T1 | NEGATIVE_BOUNDARY |
| SIS-CAND-20261025-09 | [SCOPE: Compiling Natural-Language Policies into Neurosymbolic Predicate Programs](https://arxiv.org/abs/2610.31062) | SCF | BGT | MI/EG/ID/MEAS/BT | `NEUROSYMBOLIC_POLICY_COMPILATION_EFFECT` | CL1 | I1 | T2 performance only | FRAMEWORK_IMPLEMENTATION |
| SIS-CAND-20261025-10 | [Adaptive Skill Granularity for Coding Agents](https://arxiv.org/abs/2610.31461) | ASR | BGT | DR/TD/MI/ID/MEAS/BT | `ACTION_GRANULARITY_ROUTING_RECOVERY_VALUE` | CL1; controlled recovery candidate pending full audit | I1/I2(local) | T0 | RECOVERY_BOUNDARY |

## Claim-first evidence notes

### SIS-CAND-20261025-01 — EpiSEM-Bench: Evaluating Safety and Evidence Recovery in LLM Agents under Missing Evidence

- **Primary provenance:** https://arxiv.org/abs/2610.31650 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** SDR; cross-cutting BGT; Framework TD/ID/MEAS/EG/BT; primary estimand `CRITICAL_EVIDENCE_OMISSION_FAILURE_EFFECT`; CL1; local CL2 candidate; I2(local), T1.
- **Observed evidence / confounding / boundary:** 300 matched safe/unsafe pairs, six domains, ten models. Omission safety and recovery differ; benchmark-specific independent audit; full causal mechanism and external deployment transfer unproven.
- **Interpretation:** MEASUREMENT_NEGATIVE; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-02 — Post-Audit Mirage: Identifiability Limits of Offline Agent Verification

- **Primary provenance:** https://arxiv.org/abs/2610.31130 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ROUTING_ABSTAIN; cross-cutting BGT; Framework ID/MEAS/EG/BT; primary estimand `OFFLINE_VERIFIER_IDENTIFIABILITY_BOUND`; CL0 theoretical; CL1 empirical; I0/I1, T0.
- **Observed evidence / confounding / boundary:** Paired lifecycles are indistinguishable to offline verification but have opposing deployment truth; favorable live group-labeled monitoring can distinguish, rare/missing groups can remain unresolved. Workshop-accepted per author; not archival publication verification.
- **Interpretation:** IDENTIFICATION_LIMIT; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-03 — Simulated Control Evals

- **Primary provenance:** https://arxiv.org/abs/2610.31593 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ROUTING_ABSTAIN; cross-cutting BGT; Framework MEAS/ID/BT/EG; primary estimand `SIMULATED_CONTROL_EVAL_PREDICTIVE_VALIDITY`; CL1; I1, T2 performance only.
- **Observed evidence / confounding / boundary:** LinuxArena source of executed outcomes; 5 monitors, 5%-budget RMSE 3.6pp simulated vs 10.1pp BashArena. Simulator fidelity and task distribution shift bound validity; no causal invariance.
- **Interpretation:** MEASUREMENT_INSTRUMENT; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-04 — RIDAR: Safeguarding Research Integrity in Autonomous Research Agents

- **Primary provenance:** https://arxiv.org/abs/2610.31372 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ASR; cross-cutting BGT; Framework DR/TD/EG/ID/MEAS/BT; primary estimand `RUNTIME_RESEARCH_INTEGRITY_REGULATION_EFFECT`; CL1; local intervention candidate pending full audit; I1/I2(local), T0.
- **Observed evidence / confounding / boundary:** 14 research-integrity violation types; expert gold 60 trajectories, F1=.852; 300 wild trajectories, runtime intervention reduces remaining violations 36.8%. Detector-derived outcome, task interference and independent validity require audit.
- **Interpretation:** INTEGRITY_MEASUREMENT_INTERVENTION; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-05 — Conservative Meta-Agent Search: Architecture Adaptation under Non-Stationarity

- **Primary provenance:** https://arxiv.org/abs/2610.31436 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ASR; cross-cutting CSCI/BGT; Framework DR/IA/ID/MEAS/BT; primary estimand `SHADOW_REPLAY_ARCHITECTURE_PROMOTION_NET_VALUE`; CL1; local CL2 candidate; I2(local), T0.
- **Observed evidence / confounding / boundary:** 96 simulated streams; oracle-regret .116→.104, held-out utility .44→.48; per-update false-promotion 3.4%, sealed rerun 4.8%. Search-inclusive cost highest, designed simulator; no deployed causal transport.
- **Interpretation:** REGULATION_BOUNDARY; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-06 — Certified Execution Harness for Agentic AI

- **Primary provenance:** https://arxiv.org/abs/2610.31376 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ASR; cross-cutting BGT; Framework DR/MI/EG/ID/MEAS/BT; primary estimand `SAFE_SUPERVISOR_LEAST_INTRUSIVE_POLICY_VALUE`; CL0 formal; CL1 example; I0/I1, T0.
- **Observed evidence / confounding / boundary:** Petri-net contracts and maximally permissive supervisor; safe execution conditional on four assumptions. Replanning-loop can make conventional supervisor more intrusive than a stricter alternative; conceptual formal property is not deployment proof.
- **Interpretation:** FORMAL_BOUNDARY; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-07 — ADAPT for Science: A Multi-Agent System for Self-Evolving Scientific Optimization

- **Primary provenance:** https://arxiv.org/abs/2610.30851 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ASR; cross-cutting CSCI/BGT; Framework DR/MI/MEAS/BT; primary estimand `CONSTRAINED_SCIENTIFIC_SEARCH_POLICY_VALUE`; CL1; I1, T2 performance only.
- **Observed evidence / confounding / boundary:** Eight unseen gravitational-wave detector topologies; fixed simulator budget, mean loss .204±.101; 54.9% lower than best classical baseline. Initial-condition selection, concentration and optimizer evolution bundled.
- **Interpretation:** IMPLEMENTATION_BOUNDARY; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-08 — LLM Multi-Agent Systems Are Vulnerable to Herding and Runaway Cascades

- **Primary provenance:** https://arxiv.org/abs/2610.30769 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** SDR; cross-cutting CSCI/BGT; Framework TD/IA/ID/MEAS/BT; primary estimand `CUMULATIVE_SOCIAL_SIGNAL_CASCADE_EFFECT`; CL1; local CL2 candidate; I2(local), T1.
- **Observed evidence / confounding / boundary:** Music-Lab-inspired independent exposure vs cumulative-recommendation conditions; runaway cascades beyond intrinsic appeal. Social-recommendation domain and LLM population models limit transport.
- **Interpretation:** NEGATIVE_BOUNDARY; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-09 — SCOPE: Compiling Natural-Language Policies into Neurosymbolic Predicate Programs

- **Primary provenance:** https://arxiv.org/abs/2610.31062 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** SCF; cross-cutting BGT; Framework MI/EG/ID/MEAS/BT; primary estimand `NEUROSYMBOLIC_POLICY_COMPILATION_EFFECT`; CL1; I1, T2 performance only.
- **Observed evidence / confounding / boundary:** Compiles policy to executable neural/deterministic predicates, uses adversarial counterexamples; author reports highest average task accuracy and executor performance transfer. Program, training data and adversarial optimization coupled.
- **Interpretation:** FRAMEWORK_IMPLEMENTATION; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.

### SIS-CAND-20261025-10 — Adaptive Skill Granularity for Coding Agents

- **Primary provenance:** https://arxiv.org/abs/2610.31461 (new/preprint; source date per arXiv), first coder 2026-10-25.
- **Scientific semantics:** ASR; cross-cutting BGT; Framework DR/TD/MI/ID/MEAS/BT; primary estimand `ACTION_GRANULARITY_ROUTING_RECOVERY_VALUE`; CL1; controlled recovery candidate pending full audit; I1/I2(local), T0.
- **Observed evidence / confounding / boundary:** Deterministic coding protocol; macro execution efficient when applicable, brittle under mismatch; dynamic macro-to-micro fallback recovers injected failures. Requires independent cross-runtime verification.
- **Interpretation:** RECOVERY_BOUNDARY; scientific program/framework filling, not a new primitive. No paper-level label inherits canonical CL2/CL3 or T3/T4.


## P0 claim-level backlog advanced

First-coder split review of **SIS-LIT-024 (MA-Evolve), SIS-LIT-070 (Belief State Geometry), SIS-LIT-084 (ContrAgent)** creates **9 separately scoped claims** with primary-source anchors and maturity ceilings; see [audit](../evidence-map/audits/SIS_P0_Reaudit_2026-10-25.md). Second-coder/adjudication remains PENDING; queue status updated only, historical finalized decisions preserved.

## Benchmark and conformance opportunities

1. **Missing Critical Evidence × Action Legality:** matched safe/unsafe worlds, independent audit of fact acquisition, refusal, and useful completion (EpiSEM).
2. **Indistinguishable Offline Audit × Fresh Outcomes:** require monitored group-level post-deployment evidence or abstain (Post-Audit Mirage).
3. **Policy Control Simulation Calibration:** task distribution shift, executed ground truth, monitor effects, simulator fidelity (Simulated Control Evals).
4. **RIV Detection × Remediation Non-Regression:** separate detector F1, unobserved misconduct, task utility and intervention net cost (RIDAR).
5. **Paired Shadow-Replay Promotion Gate:** switching cost, false-promotion, canary, reversal, state drift and search-inclusive resources (CMAS).
6. **Formal Supervisor × Replanning Costs:** compare maximal permissiveness, actual retry count, task utility and least-intrusive safe action (Certified Harness).
7. **Constrained Science Optimization:** fixed physical evaluation budget, unseen topologies, initial-state selection × search-policy ablations (ADAPT).
8. **Social Feedback × Inter-agent Influence:** randomize social-count visibility, monitor cascade, intrinsic quality and recovery (Herding).
9. **Policy DSL Compiler × Independent Oracle:** separate typed predicate accuracy, compiler correctness, program expressiveness, policy drift (SCOPE).
10. **Macro/Micro Recovery:** macro suitability, controlled failure injection and resource-matched fallback (Skill Granularity).

## Technical/community discovery-only

Industry engineering articles (e.g., Databricks MemCurrent, published 2026-10-21) can guide search but are not independent scientific replication. No community source elevates any CL today.

## Formal SIS Impact Decision

**PRIMARY:** `MEASUREMENT_IDENTIFICATION_DELTA`  
**SECONDARY:** `BENCHMARK_DELTA`  
**ScientificCoreDelta:** 0; **SPEC_REVISION_CANDIDATE:** NO.

Genuine pressure concerns evidence recoverability, offline/deployment identifiability, verifier construct validity, reliable adaptive promotion, research integrity and safety constraints, not new irreducible Primary Programs or Framework Capabilities. SCF/SDR/ASR + CSCI/BGT and MI/TD/DR/IA/BT/MEAS/ID/EG already represent all proposed estimands. **T3/T4 not established.**

## Provenance caveats

An arXiv listing/abstract does not warrant final claim-level causal promotion; author-reported numbers are qualified by their study-specific estimand, evaluator and environment. No noise-only core revision. No old local candidate files are marked merged as a consequence of this daily update.
