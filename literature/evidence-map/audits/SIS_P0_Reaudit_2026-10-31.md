# SIS P0 Claim-Level Re-Audit | 2026-10-31

**Authority:** SIS v0.3.1, current registry and P0 Queue. **Sources:** official ACL Anthology published Jul 2026, re-verified 2026-10-31. **Coder:** first only. **Second coder:** PENDING. **Adjudication:** PENDING. **Final Claim Level:** PENDING. No paper-wide causal promotion or automatic T3/T4.
**Method limitation:** main official abstracts and public primary metadata were inspected; detailed supplemental ablation appendices were not independently re-executed. These are conservative claim ceilings, not certified ground truth.

## SIS-LIT-048 — Verified Critical Step Optimization for LLM Agents

**StudyVersionRecord:** [Findings ACL 2026, 2026.findings-acl.1974](https://aclanthology.org/2026.findings-acl.1974/); preprint [arXiv:2602.03412](https://arxiv.org/abs/2602.03412) is *same study lineage*, not duplicate. PRM proposes critical steps, expert models propose alternatives, own policy rolls forward from replacements.

| Claim ID | Anchor and evidence | Routing / Framework | Primary estimand | First-coder ceiling and decision | I/T |
|---|---|---|---|---|---|
| 048-C1 | ACL abstract: failed policy trajectory, expert replacement, resulting policy continuation flips failure to success | SDR; BGT; TD/MI/ID/BT | `VERIFIED_LOCAL_OUTCOME_FLIP` | Local CL2 candidate for successful *selected* replacements; selected-sample and changed downstream trajectory limitation | I2-local/T0 |
| 048-C2 | ACL abstract: replacement accepted only when target policy can complete from that prefix | ASR; BGT; DR/ID/MEAS/BT | `POLICY_REACHABLE_CRITICAL_STEP_SUPERVISION_VALUE` | Local verified reachability, not entire causal mediator; full separate reachability ablation not revalidated | CL1/CL2 candidate; I1/I2-local/T0 |
| 048-C3 | GAIA-Text-103 and XBench-DeepSearch; relative 37% and 26% over SFT; supervision 16% steps | SCF; BGT; MI/MEAS/BT | `SELECTIVE_VERIFIED_STEP_POSTTRAIN_PERFORMANCE` | CL1 composite performance. Expert teacher, data selection and DPO jointly vary | I1/T1 |

**Decision:** split verified local outcome flip from policy reachability and downstream model training. Do not treat selection of successful replacements as unbiased causal effect on all original failure states; no CL3 full mediator.

## SIS-LIT-049 — Attribution-Based Analysis and Optimization of Modular Agentic Workflows / ShapleyFlow

**StudyVersionRecord:** [Findings ACL 2026, 2026.findings-acl.359](https://aclanthology.org/2026.findings-acl.359/) supersedes [arXiv:2502.00510](https://arxiv.org/abs/2502.00510); preserve one study ID. 1,500+ tasks, seven domains, nine LLMs, 2^4 configurations in fixed four-component workflow.

| Claim ID | Anchor and evidence | Routing / Framework | Primary estimand | First-coder ceiling and decision | I/T |
|---|---|---|---|---|---|
| 049-C1 | 16 coalitions varying component models at fixed workflow; benchmark outcomes by coalition | SCF; CSCI/BGT; IA/MI/ID/MEAS/BT | `FIXED_WORKFLOW_COMPONENT_UPGRADE_INTERACTION_EFFECT` | CL1 performance; local CL2 candidate only for actually controlled component replacement contrasts | I2-local/T1 |
| 049-C2 | Shapley game-theoretic decomposition of coalition value | ROUTING_ABSTAIN; BGT; IA/ID/MEAS | `SHAPLEY_ALLOCATION_VS_CAUSAL_INTERACTION` | CL0 mathematical allocation conditional on value function, *not* proof of unique causal mediator or failure responsibility | I0/T0 |
| 049-C3 | Shapley-guided configuration recommendation exceeds compared single-model workflows | ASR; BGT; DR/IA/MEAS/BT | `SHAPLEY_GUIDED_MODEL_ALLOCATION_NET_VALUE` | CL1 selected policy value; require evaluation cost and sealed heldout selection before causal/general value promotion | I1/T1 |

**Decision:** component coalition contrasts, axiomatic value allocation and optimization policy are separate claims. No blanket CL2; no transport mechanism inference.

## SIS-LIT-050 — Seeing the Whole Elephant / TraceElephant

**StudyVersionRecord:** [ACL 2026 Long, 2026.acl-long.912](https://aclanthology.org/2026.acl-long.912/), same study as [arXiv:2604.22708](https://arxiv.org/abs/2604.22708). Public source reports up to 76.5% relative attribution improvement with full vs output-only traces.

| Claim ID | Anchor and evidence | Routing / Framework | Primary estimand | First-coder ceiling and decision | I/T |
|---|---|---|---|---|---|
| 050-C1 | ACL abstract: same attribution benchmark under full and partial observability; up to 76.5% accuracy improvement | SDR; BGT; TD/ID/MEAS/BT | `TRACE_OBSERVABILITY_DIAGNOSTIC_ACCURACY_EFFECT` | CL1, local CL2 candidate **only for observation access**; not causal location of underlying fault | I2-local/T0 |
| 050-C2 | Benchmark includes full inputs, context, reproducible environments, human/developer annotation | ROUTING_ABSTAIN; BGT; EG/MEAS/ID/BT | `FULL_TRACE_LABEL_CONSTRUCT_VALIDITY` | CL1 measurement instrument; reproducibility is not perfect external Gold, label error not excluded | I1/T0 |
| 050-C3 | Paper motivates more accurate attribution with full traces, no independently verified repair-outcome intervention in abstract | SDR; BGT; TD/DR/ID/BT | `FULL_TRACE_CAUSAL_REPAIR_VALUE` | CL0 unproven mechanism hypothesis; require do(replace step) and replay with matched conditions | I0/T0 |

**Decision:** explicitly separate more observability → better diagnosis from genuine causal fault identification. No whole-paper CL2/CL3.

## Audit Ledger
**Confirmations:** 048 verified policy continuation in *selected* trajectories; 049 full coalition evaluation; 050 observed full-vs-partial trace diagnostic advantage.
**Splits:** local outcome flip vs downstream supervised training; Shapley functional allocation vs component intervention; observability vs causal fault.
**Demotions/non-promotions:** no paper-wide CL2 or CL3; theoretical Shapley allocation is not causal identification; no T3/T4; second-coder/adjudication pending.
