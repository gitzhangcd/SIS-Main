# SAR-02-C｜Minimal Ontology Semantic Clarification — Candidate v0.1

> **NON-NORMATIVE. Science Owner approval PENDING.** For SAR-02-D review only; no Master/Schema/Primitive changes.

**G-01 · State / Observation:** Distinguish the epistemic types and provenance of actual State and observed information. An observation map `O_t=g_t(X_{≤t},noise,lag)` may be perfectly informative (`g=id`) so the observed **value may equal** the actual value, while roles and evidence timing remain separate. Interpret current `X_t≠O_t` as a candidate role distinction, **not a universal payload inequality**. Its frozen wording requires owner semantic review.

**G-02 · Dynamic Component membership:** Keep `Component` as capability bearer. For a **bounded known universe** `C*`, activation `a_t`, version and provenance can be recorded in `X_t`/events (M1) and actual architecture derived from **active** members. For **open creation/deletion of independently addressable identities**, `C_t` is a legitimate **M2 semantic proposal**, *not* approved source text. Both regimes must preserve persistent/generation identifiers, origin, authorization and changes needed for the estimand. **A final membership snapshot does not preserve delete-recreate vs disable-reactivate history.**

**G-03 · Relation, Policy, Execution:** `R_t` = organization/dependency/authorized capability paths; `π_t(H_t)` = proposed selected action; guard/execution and `F` = actual allowed action, receipts, state effect. No additional primitive implied.

**G-04 · Information roles:** `Ω.Information` = exogenous information/knowledge-access conditions; `O_t` = runtime observations with origin and error/delay; `H_t` = legally available information and observation history, respecting `EvidenceTime≤DecisionPoint`. Available manuals are not automatically observation or model-internal intelligence.

**G-05 · Time:** Every temporal property/viability/trajectory claim declares evaluation horizon `T`; R5.1's existing `ScientificExperimentContract.context.time_horizon` can carry it. No new field required.

**G-06 · Degenerate cases:** Single capability-bearing component, `R=∅`, constant deterministic `π`, `NO_CHANGE`, and identity transition `F` are legitimate bounded system instances; their mere existence does not confer a causal SIS finding.

## Alternative component-membership representations — decision remains OPEN

M1: `C^*_t = C^*` fixed, `C_t^active={c∈C^*:a_t(c)=1}`, `R_t^eff=R_t∩(C_t^active×C_t^active)`, `A_t^eff=Γ(C_t^active,R_t^eff)`. Requires effective-architecture interpretation and identifier/version/lineage tracking.

M2: `S_t^{M2}=(C_t,R_t,X_t,O_t,π_t)`; `A_t^{M2}=Γ(C_t,R_t^eff)`. More direct for dynamic identity, but a real §6/§8/§19/§20 formal semantic change if adopted; also needs provenance lineage.

**No new Core Primitive, no normatively adopted `C_t`, no CoreDelta=0 guarantee, no RSI proof, no actual-model validation.** `SAR-02-C=REVIEW_CANDIDATE_COMPLETE`; `SAR-02=OPEN`.
