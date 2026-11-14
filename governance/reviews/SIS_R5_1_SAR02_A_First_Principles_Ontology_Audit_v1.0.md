# SAR-02-A｜First-Principles Ontology Inventory, Necessity & Sufficiency Stress Test

> **REVIEW ONLY · SAR-02-A CONCEPTUAL_REVIEW_COMPLETE_WITH_OPEN_GAPS · SAR-02 IN_REVIEW / OPEN · Master UNCHANGED.**  
> Source-of-truth audit conducted 2026-10-28. Do **not** treat review findings as normative changes, empirical laws, a completed official schema test, or proof of semantic completeness.

## Source, decision authority, and scope

Primary source: `SIS-v0.3.1-R5.1-Candidate-Full-Master.md` reading-copy, **14,825 lines**, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`. This is **not** an approved R5.1 release. The **Part VII-A = PROPOSED NORMATIVE PATCH** notice overrides any internal “FROZEN” language inside that proposal.

The SAR-01-D owner decision `SAR-01-D-DEC-001` conditionally accepted v0.8 as an **audit-only** scientific identity/mother-question baseline. Its C1/O1 (avoid over-including routine software engineering), C2/O2 (do not exclude descriptive/formal science for lack of causal identification), NR-13 and NR-14 remain active.

This is a self-contained scientific architecture audit of current R5.1, **not** a comparison with earlier releases.

## Executive scientific result

**Recommendation: `KEEP_CORE_PRIMITIVES; CLARIFY_SEMANTICS; DEFER_NORMATIVE_DECISION`.** The known system categories and five constructed stress cases can be represented at a useful conceptual level, without an immediate need to add an ontology primitive or a fourth Primary Program. **Complete sufficiency is not established.** Two high-priority gaps and several medium-level ambiguities remain.

### Exact ontology layers (do not flatten into “six identical primitives”)

- §5: **Context** `Ω = Task + Environment + Information + Budget + Constraints + Risk`, condition for capability.
- §6–10: **five inside-system primitive roles** `S_t = (C, R_t, X_t, O_t, π_t)`, i.e., Components, Relations, actual State, Observation, Control/Policy.
- §6 and §19–21: **Dynamics** describes evolution `X_(t+1)=F(X_t,E_t,U_t,A_t,ξ_t)`; it is *outside* the five-tuple.
- §4 and §8: Architecture `A_t = Γ(C, R_t)` is **derived**, not a sixth/seventh new primitive.
- §10, §20–21: Action `U_t` and legal history `H_t` are derived/control-related roles; not additional primitive types merely by virtue of appearing in equations.
- §11–12: Mechanism is an explanatory/causal-hypothesis role; Process is temporal; Property is an outcome. `Mechanism ≠ Process ≠ Property`.
- §13–18: **five distinct system properties** `Y = (Capability, Efficiency, Viability, Robustness, Adaptability)`. System Intelligence remains an upper-level interpretive **multidimensional construct**; not a sixth property/scalar/primitive.
- §22–33/§34–38: SCF, SDR, ASR are scientific **question families**, CSCI and X2 are cross-cutting overlays, not ontology objects.
- §40–44: scientific **claim + primary estimand** determines routing; neither system architecture nor implementation brand does.
- §65–68 and §74–82: evidence independence and claim maturity are **epistemic governance**, not necessarily system runtime components.

### Necessity vs compulsory instantiated complexity

For the *research program*, C, R, X, O, π, F and Ω have distinct explanatory roles: remove C and competence provenance disappears; remove R and permission/organization is lost; remove X or O and partial observation is unrepresentable; remove π and decision selection is fused with environment transitions; remove F and the trajectory/recovery/learning question vanishes; remove Ω and capability loses its conditional boundary. This is a **conceptual ablation argument, not a mathematical proof of unique minimality**.

Crucially, not every particular system requires nonempty or nontrivial instances of each role:
- `|C|=1, R=∅` is a legitimate singleton proposal, consonant with §1 “one or more capability-bearing components”.
- Fixed SOPs allow **deterministic** policies; static or one-step systems can use trivial state and identity transition in a modeling convention.
- No learning, generative LLM, multiple agents or positive system-over-component gain is mandatory.
These precise null/empty conventions are **review suggestions**, not a silent amendment to R5.1.

## Ontology questions that block unconditional sufficiency

### GAP-O2A-01 — HIGH: full observability vs literal `X_t ≠ O_t`

§9 defines `X_t = ActualSystemState`, `O_t = ObservedInformationAboutState` and freezes `X_t ≠ O_t`. This *epistemic-role distinction* is scientifically indispensable. **But if interpreted as universal inequality of the two values**, it is problematic for perfectly observed systems where `O_t = g(X_t)` and `g = identity` is admissible.

**Candidate clarification, not adopted:** State and Observation are different **roles/types and provenance identities**, while their values may coincide under a perfect observation mapping. Test separately: identity observer, partial observer, noisy observer, lagged observer. Do not erase the distinction even if the data are equal. This is an ambiguity with a plausible reading, **not a proven inconsistency in the source.**

### GAP-O2A-02 — HIGH: static `C` vs creation/deletion/replacement of components

§6 writes `C` without a time index, but `R_t, X_t, O_t, π_t` vary with time. §19 makes `X_t` dynamic and derives `A_t=Γ(C,R_t)`. For feedback training, fixed model identity plus changing weights may be *modeled as versioned state*, but a system that autonomously creates/removes executable tools or substitutes a model may change actual component membership.

**Two competing minimal interpretations need adversarial tests:**
- **M1:** fixed potential/super-set `C*` with activation, component-version and authority encoded in `X_t,R_t`; risk is unknown/unbounded future components or loss of identity.
- **M2:** explicit time-dependent membership `C_t` with component identity/provenance across generations; risk is a substantive formal-semantic delta even if no new object kind.
Neither is approved; `C` **must not be silently rewritten as `C_t`**. The exact recursive self-improvement/optimizer revision claim stays for SAR-04.

### Medium ambiguity backlog

- **G-03** Authority/control relations (§8) versus Policy (§10): candidate distinction is **relation/allowed authority graph** vs **history-conditioned action selection**; the source does not fully formalize this partition.
- **G-04** `Ω.Information` (§5) versus `O_t` (§9) and `H_t` (§10): distinguish exogenous knowledge/handbook from state measurement and legal decision-time information, with provenance.
- **G-05** Time: `t` and experiment `time_horizon` exist but `Ω` enumerates no explicit time coordinate. Candidate time-context clarification, not new primitive.
- **G-06** Static/no-op: null relations, constant policy, `NO_CHANGE` and identity transition should be explicitly legal conventions, not separate objects.
- **G-07** F0/F1/F2/F3 optimizer/meta-improver cross-generation semantics remain deferred to SAR-04.

## Five-system expression matrix (synthetic only)

| ID | System | Conceptual expression | Main failure / unresolved |
|---|---|---|---|
| F1 | **Single cognitive model** | `C={model}`, `R=∅`, trivial/real X, legal O, fixed π, identity/limited F; bounded capability or SCF if identified intervention | If R forced nonempty or `X≠O` treated as value inequality, valid singleton/perfect observation blocked |
| F2 | **Fixed rule + SOP + verifier** | Typed components, deterministic decision, state/event transitions and verification mechanism; SCF/ASR *only by estimand* | Scope-gate C1: a workflow score is not automatically a scientific mechanism |
| F3 | **Jev-like learned bounded decision + B3 SOP, no LLM** | Decider, option constructor, knowledge, guard and executor are separable C; R authority; O typed decision context; π learned choice with independent action authorization | Missing correct option / cognitive work already done by option designer / stale state |
| F4 | **Weak LLM + strong non-LLM body + manual** | Component and information roles + relations, dynamic actions, Y/Ω, SCF/CSCI or ASR conditional claims | Hidden strong LLM, precompiled test solution, unfair resource/knowledge contrast; no-LLM control needed |
| F5 | **Feedback learner + potential self-modifying improver** | θ, policy/optimizer versions and learning history may be in X, π and F distinguish interventions over time; SCF/SDR/ASR routes depend on primary estimand | Exact C membership reconfiguration and strong RSI validity remain OPEN |

**Assessment:** F1–F4 are **conceptually expressible with specified clarifications/evidence ceilings**. F5 is **abstractly expressible** but **not exact-complete** for component topology modification or strong RSI.

All five are *researcher-authored hypothetical models*, not real agent/LLM/Jev test results.

## Adversarial and non-regression evidence status

- **16 ontology-role inventory rows**, each with source anchor, necessity, non-redundancy and unresolved ambiguity.
- **5 synthetic systems**, each assigned C/R/X/O/π/F/Ω, system property and example estimand.
- **30 adversarial kill-test *expectations*** including singleton-empty-relations, identity observation, fixed policy, Jev option construction, no-LLM equality, hidden stronger model, dynamic tool creation and evaluation contamination. **All: EXPECTED_ONLY / NOT_RUN_REAL_SYSTEM.**
- **20 directed non-regression review rows:** no proposal adds a primitive, schema field, program, SystemIntelligenceScore or automatically adopts Part VII-A. **Formal executable non-regression not run**, no official PASS.
- **49/49 source-anchor and internally constructed fixture/schema *structural checks actually ran and passed in local Python***; independent ontology validity was **not** evaluated by these checks. Their outcomes must never be represented as empirical successes.
- Actual Jev, LLM, SOP, long-horizon feedback, independent evaluator and causal experiments: **0**.
- `G-S=CONDITIONAL_REVIEW_WITH_OPEN_GAPS`, `G-O=NOT_EXECUTED`, `G-E=NOT_EXECUTED`.

**No empirical system-level necessity, sufficiency, RSI or generalization theorem is claimed.**

## Provisional minimum change and handoff

**Decision proposal only:** `KEEP_CORE_PRIMITIVES; CLARIFY_SEMANTICS; DEFER_NORMATIVE_DECISION`.

**Next proposed work unit:** `SAR-02-B | Perfect Observation, Dynamic Component Membership & Role-Overlap Kill Audit`. Test G-01/G-02 head-to-head with small formal countermodels, then G-03/G-04/G-05/G-06. Do not proceed directly to official Master revision or claim a finished SAR-02 decision.

### Local reproducibility package

A complete review package (created in the active conversation container) includes:
- `SAR-02-A_First_Principles_Ontology_Audit_v1.0.md` full Chinese report;
- `SAR-02-A_Ontology_Inventory_v1.0.csv` (16 rows);
- `SAR-02-A_Five_System_Expressivity_Matrix_v1.0.csv` (5 rows);
- `SAR-02-A_Ontology_Kill_Test_Registry_v1.0.csv` (30 expected-only tests);
- `SAR-02-A_NonRegression_Review_v1.0.csv` (20 rows);
- `SAR-02-A_Synthetic_System_Models_v1.0.json`;
- `SAR-02-A_Verification_Log_v1.0.json`;
- reproducible build/verification script, SHA-256 manifest and ZIP.

The GitHub document is a scientific audit record and does **not** imply that all the local package files have been uploaded to GitHub.

**Status: SAR-02-A CONCEPTUAL_REVIEW_COMPLETE_WITH_OPEN_GAPS / SAR-02 IN_REVIEW / SAR-01 REVIEW_ACCEPTED_WITH_OPEN_GATES / R5.1 MASTER UNCHANGED.**
