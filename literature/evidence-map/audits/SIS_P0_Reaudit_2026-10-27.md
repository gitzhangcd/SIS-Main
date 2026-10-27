# SIS P0 Claim-Level Re-Audit｜2026-10-27

**Scientific authority:** SIS v0.3.1 and SIS-LEM-P0-v0.1 ClaimRecord. First-coder source-level review of three high-priority candidate studies; **second coder / adjudication pending**. Claim routing by estimand, not paper title. Every local CL2 candidate is provisional. No automatic inherited CL2/CL3.

## SIS-LIT-055 — When Agents Slow Down: Understanding LLM Agents' Test-Time Strategies via Elo-per-token Analysis
**Study version:** https://arxiv.org/abs/2609.15309 (research source; audit 2026-10-27). **Evidence anchors:** arXiv abstract and reported study design/results; PDF tables not used to promote causal level. Independent second-coder: PENDING.

| Claim ID | Primary-source anchor | Primary | Framework | Estimand | First-coder qualification / decision | I / T |
|---|---|---|---|---|---|---|
| 055-C1 | Abstract: four agents × four open-ended benchmarks; Elo-per-token curves | ASR | DR/MEAS/BT | `TEST_TIME_ELO_PER_TOKEN_CURVE` | CL1 descriptive: diminishing marginal gains relative to independent sampling | I1/T1 |
| 055-C2 | Abstract: split 100M-token budget at scaling inflection on FrontierCS Polyomino Packing | ASR | DR/ID/MEAS/BT | `SESSION_SPLIT_POLICY_NET_VALUE` | local CL2 candidate: +264 Elo vs one long session; +355 vs ten shorter sessions; policy/selection context narrow | I2-local/T0 |
| 055-C3 | Abstract: human contestants' superlinear contest-time improvement | ROUTING_ABSTAIN | MEAS/BT | `HUMAN_AGENT_CONTINUAL_LEARNING_COMPARABILITY` | CL0 mechanism hypothesis; cross-population trajectories not matched or causal learning proxy | I0/T0 |

**Non-inflation check:** independent outcome validation, baseline fidelity, timing, complete resource budget, relevant noninterference and transport domain are not all established. Final claim maturity, intervention mediation and independent adjudication stay pending.

## SIS-LIT-107 — Passes Alone, Fails Together: Benchmarking Semantic Coordination in Parallel LLM-Agent Development
**Study version:** https://arxiv.org/abs/2609.25396 (research source; audit 2026-10-27). **Evidence anchors:** arXiv abstract and reported study design/results; PDF tables not used to promote causal level. Independent second-coder: PENDING.

| Claim ID | Primary-source anchor | Primary | Framework | Estimand | First-coder qualification / decision | I / T |
|---|---|---|---|---|---|---|
| 107-C1 | Abstract: 417 mined Django pairs/834 runs after grading correction | SDR | TD/IA/MEAS/ID/BT | `OBSERVED_PARALLEL_PATCH_INTERFERENCE_PREVALENCE` | CL1 conditional negative: only 1 observed interference, not general safety guarantee | I1/T1 |
| 107-C2 | Abstract: controlled 12-helper Django tasks, blind merge vs oracle message | SDR | TD/IA/ID/MEAS/BT | `CONTROLLED_SEMANTIC_INTERFERENCE_AND_INFORMATION_EFFECT` | local CL2 candidate: 97% constructed interference; descriptive change message recovers 82%; intervention depends on oracle message | I2-local/T0 |
| 107-C3 | Abstract: claim that semantic coordination failure prevalent in production | ROUTING_ABSTAIN | ID/MEAS/BT | `CONSTRUCTED_TO_FIELD_PREVALENCE_TRANSPORT` | CL0 unsupported extrapolation: constructed prevalence not population estimate | I0/T0 |

**Non-inflation check:** independent outcome validation, baseline fidelity, timing, complete resource budget, relevant noninterference and transport domain are not all established. Final claim maturity, intervention mediation and independent adjudication stay pending.

## SIS-LIT-124 — Who Holds the Pen? Let Specifications, Not Agents, Sign Off
**Study version:** https://arxiv.org/abs/2609.29921 (research source; audit 2026-10-27). **Evidence anchors:** arXiv abstract and reported study design/results; PDF tables not used to promote causal level. Independent second-coder: PENDING.

| Claim ID | Primary-source anchor | Primary | Framework | Estimand | First-coder qualification / decision | I / T |
|---|---|---|---|---|---|---|
| 124-C1 | Abstract: 509 source-grounded task directions/7 models | ROUTING_ABSTAIN | MI/EG/MEAS/BT | `SPECIFICATION_UNDERSTANDING_EXECUTION_GAP` | CL1 descriptive: 79.6%–86.4% instructions satisfied; completion claims exceed official pass by 28.7–37.9 points | I1/T0 |
| 124-C2 | Abstract: SpecHarness versioned source-linked obligation state, runtime mediation | SCF | MI/EG/ID/MEAS/BT | `SPEC_AUTHORITY_RUNTIME_COMPLIANCE_EFFECT` | CL1 framework bundle, potential local CL2 candidate pending table and matched contrast; cannot assert isolated specification authority mediation | I1/T1 |
| 124-C3 | Abstract: state/authority separation as complete semantic-compliance guarantee | ROUTING_ABSTAIN | EG/ID/MEAS/BT | `SPECIFICATION_COMPLETENESS_SAFETY_BOUND` | CL0 formal/semantic boundary hypothesis: source-linked obligations cannot capture unexpressed subjective requirements | I0/T0 |

**Non-inflation check:** independent outcome validation, baseline fidelity, timing, complete resource budget, relevant noninterference and transport domain are not all established. Final claim maturity, intervention mediation and independent adjudication stay pending.

## Decisions and outstanding tests

- SIS-LIT-055: distinguish measured performance-vs-token trajectories, a particular controlled session-split strategy, and unsupported claims of universal continual learning. Token-bounded reference does not fix all optimization costs.

- SIS-LIT-107: explicitly separate rare interference in *reviewed mined* PRs from high interference in *constructed* interface breaks. Oracle communication recovers constructed cases but does not estimate real-time message-policy value. Keep numerators/denominators and the corrected same-test-set grader.

- SIS-LIT-124: distinguish observed specification compliance gaps, a bundled versioned runtime framework effect, and absolute semantic safety guarantees. Subjective/implicit requirements are out of scope of the compiled obligation set.

**First-coder action:** mark only these three rows as re-audited/pending second coder in P0 queue. **Final fields remain PENDING.** No CL3, T3 or T4 claimed; ScientificCoreDelta=0.
