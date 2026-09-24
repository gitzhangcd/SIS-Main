# SIS Literature Evidence Map｜P0

## Corpus Qualification, Claim-Level Re-Audit & Coverage-Gap Freeze

### System Intelligence Science v0.3.1 Evidence-Map Program

**Document ID:** `SIS-LEM-P0`  
**Version:** `v0.1`  
**Date:** `2026-09-24`  
**Normative upstream:** `System Intelligence Science v0.3.1`  
**Input registry:** `SIS v0.3.1 Literature Re-Coding Registry v1.0`  
**Status:** `P0 FREEZE`  

---

# 0｜P0 Executive Freeze

P0 formally converts the existing paper-level literature registry into a claim-level System Intelligence Science evidence-map program.

The governing decision is:

```math
\boxed{
Paper\ Registry
\neq
Scientific\ Evidence\ Map
}
```

and:

```math
\boxed{
ScientificClaim
=
Primary\ Routing\ Unit
}
```

A paper may contain multiple claims with different estimands, different SIS Primary Programs, different identification strength, and different claim maturity. Therefore no paper-level `PrimaryProgram` or `ClaimLevel` in Registry v1.0 is automatically inherited as final scientific evidence.

P0 freezes three tasks:

1. **Corpus Qualification** — determine which records are admissible as primary scientific evidence, discovery-only evidence, duplicates/versions, or pending verification.
2. **Claim-Level Re-Audit** — extract and independently re-code each material scientific claim using SIS v0.3.1 routing, identification, claim-maturity, boundary and transport semantics.
3. **Coverage-Gap Freeze** — freeze the current evidence deficits that will drive P1–P3 experiment and literature work.

P0 does **not** change the SIS v0.3.1 Scientific Core.

```math
\boxed{
SIS\ v0.3.1\ Core\Delta=0
}
```

The expected delta is:

```math
\boxed{
EvidenceMap\Delta>0,
\quad
BenchmarkPortfolio\Delta>0,
\quad
ScientificCore\Delta=0
}
```

---

# 1｜Upstream Scientific Authority

This P0 inherits the following SIS v0.3.1 frozen semantics without modification:

- `ScientificClaim` is the minimal Program-routing unit.
- Routing follows `ScientificQuestion → PrimaryEstimand → ScientificConformance → ProgramRouting`.
- `Estimand > Keyword`.
- Framework capability is not Program membership.
- Framework admission is not mechanism validation.
- Framework adoption must not inflate claim maturity.
- Claim maturity is governed by `CL0–CL7`.
- Claim level is upper-bounded by identification strength, measurement validity, evidence independence, boundary support and replication support.
- `ScientificExperimentContract` is shared across SCF, SDR and ASR.
- Tier 1 targets maximal causal identifiability; Tier 2 targets replication/boundary/capability-regime interactions; Tier 3 targets transportability/external validity/deployment value.

No paper, framework name, implementation label or model family is allowed to override these semantics.

---

# 2｜P0 Scientific Questions

P0 asks five meta-research questions.

## Q1｜Corpus validity

Which items in Registry v1.0 are admissible as primary scientific evidence for SIS, and which are only discovery, engineering or contextual evidence?

## Q2｜Claim validity

For each paper, what are the actual scientific claims supported by the reported design and evidence?

## Q3｜Claim maturity

What is the highest defensible SIS claim level for each claim after applying the SIS claim ceiling?

## Q4｜Program coverage

Which SCF, SDR, ASR, CSCI and BGT estimands are densely supported, weakly supported or absent?

## Q5｜Evidence gaps

Which missing evidence types prevent transition from performance/association claims toward mechanism, boundary-aware, replicated and transportable causal claims?

---

# 3｜Frozen Baseline Corpus

Registry v1.0 contains **113 records**.

Current source classification for P0 is:

| Source class | Count | P0 evidence status |
|---|---:|---|
| Peer-reviewed research | 34 | `PRIMARY_EVIDENCE_CANDIDATE` |
| Preprint research | 78 | `PRIMARY_EVIDENCE_CANDIDATE` |
| Technical/community analysis | 1 | `DISCOVERY_ONLY` |
| **Total** | **113** | — |

Therefore the initial claim-audit scientific corpus is:

```math
\boxed{
N_{primary\ research\ candidates}=112
}
```

