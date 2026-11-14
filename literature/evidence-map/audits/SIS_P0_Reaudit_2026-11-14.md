# SIS P0 Claim-Level Re-Audit｜2026-11-14

**Authority:** SIS v0.3.1 Master, Evidence Map P0 and ClaimRecord schema. **First coder only**; 3 pre-existing Studies, 9 atomic claims. **No formal CL2/CL3 promotions, no T3/T4 confirmation.** Second-coder/blind adjudication pending. Study identity never duplicated on source-version changes.

## SIS-LIT-006｜From Rollouts to Recipes / Self-Routing
- StudyVersionRecord: arXiv:2609.01422v1 https://arxiv.org/html/2609.01422 and archived **EMNLP 2026 main 464** https://aclanthology.org/2026.emnlp-main.464/ (same study). Primary method §3.3–3.5, experiments §4.2–4.5 and appendix.
- Boundary: Qwen3/Qwen3.5 math verification; rollout accuracy/confidence; GRPO/OPSD/REG/SKIP; fixed/variable sampling costs; reward leakage; OOD tasks.

| Claim ID | Source anchor / scientific question and estimand | SIS routing; Framework; evidence; I/T | First-coder decision |
|---|---|---|---|
| 006-C1 | §4 main comparisons. Does behavior-conditioned routing beat fixed training recipes? `ROLLOUT_CONDITIONAL_RECIPE_ROUTING_HELDOUT_VALUE` | ASR/BGT; DR/MEAS/ID/BT; package intervention; I1/I2-local, T1 | **CL1 confirmed report; local CL2 candidate**. Compare uniform GRPO/OPSD/fixed mixture; training stochasticity, compute and hyperparameters limit causal certainty. |
| 006-C2 | §3.3–3.5, §4.4. Does sample state modify which training action has value? `ROLLOUT_STATE_BY_OPERATOR_CONDITIONAL_INTERACTION` | ASR/CSCI/BGT; DR/MI/ID/MEAS/BT; interaction; I1, T0 | **CL1 association; CL2 pending**. Routing is adaptive, action-state confounding persists; need randomized state-stratified operator assignment. |
| 006-C3 | §4.3–4.5. Do skipped/regularized updates reduce costs without losing retained ability? `RECIPE_SKIP_POLICY_COMPUTE_RETENTION_FRONTIER` | ASR/SCF/BGT; DR/MEAS/EG/BT; policy/cost boundary; I1, T1 | **CL1 conditional performance**. Reporting dynamic routing mix does not prove individual skipped examples were harmful; test independent regression set. |

Kill test: preregistered `rollout-state × random operator × equal FLOPs × independent correctness Gold × retained ability` across model families, separating selection from optimization.

## SIS-LIT-062｜EvoOntology / revised v2
- StudyVersionRecord: arXiv:2609.15779v1 (2026-09-14) → **v2 2026-11-02** (same study; NOT a new record). Verified official HTML https://arxiv.org/html/2609.15779v2, §Method, §Experiments, §Analyses Table 5–7.
- Boundary: model/backbone; dataset schema and join path; ontology probes; typed edit admission; evaluation leakage; retrieval/tool budgets; domain transfer.

