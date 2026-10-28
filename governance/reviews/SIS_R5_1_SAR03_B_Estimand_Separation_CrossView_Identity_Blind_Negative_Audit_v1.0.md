# SAR-03-B｜Estimand Separation, Cross-View Identity & Blind Negative Routing Kill Audit

> **2026-10-29 · REVIEW WORK UNIT / SYNTHETIC + BOUNDED FINITE-MODEL AUDIT.**  
> `SAR-03-B = CONCEPTUAL_AND_FINITE_MODEL_REVIEW_COMPLETE_WITH_OPEN_INDEPENDENT_BLIND_GATE`; `SAR-03 = IN_REVIEW / OPEN`.  
> **NOT a science-owner decision, new Primary Program, independent Gold adjudication, normative Master patch, operational conformance, or empirical system study.**

## Authority and source-of-truth

User-supplied candidate `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`: 14,825 lines, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`. Important anchors:
- §22–24 SCF; §25–28 SDR; §29–33 ASR and `EvidenceTime≤DecisionPoint`;
- §34–38 CSCI/X1 and X2 (cross-cutting, not Primary);
- §40–44 `ScientificClaim→PrimaryEstimand→ScientificConformance→ProgramRouting`, `OneIdentifiedClaim→OnePrimaryProgram`, multi-claim experiments and *conditional* precedence;
- §45–50 four routing states and epistemic abstention;
- §165–170 RA1–RA6, especially **RA2 independent-coder agreement**.
- `SAR-01-D-DEC-001` scientific identity v0.8 and `SAR-02-D-DEC-001` M1/M2 conditional dual-view are **review-only** Science Owner authorizations. §9/§6/§8 and Part VII-A `PROPOSED` remain normatively unmodified.

Existing SAR-03-A input was read **from actual 50-row CSV and 30-row negative mutation fixture files**, not substituted with fabricated claims.

## 1. R-01: policy estimand versus trajectory versus mechanism

**Eight matched system vignettes** were constructed from actual SAR-03-A Claim texts. Each comprises three distinct scientific questions holding the high-level system family together but deliberately changing the **primary target estimand** (24 tasks total):
- Fixed SOP + verifier; Jev-like typed learned selector with option-construction and authority guards; weak LLM + B3 non-LLM body/manual; known potential worker set `C*`; feedback-produced procedural skill resources; failure/retry workflow; versioned optimizer; multi-worker organization.
- **SCF=8**, **SDR=8**, **ASR=8** *authored conditional expected classifications*, not external judge outcomes or measured effects.
- The same adaptive architecture may yield an *intervention on component organization→capability outcome* SCF, a *time/transition-dependent recovery estimand* SDR, and an *information-conditioned activation decision value* ASR, but these must be **distinct ScientificClaims** (§44).
- **R-01 remains HIGH:** observing a policy-induced trajectory does not by itself identify the conditional policy value; estimating time-to-recovery under a policy does not become ASR automatically; `ASR>SDR` only resolves recoverable PrimaryEstimand and cannot force an unspecified “adaptive architecture improved” label.

### Two actually executed finite counterexamples

1. `π_A(h)=VERIFY` if alarm else `NO_CHANGE`; `π_B(h)=NO_CHANGE`. At observed `h=ok`, the actions match, yet under `h=alarm` they differ. One observed action or trajectory is insufficient to identify the choice policy at unseen states.
2. Two outcome paths `(0,0,1)` and `(0,1,1)` have the same endpoint but different path sum and recovery time. An endpoint-only outcome cannot stand in for an SDR trajectory estimand.

These are toy-model existence counterexamples; no real agent performance implication follows.

## 2. R-02: M1/M2 cross-view scientific comparability

**12 matched/unmatched representation examples** were authored with an additional, clearly **review-only** `comparability` disposition; this is **NOT** a fifth canonical Program or routing status.

| Review-only comparability code | Candidate count | Interpretation |
|---|---:|---|
| `CONDITIONALLY_COMPARABLE` | 3 | Declared and matched stable identity, provenance/authority, effective relations, intervention and estimand, under explicit finite assumptions |
| `UNRESOLVED_MISSING_MAPPING` | 2 | Missing identity/causal mapping; no conclusion of equivalence |
| `NOT_EQUIVALENT` | 3 | Known structural or identity distinction, e.g. rewire vs birth, activate vs create, delete-recreate vs disable-enable |
| `INVALID_CAUSAL_COMPARISON` | 4 | Alleged causal comparison invalid due to intervention mismatch, leaked information, hidden stronger model or unmatched budget |

**Routing status is separate from comparability code.** One can have an invalid *strong causal claim* even if the descriptive experiment itself is within SIS; negative status applies to the **claim**, not automatically the whole research topic.

### Actually executed bounded structural causal countermodel

Take `Y_A=I·P` vs `Y_B=I`, baseline `I=P=1`. Both produce `Y=1`. Under `do(P=0)`, `Δ_A=-1` but `Δ_B=0`: equal observed outputs **do not imply equal causal component/intervention effects**. A changed P may be program-state inside interpreter I in M1 or an independent member in M2; scientific mapping cannot be inferred from outputs alone.

Likewise, `delete(a,g1)→create(a,g2)` versus `disable(a,g1)→enable(a,g1)` can yield the same final label `a`, with different generation/source/authority history. Both M1 and M2 require event/provenance records for identity-sensitive estimands.

The finite known-universe **512 activation path projections** were exhaustively checked under a three-component set, but are **not** proof that M1 is generally equivalent to M2.

**Minimum review test:** compare `ComponentBoundary`, actual and potential IDs, origin/generation/version/events, `EffectiveRelations`, legal `ActionAuthority`, `InformationTimeCutoff`, task/risk/resource/horizon, `InterventionSet`, and whether `PrimaryEstimand` is actually preserved. If not established, `REGIME_COMPARABILITY_UNRESOLVED` or appropriately bounded noncomparability is required; these are **audit disclosures, not new physical schema fields.**

## 3. Negative routing and scientific evidence ceilings

**12 additional negative/edge fixtures** cover fixed SOP score-only; time stamp with endpoint score; “ASR” or “RSI” naming but missing estimand; bounded formal symbolic proof; model-only score; deterministic `NO_CHANGE` conditional policy; existing-worker activation mislabeled creation; weak LLM necessity without no-brain control; postdecision information leak; and a controlled SCF effect whose sign may be null or negative.

**Aggregate 48 researcher-authored candidate labels** (selected on purpose, not representative prevalence):

| Canonical routing status | Count |
|---|---:|
| `ROUTED` | 29 (SCF=10, SDR=10, ASR=9) |
| `DESCRIPTIVE_ONLY` | 5 |
| `ROUTING_UNRESOLVED` | 6 |
| `SCIENTIFIC_NONCONFORMANT` | 8 |

There is **no independent Gold** behind these numbers; they demonstrate positive and negative stress coverage, not routing accuracy.

## 4. Independent blind review: prepared, NOT performed

The local work unit produced **48 blinded tasks** in two differently randomized anonymous CSVs:
- 24 PrimaryEstimand triplet items, 12 M1/M2 cross-view items, 12 negative-routing items;
- Worker-only ZIP contains a protocol and **two blank answer templates, no candidate answer key or grouping labels**;
- A distinct full controller ZIP contains a `Controller_Candidate_Key_v1.0.csv`, pairing metadata, finite countermodels, reproducible build and scoring source;
- `score_independent_coders.py` **rejects empty/incomplete responses**; this rejection was actually checked.
- No independent Worker A or B response received; no third-party adjudication; **no agreement rate, Cohen κ or Gold consensus** has been computed.
- The proposed agreement targets are **exploratory reviewer protocol settings**, not SIS normative thresholds. §166 RA2 remains OPEN.

**Do not distribute the controller answer key to a proposed blind reviewer before their responses are locked.** Do not publish it alongside exposed worker tasks before the blind exercise.

## 5. Actual verification and boundaries

| What was done | Correct status |
|---|---|
| Source section/line assertions against local R5.1 SHA | **19/19 PASS** |
| Finite executable countermodel assertions | **12/12 PASS** (includes 512 known-universe paths) |
| Total source/structural/toy-model checks | **67/67 PASS** |
| Proposed adversarial mutation expectations | **24 authored, not run on real systems** |
| Directed non-regression review | **20 review-only dispositions, no official runner** |
| Real Jev/LLM/SOP/RSI empirical experiments | **0** |
| Blind independent coding/adjudication | **NOT_EXECUTED** |
| G-O and G-E | **NOT_EXECUTED** |

**Open science gates:** R-01 (ASR/SDR ambiguity), R-02 (M1/M2 causal identity), R-03 claim strength conflation, R-04 CSCI/X2 inflation, R-05 RSI exactness deferred to SAR-04, RA2 independent coder nonconvergence criterion untested, plus O1/O2, G-01/G-02, NR-13/NR-14, source Part VII-A still PROPOSED.

## 6. Falsifiers and next work unit

- **Falsifier R-01:** independent coders systematically disagree SCF/SDR/ASR on *fully specified, distinct* primary estimands, after accounting for ordinary annotation mistakes and lexical ambiguity → **RA2 reopen condition** could become relevant. No such data yet.
- **Falsifier R-02:** proposed M1↔M2 mapping yields same observed output but different `do(Component)` response, source lineage, intervention permission or decision-point information, while asserting same causal estimand → comparability fails.
- **Abstention safeguard:** some claims remain `DESCRIPTIVE_ONLY`/ `ROUTING_UNRESOLVED` even with valid measurable outcomes; scientifically invalid causal assertions remain `SCIENTIFIC_NONCONFORMANT` without excluding valid weaker descriptions.

**Provisional next:** `SAR-03-C | Minimum Scientific Program Separation & Conditional Synthesis`. It must carry RA2 as **UNTESTED** unless independent blind reviewer responses and adjudication are actually completed. SAR-03-D later owner decision remains separate.

**No change to R5.1 source Master, Core Primitive, Primary Program, normative schema, release tag or main branch.**
