# SAR-01 — Scientific Identity & Model-Internal Learning Boundary (Review v0.2)

> **NON-NORMATIVE REVIEW NOTE — SAR-01 OPEN, NOT FROZEN.** This scientific analysis examines the current R5.1 candidate on its merits; it is not a historical version comparison, master modification, or formal adoption.

## Scientific direction under consideration

SIS is the cumulative science of **how task- and context-dependent capabilities and other system-level properties of capability-bearing intelligent systems form, persist, change, fail, recover and are regulated**, and which internal learning/representation, organization, information, state, feedback, control and dynamics mechanisms affect these properties. Single-component and multi-component realizations are both eligible. Training/runtime is an explicit temporal boundary. Membership is determined by scientific question and measured construct, **not** model label, component count or localization.

## Critical three-way distinction

1. **Scientific scope**: Does the research address an intelligent-system property, or an explanatory relation/trajectory/regulatory question with explicit system boundary and task/context?
2. **Scientific contribution**: Is the result only a performance observation, a useful descriptive foundation, or a testable explanatory construct/mechanism/boundary?
3. **Claim evidence strength**: What can the design and evidence actually identify? Preserve SIS CL0–CL7 and estimand-first SCF/SDR/ASR routing. Do not require identified causality merely to enter the scientific domain.

## Discriminating counterexamples and provisional dispositions

- Simple SFT 80%→85%: descriptive/component performance only; no system mechanism established by score. It may provide component capability evidence.
- Internally located attention/representation intervention with task-behavior causal interpretation: **eligible** SCF candidate; internal location alone cannot exclude it.
- Pruning/quantization with measured capability/latency/viability frontier and mechanism contrast: conditional SIS candidate; no automatic causal claim.
- Time-dependent forgetting/recovery under continual training: SDR candidate only with a trajectory estimand, not from timestamped scores alone.
- Feedback-dependent update choice: ASR candidate; fixed training schedules do not automatically identify a regulation policy.
- Meta-learning on new tasks: studying adaptation capacity can be SCF; does **not** by itself prove optimizer recursive self-modification.
- Optimizer self-modification tested on future held-out tasks: an RSI stress case across separate SCF/SDR/ASR estimands, with lineage, resource/information controls and an independent evaluator.
- Evaluator changes inflate score: scientific nonconformance rather than genuine improvement.
- A generic thermostat without a specified intelligent capability construct: not automatically SIS just because it has feedback control.

## Minimal change proposal (DO NOT IMPLEMENT YET)

- Reword Scientific Identity in a **phenomenon- and mechanism-first**, implementation-neutral way. Keep existing system tuple `S_t=(C,R_t,X_t,O_t,π_t)`, five core system properties, three Primary Programs, CSCI/X2 and the claim ladder.
- Add a compact **Scientific Scope & Boundary** interpretive rule: specify research unit/focal component, training vs runtime timescale, context/resources/information/risk, target property and testable explanatory relation (or explicitly descriptive scope). Do not turn it into a new Core primitive/mandatory schema.
- For alternate decompositions of the *same* question, variable mapping and intervention target, require a justification of scientific interpretive consistency. Different interventions and levels are not required to yield numerically equal causal estimates.
- Keep `ScientificScope`, `ScientificContribution`, and `ClaimMaturity` distinct; do not change R5.1 normative routing enums.
- Explicitly preserve the Part VII-A **PROPOSED** status; this review does not admit Capability Localization as a frozen clause.

## Independent academic checks

- [Levels of Analysis — MIT Open Encyclopedia of Cognitive Science](https://oecs.mit.edu/pub/ztivn7hx/release/1/) distinguishes scientific problem, algorithm and implementation.
- [Rubenstein et al., Causal Consistency of Structural Equation Models (UAI 2017)](https://proceedings.mlr.press/r15/rubenstein-17a.html): cross-level consistency is conditional on valid intervention mappings.
- [Geiger et al., Causal Abstractions of Neural Networks (NeurIPS 2021)](https://papers.nips.cc/paper/2021/hash/4f5c422f4d49a5a807eda27434231040-Abstract.html): meaningful causal explanation can concern a mechanism **inside** one model.
- [Finn et al., Model-Agnostic Meta-Learning (ICML 2017)](https://proceedings.mlr.press/v70/finn17a.html): learned adaptation capacity is not automatically autonomous recursive self-modification.

## Adversarial tests not yet empirically executed

- **Singleton inflation**: do not label any arbitrary fine-tune score improvement as identified system-mechanism science.
- **Internal exclusion**: do not exclude model-internal causal mechanism research merely for being intra-component.
- **Causal overgate**: do not exclude valid descriptive evidence because it does not identify causality.
- **Boundary relabeling**: scientific identity should not change solely from a cosmetic model/agent refactor when the scientific target is unchanged.

A more detailed 12-case reasoning registry and report were delivered locally in the conversation. **No full executable scientific/causal conformance claim is made.**

## Open scientific decision

Should a SIS **core explanatory** claim minimally require a testable relation between a system-level property and a mechanism/process/organization/state/control construct, while purely descriptive observations remain valid SIS foundational evidence but not equivalent to mechanism discoveries? This remains **SAR-01 OPEN** pending Core Owner discussion.
