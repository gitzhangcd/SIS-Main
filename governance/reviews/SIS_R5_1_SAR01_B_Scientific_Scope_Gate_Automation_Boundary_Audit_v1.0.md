# SAR-01-B｜Scientific Scope Gate & Automation Boundary Kill Tests

**Scientific Architecture Review | 2026-10-28 | Review-only, NOT NORMATIVE.**  
**SAR-01-B:** `CONCEPTUAL_REVIEW_COMPLETE` | **SAR-01:** `IN_REVIEW / OPEN` | **Master:** unchanged  
**Primary source:** supplied SIS R5.1 candidate (14,825 lines), SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`. This reviews its *current* scientific content, not a release-to-release diff. Its Part VII-A continues to be a **PROPOSED NORMATIVE PATCH**.

## 1. Primary scientific result

**There is no justified implementation-defined hard boundary between traditional automation and SIS.** The right distinction is:
1. **Scientific scope:** specified task-/context-dependent system-level competence or property (capability, efficiency, viability, robustness, adaptability, frontier) and credible boundary.
2. **Scientific contribution:** descriptive characterization / useful control vs a testable mechanism, system organization, transition/recovery or information-conditioned regulation claim.
3. **Claim validity:** independent of admission; a proposed causal claim may be unidentifiable or scientifically nonconformant. Do not turn causal nonconformance into an 'out of scope' classification.

A fixed, no-ML SOP may be a valid primary SIS scientific study **if the target question is a system mechanism / policy / dynamics / boundary** (e.g., independently verified error recovery, observation-conditioned decision policy, or dynamic failure propagation). Mere completion of a precompiled workflow, an isolated compression/sorting speedup, or a single component classification score is **not automatically a new system-intelligence mechanism discovery**. System intelligence remains a higher-level multidimensional construct, not a new primitive or a universal score.

## 2. Candidate five-check Scientific Scope Gate (not adopted, not an R5.1 Core enum)

| Check | Minimum review question | Prohibited shortcut |
|---|---|---|
| S1 System referent and boundaries | Which system, task distribution, context, information and risk envelope? | LLM/ML presence, architecture label or number of components as admission rule |
| S2 Target system property | Which measurable conditional capability/frontier, viability, reliability, robustness or adaptability? | Standalone model score treated as identified system intelligence |
| S3 Scientific question / estimand | Descriptive research allowed; explanatory contribution needs an identifiable mechanism/organization, transition, or policy question and competing explanation | Mere existence of a tool or timestamp decides SCF/SDR/ASR |
| S4 Evidence/provenance and prior capability | Who produced SOP and choice options, when was knowledge available, what was human/resource input, and where is evaluator independence? | Strong expert prior or benchmark answers masquerading as model reasoning |
| S5 Evidential ceiling and scope statement | What claim can the current evidence actually support, including its unknowns? | CL1 comparison upgraded to CL2+ causality, or a fixed SOP called universally intelligent |

Five **non-normative triage labels** were designed for review only: `OUTSIDE_SIS_CLAIM`, `SIS_SUPPORTING_ASSET`, `SIS_DESCRIPTIVE`, `SIS_EXPLANATORY_CANDIDATE`, `SIS_SCOPE_UNRESOLVED`. Do **not** replace canonical R5.1 routing statuses (`ROUTED`, `DESCRIPTIVE_ONLY`, `ROUTING_UNRESOLVED`, `SCIENTIFIC_NONCONFORMANT`) or its CL0–CL7 Claim Ladder.

## 3. Four scientific families and strongest attacks

| Family | Adversarial positive / negative distinction | Scientific decision |
|---|---|---|
| A. Fixed-rule SOP | Deterministic solver may succeed on unseen combinations; fixed observation-conditioned RETRY/ESCALATE policy is valid ASR candidate. But hard-coded answer bank and routine automation are not proof of generalizable system intelligence | **CONDITIONAL IN-SCOPE**; distinguish descriptive evidence from explanatory core claims |
| B. Jev-like bounded learned decision + B3 SOP | Learner choice may add value, but option generator/human SOP author may already have solved the task; typed answer may omit correct option | **IN-SCOPE** only for defined system question; learned selection and option provenance separately evaluated |
| C. Weak LLM + strong non-LLM body + manual | No-LLM rule + same body can match LLM, SOP may encode test answer, or treatment varies knowledge/calls/cost | **IN-SCOPE**; package noninferiority ≠ unique causal body effect, model necessity ≠ system success |
| D. Feedback / self-improvement | Repeated retries and performance gains do not imply optimizer self-modification. Time-stamped score history does not alone identify SDR; changed evaluator may fake gain | **IN-SCOPE / RSI EXACT CONTRACT OPEN**; distinguish policy, persistent revision and meta-improvement |

Across these groups, 28 **hypothetical** boundary fixtures were reviewed: 2 outside a core SIS claim, 1 supporting asset, 7 bounded descriptive, 17 explanatory candidates, 1 unresolved. A separate **22-item adversarial conceptual/expected-behavior registry** distinguishes different forms of false inclusion, false exclusion, leakage, route inflation, conflation of model vs system contribution, and forced routing. No actual Jev/LLM/SOP system was run.

## 4. Critical examples

- A no-LLM fixed SOP with controlled verifier contrast can be an **SCF** claim; a rule-based uncertainty-conditional policy with defined policy-value estimand can be **ASR**. Learning is not a necessary gate.
- A Jev-only classifier leaderboard is **component-level supporting evidence**; Jev + SOP with measured system-value contrast can be a primary in-scope claim. Generative text generation is not required.
- Weak-LLM/strong-system vs strong-LLM/minimal-system can compare two *system packages*; it does not isolate the body mechanism when model, knowledge and resources change simultaneously. Zero/negative LLM contribution remains a valid result.
- Existing optimizer fine-tuning a model is not automatically strong RSI. A changed improvement procedure with no primary estimand warrants **`ROUTING_UNRESOLVED`** (to be specified in SAR-04).
- Only renaming identical scientific roles `Jev` as `AgentGPT`, or `verifier` as `multi-agent`, must not change classification. A *real* change from static effect to transition-dependent estimand may legitimately change SCF to SDR.

## 5. Minimum revision suggestions (do not implement)

1. Add a compact **Scope Gate** in Scientific Identity, *not* a Core primitive.
2. Keep **ScientificScope / ScientificContribution / ClaimValidity** explicitly separate.
3. Separate precompiled procedural/cognitive contributions, option generation, learned selection, authorization, tool execution and evaluator from one another; use optional role annotation if needed.
4. Keep the higher-level System Intelligence construct multidimensional; report prior SOP design knowledge and cost, task-family splits and generalization strata.
5. Forward precise RSI self-modification/lineage semantics to SAR-04 without creating a new Program now.

## 6. Strongest objections still open

**O1 (overinclusive):** Nearly any program can be represented as component/state/control; unless system-level *intelligence-related* target and nontrivial scientific question are made genuinely discriminating, SIS could absorb all computer science.

**O2 (underinclusive):** Requiring causal identification merely to enter SIS would exclude useful CL0/CL1 descriptive science, deterministic decision systems, and formal guarantees. Restrict strong *claims*, not legitimate scientific objects.

Both require SAR-01-C wording, then SAR-01-D science-owner decision. Do not invent a learned-model or component-count gate as a shortcut.

## 7. Validation and gates — strict evidence language

- **Conceptual boundary fixtures:** 28 / 28 **authored and reviewed**.
- **Adversarial expectations:** 22 / 22 **specified**, not validated against a live system.
- **Executable metadata and fixture-rule consistency checks:** 70 / 70 **PASS**. These checks use the same researcher-authored rule/fixture scheme and therefore **do not establish semantic, empirical, or causal validity**.
- **External-model/real-SOP benchmark tests:** **0 run**. **Effect estimates: 0.**
- **Gate-S scientific-semantic review:** **CONDITIONAL**; **Gate-O real runtime:** **NOT_EXECUTED**; **Gate-E empirical science:** **NOT_EXECUTED**.
- **SAR-01:** still `OPEN`; R5.1 Master not modified or adopted.

The full local evidence package from this turn contains the detailed Chinese report, all 28 fixture rows, 22 kill-test expectations, decisions, script, exact checks and SHA-256 manifest; this GitHub file records the review result and core adjudication logic, rather than falsely claiming those local files were uploaded.

## 8. Exact R5.1 anchors and external scientific context

- §1–3, candidate reading-copy lines 160–299: scientific identity, one-or-more component composite system, no automatic complex-system superiority.
- §14 and §20, lines 804–1016: context-dependent capability frontier and trajectory.
- §22–33, lines 1051–1417: SCF, SDR, ASR scientific routes.
- §40–50, lines 4087–5169: scientific question → estimand → conformance → routing; descriptive, unresolved and nonconformant paths.
- §65–68 and §74–82, lines 5662–5789, 6474–6617: evidence separation and claim maturity.
- Proposed Part VII-A, lines 1684–4082: localization and externalized capability candidates **NOT NORMATIVE**.
- Chollet, *On the Measure of Intelligence* (2019): https://arxiv.org/abs/1911.01547 — task-specific skill, priors and skill acquisition.
- Rubenstein et al., *Causal Consistency of Structural Equation Models* (UAI 2017): https://proceedings.mlr.press/r15/rubenstein-17a.html — abstraction and intervention mapping.

**Next:** SAR-01-C | concise Scientific Identity and First-Principles Mother Problem v0.8 candidate, with explicit scope rules and at most two remaining irreducible objections. **Do not close SAR-01 until SAR-01-D science-owner review.**
