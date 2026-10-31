# SIS P0 Claim-Level Re-Audit | 2026-11-01

**Authority:** SIS v0.3.1 Scientific Core FROZEN; canonical Registry v1.3 and current P0 Queue. **Coder:** first-coder only; **second coder/adjudication:** PENDING. **Source:** verified primary arXiv/ACL Anthology abstracts and linked methodological summaries; supplemental raw experiments not independently rerun. **Evidence ceiling:** provisional only, not final CL2/CL3 or T3/T4.

## SIS-LIT-126 — Demystifying Agent Skills for Smart Contract Auditing
**StudyVersionRecord:** [arXiv:2609.29454, submitted 2026-09-24](https://arxiv.org/abs/2609.29454). 83 skill artifacts; EVMBench, 40 tasks/120 annotated vulnerabilities, seven agent–model configurations. **Critical scientific unit:** independently reported outcome contrasts are separate from inferred skill-activation mechanism.

| ClaimRecord | Source anchor / numeric observation | Primary / Cross / Framework | Estimand | Provisional ceiling / decision | I/T |
|---|---|---|---|---|---|
| 126-C1 | arXiv abstract, design/corpus: 83 heterogeneous skills, shared six-stage workflow | SCF / BGT / MI,TD,MEAS,BT | `SKILL_PACKAGE_BEHAVIORAL_DESIGN_DESCRIPTION` | CL0 descriptive + limited CL1 observational; **confirm** corpus, no causal mechanism | I0/I1 T0 |
| 126-C2 | arXiv abstract: Codex/GPT-5.5 Detect Score +22.8% **relative** and Detect Award +43.2% relative; skills available vs not available | SCF / CSCI,BGT / MI,IA,ID,MEAS,BT | `SKILL_AVAILABILITY_MODEL_CONDITIONAL_DETECTION_VALUE` | CL1; **split** effect by configuration; local CL2 *candidate only*, no independent repeated randomized assignment established | I1/I2-candidate T1 |
| 126-C3 | arXiv abstract and behavioral observation: triggering varies by backend, some configurations rarely/never load full skill | SCF / CSCI,BGT / IA,TD,ID,MEAS | `SKILL_TRIGGERING_CAUSAL_MEDIATOR_EFFECT` | CL0 hypothesis for causal mediation; **demote** mechanism interpretation (triggering endogenous to model/skill fit) | I1 T0 |

**Boundary:** model backend, harness, task, skill scope, invocation, tool overhead. **No attribution from skill availability to skill-triggering mediator without do(trigger).** Repeats, costs, and Gold quality require appendix follow-up.

## SIS-LIT-130 — Reflection in the Dark / VISTA
**StudyVersionRecord:** [ACL 2026 SRW archival paper](https://aclanthology.org/2026.acl-srw.8/) with same lineage [arXiv:2603.18388 v2 (2026-06-08)](https://arxiv.org/abs/2603.18388). Do not create a second study for preprint/conference.

| ClaimRecord | Source anchor / numeric observation | Primary / Cross / Framework | Estimand | Provisional ceiling / decision | I/T |
|---|---|---|---|---|---|
| 130-C1 | ACL abstract: GEPA on defective GSM8K seed drops from 23.81% to 13.50% | ASR / BGT / DR,ID,MEAS,BT | `DEFECTIVE_SEED_REFLECTIVE_OPTIMIZER_NEGATIVE_EFFECT` | CL1 negative under specified seed/budget; **confirm** counterexample, not universal optimizer failure | I1 T0 |
| 130-C2 | ACL abstract: VISTA recovers to 87.57% on same seed, combined hypothesis generation/rewrite/verification/restart policy | ASR / BGT / DR,MI,MEAS,BT | `VISTA_COMPOSITE_REPAIR_POLICY_VALUE` | CL1 composite performance, local CL2 candidate only if matched-budget allocation appendix verified; **split** from negative GEPA observation | I1/T1 |
| 130-C3 | ACL abstract: semantically labeled hypotheses, parallel minibatch verification, random restart and epsilon-greedy | ASR / BGT / DR,ID,EG,MEAS | `DIAGNOSTIC_LABEL_VS_EXPLORATION_OPERATOR_MEDIATION` | CL0 unproven independent mediation; **demote** from blanket CL2, requires separate factorial and full cost ledger | I0/I1 T0 |

**Boundary:** seed defect, available gradient/supervision, optimizer budget, verification set independence and stochastic search. **Do not extrapolate** one striking seed comparison to a general optimizer system law.

## SIS-LIT-131 — Gradient-Guided Multi-Judge Prompt Optimization (GMPO)
**StudyVersionRecord:** [ACL 2026 Long, Anthology ID 2026.acl-long.1089](https://aclanthology.org/2026.acl-long.1089/). Corpus version remains same study; conference record authority.

| ClaimRecord | Source anchor / numeric observation | Primary / Cross / Framework | Estimand | Provisional ceiling / decision | I/T |
|---|---|---|---|---|---|
| 131-C1 | ACL abstract: first-order segment-importance gradient approximation uses one forward/backward pass | ASR / BGT / DR,MI,MEAS,ID | `FIRST_ORDER_SEGMENT_ATTRIBUTION_COMPUTE_COST` | CL1 reported computation contrast; CL0 mathematical complexity if implementation assumptions hold; **confirm**, not proven true causal segment importance | I1 T0 |
| 131-C2 | ACL abstract: aggregate lightweight multi-judge cross-entropy to select generated candidates | ASR / BGT / DR,EG,MEAS,ID | `MULTIJUDGE_SELECTION_EVALUATOR_BIAS_EFFECT` | CL1 comparison; local CL2 candidate pending exact ablations/independent labels; **split** judge selection from gradient localization | I1/I2-candidate T1 |
| 131-C3 | ACL abstract: math, reasoning, instruction-following and safety robustness results, claimed lower overhead | ASR / CSCI,BGT / DR,MI,EG,MEAS,BT | `GRADIENT_MULTIJUDGE_COMPOSITE_HELDOUT_NET_VALUE` | CL1 cross-task performance; T2 **performance only**; **confirm** package but no causal transport/mediation | I1 T2-perf |

**Boundary:** evaluator correlation, gradient surrogate fidelity, segment lengths, budget, executor ability, heldout test contamination. Must compare single-vs-multiple judges under fixed generator, same candidate set and exact cost.

## Audit ledger
- **Confirmations:** 126 conditional detection contrast and descriptive invocation; 130 defective-seed regression; 131 segment-scoring/multi-judge composite report.
- **Splits:** 126 availability / triggering / causal mediator; 130 GEPA negative / VISTA package / individual operators; 131 gradient scoring / judge selection / total outcome.
- **Demotions / limits:** causal skill-trigger mediator, VISTA operator mediator and GMPO causal segment importance remain unproven; *no whole-paper CL2/CL3, no T3/T4*.
- **Pending:** independent second coder, appendix-level method and resource controls, formal adjudication. Queue status reflects **FIRST_CODER_ONLY** and deliberately leaves final fields unchanged.
