# SAR-03-A｜Claim-Level Program Routing Coverage & Negative Routing Stress Test

> **2026-10-28 · SYNTHETIC CONCEPTUAL REVIEW COMPLETE WITH OPEN GAPS · NON-NORMATIVE.**  
> `SAR-03-A: SYNTHETIC_ROUTING_REVIEW_COMPLETE_WITH_OPEN_GAPS`; `SAR-03: IN_REVIEW / OPEN`; `R5.1 Master: UNCHANGED`. This is NOT a final Gold classification, independent-coder consensus, empirical inference, physical-schema validation or proof of scientific completeness.

## 0. Scientific source authority / conditional review baselines

Direct source: supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`, 14,825 lines, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`. Source sections:
- §§22–24 L1051–1163: SCF mechanism / organization → system-level property; treatment-control, resource & information, manipulation checks for causal claims.
- §§25–28 L1164–1274: SDR requires a time-/transition-dependent **primary estimand**; timestamps, events and trajectory file names alone do not suffice.
- §§29–33 L1275–1418: ASR requires information-conditioned endogenous action selection; `NO_CHANGE`, `ABSTAIN`, `PROBE`, `VERIFY`, `RECONFIGURE` and others can be valid actions; evidence time ≤ decision point.
- §§34–38 L1419–1651; §94 L6991–7014: CSCI/X1 is component-capability × mechanism effect modification **with a measured construct**, not a model-ID comparison. Boundary/Generalization/Transportability/X2 is cross-cutting; replication, performance transfer, causal transportability, mechanism invariance are distinct.
- §§40–44 L4087–4258: **ScientificClaim** (not paper/framework/model/system) routes via `ScientificQuestion→PrimaryEstimand→ScientificConformance→ProgramRouting`; conditional precedence `DecisionSelection > Trajectory > StaticMechanismEffect` is not a value ranking or keyword rule. One experiment may yield multiple claims; one identified claim → one Primary Program.
- §§45–50 L5039–5174: `ROUTED`, `DESCRIPTIVE_ONLY`, `ROUTING_UNRESOLVED`, `SCIENTIFIC_NONCONFORMANT`. NoForcedRoute is required.
- §§74–82 L6474–6616: CL0–CL7 evidence maturity independent of Program Identity.
- §84 L6681–6842: `ScientificExperimentContract.program_alignment` already contains routing and optional cross-cutting axes. §§165–170 L12466–12575 define reopen conditions RA1–RA6.
- Part VII-A is explicitly `PROPOSED NORMATIVE PATCH`; do not inherit internal `FROZEN` phrasing as a normative grant.

Owner-authorized review baselines only: `SAR-01-D-DEC-001` scientific identity v0.8 and `SAR-02-D-DEC-001` conditional M1 known-bounded-vs-M2 open-component identity review representation. Neither is adopted Master text.

## 1. Audited claim-level rule, not architecture-level labeling

```text
Claim -> PrimaryEstimand -> ScientificConformance -> Route
  A. evidence-conditioned endogenous action-selection/policy value? -> ASR
  B. otherwise primary transition/trajectory/propagation/recovery? -> SDR
  C. otherwise static target mechanism / organization / capability effect? -> SCF
  D. otherwise abstain: DESCRIPTIVE_ONLY or ROUTING_UNRESOLVED
  E. an asserted strong causal/mechanistic conclusion with disqualifying
     confounding, timing, evidence dependence or missing manipulation ->
     SCIENTIFIC_NONCONFORMANT (do not erase other valid descriptive claims)
```

Precedence only adjudicates an *explicitly recoverable primary estimand*. The word `adaptive`, `feedback`, `tool`, `Jev`, `LLM`, `RSI`, `MOSA`, `Agent`, time stamp, or an action existing **never independently forces routing**.

## 2. Five simulated families and 50 researcher-authored claim fixtures

| Family | SCF / SDR / ASR illustrations | Negative routing cases |
|---|---|---|
| A — fixed SOP, rule controller | A01 fixed verifier mechanism→SCF; A02 failure trajectory→SDR; A03 error-conditioned retry policy→ASR | A04 endpoint success, A07 formal bounded solver, A08 timestamps only→DESCRIPTIVE; A05 ambiguous→UNRESOLVED; A06 mixed resources causal claim→NONCONFORMANT |
| B — Jev-like bounded learned selector + SOP | B01 controlled chooser effect→SCF; B03 stale-state error propagation→SDR; B02/B08 abstain or NO_CHANGE policy→ASR | B04 isolated classifier score→DESCRIPTIVE; B05 “System One” label→UNRESOLVED; B06 post-decision information, B07 changed option generator→NONCONFORMANT |
| C — weak LLM + strong *non-LLM* body + manuals | C02 verification mechanism→SCF; C05 tool fault recovery→SDR; C04 select verification→ASR; C03 measured component ability × mechanism→SCF plus X1 | C01 package noninferiority without component attribution→DESCRIPTIVE; C06 hidden strong LLM, C07 no no-brain control for necessity, C10 future guideline use→NONCONFORMANT |
| D — dynamic known/open component membership | D01 active population/organization effect→SCF; D02 birth–retirement trajectory→SDR; D03 choose add/retire from legal evidence→ASR | D05 non-equivalent M1/M2 estimand and D09 generic “adaptive architecture”→UNRESOLVED; D10 activation mislabeled novel identity→NONCONFORMANT; D08 timestamps endpoint→DESCRIPTIVE |
| E — feedback learning / strong-RSI hypothesis | E01 feedback-training contrast→SCF; E02 intergeneration forgetting and recovery→SDR; E03/E04 policy chooses modification target or NO_CHANGE→ASR; E10 fixed memory-promotion gate effect→SCF | E05 fixed optimizer increasing task scores→DESCRIPTIVE; E06/E09 strong RSI label with undefined estimand→UNRESOLVED; E07 manipulated evaluator/E08 reused reward→NONCONFORMANT |

