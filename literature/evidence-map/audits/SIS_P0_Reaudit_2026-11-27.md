# SIS P0 Claim-Level Re-Audit｜2026-11-27
Base 1600d7d833626ae05ff20afc9a74dfab2ae9797a. First coder only; second coder/adjudication pending. Prior registry labels are triage, not final claims. ACL VOR landing pages and PDF front pages plus selected result sections checked, not full reproduction. Source class PEER_REVIEWED unchanged. All final fields remain PENDING_CLAIM_LEVEL_AUDIT.

## SIS-LIT-052 FAMA
Source https://aclanthology.org/2026.findings-acl.1716/ ; PDF pp.34346,34351–34352, Table 1 and Fig 4.
- 052-C1 SCF/BGT; MI/IA/MEAS/ID/BT; ORGANIZATION_EFFECT; package compared with ReAct/FC/all-helper IRMA across tau-bench five runs; author reports up to 27% gains across modes; selective beats baselines in reported settings; SUPPORT CL1/I1/T1. Helper backbone (Qwen2.5-72B), cost, context, model and domain confound. Equal total resources and fixed helpers.
- 052-C2 ASR/BGT; DR/IA/MEAS/ID/BT; SELECTIVE_ACTION_UTILITY; dominant-failure-based helper subset vs all/fixed/random subsets; observed all-helper degradation in some cells; LIMIT CL1/I1/T1. Failure distributions and context length differ; not identified online causal policy advantage. Freeze failure estimates before blind tasks, match helper tokens, randomize subset.
- 052-C3 SDR candidate, routing unresolved for causal propagation; TD/ID/MEAS/BT; PROPAGATION_EFFECT target; Fig 4 failure labels from orchestrator, not causal intervention; INSTRUMENT CL0/I0/T0 for propagation claim. Gold failure injection, blind labels, matched factor removal and downstream replay.

## SIS-LIT-072 Think Earlier, Not Longer
Source https://aclanthology.org/2026.findings-acl.817/ ; PDF p.16577, Table 1, Fig 6, Table 2, sections 4–5.
- 072-C1 SDR/BGT; TD/MI/MEAS/ID/BT; TRAJECTORY_EFFECT; term abbreviation manipulates ambiguity while nominal task fixed; early entropy peak delayed/elevated and tokens increase without accuracy gain; SUPPORT/LIMIT CL1/I2-local candidate/T1. Abbreviation familiarity, tokenizer, model and effort; matched semantic-preserving perturbations.
- 072-C2 SCF/BGT; MI/MEAS/ID/BT; CAPABILITY_FRONTIER_SHIFT; clarification optimizer compared with Pure/Early-Stop/EvoPrompt, Table 1, up to 52% efficiency gain reported, cross-domain BBH/MedQA; SUPPORT CL1/I1/T2 performance only. Account for refiner cost and noninferiority margin; same total budget on hidden tasks.
- 072-C3 SCF candidate; MI/TD/ID/MEAS; MEDIATED_MECHANISM_EFFECT target; token enrichment and entropy trajectories support interpretation, not unique mediation; CL0 mechanism hypothesis/I0/T0. Intervene on ambiguity and entropy independently, test alternative semantic information pathway. No CL3.

## SIS-LIT-073 Prompt Duel Optimizer
Source https://aclanthology.org/2026.findings-acl.490/ ; PDF p.10066, Tables 1/2/7, §5.
- 073-C1 ASR/BGT; DR/MEAS/ID/BT; POLICY_VALUE; double Thompson sampling and mutation under judge budgets; best evaluation accuracy 13/16 BBH tasks reported; SUPPORT CL1/I1/T1. Candidate pool, judge, generation costs; matched candidates and lifecycle budget with blind gold.
- 073-C2 ASR/BGT; DR/MEAS/ID/EG/BT; VALUE_OF_INFORMATION candidate; judge accuracy on differing answers .59→.87 on Geometric, .89→.98 Tracking-7, .85→.99 Web of Lies for judge swap; LIMIT CL1/I2-local candidate/T1. Judge capability and cost, position bias; fixed pairs, randomized answer order and matched cost, independent gold. Label-free optimization not validation-free.
- 073-C3 SCF/BGT; MI/MEAS/ID/BT; CAUSAL_MECHANISM_EFFECT; mutation vs no mutation Table 7, 10 independent runs, nominal p<.05 on 8/16; SUPPORT/LIMIT CL1/I2-local candidate/T1. Multiple testing, candidate-generation budget; prespecified multiplicity, matched edit budget and independent test.
No final promotions or T3/T4. Three source qualifications and nine provisional claim splits. Independent second coder pending.
