# SAR-03-C｜Minimum Scientific Program Separation Contract v0.1

> **REVIEW CANDIDATE / NOT NORMATIVE / SAR-03-D OWNER DECISION PENDING / RA2 UNTESTED.** Derived only from supplied R5.1 §§22–38, 40–50, 74–82, 165–170, SAR-01-D/SAR-02-D review decisions and source-checked SAR-03-A/B cases. No R5.1 Master modification.

## Seven minimum review clauses (not physical schema)

**S0 – Claim as routing unit.** `ScientificClaim→PrimaryEstimand→ScientificConformance→ProgramRouting` (§41). Never route by paper, system, framework name, LLM/Jev/Agent label. A single experiment can support distinct claims; one identified claim has one Primary Program (§44).

**S1 – SCF.** Primary target: system property change attributed to specified mechanism, organization or component interaction; strong causal assertions require §24 scientific evidence (treatment/control, system Y, explicit estimand, matched resources/info, manipulation check and mediator evidence when claimed). The mere use of a tool is not a mechanism effect.

**S2 – SDR.** Primary target: time-/transition-/trajectory-/propagation-/containment-/recovery-dependent scientific functional. A file name, timestamp or terminal score alone is insufficient (§27–28).

**S3 – ASR.** Primary target: endogenous action choice or policy value conditional on legally available information at the DecisionPoint. `NO_CHANGE`, `ABSTAIN`, `STOP` are admissible. Choice policy, action authority and actual outcome are distinct. Temporal leakage violates conformance (§31–33).

**S4 – Claim separation and precedence.** `DecisionSelection > Trajectory > StaticMechanismEffect` (§43) is a **conditional classification priority**, not a fallback that can rescue a missing estimand. Policy/trajectory/mechanism may lie on one causal path but are not the same target quantity. Split claims when multiple quantities are actually targeted (§44).

**S5 – Keep four canonical statuses.** `ROUTED`, `DESCRIPTIVE_ONLY`, `ROUTING_UNRESOLVED`, `SCIENTIFIC_NONCONFORMANT` (§46–50) are not interchangeable. `DESCRIPTIVE_ONLY` covers valid performance/formal/descriptive evidence without mechanism identification; `ROUTING_UNRESOLVED` applies when PrimaryEstimand cannot be recovered; `SCIENTIFIC_NONCONFORMANT` flags the asserted scientifically invalid causal/mechanistic claim, not necessarily every weaker descriptive claim from that study. Do not invent a fifth canonical status.

**S6 – CSCI/X1 and X2 are crosscutting.** X1 needs an explicitly measured component **capability construct × mechanism effect**, not ModelID. X2 demands a separately stated boundary estimand; `Replication ≠ PerformanceTransfer ≠ CausalTransportability ≠ MechanismInvariance`. Neither is a new Primary Program.

**S7 – Conditional M1/M2 comparability.** M1 bounded/known `C*`, M2 `C_t` **unadopted review-only proposal**. Report identities, creator/generation/version/lifecycle, effective graph, authority/execution, information cutoff, task/budget/risk/horizon, intervention correspondence and **the same PrimaryEstimand** when asserting cross-view claims. Otherwise mark reviewer-only `REGIME_COMPARABILITY_UNRESOLVED`; if common causal target is unrecoverable, canonical `ROUTING_UNRESOLVED`; if identified causal equivalence is falsely asserted despite non-equivalent interventions, `SCIENTIFIC_NONCONFORMANT`.

## Evidence state and scientific limits

SAR-03-A: 50 author-made claims, no independent Gold. SAR-03-B: 48 unanswered blind tasks with separated controller candidate key and 12 limited finite model checks. Two of eight triad groups S6/S8 mix source system families, so do **not** call eight triads controlled same-experiment findings. Independent coder A/B/adjudicator = **NOT_EXECUTED**; reliability, κ = **UNAVAILABLE**, §166 RA2 = **UNTESTED**; G-O and G-E = **NOT_EXECUTED**.

R-01 ASR policy-vs-SDR trajectory ambiguity and R-02 M1/M2 causal identity mapping remain HIGH; RA1, RA3–RA6 and F0–F3 RSI scientific contracts remain open. Part VII-A PROPOSED. No new Primary, Primitive, Scope enum or schema field, no Master adoption/freeze.
