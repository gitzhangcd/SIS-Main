# SIS P0 Claim-Level Re-Audit｜2026-11-17

**Authority:** SIS v0.3.1 + SIS-LEM-P0 + ClaimRecord v0.1; three EXISTING StudyVersionRecords, 9 distinct ScientificClaims. Not a normative core revision.
**Evidence:** Original author arXiv full HTML used for all three. Rechecked October v3 / September v2 / September v1 version histories. First coder only; second coder and final adjudication PENDING.
**Rule:** Existing paper-level CL2 or CL1→CL2 candidate not automatically inherited. All final claim_level remain PENDING; no T3/T4 claim.

## SIS-LIT-117｜When Does Execution Provenance Help Agent Memory Retrieval?
**Primary source:** https://arxiv.org/html/2609.25913v3, arXiv v3 2026-10-25 (v1 2026-09-22); version lineage verified 2026-11-17. Sections 6–8, Tables 2/4, Appendix E Table 7. The historical Queue entry `CLAIM_SPLIT_2026-09-26_C1_CL1_C2_CL2` is not independently adjudicated, and is placed in PENDING pending second-coder review.
| Claim | Estimand / routing | Identification, ceiling, transport | Evidence / boundary / action |
|---|---|---|---|
| 117-C1 | `PROVENANCE_UNIT_SOURCE_ALIGNED_FULL_SUPPORT_2048` · SCF/BGT · MI/MEAS/ID/BT | CL1, local CL2 candidate / I1-I2-local / T0 | Full Support@2048 +19.07 points vs 512-token flat chunks; candidate granularity, token budget, scoring are controlled in selected arms but cannot attribute every benefit to graph topology. |
| 117-C2 | `CANDIDATE_SEED_FIXED_TYPED_GRAPH_PROPAGATION_FULL_SUPPORT` · SCF/BGT · MI/ID/MEAS/BT | **local CL2 candidate** / I2-local / T0 | Matched candidate/seed residual graph gain +4.55 points (95% CI [2.98,6.18]); direct fact interval includes zero; multi-fact +11.83 points; causal contrast concerns retrieval score, NOT task success or mechanism mediation. |
| 117-C3 | `RETRIEVAL_FULL_SUPPORT_TO_BLIND_JUDGED_ANSWER_ACCURACY` · SCF/BGT · EG/MEAS/ID/BT | CL1 borderline / I1 / T0 | Appendix E: flat 71.75% vs graph 77.78% strict QA (CI for paired difference [0.00,12.10]); graph vs provenance-unit control not significant; one model as answerer and judge, 315 queries; cannot infer general answerability, causal mediation or safety. |
**Decision:** preserve the locally strong controlled retrieval contrast as **candidate only**; demote the historical Queue final CL2 entry to PENDING until independent adjudication. Differentiates intervention on retrieval from mediation on downstream reasoning.
**Kill Test:** matched candidates, fixed seed scores and token budget × graph edge permutation × multi-fact vs direct × independently human-graded answers, plus task success.

