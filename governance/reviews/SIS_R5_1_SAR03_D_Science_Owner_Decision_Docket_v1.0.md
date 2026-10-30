# SAR-03-D｜Scientific Program Separation — Science Owner Decision Docket v1.0

> **DECISION READY / OWNER CHOICE = PENDING / SAR-03 = IN_REVIEW OPEN / NON-NORMATIVE.**  
> Audit docket date: **2026-10-29**. Entering SAR-03-D does **not** authorize a decision. No new Primary Program, Primitive, enum or mandatory Schema field; **no R5.1 Master edit, release, merge or scientific freeze**.

## 1. Exact decision object, authority and evidence ceiling

**Decision ID:** `SAR-03-D-DEC-001`. The question for the Science Owner is:

> Should SAR-03-C's **minimum scientific separation of SCF / SDR / ASR by each ScientificClaim's recoverable PrimaryEstimand**, four canonical negative/abstention statuses, CSCI/X2 cross-cutting boundaries, and conditional M1/M2 cross-view comparability rules be accepted **only as an audit-level scientific review baseline**, while independent coding (RA2) and all official scientific/engineering proof gates remain open?

**Source:** supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`, **14,825 lines**, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`, especially §§22–38, §§40–50, §§74–82, §§165–170 (RA1–RA6, §166 RA2). SAR-01-D `SAR-01-D-DEC-001` (Scientific Identity v0.8) and SAR-02-D `SAR-02-D-DEC-001` (M1/M2 conditional dual-view) are **approved for scientific review only**; neither was normatively inserted into R5.1.

**Evidence actually available:**
- SAR-03-A: **50** authored synthetic Claim fixtures: 26 expected routed (SCF 13 / SDR 6 / ASR 7), and 24 expected nonrouted (9 descriptive, 6 unresolved, 9 scientifically nonconformant). **Author-labelled, not empirical prevalence, not independent Gold.**
- SAR-03-B: **48** unanswered blind-review tasks, split **24** claim-estimand contrasts, **12** M1/M2 representation cases, and **12** negative cases; **12/12 bounded synthetic countermodels**; the two reviewer task sets are differently ordered, blank, and separated from the controller's author-written answer key.
- SAR-03-C: minimum 3-Program contract, **12** M1/M2 review comparability criteria, **18** negative-routing fixtures, **24** design-level non-regression reviews (**14** `DESIGN_PRESERVED` and **10** restricted/open/other), **17** retained open gates, **58/58 source/fixture/metadata assertions PASS**. These tests reflect authored materials, not independent taxonomy validity.
- **Triads S6 and S8 mix original source-claim system families**: all eight triads are *conceptual question contrasts*, **not eight matched empirical experiments**.
- Independent Worker A responses = **0**; Worker B responses = **0**; external adjudication = **0**; independent Gold = **NONE**; Cohen's κ = **UNAVAILABLE**; **`RA2=UNTESTED`**, not PASS and not `NOT_TRIGGERED`. Official `G-O=NOT_EXECUTED`, real-system `G-E=NOT_EXECUTED`.

### What is sufficiently supported now

At the **formal definition/author-constructed case level**, the following three *primary-estimand question families* are separable:

| Program | Irreducible target of the particular claim | Misleading surface attribute that must not trigger route |
|---|---|---|
| **SCF** | Mechanism/organization/component interaction → conditional system property, with intervention/matched evidence required for causal conclusion | Tool present, new Agent, static SOP, model name |
| **SDR** | Functional of state transitions, propagation, containment, recovery or time-dependent trajectory | Time stamp, trace file, terminal score alone |
| **ASR** | Endogenous action selection/policy value conditional on legally available information at the decision point | “Adaptive”, “feedback”, policy component, retries alone |

One experiment may support **multiple ScientificClaims**; **one identified Claim has one Primary Program** (§44). The priority `DecisionSelection > Trajectory > MechanismEffect` applies **only to an already recoverable PrimaryEstimand** (§42–43), never as a keyword shortcut. CSCI/X1 and Boundary/Generalization/Transportability/X2 are cross-cutting, not fourth/fifth Primary Programs.