The one technical/community analysis remains useful for discovery and interpretation but cannot independently raise SIS claim maturity.

Current paper-level claim labels in Registry v1.0 are retained only as triage metadata:

| Registry label | Count |
|---|---:|
| `CL0` | 1 |
| `CL0→CL1` | 4 |
| `CL1` | 61 |
| `CL1→CL2 candidate` | 23 |
| `CL2 candidate` | 16 |
| `CL2` | 4 |
| `CL2→CL3 candidate` | 4 |

Thus **47 records** enter the high-priority causal/mechanistic re-audit queue, while **66 records** enter the descriptive/associational confirmation queue.

Current transport triage remains:

```text
T0 = 47
T1 = 53
T2 = 13
T3 = 0
T4 = 0
```

These transport labels are provisional and must be re-audited at claim level.

---

# 4｜Corpus Qualification Contract

## 4.1 Qualification unit

The qualification unit is a **StudyVersionRecord**, not a title string.

Each study must identify:

```yaml
StudyVersionRecord:
  sis_lit_id:
  canonical_title:
  authors:
  source_type:
  venue_or_server:
  publication_status:
  version_date:
  canonical_primary_source:
  peer_review_status:
  supersedes:
  superseded_by:
  erratum_or_retraction_status:
  full_text_access_status:
  qualification_status:
  qualification_reason:
```

## 4.2 Canonical qualification states

```text
PRIMARY_VERIFIED
PRIMARY_PENDING_VERIFICATION
DISCOVERY_ONLY
DUPLICATE_VERSION
SUPERSEDED_VERSION
INSUFFICIENT_METHOD_DETAIL
OUT_OF_SCOPE
QUARANTINED
RETRACTED_OR_INVALIDATED
```

## 4.3 Primary-source requirement

A scientific claim may enter the evidence map only when the audit can anchor the claim to a primary source containing sufficient method/result detail.

Abstract-only indexing may support discovery but cannot support CL2+ promotion.

## 4.4 Version rule

Preprint → conference/journal publication must be represented as a version lineage, not as two independent studies, unless the later version materially changes the design or results.

## 4.5 Secondary-analysis rule

Community analyses, industry posts and technical summaries may:

- identify papers;
- surface limitations;
- suggest competing interpretations;
- help detect missing controls.

They may not independently increase `ClaimMaturity`.

---

# 5｜Paper-Level Registry → Claim-Level Evidence Map

The central P0 transformation is:

```math
\boxed{
StudyRecord
\rightarrow
\{ScientificClaim_1,\ldots,ScientificClaim_n\}
}
```

One paper may generate:

- a performance claim;
- a causal mechanism claim;
- a mediator claim;
- a boundary claim;
- a transfer claim;
- a null/negative claim;
- an engineering/measurement claim.

These claims may route to different Programs.

Example:

```text
Paper X
├─ Claim C1: mechanism improves outcome        → SCF
├─ Claim C2: failure propagates over time      → SDR
├─ Claim C3: state-conditioned policy is better→ ASR
└─ Claim C4: effect changes with model ability → CSCI
```

The paper itself therefore has **no normative SIS Primary Program**.

---

# 6｜Canonical ClaimRecord v0.1

P0 freezes the following claim-level audit object.

```yaml
ClaimRecord:
  identity:
    claim_id:
    sis_lit_id:
    study_version_ref:

  source_anchor:
    section:
    page_or_lines:
    table_or_figure:
    exact_author_claim: optional
    audit_paraphrase:

  scientific_question:
    question:
    claim_type:

  program_routing:
    routing_status:
    primary_program:
    secondary_programs: []
    cross_cutting_axes: []
    primary_estimand_family:
    routing_basis:

  context:
    task:
    environment:
    domain:
    model_regime:
    time_horizon:
    risk_regime:

  causal_structure:
    treatment_or_mechanism:
    control:
    mediators: []
    outcomes: []
    moderators: []
    confounders: []

  identification_audit:
    causal_contrast:
    manipulation_check:
    temporal_ordering:
    confounder_governance:
    resource_governance:
    information_governance:
    randomization_or_assignment:
    replay_or_counterfactual_support:

  measurement_audit:
    outcome_validity:
    evaluator_independence:
    measurement_reliability:
    missingness_or_observability:

  mechanism_audit:
    mediator_measured:
    mediator_manipulated:
    pathway_tested:
    competing_mechanisms_addressed:

  boundary_audit:
    declared_boundaries: []
    tested_boundaries: []
    replication_contexts: []

  transport_audit:
    source_context:
    target_context:
    performance_transfer:
    causal_transport_test:
    mechanism_invariance_test:

  evidence_role:
    SUPPORT
    LIMIT
    NULL
    CONTRADICT
    INSTRUMENT

  maturity:
    author_claim_scope:
    provisional_claim_level:
    claim_ceiling:
    final_claim_level:
    audit_decision:

  limitations:
    internal_validity:
    external_validity:
    construct_validity:
    statistical_or_compute_confounds:

  lineage:
    coder:
    second_coder:
    adjudication_status:
    audit_version:
```