## SIS-LIT-112｜Agentic TCAD Calibration Workflow for Oxide Semiconductor Transistors
**Primary source:** https://arxiv.org/html/2609.12184v2, v2 2026-09-14 (v1 2026-09-10). Sections II/III, Table II, Figures 5/6. Human approves the model deck; Sentaurus governs physics. Original experimental results checked.
| Claim | Estimand / routing | Identification, ceiling, transport | Evidence / boundary / action |
|---|---|---|---|
| 112-C1 | `TCAD_RESIDUAL_GUIDED_CALIBRATION_FIXED_REFERENCE_DEVICE` · SCF/BGT · MI/TD/MEAS/ID/BT | CL1 package / I1 / T0 | Five approved changes J=2.589→0.181 (14.3× reduction); LLM proposals, human decisions, simulator update and parameter/model activation bundled. No matched human/manual or random search cost baseline. |
| 112-C2 | `SENSITIVITY_MODEL_ACTIVATION_VS_PHYSICS_CAUSAL_IDENTITY` · ROUTING_ABSTAIN/BGT · ID/EG/MEAS/BT | CL0 physical mechanism / CL1 calibration description / I0-I1 / T0 | Effective work-function, DOS and mobility descriptors identify a calibration model, **not unique microscopic defect/transport causes**; observational equifinality is explicitly acknowledged. |
| 112-C3 | `FIXED_TCAD_MODEL_DRAIN_BIAS_GEOMETRY_PERFORMANCE_TRANSFER` · SCF/BGT · MI/MEAS/ID/BT | CL1 / I1 / T2 performance-only | Fixed post-calibration parameter set tested across drain bias & channel length (no retune), bounded voltage/current errors; physical device family and geometry limited. Does not justify T3 causal transport or deployment value. |
**Decision:** source upgraded PRIMARY_PENDING_VERIFICATION→PRIMARY_ARXIV_V2_HTML_METHOD_TABLES_REAUDITED. The v1/v2 lineage is one study. No CL2/CL3 mechanism claim.
**Kill Test:** factorial LLM/engineer update proposals × equal Sentaurus calls × sham residual cues × hidden transistor geometry with independent measured I–V.

## SIS-LIT-019｜Procedural Graphs: Self-Evolving Execution Structures for LLM Agents
**Primary source:** https://arxiv.org/html/2609.09153, v1 2026-09-08. Sections 3/5, Table 1, Table 3, Appendix E. First-coder analysis uses full author HTML, not an abstract-only score.
| Claim | Estimand / routing | Identification, ceiling, transport | Evidence / boundary / action |
|---|---|---|---|
| 019-C1 | `PROCEDURAL_GRAPH_STATE_LOCALIZED_GUIDANCE_SYSTEM_PERFORMANCE` · SCF/BGT · MI/TD/MEAS/ID/BT | CL1; local candidate / I1 / T1 | Benchmarks across models/tasks; Table 3 no-graph→subgraph-generative 80.27→89.31 MultiChallenge, but token use 6629→12295. Graph and guidance/cost jointly change. |
| 019-C2 | `RAW_FULL_GRAPH_VS_LOCAL_SUBGRAPH_GUIDANCE_INDEPENDENT_EFFECT` · SCF/BGT · MI/ID/MEAS/BT | CL1; local CL2 candidate / I1-I2-local / T0 | Table 3 reveals raw full graph, full generative graph and localized subgraph differ sharply; ALFWorld full generative 54.48 vs no-graph 72.58 vs subgraph 81.53; representation is not independently isolated from guidance token length and model calls. |
| 019-C3 | `EVOLVING_GRAPH_VALIDATION_GATE_REGRESSION_RETENTION` · ASR/BGT · DR/EG/MEAS/ID/BT | CL1, local candidate / I1 / T1 | Graph edits admitted by held-out performance; rejected candidate reuse and topology edits simultaneous; independent frozen audit and intervention versus no-update needed. |
**Decision:** non-monotonic component effect and cost must be retained, cannot promote specific graph topology to CL3 mediation. Source verified from PRIMARY_PENDING_VERIFICATION.
**Kill Test:** full graph vs localized subgraph × same guidance token budget × same base model × graph topology shuffle; separate validation gate and random update tests.

## Governance cross-check
- 117: historical CL2 claim label is **retained as audit provenance but withdrawn from the final field** pending independent second-coder review, not an assertion that its local intervention is null.
- 112: identify physics model ambiguity (calibration quality ≠ unique physical mechanism), limited performance transfer T2 only.
- 019: route regulation claim 019-C3 to ASR despite study-level SCF; preserve negative/nonmonotonic ALFWorld evidence.
- Final promotions = **0**; confirmed mechanism CL3 = **0**; new causal transport T3/T4 = **0**.
- **CorePressure:** WATCH for downstream evidence attribution, calibration identifiability, representation/cost confounds; `ScientificCoreDelta=0`; primary impact `MEASUREMENT_IDENTIFICATION_DELTA`, secondary `BENCHMARK_DELTA`.
