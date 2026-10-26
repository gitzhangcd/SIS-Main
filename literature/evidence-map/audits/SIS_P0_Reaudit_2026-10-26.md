# SIS P0 Claim-Level Re-Audit｜2026-10-26

**Authority:** SIS v0.3.1 + SIS-LEM-P0-v0.1 ClaimRecord schema. **Nine claim-level first-coder decisions across three studies**. Final CL: PENDING for every claim until second independent coder and adjudication. Provenance links and tables below. Distinguish source observation, controlled local contrast, mediation, formal bound and transport. No formal CL3/T3/T4 admissions.

## SIS-LIT-034 — Grounding Agent Memory

**Primary source/version:** https://arxiv.org/html/2609.11060v1; **first coder:** 2026-10-26; second coder and adjudication PENDING.

| Claim ID | Source anchor | Routing | Framework | Estimand | First-coder maturity determination | I / T |
|---|---|---|---|---|---|---|
| 034-C1 | §5.1 Table 1(a), no-memory strict pass 39±4 vs memory + probing 73±5 | SCF/CSCI/BGT | MI/EG/MEAS/BT | `MEMORY_PACKAGE_TASK_OUTCOME` | CL1 overall; composite effect, not independent probe mediation | I1/T1 |
| 034-C2 | §5.1 Table 1(a), memory only 70±16 vs memory + probing 73±5, 5 paired runs | ASR/BGT | DR/EG/ID/MEAS/BT | `CURATOR_PROBING_PACKAGE_INCREMENTAL_VALUE` | Local CL2 candidate (tool access AND instructions changed); effect small and imprecise; do not infer isolated probing effect | I2-local/T0 |
| 034-C3 | §3.3/§5.3 curator intervention changes memory accuracy then downstream utility | SDR/BGT | TD/EG/ID/MEAS | `MEMORY_VERIFICATION_MEDIATION` | CL0 mechanism hypothesis; no mediator randomized; curator effort excluded from task-agent costs | I1/T0 |

**Outstanding checks:** formally compare assignment/intervention and resource budgets; check evaluator independence and source anchors; validate outcome construct, missingness, competing causes, broader environments and any transport target. This is a *claim-level first-coder audit*, never an automatically confirmed whole-paper CL2/CL3.

## SIS-LIT-033 — COBRA-Skills

**Primary source/version:** https://arxiv.org/html/2609.11682v1; **first coder:** 2026-10-26; second coder and adjudication PENDING.

| Claim ID | Source anchor | Routing | Framework | Estimand | First-coder maturity determination | I / T |
|---|---|---|---|---|---|---|
| 033-C1 | §4 Table 1, Qwen average 73.5 vs SkillOpt 69.6 on six tasks | ASR/BGT | DR/MEAS/BT | `BUDGETED_SKILL_SEARCH_POLICY_VALUE` | CL1 performance; algorithm bundles bandit+evolution and differing training example budgets | I1/T1 |
| 033-C2 | §5 Table 4, Full 73.5 vs w/o Bandit 71.3 vs w/o Evolution 71.1 | ASR/BGT | DR/MI/ID/MEAS | `BANDIT_BY_EVOLUTION_LOCAL_COMPONENT_EFFECT` | Local CL2 candidate per controlled ablation; do not infer general causal mediator or additive interaction | I2-local/T0 |
| 033-C3 | §4 Table 2/§5 Fig 6, reported dollarized cost 55–58% lower, 34/36 cross-model skill transfers improve | ASR/CSCI/BGT | DR/BT/MEAS | `DOLLAR_COST_AND_PERFORMANCE_TRANSFER` | CL1 cost and T2 performance-only; target-model token consumption may be higher; not end-to-end latency nor causal transport | I1/T2 |

**Outstanding checks:** formally compare assignment/intervention and resource budgets; check evaluator independence and source anchors; validate outcome construct, missingness, competing causes, broader environments and any transport target. This is a *claim-level first-coder audit*, never an automatically confirmed whole-paper CL2/CL3.

## SIS-LIT-038 — SCALE / Do We Always Need Query-Level Workflows?

**Primary source/version:** https://aclanthology.org/2026.findings-acl.254/; **first coder:** 2026-10-26; second coder and adjudication PENDING.

| Claim ID | Source anchor | Routing | Framework | Estimand | First-coder maturity determination | I / T |
|---|---|---|---|---|---|---|
| 038-C1 | Official Findings ACL 2026 abstract: query-level workflow not always necessary; top-K task-level coverage | ASR/BGT | DR/MI/MEAS/BT | `QUERY_VS_TASK_GRANULARITY_BOUNDARY` | CL1 conditional negative result; existence of low-cost subset is not universal dominance | I1/T1 |
| 038-C2 | Official abstract: average task-performance loss 0.61%, up to 83% token reduction | ASR/BGT | DR/MEAS/BT | `COARSE_WORKFLOW_COST_UTILITY_TRADEOFF` | CL1 empirical cost-quality tradeoff; no equivalence test or worst-case guarantee; full table audit pending | I1/T1 |
| 038-C3 | Official abstract: optimizer self-prediction plus few-shot calibration replaces costly rollout evaluation | ASR/BGT | DR/EG/ID/MEAS | `SURROGATE_EVALUATOR_ADMISSION_VALIDITY` | CL0 hypothesis about trustworthy evaluation; evaluator independence, drift and search-selection bias unverified; no CL2/3 promotion | I0/T0 |

**Outstanding checks:** formally compare assignment/intervention and resource budgets; check evaluator independence and source anchors; validate outcome construct, missingness, competing causes, broader environments and any transport target. This is a *claim-level first-coder audit*, never an automatically confirmed whole-paper CL2/CL3.

## Decisions and governance

1. SIS-LIT-034: split baseline package improvement from the smaller curator-side incremental treatment. Probing tool access and guidance were co-changed; curator-side cost explicitly excluded from task-agent cost. **No single-mediator promotion**.
2. SIS-LIT-033: retain direct ablation candidates within the original experimental regime. Distinguish dollar-denominated cost from overall token/elapsed-time efficiency; distinguish T2 performance transfer from causal transport.
3. SIS-LIT-038: protect conditional negative finding against universalization and distinguish cheaper surrogate-based workflow evaluation from independently accurate evaluation. ACL Findings source is archival, but full PDF table audit remains pending.

**Queue change:** audit_priority marker changes for these three rows only; final_claim_level, final_primary_program and transport_final remain `PENDING_CLAIM_LEVEL_AUDIT`. No overwrite of historical Gold, no claimed full paper promotion.

**SIS Impact:** BENCHMARK_DELTA, with identification pressure; core freeze upheld.