---

# 7｜Claim-Level Re-Audit Rules

## 7.1 No automatic inheritance

Registry v1.0 labels such as:

```text
CL1→CL2 candidate
CL2 candidate
CL2→CL3 candidate
I2
I3
T2
```

are **triage labels only**.

They do not survive P0 audit automatically.

## 7.2 Promotion to CL2

A claim may be coded `CL2` only when the audited design supports a controlled causal contrast such as:

```math
\boxed{
do(M)\rightarrow Y}
```

and the study has adequate support for:

- causal contrast;
- manipulation check;
- temporal ordering;
- confounder governance;
- resource governance;
- information governance.

Ablation alone does not automatically imply CL2 if multiple causal factors move together.

## 7.3 Promotion to CL3

A claim may be coded `CL3` only when evidence supports:

```math
\boxed{
do(M)\rightarrow Z\rightarrow Y}
```

The paper must provide mediator/pathway-relevant evidence, not merely a plausible explanation.

## 7.4 Boundary and transport promotion

- `CL4` requires tested boundary-aware mechanism evidence.
- `CL5` requires replicated cross-context effect.
- `CL6` requires source→target causal relation preservation.
- `CL7` requires mechanism + identification + mediation + boundary + transportability + evidence independence.

Cross-model performance reuse alone is **not** CL6.

## 7.5 Mandatory demotion

A claim must be demoted when:

- a claimed mechanism is supported only by endpoint performance;
- attribution is observational but written causally;
- stronger model / more calls / more tokens are confounded with the intervention;
- evaluator and optimizer share an ungoverned self-confirmation loop;
- the causal variable universe excludes plausible true causes;
- mediator evidence is absent;
- transfer is only performance transfer;
- reported success is selected from best-of-search without selection reliability analysis.

## 7.6 Claim splitting

A broad author statement must be split whenever different subclaims have different evidence maturity.

Example:

```text
"Method X improves performance because it identifies the correct failure locus and transfers across models."
```

must become at least:

```text
C1: Method X improves performance.
C2: Method X improves failure-locus identification.
C3: Identification mediates performance improvement.
C4: Improvement replicates/transfers across models.
```

Each receives an independent maturity ceiling.

---

# 8｜Program Routing Freeze

P0 uses the SIS v0.3.1 routing order:

```text
Scientific Question
→ Primary Estimand
→ Scientific Conformance
→ Program Routing
```

## SCF

Route to `SCF` when the primary estimand is a mechanism / organization / representation / system-structure effect on a system property.

## SDR

Route to `SDR` only when the estimand depends on trajectory, transition, propagation, containment, recovery, history or long-horizon dynamics.

Temporal data alone is insufficient.

## ASR

Route to `ASR` only when the primary estimand is endogenous information-conditioned action selection.

An experiment containing an intervention is not automatically ASR.

## CSCI

Add `CSCI` only when component capability is explicitly tested as an effect modifier of a system mechanism.

Different model IDs alone are insufficient.

## BGT

Add `BGT` when the claim explicitly concerns replication, boundaries, generalization, transfer or transportability.

---

# 9｜Identification Re-Audit Matrix

Every CL2+ candidate must be scored against the following audit dimensions.

