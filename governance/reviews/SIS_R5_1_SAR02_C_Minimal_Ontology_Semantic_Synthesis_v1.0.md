# SAR-02-C｜Minimal Ontology Semantic Synthesis & Non-Regression Proposal

> **2026-10-28 · NON-NORMATIVE SCIENTIFIC REVIEW**  
> **SAR-02-C = REVIEW_CANDIDATE_COMPLETE; SAR-02 = IN_REVIEW / OPEN; Master = UNCHANGED.**  
> This review **does not** adopt a new primitive, alter the R5.1 Master, announce schema conformance, or establish a system-intelligence law.

## Source authority

Primary: user-supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`, 14,825 lines. SAR-01-D decision `SAR-01-D-DEC-001` accepted Scientific Identity v0.8 **for review use only**. SAR-02-A/B provide a 16-role source inventory, five synthetic system expressions, 24 **bounded finite-model** checks from B, and 28 conceptual kill-test expectations. R5.1 Part VII-A remains explicitly **PROPOSED NORMATIVE PATCH**. Review latest R5.1 as a scientific candidate, not a historical diff.

Source anchors: §5 L536–566; §6 L570–604; §8 L632–662; §9 L666–700; §10 L704–723; §16 L849–877; §19 L929–962; §20 L964–995; §32 L1363–1391; §33 L1395–1415; `ScientificExperimentContract.context.time_horizon` L6721.

## Recommended scientific conclusion

**`KEEP_CORE_OBJECT_ROLES + MINIMAL_SEMANTIC_CLARIFICATION + CONDITIONAL_MEMBERSHIP_REGIME`**. No newly necessary Core ontology kind was demonstrated. But complete ontology sufficiency and zero normative-semantic-delta are **not** established. In particular, the §9 `X_t ≠ O_t` notation and the §6/§8 fixed `C` formulation remain Science Owner interpretation questions.

### Six minimal semantic findings

| Issue | Minimal scientific interpretation | Disposition |
|---|---|---|
| **G-01** State–Observation | Different epistemic roles/source objects; under legal perfect observation the **payload values can coincide**, `O_t=g(X_t)` with `g=id`. Literal universal *value* inequality is refuted by the simple counterexample. | CLARIFICATION CANDIDATE, no new Primitive |
| **G-02** component membership | M1 fixed potential `C*` and M2 time-varying `C_t` are **conditionally valid** under different universe/identity assumptions. Neither representation's membership snapshot alone preserves all identity/provenance history. | HIGH; M1/M2 owner choice OPEN |
| **G-03** Relation–Policy–Dynamics | `R_t` determines availability/authority and organization, `π(H_t)` selects proposed action, guard/execution and `F` determine actual authorized execution and transition. | CLARIFICATION CANDIDATE |
| **G-04** Context Information–Observation–History | `Ω.Information` states exogenous availability, `O_t` is measured runtime information, `H_t` is legally available history; preserve source and `EvidenceTime≤DecisionPoint`. | CLARIFICATION CANDIDATE |
| **G-05** time horizon | Declare horizon `T` in the scientific question/existing experiment context; `context.time_horizon` already exists. | NO new schema/primitive |
| **G-06** singleton/no-op | Allow `|C|=1`, empty inter-component `R`, fixed policy, `NO_CHANGE`, identity `F`. Scientific claim routing remains estimand-first. | ADMISSIBILITY CONVENTION |

### G-02｜M1 versus M2 by scientific question

**M1, bounded known universe.** Assume a stable potential ID space `C*`, `active_t ⊆ C*`, and version/provenance recorded in `X_t` or ordered events. Effective `C_t^active={c in C*:active_t(c)=1}`, `R_t^eff=R_t ∩ (C_t^active×C_t^active)` and `A_t^eff=Γ(C_t^active,R_t^eff)`. This does **not** literally follow from unmodified §8 `Γ(C,R_t)` without an effective-architecture interpretation. SAR-02-B previously exhausted **512** three-step traces under a finite known three-ID universe. SAR-02-C rechecked their active-set/edge projections, not an independent full-domain proof.

**M2, open dynamic membership.** `S_t=(C_t,R_t,X_t,O_t,π_t)` and `A_t=Γ(C_t,R_t^eff)` express independently addressable creation/removal/replacement more directly. However, introducing `C_t` changes the formal semantics of §6/§8 and may affect §19/§20 dynamics/trajectory and the experiment contract. No such change was authorized or written.

**Finite counterexample boundaries.** The prior B test exhausted **16,739** mappings for capacities `n=1..5` from `n+1` identities into a closed `n`-slot universe, with no injective mapping (pigeonhole principle). This **does not** rule out a larger/open/infinite potential universe or interpreter-based behavioral simulation; behavioral equivalence does not imply component identity/intervention/provenance equivalence.

**Counterexample against overclaiming M2:** `create(a,srcX)→delete(a)→create(a,srcY)` and `create(a,srcX)→disable(a)→enable(a)` can have the *same final* `C_t={a}` but distinct component lineage and authorization. Both M1 and M2 therefore need source/creator/version/generation, permission and ordered lifecycle events as appropriate to the scientific claim. Mere membership snapshots are not sufficient.

**Proposed selection criterion** (not adopted): favor M1 for a justified closed/known capability-resource universe when activity/identity/authority/architecture can be recovered; allow M2 as a **separate time-indexed representation proposal** when the estimand is about genuine new capability-bearing identity under an open membership boundary. Preserve observational **and intervention/lineage** semantics. A component version change does not automatically imply a new identity.

## Directed non-regression (review, not conformance)

Preserve five measured properties; Context, Components/Relations/State/Observation/Control plus external Dynamics; architecture derived not primitive; Mechanism≠Process≠Property; SCF/SDR/ASR and CSCI/X2; ScientificClaim/Estimand-first routing; CL0–CL7, reference independence and time cutoff; no sixth `SystemIntelligenceScore`; no new Program, Primitive, or required schema field; Part VII-A PROPOSED.

**Still open:** §9's frozen symbolic role/value wording (G-01), §6/§8/§19/§20 change if M2 (G-02), effective-architecture semantics for M1, SAR-01 O1/O2, NR-13/NR-14, strong RSI cross-generation lineage (SAR-04), executable `G-O` and empirical `G-E`. **`ScientificCoreDelta=0` has NOT been verified.**

22 directed non-regression reviews produced; statuses include `DESIGN_PRESERVED`, `SEMANTIC_CLARIFICATION_OPEN`, `SCIENTIFIC_SEMANTIC_DELTA_OPEN`, `NOT_EXECUTED`. No formal conformance PASS.

## What was actually checked

- **SAR-02-B inherited evidence:** 14/14 R5.1 source anchors, 24/24 bounded model checks (512 membership traces, 16,739 finite mapping candidates); these are previous-step tests, not rerun as independent empirical replications.
- **SAR-02-C new checks:** 25/25 source-and-synthetic-model assertions, including R5.1 line anchors, existing `time_horizon`, 512 membership/edge-projection comparisons, distinguishable component event histories, authority, temporal information cutoff, horizon and no-op examples.
- **Real Jev/LLM/SOP/RSI execution:** 0. **Official schema/runtime nonregression:** 0. **Effect/transfer estimates:** 0.
- `G-S=CONDITIONAL_REVIEW_CANDIDATE`, `G-O=NOT_EXECUTED`, `G-E=NOT_EXECUTED`.

A complete local review package also contains the six-issue matrix, 12-dimension M1/M2 comparison, 22 nonregression dispositions, 11 open gates, exact reproducibility script, hashes, and owner decision preview. This GitHub record is the canonical *review summary*; it does not claim the full local ZIP was pushed to GitHub.

## SAR-02-D (decision not yet made)

Science Owner must choose between: **A** conditional dual-view audit policy (recommended, M1 known bounded / M2 open-identity *proposal*), **B** M1 only and defer M2, **C** M2 as a new default *proposal* needing wider nonregression, or **D** defer pending more formal scrutiny. In all branches normative Master modification requires a **separate** authorization. **SAR-02 remains OPEN.**
