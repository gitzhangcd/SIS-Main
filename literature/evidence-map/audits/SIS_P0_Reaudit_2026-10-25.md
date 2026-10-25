# SIS P0 Claim-Level Re-Audit｜2026-10-25

**Authority:** SIS v0.3.1, Evidence Map P0 v0.1, ClaimRecord v0.1. **First coder:** assistant. **Independent second coder:** PENDING; **adjudication:** PENDING. Paper-level Registry and I/T tags are triage metadata, not final scientific claims.

## SIS-LIT-024 — MA-Evolve / Equal Inference Cost

**Primary:** https://arxiv.org/html/2609.04217v1 ; §V–VII, Figure 1 and iso-call setup. Frozen shared Qwen2.5-7B, ALFWorld n=134, WebShop n=80; model-call metering; differing token/task costs and task choice limit transport.

| Claim ID | Source anchor and bounded estimand | Scientific route / evidence | First-coder determination |
|---|---|---|---|
| 024-C1 | §VI / Fig 1: single executor evolution vs unevolved +0.097 on ALFWorld, McNemar p=.021. `FROZEN_EXECUTOR_EVOLUTION_EFFECT` | SCF, CSCI/BGT, MI/IA/ID/MEAS/BT; I2-local/T0; intervention/performance | CL1 global; **local CL2 candidate** with frozen backbone and call budget. Confirmation of restricted effect, not a general law. |
| 024-C2 | §VI / Fig 1: full team .769 vs single .754, p=.80, evaluation calls x1.8; WebShop .185 vs .245, p=.12. `ISO_CALL_TEAM_ADDED_VALUE` | SCF, CSCI/BGT, IA/MEAS/ID/BT; I1/I2-local/T1; NEGATIVE/NULL | **CL1 null/boundary**; p=.80 does **not** establish equivalence or universal zero causal effect. Reject broad 'teams never help' interpretation. |
| 024-C3 | §VII leave-one-in: executor absorbs gains, planner/critic low influence; `ROLE_MEDIATED_PERFORMANCE_EFFECT` | SCF, CSCI/BGT, IA/ID/MEAS; I1/T0 | CL1 diagnostic association; **CL0 mechanistic mediation hypothesis**, since role deletion, search budget and evolved prompt content are coupled. Split/demote mechanism claim. |

## SIS-LIT-070 — Belief State Geometry In-Context

**Primary:** https://arxiv.org/abs/2609.17376 ; abstract, 40 HMMs and six model families; extended technical analysis available but original full tables/appendices still require coder inspection. Explicit **FULLTEXT_TABLE_AUDIT_PENDING**. This is a triage-level first coder split, not formal proof of mediation.

| Claim ID | Source anchor and bounded estimand | Scientific route / evidence | First-coder determination |
|---|---|---|---|
| 070-C1 | Abstract: linear probes decode HMM belief states, peak R² .83–.99; `HMM_BELIEF_STATE_DECODABILITY` | SCF, BGT, MEAS/ID/BT; I1/T1; representation measurement | **CL1 confirmed as reported measurement**, not causal use of representation. Probe access alone cannot prove online computation uses it. |
| 070-C2 | Abstract: steering/patching probe subspace changes prediction relative to controls; `BELIEF_SUBSPACE_PERTURBATION_EFFECT` | SCF, BGT, MI/ID/MEAS/BT; I2-local/T0; intervention | **Local CL2 candidate only**; full-text manipulation controls/side effects and counterfactual mediator specificity must be re-audited. |
| 070-C3 | Author interprets approximate Bayesian belief representation as mechanism mediating in-context learning; `BELIEF_STATE_MEDIATION` | SCF, BGT, MI/ID/MEAS; I1/I2-local/T0 | **CL0 mechanism hypothesis / CL3 NOT established**; decodability plus steering does not isolate full computation of belief-state mediator; restricted HMM setting. |

## SIS-LIT-084 — ContrAgent / Symbolic Temporal Contracts

**Primary:** https://arxiv.org/html/2609.18128v1 ; §3-6, Table 1, online/offline comparisons and Appendix. The deterministic automaton guarantees apply to grounded predicates, stated assumptions and monitor interface, not unobservable semantic intent.

| Claim ID | Source anchor and bounded estimand | Scientific route / evidence | First-coder determination |
|---|---|---|---|
| 084-C1 | §3-4 / Table 1: LTLf contracts compile to DFA for online gating and offline labeling of same observed trace; `TEMPORAL_CONTRACT_CONFORMANCE` | SCF, BGT, MI/EG/MEAS/BT; I0/T0; formal engineering | **CL0 formal conditional claim**; correctness of compilation does not prove predicates cover true unsafe events. |
| 084-C2 | §5-6 online guard vs guardrail baselines, deterministic verdicts and much lower per-call latency; `CONTRACT_GATE_EXECUTION_EFFECT` | SDR (safety execution) with BGT, TD/MI/ID/MEAS/BT; I1/I2-local/T1 | CL1 performance; **local CL2 candidate** if identical input/contract and budgets controlled; combined predicate/monitor/gate implementation remains bundled. |
| 084-C3 | §6 tool-call trace offline labeling vs LLM judge; `DETERMINISTIC_TRACE_EVALUATION_VALIDITY` | ROUTING_ABSTAIN with BGT, MEAS/EG/ID/BT; I1/T1; instrument | **CL1 evaluator reliability**, not independent ground truth when hidden semantic violations escape predicates. Split measurement from enforcement. |

## Governance and impact

**9 separated scientific claims / 3 studies**, including explicit null/negative finding, local intervention candidates, formal claims and downgraded overbroad causal/mediator interpretations. **No final CL2, CL3, T3 or T4 promotion.** All prior finalized queue records remain intact; only these three pending rows get `FIRST_CODER_REAUDITED_2026-10-25_PENDING_SECOND_CODER` in the audit-status field. Second coder must check version-specific main tables, allocation/manipulations, evaluator independence, budget/conditioning, and boundary/transport before adjudication.

**SIS Impact:** `MEASUREMENT_IDENTIFICATION_DELTA`, secondary `BENCHMARK_DELTA`; Scientific Core frozen. Negative evidence preserved; not a fourth Program or a new Framework primitive.
