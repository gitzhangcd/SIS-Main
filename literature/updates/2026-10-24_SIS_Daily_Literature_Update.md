# SIS Daily Literature Update — 2026-10-24

**SIS authority:** v0.3.1 (frozen); **source batch:** arXiv cs.AI list for 2026-10-23 (103 new submissions; 366 total listed), arXiv submissions 2026-10-21/22 UTC. **Prior daily coverage:** 2026-10-23 (not yet on main). **Publication class:** 10 preprints (including nonarchival workshop version); no new peer-reviewed publication claim.

## Provenance and lineage gate

`main` registry v1.3 predates outstanding 2026-10-09–23 daily staging materials. The following are **dated provisional candidate IDs only** (not permanent SIS-LIT IDs), checked against the canonical 145-record registry and the 2026-10-23 brief titles; pending prior-batch reconciliation and version-lineage checks. Do not claim full retrospective deduplication until outstanding files are merged. No CL2/CL3 automatically inherited; levels below are first-pass at claim granularity.

## New primary-source candidates

| Candidate | Primary-source DOI/ID | Primary | Cross-cutting | Framework | Estimand | Maturity | Identification | Transport | Evidence role | Priority |
|---|---|---|---|---|---|---|---|---|---|---|
| SIS-CAND-20261024-01 ARATest｜From Prose to Properties | [arXiv:2610.30495](https://arxiv.org/abs/2610.30495) | ROUTING_ABSTAIN | BGT | MEAS/EG/ID/BT | CLAIM_PROPERTY_EXECUTION_VALIDITY | CL1 | I1 | T0 | MEASUREMENT_INSTRUMENT | Must Read |
| SIS-CAND-20261024-02 Can LLMs Improve Their Own Harness? | [arXiv:2610.30499](https://arxiv.org/abs/2610.30499) | SCF | CSCI/BGT | MI/TD/ID/MEAS/BT | HELDOUT_HARNESS_REVISION_VALUE | CL1 | I1 | T1 | NEGATIVE_BOUNDARY | Must Read |
| SIS-CAND-20261024-03 RoleFlow / SECPO | [arXiv:2610.30429](https://arxiv.org/abs/2610.30429) | ASR | CSCI/BGT | DR/IA/ID/MI/MEAS/BT | SINGLE_EDIT_STRUCTURAL_REGULATION_VALUE | CL1; local CL2 candidate | I2(local) | T2 performance only | LOCAL_INTERVENTION | Must Read |
| SIS-CAND-20261024-04 BELT / Same Beliefs, Different Policies | [arXiv:2610.30450](https://arxiv.org/abs/2610.30450) | ASR | BGT | DR/MEAS/ID/BT | PRICE_CONDITIONAL_TERMINATION_POLICY_VALUE | CL1 | I1 | T2 performance only | REGULATION_BOUNDARY | Must Read |
| SIS-CAND-20261024-05 MemPABench / Why Bother Me Again? | [arXiv:2610.30485](https://arxiv.org/abs/2610.30485) | ROUTING_ABSTAIN | BGT | EG/DR/MEAS/BT | PREFERENCE_CONDITIONAL_ACTION_VALIDITY | CL1 descriptive | I1 | T0 | MEASUREMENT_NEGATIVE | Must Read |
| SIS-CAND-20261024-06 Multi-Actor Event Worlds | [arXiv:2610.30488](https://arxiv.org/abs/2610.30488) | SDR | CSCI/BGT | TD/ID/MEAS/BT | OTHER_ACTOR_UNOBSERVABILITY_EFFECT | CL1 | I1 | T1 | NEGATIVE_BOUNDARY | Must Read |
| SIS-CAND-20261024-07 What the Trace Shows and What the Label Says | [arXiv:2610.30491](https://arxiv.org/abs/2610.30491) | ROUTING_ABSTAIN | BGT | TD/ID/MEAS/EG/BT | TRACE_LABEL_CONSTRUCT_VALIDITY | CL1 | I1 | T0 | MEASUREMENT_NEGATIVE | Must Read |
| SIS-CAND-20261024-08 AgentTriage | [arXiv:2610.30738](https://arxiv.org/abs/2610.30738) | ROUTING_ABSTAIN | BGT | TD/ID/EG/MEAS/BT | REPLAYABLE_GROUNDED_DIAGNOSIS_VALIDITY | CL1 | I1 | T1 | MEASUREMENT_INSTRUMENT | Must Read |
| SIS-CAND-20261024-09 Externalise the Memory | [arXiv:2610.30478](https://arxiv.org/abs/2610.30478) | SCF | CSCI/BGT | MI/EG/MEAS/BT | EXTERNAL_RETRIEVAL_VS_WEIGHT_DISTILLATION_EFFECT | CL1; local CL2 candidate | I2(local) | T0 | NEGATIVE_BOUNDARY | Must Read |
| SIS-CAND-20261024-10 Feedback That Backfires in Games | [arXiv:2610.30205](https://arxiv.org/abs/2610.30205) | SDR | CSCI/BGT | TD/ID/EG/MEAS/BT | FAILED_ACTION_REEXPOSURE_EFFECT | CL1; local CL2 candidate | I2(local) | T1 | NEGATIVE_BOUNDARY | Worth Skimming |

## First-pass evidence notes

### SIS-CAND-20261024-01 — ARATest｜From Prose to Properties

- **Primary record / publication:** arXiv:2610.30495, preprint. 
- **Scientific re-code:** ROUTING_ABSTAIN; cross-cutting BGT; capabilities MEAS/EG/ID/BT; primary estimand CLAIM_PROPERTY_EXECUTION_VALIDITY; CL1, I1, T0.
- **Evidence role and result:** MEASUREMENT_INSTRUMENT. 54/243 claims faithful declared; 32 holds, 8 violations, 14 inconclusive; 553 seeded faults/19 valid controls; declaration coverage is limited; no automatic causal claim.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-02 — Can LLMs Improve Their Own Harness?

- **Primary record / publication:** arXiv:2610.30499, preprint. 
- **Scientific re-code:** SCF; cross-cutting CSCI/BGT; capabilities MI/TD/ID/MEAS/BT; primary estimand HELDOUT_HARNESS_REVISION_VALUE; CL1, I1, T1.
- **Evidence role and result:** NEGATIVE_BOUNDARY. 27 lineages; two revisions +2.80 held-out RHAE points, 95% CI [-1.44,7.35]; development/held-out gap; cannot infer universally ineffective self-improvement.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-03 — RoleFlow / SECPO

- **Primary record / publication:** arXiv:2610.30429, preprint. 
- **Scientific re-code:** ASR; cross-cutting CSCI/BGT; capabilities DR/IA/ID/MI/MEAS/BT; primary estimand SINGLE_EDIT_STRUCTURAL_REGULATION_VALUE; CL1; local CL2 candidate, I2(local), T2 performance only.
- **Evidence role and result:** LOCAL_INTERVENTION. Single-edit no-edit same-state contrast; 7 benchmarks, +4.7 points over strongest competitor; edit selection and policy learning remain coupled.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-04 — BELT / Same Beliefs, Different Policies

- **Primary record / publication:** arXiv:2610.30450, preprint. 
- **Scientific re-code:** ASR; cross-cutting BGT; capabilities DR/MEAS/ID/BT; primary estimand PRICE_CONDITIONAL_TERMINATION_POLICY_VALUE; CL1, I1, T2 performance only.
- **Evidence role and result:** REGULATION_BOUNDARY. Token reductions 41%/51% on OOD math without accuracy loss; learned belief reused across token prices, code and agentic transfer not causal transport.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-05 — MemPABench / Why Bother Me Again?

- **Primary record / publication:** arXiv:2610.30485, preprint. 
- **Scientific re-code:** ROUTING_ABSTAIN; cross-cutting BGT; capabilities EG/DR/MEAS/BT; primary estimand PREFERENCE_CONDITIONAL_ACTION_VALIDITY; CL1 descriptive, I1, T0.
- **Evidence role and result:** MEASUREMENT_NEGATIVE. Four simulated users, 14 preferences, 99 sessions; retrieval memory did not exceed no-memory; file memory can overapply preferences; synthetic-user boundary.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-06 — Multi-Actor Event Worlds

- **Primary record / publication:** arXiv:2610.30488, preprint. 
- **Scientific re-code:** SDR; cross-cutting CSCI/BGT; capabilities TD/ID/MEAS/BT; primary estimand OTHER_ACTOR_UNOBSERVABILITY_EFFECT; CL1, I1, T1.
- **Evidence role and result:** NEGATIVE_BOUNDARY. Diplomacy and market event logs; prediction strong with all actors' observed actions but weak when others unobserved; actor-action confounding and counterfactual action support limit attribution.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-07 — What the Trace Shows and What the Label Says

- **Primary record / publication:** arXiv:2610.30491, preprint. 
- **Scientific re-code:** ROUTING_ABSTAIN; cross-cutting BGT; capabilities TD/ID/MEAS/EG/BT; primary estimand TRACE_LABEL_CONSTRUCT_VALIDITY; CL1, I1, T0.
- **Evidence role and result:** MEASUREMENT_NEGATIVE. Six models x 30 cases; human verification agreement 67/81 and 14 disagreements; step/token limits alter observable correctness; detector label not ground truth.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-08 — AgentTriage

- **Primary record / publication:** arXiv:2610.30738, preprint. 
- **Scientific re-code:** ROUTING_ABSTAIN; cross-cutting BGT; capabilities TD/ID/EG/MEAS/BT; primary estimand REPLAYABLE_GROUNDED_DIAGNOSIS_VALIDITY; CL1, I1, T1.
- **Evidence role and result:** MEASUREMENT_INSTRUMENT. Five runtimes, 120 adjudicated cases; grounded joint diagnosis .858, required evidence coverage .966; relies on normalized traces, trusted pre-run oracle and overlay provenance.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-09 — Externalise the Memory

- **Primary record / publication:** arXiv:2610.30478, preprint. 
- **Scientific re-code:** SCF; cross-cutting CSCI/BGT; capabilities MI/EG/MEAS/BT; primary estimand EXTERNAL_RETRIEVAL_VS_WEIGHT_DISTILLATION_EFFECT; CL1; local CL2 candidate, I2(local), T0.
- **Evidence role and result:** NEGATIVE_BOUNDARY. Pre-registered matched protocols: weight distillation +1 pp nonsignificant and underpowered; attaching retrieval +34 pp; harder-task +6 pp CI crosses zero; nonarchival workshop not peer-reviewed archival.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

### SIS-CAND-20261024-10 — Feedback That Backfires in Games

- **Primary record / publication:** arXiv:2610.30205, preprint. 
- **Scientific re-code:** SDR; cross-cutting CSCI/BGT; capabilities TD/ID/EG/MEAS/BT; primary estimand FAILED_ACTION_REEXPOSURE_EFFECT; CL1; local CL2 candidate, I2(local), T1.
- **Evidence role and result:** NEGATIVE_BOUNDARY. Fixed controlled probes, 8 small models, illegal move record raises repetition preference G=-1.38 nats/token; does not generalize to losing moves or every model.
- **Claim ceiling:** no identified CL3 mediation or T3/T4 causal transport; performance, local controlled contrasts and benchmark validity must not be conflated.

## P0 queue advancement

First coder separately re-audited **SIS-LIT-010**, **SIS-LIT-122**, **SIS-LIT-128** into nine claim-level decisions. Details: `literature/evidence-map/audits/SIS_P0_Reaudit_2026-10-24.md`. No final CL2/CL3 promotion; second coder/adjudication pending. The existing queue is authoritative for final labels.

## Benchmark / measurement proposals

1. **Claim property → executable falsifier → reproducible witness** with explicit inconclusive state (ARATest); separation between authored claims and verifiers.
2. **Harness adaptation evaluation:** fixed development/held-out tasks, matched budget, full lineage, capability retention, and confidence intervals.
3. **Single-edit no-edit regulation:** same-state, matched-information paired intervention with action cost and cross-executor stratification.
4. **Trace detector validity:** same trace, human Gold and counterfactual tool-output corruption; separately report trace observation, detector label, impact, budget censoring.
5. **Memory use:** fixed weights × external retrieval × task/preference drift with over-application and negative transfer measures.
6. **Other-actor dynamics:** observed-all-actor vs partially observed multi-actor event prediction, cost-calibrated decision utility.
7. **Adaptive stopping:** oracle hindsight vs learned belief vs price-adapted policy, with net utility and tail failures.

## Formal SIS Impact Decision

**PRIMARY:** `MEASUREMENT_IDENTIFICATION_DELTA`; **SECONDARY:** `BENCHMARK_DELTA`; **ScientificCoreDelta:** 0; **SPEC_REVISION_CANDIDATE:** NO.

Genuine pressure: independent claim/test validity, detector construct validity, controlled edit attribution, and negative performance/retention results. Current SCF/SDR/ASR, CSCI/BGT, and MI/TD/DR/IA/BT/MEAS/ID/EG can express all selected estimands. No scientific-core or program addition justified.

## Source-class safeguard

Community articles are discovery-only and do not independently promote claims. Literature claims are not final Gold; all proposed causal interpretations require primary-text verification of allocation, confounds and manipulation checks.