| Dimension | Audit question |
|---|---|
| Causal contrast | Is there a defensible treatment/control contrast? |
| Manipulation check | Did the intended mechanism actually change? |
| Temporal ordering | Does treatment precede mediator/outcome? |
| Confounder governance | What else changes with treatment? |
| Resource governance | Are calls/tokens/compute/time/human effort matched or modeled? |
| Information governance | Does one arm receive extra information? |
| Evaluator independence | Can the intervention influence its own judge/acceptance criterion? |
| Measurement validity | Does the metric measure the claimed property? |
| Observability | Could missing channels create false attribution? |
| Counterfactual/replay | Is there branch/replay/fault-injection evidence? |
| Mediator support | Is the proposed pathway actually measured/tested? |
| Boundary support | Are failure regimes and moderators tested? |
| Replication | Does the effect recur in distinct contexts? |
| Transport | Is the causal relation tested source→target? |

No single aggregate score replaces these fields.

---

# 10｜Transportability Re-Audit

P0 freezes four distinct transport concepts:

```text
Replication
PerformanceTransfer
CausalTransportability
MechanismInvariance
```

They must never be collapsed.

For each T2 candidate, the audit must ask:

1. Is the intervention the same in source and target?
2. Are treatment and outcome semantics comparable?
3. Are resource and information conditions aligned?
4. Is the causal contrast re-estimated in the target?
5. Is the mediator/pathway also tested in the target?

Only (4) supports causal transportability; (5) is required for mechanism invariance.

---

# 11｜P0 Coverage-Gap Freeze

Based on Registry v1.0 and SIS v0.3.1, P0 freezes the following evidence gaps.

## GAP-01｜Causal Transportability Gap — CRITICAL

Current registry:

```text
T3 = 0
T4 = 0
```

There is substantial performance transfer, but no currently qualified causal-transportability or mechanism-invariance evidence.

## GAP-02｜Mechanistic Mediation Gap — CRITICAL

Many studies contain interventions and outcome gains, but far fewer test:

```math
do(M)\rightarrow Z\rightarrow Y
```

This is the main barrier between CL2 and CL3.

## GAP-03｜CSCI Identification Gap — HIGH

Many papers vary model IDs, but few use explicit factorial / interaction designs to estimate:

```math
Effect(M)=f(ComponentCapability)
```

This is the key gap for the former EI-SMCT question.

## GAP-04｜ASR Selective-Action Gap — HIGH

The literature increasingly studies routing, stopping, probing, memory use, budget allocation and enforcement, but few experiments expose a complete action space including:

```text
NO_CHANGE
ABSTAIN
PROBE
VERIFY
RETRY
ESCALATE
RECONFIGURE
INTERVENE
STOP
```

under matched action costs.

## GAP-05｜SDR Ground-Truth Dynamics Gap — HIGH

Many failure-attribution papers infer propagation from observed traces. Fewer combine:

```text
known injected fault
+ full state-transition ground truth
+ propagation
+ containment
+ recovery
+ terminal outcome
```

in the same experiment.

## GAP-06｜Evidence Independence / Self-Confirmation Gap — HIGH

Optimizer-generated judges, tests, rubrics, synthetic evidence and self-reflection may share failure modes with the optimized system. Independent evaluation authority is often incomplete.

## GAP-07｜Selection Reliability Gap — MEDIUM-HIGH

Many optimization papers report best candidate or mean lift, but fewer ask whether the optimizer reliably selects the right intervention under a fixed budget.

Required metrics should include:

```text
SelectedRepairReliability@Budget
FalseRepairRate
RegressionRate
Repeatability
WorstConditionLift
```

## GAP-08｜Tier-3 Mechanism Transport Gap — HIGH

Real-world vertical demonstrations exist, but few preserve a clearly identified mechanism from controlled systems into Medical AI, scientific systems, coding, design or other real-world contexts.

---

# 12｜Calibration Set Freeze

Before scaling to all 112 primary research candidates, P0 freezes a 12-study calibration set balanced across Programs and evidence patterns.

## SCF calibration

1. `SIS-LIT-024` — MA-Evolve / Equal Inference Cost
2. `SIS-LIT-084` — ContrAgent
3. `SIS-LIT-102` — Grow the Harness, Not the Context
4. `SIS-LIT-108` — Reasoning as Gradient

## SDR calibration

5. `SIS-LIT-077` — Chronicle
6. `SIS-LIT-086` — Flag Game
7. `SIS-LIT-089` — ARCHITECT
8. `SIS-LIT-103` — CausalLoss-Fin

## ASR calibration

