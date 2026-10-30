# SAR-04-B｜Meta-Improver Identity, Versioned Causal Contrast & Future-Improvement Kill Audit v1.0

> **2026-10-29 · CONCEPTUAL/EXECUTABLE SYNTHETIC AUDIT · NON-NORMATIVE · SAR-04 IN_REVIEW/OPEN.**  
> `SAR-04-B=SYNTHETIC_CAUSAL_CONTRACT_AUDIT_COMPLETE_WITH_OPEN_GATES`.  
> **RA2 UNTESTED; G-O/G-E NOT_EXECUTED; actual RSI operator causal effects NOT_ESTIMATED; Master UNCHANGED/NOT_FROZEN.**

## 1. Actual input and source authority

Read **original** user-supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md` (14,825 physical lines; SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`). Anchors verified for §1/2/6/9/10, §§19–33, §39E/39R, §§40–50, §84 and RA1/RA2/RA6 (§§165/166/170), **35/35 source headings** in this pass.

Read original SAR-04-A files (not just prior summaries):
- `30` synthetic five-architecture F0–F3 cases;
- `20` previously executed limited toy countermodel records;
- `36` `EXPECTED_ONLY` negative RSI test descriptions;
- `24` directed design-only nonregression records, all official conformance `NOT_EXECUTED`;
- `18` open gates;
- `8` preliminary literature records.

Source does **not** contain frozen F0–F3 RSI semantics or a dedicated recursive self-improvement contract. It does contain §§19–21 Dynamics/Trajectory/History, §§24–33 SCF/SDR/ASR evidence/decisions, §41 claim/estimand-first routing, §84 one canonical ScientificExperimentContract, RA1–RA6 potential reopening conditions. §39E and §39R are in **Part VII-A `PROPOSED NORMATIVE PATCH`**, not an adopted norm. F0–F3 are **review candidates only**, not SIS official new enum or Primary Program. SAR-01-D, SAR-02-D and SAR-03-D previous Science Owner approval statuses are for **review baselines only**.

## 2. Required scientific units: target, improver, independent evaluator

**Review-only identity/evidence objects**:
- `T_g` — versioned, frozen **improvee**: target system/harness/SOP/model/decision-policy on which future modifications are attempted.
- `I_g` — effective **improver**: installed proposal + evaluation-guided selection + promotion/rollback procedure that generates future target updates. Track executable/semantic version, actor who modified it, independent approver/authority, effective invocation and state/lineage receipts.
- `E*` — version-locked **external evaluator** and reference authority, protected from modifications by the tested operator.
- `j ∼ D_future` — a **future improvement opportunity** with a frozen starting `T_g` and defined risk, budget, task information/exposure, allowed interventions and observable outcomes.

**Four separate assertions, none collapses to the next**:
1. The target `T_g` was persistently modified;
2. The changed asset originated from the system, with provenance/authority rather than a human external patch;
3. The **improver** `I_g→I_(g+1)` was actually modified, installed and invoked — **structural F3 candidate**;
4. The newer improver has greater **prospective net improvement value** under matched opportunities and independent evaluation — **strong F3 hypothesis**, currently **NOT ESTIMATED**.

Better target output with unchanged improver does **not** prove F3; a new improver file not installed does **not** establish effective structural F3; even one effective improver edit does **not** establish improved future learning-to-improve, infinite RSI or a universal intelligence law.

## 3. Prospective causal contract — proposal, not observed experiment

**Proposed estimand**, separately defined from target-task outcome:

`theta_meta = E_j [ U(Apply(I_(g+1), T_g, j), E*) - U(Apply(I_g, T_g, j), E*) ]`

Here `j` indexes independent **future improvement opportunities**, and `U` is pre-registered task quality minus actual compute/latency/human/risk and failed-edit/rollback cost. To estimate this causally in a real study, at minimum:

1. Freeze common `T_g`, versions of actual *loaded* `I_g` / `I_(g+1)`, `E*` and data exposures prior to trial. Compare actual execution semantics, not just filenames or hashes. Record author/permission and promotion/rollback receipts.
2. Draw new improvement opportunities unseen at improver development/promotion; isolate `D_dev`, `D_promote`, **sealed `D_future`** and their timestamps. Neither tested improver sees the future outcomes, hidden Gold or external evaluation policy. EvidenceTime ≤ DecisionPoint.
3. Randomize assignment across opportunities or execute **paired isolated cloned environments** with the same starting target and allowed info; control carryover/cross-arm contamination, characterize assignment probabilities and task-family clusters.
4. Match caps and tool options; record **actual** calls/tokens/time/human resource and risk, and include them in a pre-registered net-utility measure. Identical budget cap alone does not mean equal consumed resources.
5. Analyze **opportunities** as units; repeated task scores within one opportunity are not independent experiments. Pre-register paired/clustered uncertainties, heterogeneity, negative/no-change/failure attempts, rollbacks and ITT-like all-proposals reporting.
6. Add sham unchanged-improver, frozen operator, F0 extra retries, F1 external skill/SOP, F2 target-policy change, model-swap and human-author controls as available. Cross-view M1/M2 interventions require identity/authority/estimand mapping, not just equal outputs.

