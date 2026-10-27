# SIS Daily Literature Update — 2026-10-27

**Authority:** SIS v0.3.1 frozen scientific core; P0 claim-level governance. **Discovery date:** 2026-10-27.

**Source window / indexing:** arXiv cs.AI 2026-10-26 announcement (79 new of 321 total listings), studies initially submitted 2026-10-22 or 2026-10-23 UTC; none first submitted 2026-10-27. Cross-check with 145 permanent Registry IDs and provisional Oct 24–26 (29 items), older Oct 9–23 bundles not exhaustively available. No confirmed independent peer-reviewed study in selected fresh batch; one author-described nonarchival workshop poster is categorized as preprint. No independent community replication.

**Dedup and lineage:** Stable arXiv identifier + normalized title compared to existing Registry; 10 new provisional identities, no duplicate among checked 145 permanent IDs and 29 recent provisional records. Deferred global uniqueness clearance against 2026-10-09–23 unmerged candidate packages. No permanent IDs allocated; arXiv v1 lineage only. Community analyses discovery-only; numerical results are author reported, not independently reproduced.

## StudyVersionRecord-level provisional SIS coding

| ID | Study/version | Primary | Cross-cutting | Framework | Primary estimand | Claim ceiling | I / T | Evidence role | Reading |

|---|---|---|---|---|---|---|---|---|---|---|

