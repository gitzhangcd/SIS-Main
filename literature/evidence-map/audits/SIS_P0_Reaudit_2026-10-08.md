# SIS P0 Claim-Level Re-Audit — 2026-10-08

This is a durable **claim-level audit supplement**, not a replacement for the master SIS_P0_Audit_Queue.csv. The master CSV remains pending synchronization.

| Study | Claim unit | Primary / estimand | Claim-level decision | Identification / boundary |
|---|---|---|---|---|
| SIS-LIT-003 AutoSaddler | Overall harness-update package | SDR / RECOVERY_EFFECT | CL1 CONFIRMED | I1; multiple benchmarks but bundled mechanism; T1 |
| SIS-LIT-003 AutoSaddler | Debugging, targeted patch and validation components | ASR / POLICY_VALUE | CL2 CANDIDATE | I1/I2; dev-set and budget confounding not fully audited |
| SIS-LIT-004 DCFA | Step attribution accuracy | SDR / DIAGNOSTIC_ATTRIBUTION_ACCURACY | CL1 CONFIRMED | I1; Who&When and trace observability; T0 |
| SIS-LIT-004 DCFA | Causal error propagation | SDR / PROPAGATION_EFFECT | CL2 NOT SUPPORTED | Local counterfactual-inspired scoring is not independent do-intervention |
| SIS-LIT-126 Demystifying Agent Skills | Skill availability | SCF / CAUSAL_MECHANISM_EFFECT | CL2 CANDIDATE | I1/I2; specific model/harness, limited repeats; T1 |
| SIS-LIT-126 Demystifying Agent Skills | Component capability interaction and activation mediation | SCF / MECHANISM_INTERACTION_EFFECT | CL1 CONFIRMED | Non-factorial model/config comparisons; mediator not manipulated |
| SIS-LIT-127 SkillPivot | Update strategy contrast | ASR / POLICY_VALUE | CL2 CONFIRMED | I2; matched alternatives and repeated evaluation; T2 |
| SIS-LIT-127 SkillPivot | Correct causal repair locus | ASR / INTERVENTION_LOCUS_SELECTION_EFFECT | CL1 CONFIRMED | No oracle-locus vs wrong-locus controlled intervention |
| SIS-LIT-130 VISTA | Seed-conditioned optimizer strategy contrast | ASR / POLICY_VALUE | CL2 CANDIDATE | I1/I2; defective seed and compute/repeat controls require full audit; T1 |
| SIS-LIT-130 VISTA | Claimed hypothesis/verification mechanism | ASR / ACTION_SELECTION_EFFECT | CL1 CONFIRMED | Bundled changes; no mediator intervention |

## Primary-source anchors
- SIS-LIT-003: https://arxiv.org/abs/2608.23041
- SIS-LIT-004: https://arxiv.org/abs/2609.04749
- SIS-LIT-126: https://arxiv.org/abs/2609.29454
- SIS-LIT-127: https://arxiv.org/abs/2609.29154
- SIS-LIT-130: https://aclanthology.org/2026.acl-srw.8/

## Pending queue synchronization
Registry v1.3 now includes SIS-LIT-132–145. Append 14 corresponding records to the master P0 CSV and transfer these five split decisions to its status/final fields. Preserve the full claim-level decisions in this supplement; a single paper cannot inherit a universal CL. Do not promote T3/T4. Independent second-coder adjudication remains pending.
