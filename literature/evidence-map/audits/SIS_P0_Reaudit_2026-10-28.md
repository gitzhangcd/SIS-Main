# SIS P0 Claim-Level Re-Audit｜2026-10-28

**Authority:** SIS v0.3.1; SIS-LEM-P0-v0.1 and ClaimRecord v0.1. **Scope:** three previously unresolved high-priority studies, nine independent claims, first-coder source-level review. No paper-level label inherited as final maturity; independent second coder and adjudication PENDING.

## SIS-LIT-014 — Where Reliability Lives

**StudyVersionRecord:** [arXiv:2609.03192](https://arxiv.org/abs/2609.03192), 2026-09-02 preprint. **Verified anchor:** abstract, Introduction §§1, experiments §§4–5 (HTML). **Routing context:** fixed cognition vs institutional-epistemic mechanisms; separately fixed institution vs cognition substitutions. A single designed settlement; not a crossed factorial of cognition × institution.

| Claim ID | Source anchor / factual contrast | Primary / Framework | Estimand | First-coder maturity decision | I / T |
|---|---|---|---|---|---|
| 014-C1 | §§1,4.1: single-commit provenance-rule ablation while cognition fixed changes collective attribution | SCF; MI/IA/ID/MEAS/BT | `INSTITUTION_PROVENANCE_INTERVENTION_ATTRIBUTION_EFFECT` | local CL2 candidate, narrow designed-world setting; registered interventions not universal mechanism | I2-local/T0 |
| 014-C2 | §§4.3–4.5: first-hand true witness flips marginal belief-channel value positive in 9/11 seeds after negative/no-value witness-free phases | SDR; TD/EG/ID/MEAS/BT | `EVIDENCE_CHANNEL_BY_WITNESS_AVAILABILITY_EFFECT` | local CL2 candidate; strong boundary reversal, not universal positive belief-channel effect | I2-local/T0 |
| 014-C3 | §§5.1–5.4: five pre-declared institutional properties survived cognition ablation/reset/substitution/corruption; 2,581 substituted-panel false-completion claims, none accepted | SCF; MI/IA/EG/MEAS/BT | `INSTITUTIONAL_INVARIANT_SURVIVAL_UNDER_COGNITION_CHANGE` | CL1 conditional invariants + designed interventions; no general CL3/CL4 or real-world safety guarantee | I2-local/T0 |

**Non-inflation:** Authors explicitly report registered predictions falsified and adverse comparator performance. The cognition and institution manipulations are not a crossed factorial; none tests an optimizer acting adversarially against enforcement. Formal institutional guards vs task throughput are distinct. Do not equate zero observed accepted false completions to zero future risk.

## SIS-LIT-026 — ExecCritic: Learn to Test, Test to Improve for Coding Agents

**StudyVersionRecord:** [arXiv:2609.09133](https://arxiv.org/abs/2609.09133), 2026-09-08 preprint; [Microsoft Research primary author page](https://www.microsoft.com/en-us/research/publication/execcritic-learn-to-test-test-to-improve-for-coding-agents/). **Verified anchor:** abstract, §§1,5 (HTML); SWE-bench Verified. Test and Repair independently trained; qualified test frozen before Repair edits source code.

| Claim ID | Source anchor / factual contrast | Primary / Framework | Estimand | First-coder maturity decision | I / T |
|---|---|---|---|---|---|
| 026-C1 | Abstract/§5.2: holding base Repair fixed, weak Test feedback drops solved 61.2%→57.3%; stronger Test feedback lifts 61.2%→65.3% | SDR; TD/EG/ID/MEAS/BT | `TEST_QUALITY_CONDITIONAL_REPAIR_FEEDBACK_EFFECT` | local CL2 candidate for test-source effect; strong negative/positive direction | I2-local/T0 |
| 026-C2 | §5.2: Test training raises Base-to-Gold rate 22.2%→62.2% | SCF; MI/EG/MEAS/ID/BT | `SPECIALIZED_TESTER_TRAINING_VALIDITY_GAIN` | CL1; training stages and reward confounded, not mediation | I1/T0 |
| 026-C3 | §5.2: trained Repair 68.3% no-test; final composed 72.6%; untrained baseline no-test 61.2% | SDR; TD/DR/EG/MEAS/BT | `SEPARATED_TEST_REPAIR_SYSTEM_NET_EFFECT` | CL1 bundle; extra test/repair compute not matched; do not attribute full +11.4 points to test independence | I1/T0 |

**Non-inflation:** Passing a frozen generated test is not official Gold correctness; improved train-time tester may encode issue-specific targets. Composition includes training differences, test-generation compute and additional revisions. T3/T4 unsupported.

## SIS-LIT-027 — EDGE: Error Dependency Graph-Guided Multi-Error Attribution

**StudyVersionRecord:** [arXiv:2609.01360](https://arxiv.org/abs/2609.01360), 2026-09-01; canonical peer-reviewed [EMNLP Findings 2026](https://aclanthology.org/2026.findings-emnlp.387/), October 2026. **Verified anchor:** Abstract, Introduction §§1, methods/experiments in full HTML. Preserve same study identity across preprint→conference.

| Claim ID | Source anchor / factual contrast | Primary / Framework | Estimand | First-coder maturity decision | I / T |
|---|---|---|---|---|---|
| 027-C1 | Abstract/§1: error-dependency graph + two-stage classifier increases category-level multi-error attribution on TRAIL and MAST across most settings | SDR; TD/ID/IA/MEAS/BT | `DEPENDENCY_GUIDED_MULTI_ERROR_ATTRIBUTION_VALIDITY` | CL1 prediction performance; graph + detection stages bundled | I1/T1 |
| 027-C2 | §1/method: candidate dependencies validated by counterfactual rollout; distinguish validated subset from correlation edges used to improve detection | SDR; TD/MI/ID/BT | `VALIDATED_ERROR_EDGE_INTERVENTION_EFFECT` | local CL2 candidate restricted to experimentally replayed edges; not all dependency graph edges causal | I2-local/T0 |
| 027-C3 | TRAIL vs MAST and adapted Who&When prompts: diagnostic advantage in distinct taxonomies | SDR; TD/ID/MEAS/BT | `ERROR_DEPENDENCY_DIAGNOSIS_BOUNDARY_REPLICATION` | CL1/T1 performance replication only; no causal transport or invariant mechanism | I1/T1 |

**Non-inflation:** Counterfactual validation of selected links cannot establish all observed category dependencies as a complete causal error chain. Model-based judges/labels are measurement instruments, not independent intervention-ground truth for every predicted error.

## Governance decisions

- **Promotions:** no final CL2/CL3 promotion without independent second coder; only local CL2 candidate status documented.
- **Confirmations:** 014 designed institutional-invariant conditional result; 026 weak-test negative feedback; 027 multi-error predictive benefit.
- **Splits:** each three-way split separates observable effect, local manipulation and broad mechanism/transport extrapolation.
- **Demotions/ceilings:** no global institution safety claim; no global feedback-help claim; no full error-dependency causal mediation.
- **Second coder:** PENDING for 014/026/027. **Adjudication:** PENDING. **T3/T4:** no new evidence.
