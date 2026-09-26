# SIS P0 Claim-Level Re-Audit｜2026-09-26

**Authority:** SIS v0.3.1  
**Audit program:** SIS Literature Evidence Map P0  
**Primary source audited:** SIS-LIT-117 — *When Does Execution Provenance Help Agent Memory Retrieval?*  
**Decision mode:** source-anchored claim splitting; no paper-level maturity inheritance.

## Why this record was prioritized

SIS-LIT-117 entered the queue as a `CL2 candidate`. The full paper contains at least two scientifically distinct effects that cannot share one maturity label:

1. a **candidate-view / provenance-unit effect** that changes the retrieval representation and eligible information surface together;
2. a **graph-conditioned residual-ranking effect** tested while holding the provenance-unit candidates and dense scores fixed.

The paper-level candidate label is therefore split.

## Claim C1｜Source-aligned provenance-unit candidate view

**Claim ID:** `SIS-LIT-117-C1`

**Paper understanding.** The study asks whether memory retrieval improves when retrieval units are aligned with execution provenance rather than flat text chunks. On a synthetic repository-maintenance corpus, provenance-aligned candidates substantially improve budgeted evidence completion relative to flat chunk retrieval.

**SIS routing**
- Primary Program: `SCF`
- Framework Capability: `MI; MEAS; ID`
- Primary Estimand: `CAUSAL_MECHANISM_EFFECT`
- Evidence Role: `SUPPORT + BOUNDARY`
- Final Claim Maturity: `CL1`
- Identification Strength: `I1`
- Transport Stage: `T0`

**Audit decision:** `SPLIT / CEILING AT CL1`

**Reason.** The candidate-view intervention is not a pure segmentation contrast: the eligible information fields and candidate boundaries differ between provenance units and flat chunks. The observed performance difference therefore supports a representation/package effect, but does not isolate which specific representation property caused the gain.

**Boundary evidence.** Benefits concentrate on linked and multi-fact evidence needs rather than direct single-fact retrieval.

## Claim C2｜Typed provenance graph residual over fixed candidates

**Claim ID:** `SIS-LIT-117-C2`

**Paper understanding.** Starting from the same provenance-unit candidates and fixed dense scores, the study adds a trained residual graph model over typed execution/provenance relations. This yields a controlled test of whether graph-conditioned propagation changes retrieval quality beyond the dense candidate view.

**SIS routing**
- Primary Program: `SCF`
- Framework Capability: `MI; ID; MEAS`
- Primary Estimand: `CAUSAL_MECHANISM_EFFECT`
- Evidence Role: `SUPPORT + NULL + BOUNDARY`
- Final Claim Maturity: `CL2`
- Identification Strength: `I2`
- Transport Stage: `T0`

**Audit decision:** `CL2 CONFIRMED FOR CONTROLLED GRAPH-CONDITIONED EFFECT`

**Primary result anchor.** With candidates and seed scores held fixed, the residual graph model improves Full Support@2048 by **4.55 percentage points** with a reported **95% CI of [2.98, 6.18]**; Recall@5 and MRR also increase. The effect is heterogeneous: it is near-null for direct evidence needs and materially larger for linked and multi-fact cases.

**Negative / null evidence retained.**
- random rewiring weakens the benefit;
- artifact I/O edge removal shows no detectable aggregate contribution;
- removing local chunk-adjacency edges can improve results, indicating that more graph connectivity is not uniformly beneficial.

**Why not CL3.** The graph treatment is causally contrasted against a fixed-candidate control, but a distinct mediator pathway is not independently measured and manipulated. The study therefore establishes an intervention effect, not a fully identified `do(M) -> Z -> Y` mechanism.

**Transport ceiling.** The evaluation uses one constructed corpus and does not re-estimate the causal effect in an independent target domain; `T0` is retained.

## P0 implications

1. **Paper-level CL labels are insufficient.** One study contains both a broad package effect with a CL1 ceiling and a cleaner controlled effect supporting CL2.
2. **Negative edge-family evidence matters.** The result is not “graphs help”; relation semantics and task structure determine whether propagation helps, is neutral, or adds noise.
3. **Mechanism claims still stop below CL3.** A controlled component intervention is not the same as mediator/pathway identification.
4. **Transportability remains open.** No T3/T4 evidence is created by this audit.

## Queue actions

- SIS-LIT-117-C1: `CL1`, `SCF`, `T0`.
- SIS-LIT-117-C2: `CL2`, `SCF`, `T0`.
- Paper-level status: `CLAIM_SPLIT_2026-09-26_C1_CL1_C2_CL2`.
