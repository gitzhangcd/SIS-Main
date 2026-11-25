# SIS P0 Claim-Level Re-Audit｜2026-11-25｜DeepEvidence

**Study:** SIS-CAND-20261125-11 (provisional, no permanent ID)  
**Source:** https://doi.org/10.1038/s42256-026-01266-0; VOR PDF, pp. 1142–1156. Base main `cf61e464471c4cf6cac602ca6e6b1afb50b21a2b`.  
**Authority:** SIS v0.3.1, SIS-LEM-P0 v0.1, ClaimRecord v0.1. First coder only; second coder/adjudication pending.  
**Qualification:** PRIMARY_VERIFIED; preprint arXiv:2601.11560 matched to same Study; use VOR numbers. Source anchors below are printed article pages. Exact run logs, supplement and independent replication remain pending.  

| Claim | Source anchor / contrast | Program and canonical estimand | Maturity and audit decision |
|---|---|---|---|
| SIS-CAND-20261125-11-C1 | Fig. 1e, pp.1143–44; GPT-5 agent arms across four benchmarks; 40.0/64.7/47.1/96.0% DeepEvidence. | SCF; CAUSAL_MECHANISM_EFFECT candidate; MI/MEAS/ID/BT; BGT | CL1 / I1 / T1. CONFIRM local package performance. Resource/information governance incomplete; not isolated component effect. |
| SIS-CAND-20261125-11-C2 | Fig. 5f p.1149; ReAct+MCP vs +CodeExec: P/R/gap 1.1/3.7/25.0 → 17.8/36.8/80.0%. | SCF; CAUSAL_MECHANISM_EFFECT; MI/MEAS/ID/BT | CL1 ceiling, local CL2 candidate / I1 / T0. SPLIT package effect; actual access and budget may change. |
| SIS-CAND-20261125-11-C3 | Fig. 5f p.1149, Discussion p.1150; full 38.6/44.1/89.5 vs BFRS-only 24.5/26.5/65 and DFRS-only 19.9/37.1/80; generic orchestrator 15.3/33.9/70 vs strong single 17.8/36.8/80. | SCF; ORGANIZATION_EFFECT; MI/IA/MEAS/ID/BT | CL1 / I1 / T0. CONFIRM local configuration contrast/NEGATIVE_BOUNDARY; CL2 candidate, not isolated topology effect. |
| SIS-CAND-20261125-11-C4 | Fig. 5f, Discussion p.1150; BFRS/DFRS complementarity and graph-mediated improvements proposed; no isolated graph manipulation, full factorial or identified mediator. | SCF; MEDIATED_MECHANISM_EFFECT; MI/IA/ID/EG/BT | CL0 hypothesis / I0 / T0. DEMOTE mechanistic inference; test competing explanations. |
| SIS-CAND-20261125-11-C5 | Fig. 5g pp.1148–49; manual review 10 graphs, 316 items; 100% provenance, 99.7% normalization, 93.3% alignment, 0.6% duplicate. | ROUTING_ABSTAIN; measurement / evidence governance, MEAS/EG/BT | CL1 / I1 / T0. CONFIRM bounded descriptive measurement; no intervention, clinical truth or universal reliability claim. |
| SIS-CAND-20261125-11-C6 | Fig. 5d p.1149 and Methods p.1153; 20 Cochrane version pairs with changed conclusions; gap detection 90%, recall@30 44.14%; Biomni 50%/30.17%. | SCF; CAUSAL_MECHANISM_EFFECT candidate; MI/MEAS/EG/ID/BT; BGT | CL1 / I1 / T0. CONFIRM performance on enriched retrospective sample; no-update negatives and prospective validation pending. |

## Non-routing and independence gates

- SDR trajectory/perturbation and ASR decision-policy value are future research questions, not empirical recovery or regulation claims of this paper. CSCI capability moderation untested (common backbone only). T1 cross-task performance for C1, no T3/T4.
- Mediation candidates: tool-selection error, entity coverage, multi-hop path quality, graph state retention, source alignment. No identified mediation effect, no CL3.
- Kill tests: equal access/budget, strong single-agent controls, BFRS×DFRS complete factorial, frozen evidence representation contrast, graph corruption and recovery, prospective no-update controls, independent blinded evaluation. Report paired uncertainty, repeated runs, source/version snapshots and resource costs.
- Fig. 1e vs prose HLE discrepancies and Fig. 5d vs 5f denominators unresolved; keep separate. Preprint LitQA2 80.0% vs VOR 64.7%, no pooling. 
- Six first-coder provisional claim records in [JSONL](../claims/2026-11-25_DeepEvidence_candidate_claim_records.jsonl). `identity.sis_lit_id=null` intentionally: provisional candidate not admitted to permanent audit queue. `final_claim_level=null` throughout.
- Formal Impact: MEASUREMENT_IDENTIFICATION_DELTA, secondary BENCHMARK_DELTA; ScientificCoreDelta 0; no formal CL/Program/transport promotion. No alteration to frozen SIS P0 or existing permanent queue.
