# SAR-05-A｜Capability Localization, Cognitive Floor & Weak-Brain/Strong-Body Compensation — Source-Grounded Scientific Audit v1.0

> **2026-10-29 · REVIEW-ONLY SCIENTIFIC AUDIT / NOT NORMATIVE.**
> `SAR-05-A=SOURCE_GROUNDED_CONCEPTUAL_AND_FINITE_TOY_AUDIT_COMPLETE_WITH_OPEN_GATES`; `SAR-05=IN_REVIEW/OPEN`.  
> **No real agent/LLM/SOP/human causal trial, no cognitive-floor identification, no causal compensation estimate, no independent Gold. `RA2=UNTESTED`; `G-O/G-E=NOT_EXECUTED`; normative Master unchanged and not frozen.**

## 0. Exact scientific source and authority boundary

Original supplied **`SIS-v0.3.1-R5.1-Candidate-Full-Master.md`**, 14,825 physical lines, SHA-256 **`92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`**; **59 exact section/heading/line anchors directly checked**.

**Existing R5.1 support:** §5 L536–566 establishes `Capability(S|Ω)`, conditional on Task, Environment, Information, Budget, Constraints and Risk. §§11–13 distinguish Mechanism, Process, Property. §§22–24 define SCF intervention and resource/information/manipulation evidence. §§34–36 require a *measured ComponentCapability construct*, not ModelID, to support CSCI interaction; §§37–38 separate replication, performance transfer, causal transport and mechanism invariance. §84's single ScientificExperimentContract includes component identity, resource_capacity and realized_resources, causal roles, intervention, evidence, design, boundary, identification, estimand, evaluator/lineage. §§165–170 RA1–RA6 reopening rights are retained.

**Important proposal boundary:** R5.1 **Part VII-A** §39A–§39AF already provides extensive **candidate** localization/internalized/externalized capability, training-v-runtime, human role, mechanism interaction, negative tests and EI-SMCT discussion. It explicitly states `Scientific status: PROPOSED NORMATIVE PATCH` at L1691. Later internal “正式冻结” statements and §39AF proposed freeze **are NOT separate owner-approved normative adoption**. The exact phrase **`Cognitive Floor` / `认知下限` does not occur in the original candidate**: a floor construct below is **new, review-only, not an adopted SIS law**. Neither earlier SAR-01–04 decision authorizes Master changes.

## 1. Minimum different scientific roles

**A — Localization:** `L(r|F,S,t)` is *where* the capability-bearing resource is positioned relative to focal component `F`, composite system boundary `S`, and evaluation time `t`. Source proposed zones: intra-component, extra-component/intra-system, extra-system before legal acquisition. A tool or human may move causal role across boundaries; simply naming the tool or system does not establish an effect.

**B — Component-level capability construct:** a measured, task-relevant **vector or set of abilities** `c(F|B0,Ω)` under declared minimal/baseline support B0. Model brand/ID and one accuracy score are proxies/identifiers, not the construct. Retrieval, patient record or system prompt entering runtime context does **not** become model-parameter learning (§39F/R, proposal). A strong specialist or calculator outside `F` may actually perform some of the cognitive/computational work.

**C — System-level capability and causal contribution:** `Capability(S|Ω)` is a conditional system property. The identified effect of a target mechanism/support `M` requires controlled treatment/control, measurement, information, budget, risk, manipulation and relevant mediator evidence (§24). **`Localization ≠ Magnitude ≠ CausalAttribution`** in Part VII-A §39A is adopted here **only as a review interpretation**.

**D — Human and evaluator separation:** a physician/analyst consulted in a real decision is a potential runtime resource under a declared boundary; an independent expert constructing Gold/reference is an **evaluator**, not a hidden system component. Avoid label/reference leakage (§39Q/V, proposal).

## 2. Minimal compensation study and three distinct estimands

**2×2 (review baseline):** measured weak/strong **component capability construct** × external mechanism ON/OFF at the same task distribution, information availability and resources. Define a *candidate controlled* effect

`Δ_M(c,i;Ω,R)=E[Y|do(M=1),c,i,Ω,R]−E[Y|do(M=0),c,i,Ω,R]`.

**Effect modification:** `Ψ_sub=Δ_M(c_weak,i;Ω,R)−Δ_M(c_strong,i;Ω,R)`. If positive in an identified, task-valid and resource-controlled comparison, the **support mechanism helped the weak component more in this boundary**; it is **not** general proof of replacement of model intelligence, nor that the focal model acquired cognitive ability.

**2×2×2 minimal disentanglement:** `measured component regime × mechanism/scaffold ON/OFF × runtime external information ON/OFF`. Separate **mechanism effect at fixed evidence**, **extra information effect**, and **whole package effect**; do not attribute a corpus revealed only to treatment to the verifier or organization. Tools (including non-LLM rules/strong specialist models) and **runtime human involvement** may require separate factors, permissions, workload and reference firewalls.

