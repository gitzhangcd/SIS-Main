# SAR-02-B｜Perfect Observation, Dynamic Component Membership & Role-Overlap Kill Audit

> **EXECUTED CONCEPTUAL + BOUNDED FORMAL AUDIT ONLY** — 2026-10-28.  
> `SAR-02-B = FORMAL_COUNTERMODEL_REVIEW_COMPLETE_WITH_OPEN_GAPS`; `SAR-02 = IN_REVIEW/OPEN`; `R5.1 Master = UNCHANGED`.  
> No normative primitive, relation, policy, `C_t`, `X≠O` revision, schema update or science-law freeze has been approved.

## 1. Scientific inputs, exact source and authorization

- Supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md` (14,825 lines; SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`).
- Direct anchors: §5 L536–566 Context; §6 L570–604 `S_t=(C,R_t,X_t,O_t,π_t)`; §8 L632–662 `A_t=Γ(C,R_t)`; §9 L666–700 `X_t ≠ O_t`; §10 L704–723 `U_t=π(H_t)`; §16 L849–877 Viability; §19 L929–962 Dynamics; §20 L964–995 trajectory; §32 L1363–1391 NO_CHANGE/ABSTAIN; §33 L1395–1415 evidence-time integrity.
- Prior decisions: `SAR-01-D-DEC-001` conditionally accepted Scientific Identity v0.8 **for review use only**; `SAR-02-A` identified G-01/G-02 HIGH and role overlaps MEDIUM.
- Part VII-A remains **PROPOSED NORMATIVE PATCH** and is not incorporated as frozen science.

## 2. High-priority formal countermodels

### G-01｜Full observability can have equal values, separate epistemic roles

Take state values `X∈{0,1}` and `O=g(X)` with `g=id`. Then `observed_payload(O)=state_value(X)` for both possible inputs. **This refutes reading §9's boxed `X_t≠O_t` as a universal inequality of observed and actual values.** But `StateRecord(kind=STATE,t,value)` and `ObservationRecord(kind=OBS,t,value,source)` remain distinct typed/source-bound scientific objects, even if their payloads coincide.

Partial `g(x)=x mod 2` (not injective), noisy bit observations, and delayed observations show why the two roles remain necessary in the general SIS domain.

**Disposition:** `ROLE_SEPARATION_KEEP` / `UNIVERSAL_PAYLOAD_INEQUALITY_REJECT`. The original source may intend role inequality; therefore this is a *semantic ambiguity under the literal reading*, not proof of formal inconsistency in the authors' intended model. **Minimum future clarification only:** allow perfect `g=id`, maintain type/provenance/decision-time distinction. No new Primitive.

### G-02｜Finite potential membership is constructively sufficient under conditions, not universally sufficient

Original §6 uses fixed `C` whereas `R_t,X_t,O_t,π_t` vary and §19 only specifies transition of `X_t` using derived architecture.

**M1 constructive encoding:** For known finite `C*={a,b,c}`, define `active_t=C_t⊆C*`, record membership+version in augmented state `\tilde X_t=(X_t,active_t,version_t)`, and project effective relations `R_t^eff=R*∩(C_t×C_t)`. All **512** possible 3-step membership paths over these 8 component subsets were checked, recovering membership and active edges in each case. Such encoding is *conditional* on a known universe, stable IDs, explicit activation state and effective-architecture projection.

**M1 counterexample within finite closed bound:** If `C*={a,b}` is fixed and the runtime system creates three *simultaneously distinct* capability-bearing identities `{a,b,c}`, there is no identity-preserving injection into those two slots. The bounded checker exhaustively enumerated **16,739** candidate mappings for target capacity `n=1..5` and `n+1` identities; none was injective. This is a pigeonhole restriction **of finite closed C***, not a general SIS impossibility theorem.

**M2 alternative:** Time-index membership `C_t` and derive `A_t=Γ(C_t,R_t)`; fits open-world creation/deletion more directly but **would change the formal semantics of §6/§8** if adopted. A generic fixed interpreter with arbitrary programs encoded into state, or an open/infinite potential universe, may preserve behavioral ability without component-provenance or authorization identity; neither possibility is ruled out by these finite models.

**Disposition:** `FINITE_KNOWN_UNIVERSE_EXPRESSIBLE` / `FINITE_CLOSED_NEW_IDS_INSUFFICIENT_FOR_IDENTITY_PRESERVATION` / `GENERAL_UNRESTRICTED_QUESTION_OPEN`. Compare M1 and M2 in SAR-02-C; **do not silently change C→C_t**. Strong RSI provenance and modification-lineage remain for SAR-04.

## 3. Four role-overlap tests and minimum semantic disposition