9. `SIS-LIT-018` — AgentGrad
10. `SIS-LIT-055` — When Agents Slow Down
11. `SIS-LIT-104` — How Strongly Should Task State Influence an LLM Agent?
12. `SIS-LIT-106` — FIRE

This set intentionally includes:

- positive effects;
- negative/null evidence;
- iso-compute controls;
- randomized controls;
- replay/counterfactual intervention;
- mediator candidates;
- component-capability interaction;
- stopping/resource allocation;
- influence regulation;
- causal-variable coverage.

Calibration success is required before bulk claim extraction.

---

# 13｜Execution Plan after P0 Freeze

## P0.1｜Corpus Identity, Version & Source Qualification

**Input:** 113 Registry records.  
**Output:** canonical `StudyVersionRecord` for every record, duplicate/version lineage, primary-source status and qualification state.

Pass condition:

```text
100% records assigned a qualification status
100% primary-evidence candidates have a resolvable canonical source or are explicitly PENDING
0 silent duplicate counting
```

## P0.2｜12-Study Claim Extraction Calibration

**Input:** frozen calibration set.  
**Output:** claim records, dual routing, maturity audit and adjudication log.

Operational calibration targets (P0 process thresholds, not SIS scientific laws):

```text
Primary Program routing agreement: Cohen's κ ≥ 0.80
CL0–CL3 exact/adjacent agreement: ≥ 90%
Source-anchor completeness: 100%
Unresolved disagreements: 0 before scale-up
```

## P0.3｜High-Priority Causal / Mechanistic Re-Audit

**Input:** 47 candidate records.  
**Priority:** all current `CL2`, `CL2 candidate`, `CL1→CL2 candidate`, `CL2→CL3 candidate` records.

Main goal:

```text
confirm / demote / promote / split / quarantine
```

No candidate label survives without explicit source-anchored justification.

## P0.4｜Descriptive / Associational Re-Audit

**Input:** remaining 66 records.  
**Goal:** confirm descriptive/performance claims, extract negative evidence, identify hidden causal language, and detect claims that should enter the causal queue.

## P0.5｜Coverage Matrix & Evidence Map Freeze

Produce:

```text
Program × Estimand × ClaimLevel
Program × IdentificationDimension
Program × BoundaryVariable
CSCI × ComponentCapabilityRegime
BGT × TransportStage
FrameworkCapability × ScientificUtility
```

and freeze the first SIS Evidence Map release.

---

# 14｜P0 Non-Negression Rules

P0 must not:

1. create a fourth Primary Program because a new implementation label appears;
2. promote a Framework into a Scientific Primitive;
3. promote claim maturity from paper reputation, venue prestige or benchmark score;
4. equate cross-model performance transfer with causal transportability;
5. equate ablation with causal mechanism without checking intervention specificity;
6. collapse paper-level and claim-level routing;
7. delete negative/null evidence because it weakens an attractive narrative;
8. let community analyses overwrite primary-source evidence;
9. use SIS/ARSO/MOSA/EI-SMCT names as routing features;
10. modify SIS v0.3.1 Core merely to fit a literature taxonomy.

---

# 15｜P0 Deliverables

P0 freezes the following repository deliverables:

```text
literature/evidence-map/
├── SIS_Literature_Evidence_Map_P0.md
├── SIS_P0_ClaimRecord_Schema.yaml
└── SIS_P0_Audit_Queue.csv
```

Future execution outputs should add:

```text
claims/
  claim_records.jsonl
adjudication/
  calibration_adjudication.md
matrices/
  program_estimand_claimlevel.csv
  identification_coverage.csv
  transportability_matrix.csv
reports/
  P0_final_evidence_map_freeze.md
```

---

# 16｜P0 Freeze Decision

The current literature corpus does **not** justify a SIS v0.3.2 Scientific Core revision.

It does justify a stricter evidence program.

```math
\boxed{
PaperLevelRegistry
\rightarrow
ClaimLevelEvidenceMap
}
```

The immediate research priority is therefore not to add concepts, but to determine:

```math
\boxed{
Which\ claimed\ system\ effects
are\ merely\ performance\ associations,
which\ are\ controlled\ causal\ effects,
which\ have\ mechanistic\ mediation,
and\ which\ survive\ boundary\ and\ transport\ tests?
}
```

**P0 status:** `FREEZE PASS`  
**Next executable stage:** `P0.1｜Corpus Identity, Version & Source Qualification`.