### Canonical statuses are immutable as review invariants

`ROUTED`, `DESCRIPTIVE_ONLY`, `ROUTING_UNRESOLVED`, `SCIENTIFIC_NONCONFORMANT` (§45–50) remain four distinct claim-level statuses. `REGIME_COMPARABILITY_UNRESOLVED` is solely a **review annotation**, not a fifth canonical routing status. Valid descriptive/formal/null/negative evidence should not be excluded from SIS merely because causal identification is absent. A fatal causal claim defect applies to that claim, not automatically the entire study.

## 2. Strongest opposing argument — three logically distinct attacks

**A. Definitional separability is at risk of being tautological.** SCF, SDR and ASR are made distinguishable by writing the task's PrimaryEstimand in their own defining language. A study's result can be unchanged while the researcher rephrases it as a “policy-value”, “recovery-trajectory”, or “architecture mechanism” statement. If independent scientists cannot infer the same primary scientific question from complete study contracts (not just labels), the taxonomy's **reliability and discriminant validity remain unestablished**. The 50/48 authored fixture checks test consistency under the same author's framing. They do not test independent agreement. **RA2 §166 is UNTESTED.**

**B. A coupled closed-loop estimand may be irreducible to the neat partition.** Consider a system that observes errors, **chooses to add/retire agents**, thereby changes its capability resource set and transition mechanism, and is measured on a joint resource-constrained long-horizon viability functional. It may be tempting to route the same claim to ASR (choice), SDR (trajectory), or SCF (topology→capability), or to split it. Splitting is legitimate only if it **preserves the actual target quantity and evidence meaning**. If an independently established `Q*` cannot be losslessly represented by SCF/SDR/ASR or cross-cutting CSCI, **RA1 (§165) requires reopening the program architecture**, not forcing a label. **No such irreducible `Q*` has been empirically established here; this is a falsification target.**

**C. Representation-dependent component identity can change the estimand.** Under M1 a new executable procedure may be `State` inside a fixed interpreter; under M2 it may become a new `Component` with a separately addressable intervention. Same endpoint output does not imply the same `do(Component)` response, permission boundary, failure attribution, or identity lineage. The SAR-03-B bounded `Y_A=I·P` versus `Y_B=I` countermodel shows equal baseline outcomes and different `do(P=0)` responses under its constructed assumptions. If M1/M2 mapping cannot preserve the scientific intervention/target, **`ROUTING_UNRESOLVED`** for an underspecified common estimand or **`SCIENTIFIC_NONCONFORMANT`** for an asserted invalid causal equivalence must remain possible.

**Strongest possible rejection of Option A:** Do not call the three programs an accepted scientific taxonomy even for review until truly **independent coders** can reproducibly distinguish R-01 cases and adjudicate R-02 across representations; otherwise *conditional acceptance risks ossifying same-author conventions before measuring the RA2 risk*.

### Scientific response favoring Option A (not approval)

A **review-only provisional baseline** may be useful to proceed with focused SAR-04 (RSI exact scientific contract) and generate stronger falsifiers, provided it is labelled **conditional**, all independent-judgment gates remain open, and no claim of exhaustive or empirically validated Program identity is made. It is inappropriate to count the 58/58 source/fixture checks as evidence of coder agreement.

## 3. Three distinct Science Owner options — all PENDING now

| Choice | Decision code | Consequence **only after explicit owner selection** |
|---|---|---|
| **A — recommended** | `CONDITIONAL_ACCEPT_PROGRAM_REVIEW_BASELINE` | Conditionally accept **three-Program minimum route + four canonical statuses + crosscutting X1/X2 + M1/M2 comparability/abstention** only for later *review* work. Mark SAR-03 `REVIEW_ACCEPTED_WITH_OPEN_GATES`; SAR-04 `READY_TO_START`. **Keep RA2=UNTESTED, R-01/R-02 HIGH OPEN, RA1/RA3–RA6 reopen conditions active, G-O/G-E NOT_EXECUTED.** No Master edit/freeze. |
| **B** | `REVISE_PROGRAM_SEPARATION` | Keep SAR-03 `IN_REVIEW/OPEN`; conduct a minimal SAR-03-C revision on **policy-value vs trajectory** and **representation-dependent identity/estimand**, with explicit ambiguous cases. Do **not** add a Primary Program by default. |
| **C** | `DEFER_PENDING_INDEPENDENT_BLIND` | Keep SAR-03 `IN_REVIEW/OPEN`; obtain two independent completed blinded reviewer responses and third-party adjudication before adopting even a conditional scientific review baseline. The locked reviewer packet and candidate key must remain separated. |