| Issue | Formal stress contrast | Minimal interpretation; status |
|---|---|---|
| **G-03** Relation–Policy–Dynamics | Same authority `R`, different `π` ⇒ distinct proposed actions; same `π`, different `R` ⇒ accept/deny; same authorized action with different `F` ⇒ different actual state | `R` expresses permission/organizational edge; `π` selects proposed action from legal history; execution guard/`F` produces executed outcome. **CLARIFY, no new Primitive.** |
| **G-04** Context.Information–Observation–History | Same actual/sensed state with two valid prior manuals yields different actions; future manual with `available_at>DecisionPoint` must be excluded | Distinguish exogenous authorized knowledge, dynamic observation and legal `H_t` with provenance/availability cutoff; respect §33. **CLARIFY, no new Primitive.** |
| **G-05** Time horizon | `x_t=t`, viable iff `x≤1`: full-horizon viability holds for `T=1`, fails for `T=3`, despite identical `t=0` | Declare horizon `T` in conditions/evaluation contract (existing Context/Constraints/contract semantic slot possible). **CLARIFY, not a new object kind.** |
| **G-06** Singleton / deterministic NO_CHANGE | `C={solo},R=∅,π(H)=NO_CHANGE,F(x,NO_CHANGE)=x` | Degenerate or fixed systems are legitimate SIS scientific *models*; scientific contribution remains claim-scoped. **ADMIT via modeling convention.** |

**Critically, capability source, authority, selected action and actual execution must not be conflated:** Jev/LLM output is not execution receipt or independent reference.

## 4. What “irreducible” actually means here

- **G-01:** an irreducible **scientific role distinction** (`State` vs `Observation`), *not* an irreducible value inequality.
- **G-02:** nonreducibility holds only under explicit **finite closed identity-preserving** assumptions. It cannot be promoted to a universal need for `C_t` without stronger assumptions. Behavioral equivalence is weaker than component identity/provenance equivalence.
- **G-03/G-04:** role separation is supported by discrimination examples; extra primitive kinds are not justified.
- **G-05/G-06:** necessary to declare scientific boundary/degenerate conventions; no primitive proliferation warranted.

## 5. Actual bounded executions, conceptual fixtures and evidential ceilings

| Result | Exact status |
|---|---|
| R5.1 source SHA and 14 line-anchor checks | **14/14 PASS** — source identity/locations only |
| Finite toy-model / exhaustive check assertions | **24/24 PASS** (includes 512 C-membership paths and 16,739 identity-slot candidate mappings) |
| Adversarial Kill Test registry | **28 expected behaviors specified, 0 external system executions** |
| Directed non-regression review | **22 design/semantic dispositions; no formal schema/runtime execution** |
| Actual Jev/LLM/SOP/optimizer trials | **0** |
| `G-S` | **CONDITIONAL_WITH_OPEN_SEMANTIC_GAPS** |
| `G-O` | **NOT_EXECUTED** |
| `G-E` | **NOT_EXECUTED** |

Local reproducible package in the active conversation contains complete Chinese report, 24 case-level executable results, 6-issue sufficiency matrix, 28 expected-only kill fixtures, 22 non-regression review rows, `reproduce_sar02b.py`, JSON verification log, SHA-256 manifest and ZIP. This GitHub file is a review record and does **not** assert every local artifact was committed verbatim.

## 6. Directed non-regression and open safeguards

**Preserved by proposed interpretation, not formally proven by a normative runner:** five system-level properties; one-or-more components; separate `Ω` and `S_t`; five tuple roles plus external Dynamics; derived architecture; fixed/no-op policies as permissible special cases; Mechanism≠Process≠Property; `SCF/SDR/ASR`, `CSCI/X2`; claim/estimand-first routing; evidence time and reference independence; CL0–CL7; no new Core schema fields/UniversalIntelligenceScore; Part VII-A remains PROPOSED.

**Still OPEN:** G-01 source wording and owner semantic approval, G-02 identity-preserving open membership alternative, G-03/G-04/G-05/G-06 precise conventions, SAR-01 O1/O2 and NR-13/NR-14; formal implementation and empirical gates. `ScientificCoreDelta=0` has not been certified and **no Master patch was applied**.

## 7. Recommendation and subsequent work

`KEEP_CORE_OBJECT_ROLES; CLARIFY_SEMANTICS_WITHOUT_NEW_PRIMITIVE; G02_M1_VS_M2_DECISION_DEFERRED`.

**Next: `SAR-02-C | Minimal Ontology Semantic Synthesis & Non-Regression Proposal`** — consolidate only six minimal clarifications and isolate G-02 M1/M2 with strongest arguments; prepare the single owner decision for SAR-02-D. Only SAR-02-D can approve a review baseline; normative Master updates require separate later authorization.

**Overall:** `SAR-01 = REVIEW_ACCEPTED_WITH_OPEN_GATES`; `SAR-02 = IN_REVIEW/OPEN`; `SAR-03–SAR-10 = NOT_STARTED`; `main` untouched.
