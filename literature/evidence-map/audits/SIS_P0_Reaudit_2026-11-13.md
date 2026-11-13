# SIS P0 Claim-Level Re-Audit｜2026-11-13

Authority: `specs/System_Intelligence_Science_v0.3.1.md`, Registry v1.3 and existing P0 Queue. FIRST CODER ONLY; paper-level CL2/CL3 does not pass through to individual claims. Source evidence: original arXiv HTML abstracts, methods and selected results; no independent rerun or second coder. Revisited high-priority inherited paper-level CL2 labels.

## SIS-LIT-104｜How Strongly Should Task State Influence an LLM Agent?
Primary: https://arxiv.org/abs/2609.25686 ; fulltext: https://arxiv.org/html/2609.25686 (2026-09-22). Qualification PRIMARY_HTML_METHOD_RESULTS_REAUDITED_2026-11-13.

| Claim | Estimand | Scientific routing / Evidence / Identification / Transport | First-coder decision |
|---|---|---|---|
| 104-C1 | STATE_COUPLING_LADDER_CONDITIONAL_TASK_SUCCESS | ASR/CSCI/BGT; DR/MI/MEAS/ID/BT; intervention package; I2-local/T1 | **CL1 confirmed, local CL2 candidate**: transcript/checklist/directive/enforcement compared with fixed model and task; benefits depend on state availability and model obedience; contrast is not invariant. |
| 104-C2 | ENFORCEMENT_GATE_MATCHER_ERROR_NEGATIVE_EFFECT | SDR/ASR/BGT; TD/DR/EG/ID/BT; negative boundary; I2-local/T1 | **CL1 negative boundary**: Airline 235B model pass1 0.39→0.54 but PM-Bench matcher-based enforcement worsens 35B performance; state decidability and matcher quality confound interpretation. |
| 104-C3 | STATE_DIRECTIVE_BY_MODEL_CAPABILITY_EFFECT_MODIFICATION | ASR/CSCI/BGT; IA/DR/ID/BT; interaction; I1/I2-local/T1 | **CL1; local CSCI candidate**, not T3: larger model reasoning shrinks ladder separation, no universal state-control superiority. |

Boundary: model ability, reasoning budget, state correctness, receipt matching, domain, authority, invalid enforcement. Kill test: fixed task × model × exact state × deliberate matcher corruption × enforcement ablation, matched budget and blinded independent Gold.

**Governance correction:** previous Queue `CL2_PROMOTED_2026-09-24` was paper-level inheritance without explicit claim-specific adjudication, withdrawn to `PENDING_CLAIM_LEVEL_AUDIT` pending second coder. This is an administrative withdrawal of unqualified promotion, not a finding that local intervention lacks effect.

## SIS-LIT-106｜FIRE: Failure-Informed Runtime Engineering for Reliable Language-Model Agents
Primary: https://arxiv.org/abs/2609.26048 ; fulltext: https://arxiv.org/html/2609.26048 (2026-09-22). Qualification PRIMARY_HTML_METHOD_RESULTS_REAUDITED_2026-11-13.

| Claim | Estimand | Routing / Evidence / Identification / Transport | First-coder decision |
|---|---|---|---|
| 106-C1 | REAL_POLICY_CONTENT_VS_TIMING_MATCHED_SHAM_ELIGIBLE_SUCCESS | ASR/BGT; DR/TD/ID/MEAS/BT; randomized five-arm; I2-local/T1 | **CL1 verified, candidate CL2 claim**, no formal promotion. Eligible tasks 61% real policy vs 39% none, 36% timing sham; *prespecified real-vs-sham contrast p=0.061*, while new baseline contrast p=0.032. Evidence supports conditional effects but the primary contrast does not pass the conventional 0.05 threshold. |
| 106-C2 | REPEATED_DELIVERY_SUCCESS_VS_BEST_OF_TWO_CEILING | SDR/CSCI/BGT; TD/MI/MEAS/BT; performance boundary; I1/I2-local/T1 | **CL1**: 87-task Terminal-Bench 2.1; Sol pass² 64.4→73.6%, best-of-two +1.2pp. Repeatability improvement is not creation of new possible solutions. |
| 106-C3 | TRIGGERED_POLICY_CORRECTIVE_BEHAVIOR_MEDIATION | ASR/SDR/BGT; DR/TD/EG/ID/BT; intermediate mechanism candidate; I1/I2-local/T0 | **CL1 conditional mechanism evidence only**: intended corrective behavior 22/24 with real policy, no rival arm more than 14; observational funnel does not establish formal CL3 mediation. |