**Conditional classifications, NOT observed scientific results:** among 50 hypothetical claim fixtures, 26 are expected `ROUTED` (**SCF=13; SDR=6; ASR=7**), 9 `DESCRIPTIVE_ONLY`, 6 `ROUTING_UNRESOLVED`, and 9 `SCIENTIFIC_NONCONFORMANT`. The 24 non-routed claims explicitly have `primary_program=NONE`. The fixture mixture is selected for adversarial coverage, not sampled from literature.

### Same scientific experiment with different claims (three synthetically grouped triads)

- `E-FIX-01`: A01 SCF verifier; A02 SDR propagation/recovery; A03 ASR conditional retry/escalate.
- `E-WEAK-01`: C02 SCF verifier; C05 SDR tool-outage recovery; C04 ASR uncertainty-conditional verification.
- `E-STRUCT-01`: D01 SCF assigned component set; D02 SDR time-varying birth/retirement; D03 ASR observed-load-based component add/retire selection.

Three programs coexist **across different ScientificClaims**, never as three Primary Programs for one identified claim.

### X1/X2 evidence non-inflation

Only C03 is an explicit synthetic CSCI/X1 *construct-level* interaction example: it separately measures capability to use/interpret tools and the controlled verifier mechanism. Multiple model names alone are not X1. A07/A10/B10 explore bounded generalization or context boundary as X2 review examples, **not** an automatic causal-transport finding. A descriptive claim with X2 focus can remain `DESCRIPTIVE_ONLY`.

## 3. Finite deterministic checks actually executed (not independent Gold)

The active local audit bundle contains full source-linked 50-row CSV/JSON fixtures, 30 adversarial mutation fixtures, a 22-row design non-regression review, source-anchor validation, Python rules/test runner, SHA-256 manifests and a ZIP. The checks actually run:
- **29/29** exact section/line anchor assertions on the supplied R5.1 candidate;
- **50/50** consistency checks between reviewer-authored expected labels and a deterministic review-only routing rule;
- **30/30** reviewer-authored mutated negative/invariance fixtures checked by the same rule;
- **3/3** same-experiment/different-claim SCF/SDR/ASR triads;
- Four canonical status categories explicitly represented; CSCI/X2 orthogonality checked.

These are **internal fixture/logic checks**, not independent expert adjudication, not executed real-model experiments, and not evidence of an empirical SIS law or independent cross-program discrimination accuracy. **Real systems evaluated = 0; formal schema/runtime conformance = NOT_EXECUTED; G-E = NOT_EXECUTED.** The arbitrary 50-case fixture distribution is not prevalence.

## 4. Strongest open scientific objections

| ID | Priority | Scientific failure mode | Minimum next test |
|---|---|---|---|
| **R-01** | HIGH | Policy selection changes long-run transitions, so ASR/SDR assignments can vary with a weakly specified estimand; precedence should not rescue an ambiguous case | Matched-pair question rewrite and blind independent claim coding; use `ROUTING_UNRESOLVED` when estimand cannot be recovered |
| **R-02** | HIGH | M1 active-component changes and M2 new-identity changes can appear behaviorally equal while the causal intervention/identity/estimand differs | Require stable ID, creator, version, effective graph, authority, event lineage and intervention/estimand mapping, or `REGIME_COMPARABILITY_UNRESOLVED` |
| **R-03** | MEDIUM | A routable hypothesis confused with *identified* causal evidence; low-level descriptive/fixed-system research falsely excluded or falsely promoted | Independent review of status vs CL ceiling; preserve CL0/CL1 and negative/zero effect |
| **R-04** | MEDIUM | CSCI and X2 become automatic tags based on model names or nominal contexts | Blind construct-vs-name and tested-boundary-vs-reported-domain comparisons |
| **R-05** | DEFERRED | Strong RSI may require more exact meta-improver identity, evaluator/time and intergeneration estimand semantics | SAR-04 exact F0–F3 / meta-improver scientific contract and RA1 reopen tests |

## 5. Non-regression and recommended minimum action

**22** source-anchored design non-regression dispositions were reviewed; neither a new Core Primitive, new Primary Program nor compulsory `ScientificExperimentContract` field is justified by the present synthetic set. Existing source §42/43/44 routing, §45–50 abstention, §94 CSCI and the X1/X2 cross-cutting status remain review invariants.

**Scientific status:** `G-S=CONDITIONAL_REVIEW_WITH_OPEN_GAPS`, `G-O=NOT_EXECUTED`, `G-E=NOT_EXECUTED`. Source R5.1, §9/§6/§8 semantic ambiguities, unadopted Part VII-A, SAR-01 O1/O2, NR-13/NR-14 and SAR-02-D open gates all persist.

**Proposed next unit:** `SAR-03-B | Estimand Separation, Cross-View Identity & Blind Negative Routing Kill Audit` targeting R-01/R-02 and independent-coder classification. **SAR-03 remains IN_REVIEW/OPEN** until further synthesis and explicit science-owner decision. Do not change, merge, freeze or publish official R5.1 Master based on this review.