**Strongest counterargument:** If the older and newer improvers are evaluated on different initial targets, different opportunity sets, different evaluators or mismatched budgets, a positive `theta_meta` cannot be attributed to *improver version alone*. Even perfect version identity records do not establish counterfactual exchangeability; real causal identification and transportability must be separately justified.

## 4. Actually executed synthetic checks, with exact evidentiary ceiling

Local self-contained Python builder `build_sar04b.py` actually performed **107/107** source/input/fixture/finite assertions successfully. They include 35 exact source-heading checks, validation of original SAR-04-A 30/20/36/24/18/8 records, 24 constructed paired-opportunity matching assertions and **20 bounded adversarial toy tests** spanning installation, changed target vs improver, evaluator checksum/ownership, future information leakage, compute/cost, evolve-set overfit, discarded failures/rollbacks, human origin, M1/M2 identity and `do(P)` mismatch, permission, stronger-model substitution, `NO_CHANGE`, external SOP persistence, operator version and strong gain, recursion, and pseudoreplication.

**Toy paired value calculation, NOT real evidence**: 24 artificially generated future opportunities (8 easy, 8 medium, 8 hard), each with old/new operator arm, hence 48 *arm rows* but only 24 opportunity units. Both arms share a constructed initial target hash, same evaluator hash and matched 2-call budget cap, but the new algorithm deliberately chooses a stronger change on hard tasks and therefore consumes more actual calls. Under fixed constructed `U = quality - 0.25*actual_calls`, the sample paired synthetic mean is **+0.250** utility units. **This number was constructed by the code's chosen rules: NO real agent ran and NO real or population causal effect was estimated.** E* and D_future are simulated tokens, not genuine sealed independent evaluation assets.

The inherited 36 `EXPECTED_ONLY` Kill Tests **remain not run on real systems**. They have individual mapping to the new 20 finite checks, where applicable. Directed nonregression: 24 entries inherited with **formal runner NOT_EXECUTED**, not certification. 18 prior open gates **all retained**; 7 new exact future-trial/control gates recorded; **25 total open**, none closed.

## 5. Main findings / scientific limitations

- **R4-02/B-01:** Does installed `I` really represent a self-modified *future updater*, or only a target `T`, policy, data/specialist allocation, human-coded patch, uninvoked file or evaluator alteration? Requires function semantics + actual authority/execution, not only code SHA.
- **R4-03/R4-05/B-02:** Strong future-meta-improver effect `theta_meta` **NOT_ESTIMATED**; positive target-task performance from frozen `I` is insufficient.
- **R4-04/B-03:** `E*` evaluator modification, holdout/evolve contamination and selective inclusion of accepted versions can fake performance gain.
- **R4-07/B-05:** M1 known active-component reuse versus M2 minted independent identity may change `do(Component)`, permission, lifecycle and estimand. Behavioral equality ≠ causal/intervention equivalence.
- **R4-09/B-04:** Extra compute/attempts, different tool rights and human source are mechanisms/confounders requiring fair controls and explicit attribution.
- **RA1/RA6:** A joint “strategy→improver→structure→future viability” target is a **scientific falsification candidate**; no independently established irreducible fourth Program was found.
- **RA2:** independent Primary Program coding remains **UNTESTED**; this toy audit cannot close earlier SAR-03 route reliability obligations.

## 6. Status, ownership, handoff

`SAR-04-B=SYNTHETIC_CAUSAL_CONTRACT_AUDIT_COMPLETE_WITH_OPEN_GATES`; `SAR-04=IN_REVIEW/OPEN`; `SAR-04-C/D=NOT_STARTED`; `G-O=NOT_EXECUTED`; `G-E=NOT_EXECUTED`; `RA2=UNTESTED`; `Source Part VII-A=PROPOSED`. **No new Core Primitive, Physical Schema field, Primary Program, normative F0–F3 definition or Master alteration.**

**Next recommended work unit:** `SAR-04-C｜Minimum RSI Scientific Contract Synthesis, Boundary Counterexamples & Non-Regression`. Science Owner SAR-04-D choice would remain a distinct later decision and cannot be inferred from this work-unit request.

## 7. Local package (not byte-for-byte mirrored in GitHub)

Full reproducible source + data bundle: `/mnt/data/SIS-R5.1-SAR04-B_Review_Package_v1.0.zip` (18 files, SHA-256 `91d5e74db8710ae253eb28532e4c408bb4348e9f5cafa07fc7b9ed43cf162770`). Includes full science report, trial protocol, 5 identities, 24 constructed paired opportunities/48 arms, 20 executed synthetic kills, 36 prior-kill coverage, 12 control dimensions, 12 M1/M2 cases, 24 design NR, 25 open gates, 35 exact source anchors, provenance, checks, JSON receipt, Python builder and SHA256SUMS. The GitHub review branch provides **scientific narrative and review indexes**, not an assertion that complete ZIP was pushed verbatim.

Source literature is user-maintained `main/literature` registry and prior SAR-04-A; no new paper or empirical evidence was independently established by this work unit.