| Claim ID | Source anchor / estimand | SIS routing; Framework; evidence; I/T | First-coder decision |
|---|---|---|---|
| 062-C1 | §Main Results. Externalized schema/content/tool ontology improves heterogeneous data use; `EVIDENCE_GROUNDED_ONTOLOGY_SYSTEM_PERFORMANCE` | SCF/CSCI/BGT; MI/IA/EG/MEAS/BT; package; I1, T1 | **CL1 package; local CL2 candidate**. BIRD Initial +5.1pp, evolution additional +3.7pp (author report); mechanism not identified. |
| 062-C2 | §Analyses Table 5: Full 89.5 Traj-Wise vs w/o Gate 78.3, w/o Attribution 83.2; `PAIRED_VALIDATION_GATE_ATTRIBUTION_INCREMENT` | ASR/BGT; DR/EG/ID/MEAS/BT; controlled ablation; I2-local, T1 | **CL1 observed ablation; local CL2 candidate**. Gate -11.2pp and attribution -6.3pp when removed; not fully orthogonal or equal-successful-edit-count, no CL3. |
| 062-C3 | §Table 6–7: Mappings/Evidence masking and three-level editing; `ONTOLOGY_CONTENT_MAPPING_EVIDENCE_STRUCTURE_CONDITIONAL_EFFECT` | SCF/CSCI/BGT; MI/IA/ID/MEAS/BT; negative boundary; I2-local, T1 | **CL1 with local intervention candidate**. w/o Mappings -13.4pp, w/o Evidence -8.7pp; masking can change interface and available information, so mediator not isolated. |

Kill test: fixed executor × frozen task × `content/schema/tool` factorial × `gate` × `probe-evidence exposure` vs matched size/latency, independent semantic Gold and unseen data sources.

## SIS-LIT-066｜Symbolic Separation / Virtual Knowledge Graph
- StudyVersionRecord: arXiv:2609.17107v1 https://arxiv.org/html/2609.17107 (primary methods/experiments); existing Study identity. Real telemetry scale **49.9 TB**, but evaluation scenario counts and representativeness must remain in scope.
- Boundary: ontology correctness, relation schema, temporal validity, graph update timing, query verifier, LLM and tool budget, telemetry domain and data scale.

| Claim ID | Source anchor / estimand | SIS routing; Framework; evidence; I/T | First-coder decision |
|---|---|---|---|
| 066-C1 | §IV end-to-end: Does symbolic grounding package improve operational task success? `SYMBOLIC_VKG_VALIDATED_DATA_ACCESS_PACKAGE_GAIN` | SCF/BGT; MI/EG/MEAS/ID/BT; package; I1, T1 | **CL1**. Author reports 43%→86% and token cost ÷2.4; pipeline/validation/ontology differ together, no standalone causal graph effect. |
| 066-C2 | §III-C pre-execution validator. Does it detect relation misuse missed by syntactic checks? `DOMAIN_SEMANTIC_CONTRACT_VS_SYNTAX_ERROR_REJECTION` | SDR/BGT; TD/MI/EG/ID/BT; measurement/negative; I1/I2-local, T0 | **CL1 structural contrast; local CL2 candidate**. Validated graph traversal can reject some illegal joins, not prove semantic fidelity against independent domain Gold. |
| 066-C3 | §IV comparison. Does smaller executor with semantic boundary beat stronger ungrounded model? `COMPONENT_CAPABILITY_BY_SEMANTIC_GROUNDING_EFFECT_MODIFICATION` | SCF/CSCI/BGT; IA/MI/MEAS/ID/BT; conditional interaction; I1, T1 | **CL1**, model size and architecture/available data confounded; no T3 cross-executor causal transport. |

Kill test: fixed model × independently validated graph correctness × constrained/unconstrained interface × deliberate stale edge × equal resource × unseen telemetry, external expert blind adjudication.

## Governance & Core pressure
- 3 studies, 9 atomic first-coder records; confirmed recorded observations, split package from proposed mechanisms, no formal CL2/CL3 promotions; T3/T4 = 0. Existing original paper-level labels remain historical only, NOT final claim levels.
- Qualification: 006 official archived EMNLP + arXiv HTML verified; 062 revised v2 method and Tables 5–7 inspected; 066 original HTML method/results inspected. No full raw replication. Second coder/adjudication PENDING.
- CorePressure **WATCH**, especially world-state/history consistency, semantic-prior admission, and real evidence-use identifiability. These map to SDR/ASR/SCF, MEAS/ID/EG/MI/TD/DR/IA/BT; no uncovered scientific estimand or irreplaceable capability. **ScientificCoreDelta=0**.