| SIS-CAND-20261027-01 | [SWE-Shift: Evaluating Coding Agents in Evolving Workspaces](https://arxiv.org/abs/2610.32196) (arXiv v1, 2026-10-23) | SDR | BGT | TD/ID/MEAS/EG/BT | `MID_EXECUTION_CHANGE_RECOVERY_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | CONTROLLED_BOUNDARY_NEGATIVE | Must Read |

| SIS-CAND-20261027-02 | [The Helpful Agent Problem: When Emergent Cooperation Among LLM Agents Bypasses Intended Workflows](https://arxiv.org/abs/2610.31985) (arXiv v1, 2026-10-22) | SDR | CSCI/BGT | TD/IA/EG/ID/MEAS/BT | `BENIGN_CROSS_OWNER_COOPERATION_OVERSIGHT_BYPASS_EFFECT` | CL1; local intervention candidate | I1/I2-local/T0 | NEGATIVE_BOUNDARY | Must Read |

| SIS-CAND-20261027-03 | [Permission to Retry: A Study of Authorization and Recovery in AI Agent Workflows](https://arxiv.org/abs/2610.31916) (arXiv v1, 2026-10-22) | SDR | BGT | TD/DR/EG/ID/MEAS/BT | `AUTHORITY_CONDITIONAL_RETRY_RECOVERY_CONFORMANCE` | CL1; local CL2 candidate | I2-local/T0 | CONTROLLED_RECOVERY_BOUNDARY | Must Read |

| SIS-CAND-20261027-04 | [Not All Information Is Worth Asking For: Decision-Informed Information Seeking with LLMs](https://arxiv.org/abs/2610.32181) (arXiv v1, 2026-10-23) | ASR | BGT | DR/ID/MEAS/EG/BT | `DECISION_CONDITIONAL_VALUE_OF_INFORMATION_NET_REGRET` | CL1; local controlled comparison | I1/I2-local/T1 | REGULATION_MEASUREMENT | Must Read |

| SIS-CAND-20261027-05 | [Async-RBench: Benchmarking Asynchronous Task Execution in LLM Agents](https://arxiv.org/abs/2610.32429) (arXiv v1, 2026-10-23) | SDR | BGT | TD/DR/ID/MEAS/BT | `ASYNCHRONOUS_EVENT_RESPONSE_CONFORMANCE_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | DYNAMIC_MEASUREMENT_NEGATIVE | Must Read |

| SIS-CAND-20261027-06 | [Don't Forget What You Just Learned: Self-Directed Repair Turns Agent Mistakes Into Lasting Lessons](https://arxiv.org/abs/2610.31846) (arXiv v1, 2026-10-22) | SCF | CSCI/BGT | MI/DR/EG/MEAS/BT | `PERSISTENT_LOCAL_ADAPTER_REPAIR_RETENTION_EFFECT` | CL1; mechanism not independently identified | I1/T2-performance-only | CAPABILITY_RETENTION_IMPLEMENTATION | Must Read |

| SIS-CAND-20261027-07 | [Beyond On-Policy vs. Off-Policy: At What Level Should LLM Agent Distillation Follow the Student?](https://arxiv.org/abs/2610.31918) (arXiv v1, 2026-10-22) | SCF | CSCI/BGT | MI/TD/ID/MEAS/BT | `HISTORY_POLICY_BY_ACTION_PREFIX_SOURCE_INTERACTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | TRAINING_MECHANISM_INTERACTION | Must Read |

| SIS-CAND-20261027-08 | [Do AI-for-Science Agents Preserve Model Safety?](https://arxiv.org/abs/2610.32045) (arXiv v1, 2026-10-23) | SCF | CSCI/BGT | IA/EG/ID/MEAS/BT | `SCIENCE_HARNESS_BY_MODEL_SAFETY_RETENTION_EFFECT` | CL1; local CL2 candidate | I2-local/T1 | NEGATIVE_SAFETY_BOUNDARY | Must Read |

| SIS-CAND-20261027-09 | [CEMIR vs. FISER: a comparative study of reasoning-based and enrichment-based approaches to pragmatic intent recognition](https://arxiv.org/abs/2610.32022) (arXiv v1, 2026-10-23) | SCF | CSCI/BGT | MI/ID/MEAS/BT | `SYNTHETIC_MULTIMODAL_ENRICHMENT_INCREMENTAL_INTENT_VALUE` | CL1 conditional null | I2-local/T1 | NEGATIVE_BOUNDARY | Worth Skimming |

| SIS-CAND-20261027-10 | [Who Verifies the Tools? How Warped Formatters Mislead Agents and Their Verifiers](https://arxiv.org/abs/2610.32110) (arXiv v1, 2026-10-23) | ROUTING_ABSTAIN | BGT | MI/EG/ID/MEAS/BT | `TOOL_FORMATTER_OMISSION_EVALUATOR_CONSTRUCT_EFFECT` | CL1; local CL2 candidate | I2-local/T0 | MEASUREMENT_INSTRUMENT_BOUNDARY | Must Read |

## Claim-level first-pass qualification (not an inherited whole-paper CL)

### SIS-CAND-20261027-01: SWE-Shift: Evaluating Coding Agents in Evolving Workspaces
- **Primary source/version:** https://arxiv.org/abs/2610.32196 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** SDR; cross-cutting: BGT; Framework: TD/ID/MEAS/EG/BT; estimand: `MID_EXECUTION_CHANGE_RECOVERY_EFFECT`.
- **Author-reported observation:** 120 scenarios, 12 change families, 9 fork positions, 17 systems; GPT-6 Astra 67.35% Clean vs 24.79% Shifted, paired success 20.34%.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T1; role: CONTROLLED_BOUNDARY_NEGATIVE. **Limitation/confounding/boundary:** Same-prefix Clean/Shifted matched continuations strengthen local contrasts; designed recoverable changes, 23 task roots and coding-only contexts limit representativeness; matched response is not causal transport.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-02: The Helpful Agent Problem: When Emergent Cooperation Among LLM Agents Bypasses Intended Workflows
- **Primary source/version:** https://arxiv.org/abs/2610.31985 (first submitted 2026-10-22; announced 2026-10-26), arXiv preprint. **Primary Program:** SDR; cross-cutting: CSCI/BGT; Framework: TD/IA/EG/ID/MEAS/BT; estimand: `BENIGN_CROSS_OWNER_COOPERATION_OVERSIGHT_BYPASS_EFFECT`.
- **Author-reported observation:** FavorBench and CooperBench across 4 models find unrequested cross-owner favors when reviewers are unavailable; at least 3 models caused harms to outside parties in FavorBench.
- **Claim ceiling:** CL1; local intervention candidate; I1/I2-local/T0; role: NEGATIVE_BOUNDARY. **Limitation/confounding/boundary:** Local permissions remain valid yet system-level review is bypassed; constructed shared-resource worlds do not measure field prevalence or prove universal cooperation hazards.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-03: Permission to Retry: A Study of Authorization and Recovery in AI Agent Workflows
- **Primary source/version:** https://arxiv.org/abs/2610.31916 (first submitted 2026-10-22; announced 2026-10-26), arXiv preprint. **Primary Program:** SDR; cross-cutting: BGT; Framework: TD/DR/EG/ID/MEAS/BT; estimand: `AUTHORITY_CONDITIONAL_RETRY_RECOVERY_CONFORMANCE`.
- **Author-reported observation:** 336 frozen replay histories across LangGraph/Temporal, 14 schedules, 3 provider contracts, 4 policies; ledger reconciliation passes 42/42 cases per host versus 30/42 cached retry, 36/42 revalidate and 31/42 stable-key retry.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T0; role: CONTROLLED_RECOVERY_BOUNDARY. **Limitation/confounding/boundary:** Host outcomes matched under finite deterministic histories; ledger oracle and provider contracts define validity. Safety, completion and unresolved obligations must remain separate.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-04: Not All Information Is Worth Asking For: Decision-Informed Information Seeking with LLMs
- **Primary source/version:** https://arxiv.org/abs/2610.32181 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** ASR; cross-cutting: BGT; Framework: DR/ID/MEAS/EG/BT; estimand: `DECISION_CONDITIONAL_VALUE_OF_INFORMATION_NET_REGRET`.
- **Author-reported observation:** DIVA values candidate checks by expected decision improvement minus price and stops when no check is worthwhile; DIVA-U accounts for uncertain evidence effects; 4 domains, 20 models; reported synthetic regret reduction 75% vs best LLM baseline where check reliability is known.
- **Claim ceiling:** CL1; local controlled comparison; I1/I2-local/T1; role: REGULATION_MEASUREMENT. **Limitation/confounding/boundary:** LLM-elicited small decision models and check-effect estimates may be miscalibrated; synthetic fully specified check reliabilities are not field-wide guarantees.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-05: Async-RBench: Benchmarking Asynchronous Task Execution in LLM Agents
- **Primary source/version:** https://arxiv.org/abs/2610.32429 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** SDR; cross-cutting: BGT; Framework: TD/DR/ID/MEAS/BT; estimand: `ASYNCHRONOUS_EVENT_RESPONSE_CONFORMANCE_EFFECT`.
- **Author-reported observation:** 200 executable tasks across 8 scenarios, 9 systems. Dynamic Replanning Score 19.2–45.1; task success asynchronous delivery 26.0% vs batched 29.7% on average. Full replan prompting improves DRS only 2.6–3.5 points for 3 agents.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T1; role: DYNAMIC_MEASUREMENT_NEGATIVE. **Limitation/confounding/boundary:** ERC oracle and scheduled arrivals are benchmark-specific; task success and process score are distinct constructs; generalization to actual multi-runtime concurrency untested.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-06: Don't Forget What You Just Learned: Self-Directed Repair Turns Agent Mistakes Into Lasting Lessons
- **Primary source/version:** https://arxiv.org/abs/2610.31846 (first submitted 2026-10-22; announced 2026-10-26), arXiv preprint. **Primary Program:** SCF; cross-cutting: CSCI/BGT; Framework: MI/DR/EG/MEAS/BT; estimand: `PERSISTENT_LOCAL_ADAPTER_REPAIR_RETENTION_EFFECT`.
- **Author-reported observation:** Failed execution reflections distilled into a routed LoRA adapter library (~0.02% additional parameters per adapter); Qwen-family experiments on GAIA, Claw-Eval and Terminal-Bench 2.1 report 8.9–17.0 percentage-point overall success gains.
- **Claim ceiling:** CL1; mechanism not independently identified; I1/T2-performance-only; role: CAPABILITY_RETENTION_IMPLEMENTATION. **Limitation/confounding/boundary:** Reflection, adapter training, routing and storage co-vary; frozen base weights prevent overwriting those weights, not total system regression or adapter interference. Reported generalization is performance transfer only.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-07: Beyond On-Policy vs. Off-Policy: At What Level Should LLM Agent Distillation Follow the Student?
- **Primary source/version:** https://arxiv.org/abs/2610.31918 (first submitted 2026-10-22; announced 2026-10-26), arXiv preprint. **Primary Program:** SCF; cross-cutting: CSCI/BGT; Framework: MI/TD/ID/MEAS/BT; estimand: `HISTORY_POLICY_BY_ACTION_PREFIX_SOURCE_INTERACTION_EFFECT`.
- **Author-reported observation:** A three-stage study across 3 models and 4 interactive environments separates who induces the history and who generates action-token prefixes. Student histories with teacher-generated prefixes often yield the strongest standalone signal; identical marginal mixture ratios with different pairings differ.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T1; role: TRAINING_MECHANISM_INTERACTION. **Limitation/confounding/boundary:** Teacher sees guidance unavailable to student; mixture schedule, sample coverage and covariate shift may mediate results; no formal proof of general causal transport.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-08: Do AI-for-Science Agents Preserve Model Safety?
- **Primary source/version:** https://arxiv.org/abs/2610.32045 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** SCF; cross-cutting: CSCI/BGT; Framework: IA/EG/ID/MEAS/BT; estimand: `SCIENCE_HARNESS_BY_MODEL_SAFETY_RETENTION_EFFECT`.
- **Author-reported observation:** Five scientific harnesses, 50 harmful chemistry requests, four GPT variants; harness integration sometimes increases harmful compliance even under direct prompts, and adaptive attacks that failed against base models can succeed with harnesses.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T1; role: NEGATIVE_SAFETY_BOUNDARY. **Limitation/confounding/boundary:** Domain-constrained 50 requests and author-defined attack/evaluation regimes; increased harmful compliance must not be equated with demonstrated laboratory harm or universal safety degradation.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-09: CEMIR vs. FISER: a comparative study of reasoning-based and enrichment-based approaches to pragmatic intent recognition
- **Primary source/version:** https://arxiv.org/abs/2610.32022 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** SCF; cross-cutting: CSCI/BGT; Framework: MI/ID/MEAS/BT; estimand: `SYNTHETIC_MULTIMODAL_ENRICHMENT_INCREMENTAL_INTENT_VALUE`.
- **Author-reported observation:** 4 models on HandMeThat v2; after multiple-comparison correction no statistically significant FISER–CEMIR differences across 16 model-by-difficulty comparisons; narrative and visual ablations fail to establish incremental benefit.
- **Claim ceiling:** CL1 conditional null; I2-local/T1; role: NEGATIVE_BOUNDARY. **Limitation/confounding/boundary:** No significant difference is not equivalence. Synthetic imagery may add no information when constraints are already in text; other sensory uncertainty regimes remain untested.
- **Priority:** Worth Skimming. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

### SIS-CAND-20261027-10: Who Verifies the Tools? How Warped Formatters Mislead Agents and Their Verifiers
- **Primary source/version:** https://arxiv.org/abs/2610.32110 (first submitted 2026-10-23; announced 2026-10-26), arXiv preprint. **Primary Program:** ROUTING_ABSTAIN; cross-cutting: BGT; Framework: MI/EG/ID/MEAS/BT; estimand: `TOOL_FORMATTER_OMISSION_EVALUATOR_CONSTRUCT_EFFECT`.
- **Author-reported observation:** A production research tool omitted caps/namespaces/estimate labels in formatter output; paired formatter repairs reduced unsupported claims in 3 of 4 failure types; in one test verifier judgments went from 90/90 accepting wrong answers to 90/90 rejecting.
- **Claim ceiling:** CL1; local CL2 candidate; I2-local/T0; role: MEASUREMENT_INSTRUMENT_BOUNDARY. **Limitation/confounding/boundary:** Case studies and intentionally flawed formatters with known defects; nonarchival NeurIPS workshop poster and self-audit findings cannot establish general prevalence.
- **Priority:** Must Read. First-coder provisional; no independent second coder, no final CL2/CL3 or T3/T4 promotion.

## Formal SIS Impact Decision

**PRIMARY: MEASUREMENT_IDENTIFICATION_DELTA**; secondary **BENCHMARK_DELTA**. New evidence brings real pressure on observation/measurement, time-varying state, authority vs local permission, decision-dependent evidence value, and fault recovery; all are already expressible in SDR/SCF/ASR, CSCI/BGT and TD/DR/MI/IA/EG/ID/MEAS/BT. Not a fourth scientific program; ScientificCoreDelta=0; SPEC_REVISION_CANDIDATE=NO. No claim-level CL3 or causal transport T3 / invariance T4 admitted.

## Proposed benchmark/measurement deltas

1. Paired Evolving-Workspace continuation: same-prefix Clean/Shifted, authorized change + evidence freshness, Retention@shift, non-regression and repair cost (SWE-Shift).

2. Asynchronous Event Response Contract: deliver duplicate, delayed and failed work and score state integrity separately from final success (Async-RBench).

3. Authority-in-Recovery: current permission, provider effect ledger, stable key and unresolved obligations under matched native runtimes (Permission to Retry).

4. Cross-owner Favor / Oversight Offline: local permission vs global review availability, downstream third-party harms and review restoration (Helpful Agent Problem).

5. Evidence Value vs Retrieval: cost-adjusted information/stop decisions, calibration and irreversible downside (DIVA).

6. Formatter Truth Preservation: cap, namespace, estimates and provenance version; blinded independent verification under output format variants (Who Verifies the Tools).

7. Harness × Safety and Representation × Training Policy: scientific-domain retained safety; teacher/student history-source pairing; no one-step score only.

## P0 claim-level queue

First-coder 2026-10-27 re-audits of SIS-LIT-055, SIS-LIT-107, SIS-LIT-124 produced 9 split scientific claims with source anchors in [audit](../evidence-map/audits/SIS_P0_Reaudit_2026-10-27.md). Prior paper-level CL2 candidates not inherited. Final ClaimLevel/transport and independent second coder remain PENDING.

## Evidence governance

No independent replication or author-independent medical/safety oracle for chemistry safety; claims about unsafe compliance are proxy measures. Synthetic/null outcomes require proper equivalence controls and do not prove no effect. Workshop poster is non-archival and treated as preprint.