**Weak+support vs strong+simple comparison:** pre-specified equivalence/noninferiority margin, matched risk and resource budgets, task distribution and evaluator; even success is **conditional system performance** comparison, not weak-model cognition equivalence. Count actual compute/human cost and harms.

Candidate rival mechanisms: **SUBSTITUTION, COMPLEMENTARITY, SATURATION, THRESHOLD, NULL_INTERACTION, NEGATIVE_NET_EFFECT** — each possible and none guaranteed.

## 3. Cognitive Floor: a proposed context-/mechanism-/risk-specific partial-order frontier

No source-frozen single scalar “minimum cognition”. Candidate `A(M,Ω,τ,q)={c:Pr(Y≥τ|do(M),c,Ω)≥q}`; study minimal elements under defensible partial ordering of **component capability constructs** (extraction, verification, routing, calibration). Different task, time, evaluator, risk, available information or M changes this set. It may have **multiple incomparable minima**, be non-monotonic or remain unidentified.

A 3×3 bounded artificial capability grid has two incomparable minimal successful points **`(1,2)` and `(2,1)`** under its **author-chosen predicate**. It refutes a universal one-number assumption **within that toy**, not a cognitive-floor hypothesis about any deployed model. Define a distinct **tool-eligibility threshold** and do not equate it with universal cognitive floor. A deterministic no-LLM comparator is valid for eligible algorithmic tasks, but may be invalid for open-ended tasks requiring a missing capability; mark eligibility/positivity rather than always assigning “zero brain”.

## 4. What was actually executed — exact ceiling

The local `build_sar05a.py` read source and **nine historic scientific review ZIP archives** (CRC checked) and actually executed **171/171 bounded source/input/fixture/numeric assertions** (NOT real model experiments). It generated:
- **59/59** original R5.1 exact heading/line checks; **15** source/science-claim authority crosswalks distinguishing R5.1 source vs **proposed** Part VII-A;
- **48** researcher-authored synthetic scientific claims, 6 system families ×8 examples, including valid descriptive, unresolved, nonconformant and SCF/SDR/ASR claim-target status;
- **7** arithmetic toy outcome regimes × **8** factorial cells = **56** toy outcomes and **14** constructed interaction contrasts: substitution, complementarity, saturation, threshold, null, negative, information-only;
- **9** manually designed two-dimensional partial-order cognitive-floor toy points with 2 incomparable minima;
- **36** AUTHOR_AUTHORED `EXPECTED_ONLY` negative/kill hypotheses, **zero** real-system executions;
- **20** candidate prospective design safeguards, **34** design-level nonregression reviews **formal runner all NOT_EXECUTED**;
- **45** open gates = 31 carried from previous review +14 SAR-05-A-specific; **none closed**.

**Do not interpret 171 PASS as 171 independent scientific experiments**. Strong compensation effects = `NOT_ESTIMATED`, real component cognitive floor = `NOT_IDENTIFIED`, independent Gold = `NONE`, real LLM/SOP/tool/human factorial studies = **0**, `RA2=UNTESTED`, `G-O=NOT_EXECUTED`, `G-E=NOT_EXECUTED`.

## 5. Adversarial scientific issues and non-regression

**High risk S5-01:** "Cognitive Floor" not a source-frozen construct. **S5-02:** capability location not causal contribution. **S5-03:** package-score comparisons cannot identify compensation. **S5-04/05:** ModelID/one score and infeasible no-LLM controls cannot establish the cognitive floor. **S5-06:** hidden runtime expert/evaluator contamination. **S5-07/08:** external info + stronger specialist tool attribution. **S5-09:** CSCI interaction unmeasured. **S5-10:** ceiling/bad proxy masquerades as saturation. **S5-11:** human/computational cost and patient/science risk. **S5-12:** transportability not tested. All **OPEN or NOT_EXECUTED**.

Review-only conservation: keep exactly 3 Primary Programs and 4 canonical routing statuses, CSCI/X2 crosscutting; preserve 5 Core roles, §84 existing experiment contract, owner SAR-01..04 **review-only** decisions, unadopted M2 dynamic `C_t`, source Part VII-A **PROPOSED**, RA1–RA6 science reopen rights and independence of scientific reference. No new Core capability primitive, mandatory physical schema or Master patch. 34 design nonregression items do **not** establish `ScientificCoreDelta=0` under an actual normative implementation.

## 6. Next substeps, not executed yet

**SAR-05-B｜Capability Construct Validity, Cognitive Floor Partial-Order & Compensation Identifiability Kill Audit**: independent construct validity, zero/no-model eligibility, factorial treatment information and external specialists, ceiling sensitivity, sham tool and human runtime, matched causal evidence, negative tests. Then SAR-05-C synthesis and SAR-05-D independent Science Owner choice, not automatic approval.

**SAR-05 remains `IN_REVIEW/OPEN`; SAR-05-A conceptual+bounded review complete; B/C/D NOT_STARTED.** The full local reproducibility bundle contains the full scientific report and raw outputs; GitHub review branch holds this sourced review and structured indexes, not a byte-identical mirrored archive.
