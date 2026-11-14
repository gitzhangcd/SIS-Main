# SAR-05-A｜Prospective Matched Capability/Support Causal Study Protocol v0.1

> **PROTOCOL DESIGN ONLY: not an executed agent study, not an added SIS physical schema.** Relevant R5.1 §§5,22–24,34–38,84; Part VII-A §39D–Q is `PROPOSED NORMATIVE PATCH`.

## Target questions, distinct estimands

**Mechanism effect at fixed component capability and information:** `Δ_M(c,i,Ω,R)=E[Y(c,do(M=1),i,Ω,R)]−E[Y(c,do(M=0),i,Ω,R)]`. The support intervention M must be specified: SOP/verification/routing/organization, not merely “strong body”.

**Effect modification / CSCI:** `Ψ=Δ_M(c_w,i)-Δ_M(c_s,i)`, including outcome uncertainty and measured c construct. Larger weak gain can be conditional substitution; larger strong gain can be complementarity; near-zero/ceiling can be saturation or measurement failure; negative is harm/overhead. No pattern is presumed.

**System-package comparison:** `D=E[Y(	ext{weak},	ext{support package})]-E[Y(	ext{strong},	ext{simple package})]` may describe conditional effectiveness or noninferiority with prespecified δ. It is **NOT** a mechanism-specific causal estimand unless package factors were governed; equality does not mean internal cognition identity.

**Cognitive-floor claim:** candidate minimal *partial-ordered construct vector* that meets pre-registered Y and risk thresholds for Ω and M, acknowledging missing/infeasible no-model regions. It is distinct from a threshold to use a particular tool interface.

## Minimal study design

1. Pre-register task types, calibration/accuracy/safety/latency/cost endpoint family and risk/budget horizon, claim-level primary estimand and falsifiers.
2. Freeze focal component exact weights/adapters/prompt/version, and B0 baseline support; don't infer measured ability from model name.
3. Stratify using independently measured domain-appropriate component construct c; allow non-LLM/no-model controls **only when task-eligible** and explicitly classify ineligible cells.
4. Allocate component weak/strong × scaffold/verifier OFF/ON × separately available baseline/runtime external info OFF/ON (2×2×2=8 cells) for controlled mechanism vs information effects. Separate additional specialist tools, human runtime and training differences; don't fake matched information in a treatment whose purpose is information acquisition.
5. Match offered resource caps *and* measure realized tokens, calls, compute, latency, human effort, tool access, and opportunities for failure/rollback; compare both quality and net value.
6. Independently freeze evaluator Gold/reference; human reference constructors must be outside the evaluated runtime, or declared runtime participants and no longer independent.
7. Check actual manipulation fidelity for M and I, information cutoff/treatment, component eligibility, no interference and treatment assignment. Pre-register uncertainty, missingness, task/cluster dependence, evaluator calibration, ceiling and negative/harm outcomes.
8. Disaggregate outcomes by domain, difficulty, risk and component construct; for external information, distinguish task baseline/probe/derived evidence from hidden reference and avoid post-treatment leakage.
9. Separate same-context replication from performance transfer, causal transport, and mechanism invariance (R5.1 §38).
10. Never report universal replacement of model intelligence or a scalar Cognitive Floor solely from system-package equality. Strong evidence requires independent causal identification.

## Evidence state and contract ownership

All proposed future real-study elements are **NOT_EXECUTED**. This may be represented in existing §84 ScientificExperimentContract using context, component, capacity, information, causal_roles, intervention, design, measurements, boundary and lineage, *without making new required Core fields*. `RA2=UNTESTED`, `G-O/G-E=NOT_EXECUTED`, `CognitiveFloor=NOT_IDENTIFIED`, `CompensationEffect=NOT_ESTIMATED`; no new Master text.