**No selection is implied by the user's request to enter SAR-03-D.** The Science Owner may expressly choose A, B or C in a separate message; only then create an immutable *decision receipt* and authoritative decision register.

## 4. Binding boundaries under any option

1. `ScientificScope ≠ ScientificContribution ≠ ClaimValidity`: do not force routine automation into SIS core science or exclude CL0/CL1 descriptive/formal evidence.
2. `Claim→PrimaryEstimand→ScientificConformance→Routing`; preserve *one identified Claim→one Primary*. Mixed claim text may require splitting or abstaining.
3. Retain exactly the **four canonical routing statuses**; distinguish descriptive and unresolved from scientifically nonconformant claims; independently constrain CL0–CL7 claim strength.
4. X1 requires a measured ComponentCapability construct × mechanism interaction, not mere model-ID comparison; X2 separates replication/performance transfer/causal transport/mechanism invariance, not a new Program.
5. M1 known/bounded `C*` versus M2 unadopted `C_t` **are not globally equivalent**: require identity, creator/generation, version/lifecycle, effective graph, authorization/execution, information cutoff, task/resource/risk/horizon, intervention and **PrimaryEstimand preservation** for cross-view comparisons. Otherwise signal `REGIME_COMPARABILITY_UNRESOLVED` as review-only and abstain/limit the scientific Claim.
6. `RA2=UNTESTED` cannot be relabelled `PASS`, `NOT_TRIGGERED` or “Gold reliability verified”. The **proposed** blind coding raw-agreement and Cohen κ thresholds in SAR-03-B are **not normative** and do not replace §166.
7. **Other reopen/evidence gates remain:** R-01/R-02, RA1/RA3–RA6, O1/O2, G-01/G-02 (source §9 and §6/§8 semantics), NR-13 Scientific Identity normative delta, NR-14/G-07 RSI F0–F3, independent evaluator/reference, G-O/G-E, and the `PROPOSED NORMATIVE PATCH` Part VII-A.
8. **No modification/merge of** `main/specs/System_Intelligence_Science_v0.3.1.md`, no adoption of `C_t`, no new Core Primitive/Program/enum/mandatory Schema, no theory/finding/release freeze.

## 5. Decision receipt placeholder — NOT an approval

- `decision_id: SAR-03-D-DEC-001`
- `decision_owner: SCIENCE_OWNER_USER`
- `actual_owner_choice: PENDING`
- `decision_status: OWNER_DECISION_PENDING`
- `SAR-03: IN_REVIEW / OPEN`
- `RA2: UNTESTED`; `IndependentCoderA/B: NOT_EXECUTED`; `Kappa: UNAVAILABLE`
- `G-O: NOT_EXECUTED`; `G-E: NOT_EXECUTED`
- `R5.1_Master: UNCHANGED_NOT_ADOPTED_NOT_FROZEN`
- `next_action: SCIENCE_OWNER_SELECT_A_B_C`

Historical inputs: [SAR-03-C scientific synthesis](SIS_R5_1_SAR03_C_Minimum_Scientific_Program_Separation_Synthesis_v1.0.md), [SAR-03-C minimum contract](SIS_R5_1_SAR03_C_Minimum_Program_Separation_Contract_v0.1.md), [SAR-03-C open gates](SIS_R5_1_SAR03_C_Open_Decision_Gates_v1.0.csv), [SAR-03-B independent blind protocol](SIS_R5_1_SAR03_B_Independent_Blind_Coding_Protocol_v1.0.md).

**Until owner selection, this document is an official *decision docket*, never a record of approval.**