Boundary: tasks eligible for policies, prior failures used to derive policies, frozen portfolio, repeated tries, timing sham, provider model, cost, off-target harm. Kill test: preregistered larger randomized real/sham, policy-eligible vs ineligible, held-out tasks, direct mediator intervention, economic costs and regression.

**Governance correction:** old `CL2_CONFIRMED_2026-09-24` in Queue withdrawn to `PENDING_CLAIM_LEVEL_AUDIT` until claim-specific independent adjudication, particularly given prespecified p=0.061.

## SIS-LIT-091｜Beyond Prompts / PRISM
Primary: https://arxiv.org/abs/2609.05736 ; fulltext https://arxiv.org/html/2609.05736 (v2, 2026-09-09). Qualification PRIMARY_HTML_ABLATION_REAUDITED_2026-11-13.

| Claim | Estimand | Routing / Evidence / Identification / Transport | First-coder decision |
|---|---|---|---|
| 091-C1 | SELECTED_HARNESS_FIXED_MODEL_HELDOUT_LIFT | SCF/CSCI/BGT; MI/IA/MEAS/ID/BT; package effect; I1/I2-local/T1 | **CL1**, local CL2 candidate: BFCL, τ² Retail, τ² Telecom held-out lifts 14.2, 14.9, 10.1pp. Optimizer and edit surface vary, do not attribute gain to prompt alone. |
| 091-C2 | FAILURE_SURFACE_ROUTING_VS_EDIT_PATTERN_INCREMENTAL_EFFECT | ASR/BGT; DR/MI/ID/BT; component ablation; I1/I2-local/T0 | **CL1 component ablation**, separate routing versus constrained middleware contributions not fully identified by bundled changes. |
| 091-C3 | BUDGETED_SELECTED_HARNESS_LOWER_TAIL_RELIFT95 | ASR/BGT; MEAS/DR/EG/ID/BT; measurement instrument; I1/T1 | **CL1**, benchmark-level selection reliability, not a certified universal confidence lower bound or cross-executor mechanism transport. |

Boundary: outer proposer strength, inner fixed executor, gate split, stochastic selection, budget, middleware restrictions, tool schema and simulated users. Kill test: factorial prompt × middleware × routing × pattern constraints, equal-cost seeds and held-out independent evaluators.

## Governance and Scientific Core Reopen Watch

- 3 studies, 9 atomic first-coder claims; 0 formal CL2/CL3 promotions; 0 confirmed T3/T4; 2 legacy paper-level CL2 labels administratively withdrawn from the **final claim** columns.
- Claims 104-C1, 106-C1, 091-C1 and 091-C2 may be independently re-examined as local CL2 candidates. No claim transfers its historical label unreviewed.
- Second coder PENDING, blinded adjudication PENDING. Claim-specific full-text evidence verified at selected methods/results sections; raw execution/independent replication NOT performed.
- ScientificCoreDelta=0. CorePressure=WATCH for *measurement identification of instrument-dependent failure labels*, *latent regression under memory/adaptation*, and *semantic specification fidelity*; all expressible by existing MEAS/ID/EG/SCF/SDR/ASR, hence NOT SPEC_REVISION_CANDIDATE.
