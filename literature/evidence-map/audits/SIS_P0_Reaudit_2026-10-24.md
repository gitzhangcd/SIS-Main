# SIS P0 Claim-Level Re-Audit｜2026-10-24

**Authority:** SIS v0.3.1 Master; Evidence Map P0 v0.1; ClaimRecord v0.1.
**First coder:** assistant (primary-source audit). **Second coder/adjudication:** PENDING. Prior Registry CL2 and I2 labels are only triage metadata; no final claim-level promotion here.

## SIS-LIT-010｜Control-Data Flow Separation

**Primary:** https://arxiv.org/abs/2609.00621 ; §3 typed control vs mutable data; §4-5 experiments, Tables 1-3. Four settings BBH, review generation, synthetic/industry insurance. Bundle includes frozen prompt slot, type validation, retries/fallback.

| Claim | Precise contrast / anchor | SIS semantic routing | Identification, boundary, decision |
|---|---|---|---|
| 010-C1 | §4-5, separated framework vs naive optimizer; review Jaccard 31.0 to 44.4 | SCF/BGT, MI/MEAS/BT, STRUCTURED_CONTROL_PACKAGE_PERFORMANCE_EFFECT | CL1, I1/T1. Bundled protocol, parser and optimization context; CONFIRM performance, not mechanism. |
| 010-C2 | §3 + §5, typed validated control and eventual protocol-validity in studied setups | SCF/BGT, MI/ID/MEAS/BT, TYPED_PROTOCOL_VALIDITY_EFFECT | Local CL2 candidate, I2/T0. Deterministic schema enforcement, but 'eventual' measure includes fallback/retry and conditions on acceptance. SPLIT local effect. |
| 010-C3 | §5 Table 3, hypothesis that control-data separation by itself mediates all performance gain | SCF/CSCI/BGT, MI/IA/ID, SEPARATION_MEDIATED_TASK_GAIN | CL0 mechanistic hypothesis; no independent mediator intervention. DEMOTE overbroad causality. |

## SIS-LIT-122｜Where Does Exactly-Once Live?

**Primary:** https://arxiv.org/html/2609.29095v1 ; §4 LIMBO sandbox, §5 fault regime, §6 limitations. 25,930 episodes, 9 models, 3 harnesses, 2 contracts, 15 recovery conditions, 12 fault types; simulations and shared gateway limit external validity.

| Claim | Precise contrast / anchor | SIS semantic routing | Identification, boundary, decision |
|---|---|---|---|
| 122-C1 | §4-5 readable acknowledgement loss vs in-flight / redelivery errors; duplicate outcomes | SDR/CSCI/BGT, TD/IA/ID/MEAS/BT, FAULT_REGIME_CONDITIONAL_DUPLICATION_EFFECT | Controlled fault intervention local CL2 candidate, I2/T1 sandbox. Explained-variance model/contract shares are not causal mediation. SPLIT by fault regime. |
| 122-C2 | §5 key availability / idempotency contract, 28% to 4% duplicates in defined experiments | SDR/CSCI/BGT, TD/ID/MEAS/BT, IDEMPOTENCY_KEY_CONTRACT_EFFECT | Local CL2 candidate, I2/T1. Depends on key adoption, delays and ledger outcome, not a global rate. RETAIN conditional candidate. |
| 122-C3 | theorem and §6 late commit without bounded in-flight time: no verification-only exactly-once guarantee | SDR/BGT, TD/ID/BT, LATE_COMMIT_VERIFICATION_IMPOSSIBILITY_BOUNDARY | CL0 formal conditional boundary, not empirical CL7 system law. CONFIRM theoretical conditionality. |

## SIS-LIT-128｜Canopy

**Primary:** https://arxiv.org/abs/2609.30017 ; §3 theory, §4 Table 1 and Appendix D/E; matched-budget routing, top-k identification, inference search, caching, trimming. Performance outcomes and resource currencies differ by application.

| Claim | Precise contrast / anchor | SIS semantic routing | Identification, boundary, decision |
|---|---|---|---|
| 128-C1 | §4 matched budgets; top-10 recall .370 vs .126, 1000 model pool | ASR/BGT, DR/MEAS/BT, MULTIFIDELITY_PROBING_POLICY_VALUE | CL1 global; local CL2 candidate, I2/T2 performance. Same-budget comparisons, but no universal effect across tasks. CONFIRM/SPLIT. |
| 128-C2 | §3 Theorem 3 regret bound with additive number-of-discontinuities term K | ASR/BGT, DR/BT, DISCONTINUITY_CONDITIONAL_REGRET_BOUND | CL0 formal theorem dependent on detection / Lipschitz / dispersion assumptions; not empirical mechanism. SPLIT theoretical boundary. |
| 128-C3 | §4/Appendix E: search gain changes with task/model; GSM8K near null (-.005) vs MATH / GPQA positive | ASR/CSCI/BGT, DR/IA/MEAS/BT, COMPONENT_CAPABILITY_BY_ROUTER_EFFECT | CL1 boundary; localized CL2 candidate, I1/I2, T1/T2 performance only. Full interaction not isolated. CONFIRM conditionality. |

## Review governance

Nine separated claim units, three studies. **No final CL2 or CL3 promotion.** Second coder, independent full-text table extraction and adjudication are pending; no T3 causal transport or T4 mechanism invariance. Preserve previously finalized queue claims; do not overwrite by paper-level assignments. For these rows the queue should record FIRST_CODER_REAUDITED_2026-10-24_PENDING_SECOND_CODER while keeping final_claim_level and transport_final unchanged.

**Formal Impact:** MEASUREMENT_IDENTIFICATION_DELTA; secondary BENCHMARK_DELTA; no Scientific Core revision.
