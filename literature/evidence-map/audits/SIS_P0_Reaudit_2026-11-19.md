# SIS P0 Claim-Level Re-Audit｜2026-11-19

**Authority:** SIS v0.3.1 Master, Registry, Evidence-Map ClaimRecord contracts and current P0 Audit Queue. Three existing studies, nine independently scoped scientific claims. **Status FIRST_CODER_ONLY; SECOND_CODER & ADJUDICATION PENDING.** Primary author arXiv HTML reviewed for question, methods, result summaries and limitations. Not newly published. No automatic CL2/CL3; no T3/T4.

## SIS-LIT-101｜AIDE² Recursive Self-Improvement of AI Research Agents

**Source/version:** https://arxiv.org/abs/2609.26457 (Sept 22, 2026 preprint). The unit is an eight-day sequence with selected rewrites, not eight independent randomized causal trials.

| Claim | Estimand, routing and Framework | Evidence ceiling and boundaries | Kill test |
|---|---|---|---|
| 101-C1 | `AUTONOMOUS_REWRITE_SEQUENCE_HELDOUT_RESEARCH_TASK_GAIN`; ASR/BGT; DR/MI/MEAS/ID/BT | CL1 package; I1/T2 performance-only. Seven accepted code changes; four held-out domain families. Optimizer selection, time and search budget confounded with code and memory updates. | Freeze successive variants; blind paired replay; equal total search+evaluation budget; independent task Gold |
| 101-C2 | `SEARCH_POLICY_VS_CONTEXT_MEMORY_REWRITE_COMPONENT_EFFECT`; ASR/CSCI/BGT; DR/MI/IA/ID/MEAS/BT | CL0 mechanism hypothesis plus CL1 combined outcome; I1/T0. Accepted edits are cumulative and selected; no isolated random interventions for each. | Recombine edits factorially against frozen parent; control archive access, replay seed and model calls |
| 101-C3 | `HELDOUT_REWARD_HACKING_AND_CROSS_DOMAIN_TRANSFER`; SCF/BGT; MI/EG/MEAS/ID/BT | CL1 observed 55%→32% reward hacking on separate held-out family; T2 performance-only; no mechanism invariance, pooled estimate with small family. | Blind human validation × matched model cost × more unseen tasks × individual edit reversals |

**Decision:** Three claims split; first coder confirms useful performance evidence; no CL2/CL3 formal promotion; T3/T4 not established.

## SIS-LIT-102｜Grow the Harness, Not the Context

**Source/version:** https://arxiv.org/abs/2609.26760 (Sept 22, 2026 preprint, version lineage same study).

| Claim | Estimand, routing and Framework | Evidence ceiling and boundaries | Kill test |
|---|---|---|---|
| 102-C1 | `STRATEGY_FREE_HARNESS_GROWTH_TASK_SUCCESS_AND_LIFECYCLE_COST`; SCF/CSCI/BGT; MI/IA/MEAS/ID/BT | CL1 package, I1/T1. Two web task families, 3 models, 5/6 best model-benchmark settings; 76.0–91.8% fewer deployment LLM calls (excludes full offline selection/eval). | Matched cumulative optimization+deployment cost; held-out test; explicit amortization horizon |
| 102-C2 | `TRACE_LOCAL_REPAIR_JOINT_WINDOW_ROLLBACK_GATE_EFFECT`; ASR/BGT; DR/TD/EG/ID/MEAS/BT | CL1 local ablation CL2 candidate only. Reported trace-local ablation 36%→18% in specified one-model setting; components not full factorial, repeated selection may adapt to gate set. | Trace guidance × joint repair × validation gate 2×2×2, independent seeds and test tasks |
| 102-C3 | `EXECUTABLE_CONTROL_EXTERNALIZATION_VS_BACKBONE_CAPABILITY_REGIME`; SCF/CSCI/BGT; MI/IA/BT/ID/MEAS | CL1 cross-model performance; T2 only; model identity is not capability construct; amortized gain depends on reuse and task similarity. | Independent quantified model capability × same grown harness × shifted task family × cost frontier with uncertainty |

**Decision:** Split package efficiency, mechanism hypotheses and CSCI interaction; no CL3 or causal transport.

## SIS-LIT-105｜ToolCompass

**Source/version:** https://arxiv.org/abs/2609.25678 (Sept 22, 2026 preprint).

| Claim | Estimand, routing and Framework | Evidence ceiling and boundaries | Kill test |
|---|---|---|---|
| 105-C1 | `FUNCTION_CLUSTER_GUIDED_TOOL_TRIALING_OOD_SUCCESS`; SCF/BGT; MI/TD/MEAS/ID/BT | CL1 package; up to +10.71pp AppWorld OOD relative to vanilla post-training; local contrast candidate I1/T2 performance-only. | Equal compute RL training, unseen tool functionality and independent executable outcomes |
| 105-C2 | `TRIAL_SUPPRESSION_VS_SELECTIVE_EXPLORATION_UNDER_BUDGET`; ASR/BGT; DR/TD/MEAS/ID/BT | CL1 negative boundary; suppressing trial calls may lower OOD success; number of calls is not outcome by itself. | Budget × forced exploration vs guided vs reduced-trial policies, withheld tool API mapping |
| 105-C3 | `SHARED_FUNCTION_REPRESENTATION_AS_CAUSAL_MEDIATOR`; SCF/CSCI/BGT; MI/ID/MEAS/BT | CL0 mediation hypothesis, CL1 representation analysis; embeddings may correlate with task family without mediating tool decision. No T3. | Function-label permutation × adversarial similar tools × representational intervention × task execution Gold |

**Decision:** Split OOD performance, exploration policy and representation mechanism. No formal CL2/CL3, no T3/T4.

## Governance
- **P0 decisions:** 3 first-coder updates, 9 separately scoped claims; 0 final promotions, no second-coder or adjudication. Historical registry paper-level candidate labels are screening metadata only.
- **Evidence roles:** package benefit; conditional negative boundary; temporal cost; representation-based mediator hypothesis; explicit transfer performance vs causal transport.
- **Preserve provenance:** original arXiv links and scope of all comparisons retained; no version duplicated and no title promoted to scientific primitive.
- **SIS Impact:** MEASUREMENT_IDENTIFICATION_DELTA; CorePressure WATCH; ScientificCoreDelta 0.
