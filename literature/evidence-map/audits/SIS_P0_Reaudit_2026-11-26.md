# SIS P0 Claim-Level First-Coder Re-Audit｜2026-11-26
Authority: SIS v0.3.1 §§40–44, 54–68, 74–82, 91–94 and P0 ClaimRecord Schema. Base 816c7b56334bc263dc30bdabb7cdb635f5c27807. Three existing studies; nine split claims; official ACL proceedings and selected PDF sections/tables checked (first pages visually inspected). Not independent replication. Final fields unchanged pending second coder/adjudication. I/T are registry aids.

## SIS-LIT-051 VISTA
Source https://aclanthology.org/2026.acl-srw.8/ ; https://aclanthology.org/2026.acl-srw.8.pdf ; abstract, Fig. 1, Table 2, discussion.
- 051-C1: SDR/BGT; TD/MI/MEAS/ID/BT; TRAJECTORY_EFFECT; defective seed and GEPA trajectory: 23.81% initial to 13.50%; negative performance CL1/I1/T0. Defect severity, model, seed, budget; replicate controlled structural vs semantic defect, random seeds.
- 051-C2: ASR/BGT; DR/MI/EG/MEAS/ID; POLICY_VALUE; VISTA full hypothesis-verification/restart package reaches 87.57% in Table 2; CL1/I1/T1, local effect candidate not promoted. Hypothesis labeling, verification, restarts and compute co-vary. Equal-cost factorial and sham verification.
- 051-C3: SCF/BGT; MI/MEAS/ID/BT; CAPABILITY_FRONTIER_SHIFT; cross-model frozen prompt performance Table 2 86.05% vs GEPA 22.74%; CL1/I1/T2 performance only. Not T3 mechanism transport. Cross-family holdout, fixed prompts and matched refiner; independent Gold.
## SIS-LIT-044 Structured Reflection
Source https://aclanthology.org/2026.findings-acl.618/ ; https://aclanthology.org/2026.findings-acl.618.pdf ; abstract and Table 2, recovery evaluation.
- 044-C1: SDR/BGT; TD/MI/MEAS/ID; RECOVERY_EFFECT; repair after perturbation-derived tool errors (open baselines Repair@1 <=9.6%); paper reports trained method improves repair. CL1/I1/T1. Error spectrum, attempts, synthetic vs native errors; matched replay of real failures.
- 044-C2: SCF/BGT; MI/MEAS/ID/EG; CAUSAL_MECHANISM_EFFECT; structured reflection/reward training package contributes to reported BFCL and repair improvements. CL1/I1/T1; separate reflection trace, reward, training budget via factorial, no CL2 automatic.
- 044-C3: ASR/BGT; DR/TD/MEAS/ID/BT; POLICY_VALUE; when to invoke reflection vs continue, retain valid actions and cost. CL0 hypothesis/I0/T0: known erroneous inputs do not identify detector/trigger net value. Blind true/false trigger and ordinary valid trajectories.
## SIS-LIT-037 PROTEA
Source https://aclanthology.org/2026.acl-demo.3/ ; https://aclanthology.org/2026.acl-demo.3.pdf ; §§3–4 and conclusion.
- 037-C1: SDR/BGT; TD/EG/MEAS/ID; PROPAGATION_EFFECT candidate; backward-generated node expectations and rubric scores localize candidate bottlenecks; CL0/I0/T0 as causal localization claim. No independent intermediate Gold; terminal-answer leakage, alternative valid paths. Compare blind injected causes and counterfactual node swaps.
- 037-C2: SDR/BGT; TD/MI/MEAS/ID/BT; RECOVERY_EFFECT; two developer-authored/approved revisions improve document inspection 64.3→83.9%, Hit@5 .30→.38; CL1/I1/T1, combined human/system before-after, not independent patch effect. Held-out tasks, random node patch and matched human baseline.
- 037-C3: ASR/BGT; DR/EG/MEAS/ID; POLICY_VALUE; fixed-suite automatic iteration stress test: 4/5 minimal-prompt workflows improve best score vs no rewrite; CL1/I1/T0, fixed-suite selection and small sample. Freeze holdout, count all attempts/cost, report regressive edits and retention.
Decision: source verification and first-coder splits only. No final CL2/3 or T3/4; no new permanent ID. Historical registry paper tags preserved. Second coder pending.
