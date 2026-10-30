# SAR-03-B｜Independent Blind Negative Routing Protocol v1.0

> **PROTOCOL AND TASKS PREPARED — INDEPENDENT BLIND REVIEW NOT EXECUTED.**  
> This is research planning material, not approved R5.1 runtime contract, scientific Gold, or independent coder agreement.

## Packages and blinding

**48 unlabeled tasks** (24 paired/triple Estimand items across 8 contexts; 12 M1/M2 identity and intervention cases; 12 negative/abstention cases) were prepared as:
- `Blind_Worker_A_Tasks_v1.0.csv` and `Blind_Worker_B_Tasks_v1.0.csv`, **48 rows each**, different randomized order, same anonymized join IDs and **blank answers**.
- `Blind_Protocol_v1.0.md` and worker-only ZIP `SAR-03-B_Blind_Reviewer_Packet_v1.0.zip`, distributed **without** candidate keys or source case mappings.
- Controller-only ZIP `SIS-R5.1-SAR03-B_Review_Package_v1.0.zip` contains the **author-generated candidate key** and raw case mapping, adjudication template, reproducible synthetic fixture script and independent-review scoring script.

**IMPORTANT:** Neither GitHub review branch nor this protocol publishes the reviewer-facing answer key. Do not distribute the controller ZIP to blind annotators before their answers are locked. The candidate key is not independently verified Gold.

## Worker instructions (non-normative)

1. Assign two genuinely independent coders; isolate answers, source claim IDs, scenario triad pairings, labels and hypotheses.
2. Provide only the worker-only packet and the authoritative R5.1 sections §§22–33, 34–38, 40–50, 165–170, with access to **routing definitions but not expected answers**.
3. Each coder must return: `routing_status` in the **four canonical values**; `primary_program` one of SCF/SDR/ASR if ROUTED, else NONE; `crossview_comparability` one review-only status for M1/M2 comparisons, otherwise NOT_APPLICABLE; concise estimand rationale and 0–1 confidence.
4. An independent third adjudicator reviews disagreements **without candidate key first** and records whether the root cause is under-specified estimand, model-name anchoring, M1/M2 identity/authority ambiguity, absence of counterfactual evidence, or genuine potential program non-reducibility.
5. Only after coders and adjudicator lock responses may the controller compare with researcher-authored candidate key and score reproducibility.

## What to score once real responses exist

- 4-way routing status raw agreement, four-way confusion matrix, Cohen κ with class counts/prevalence, and status-stratified disagreement patterns.
- Primary Program agreement **only on claims both coders route**, with pairwise ASR/SDR vs SCF disagreement counts.
- M1/M2 comparability agreement separately; `NOT_EQUIVALENT` is *not* a fifth canonical Program route.
- Qualitative high-severity audit: unsupported same-estimand across M1/M2, postdecision information leakage, model-/framework-name forced route, wrong `NO_CHANGE` handling, claim-strength overstatement.
- Prospective provisional reviewer targets: four-status raw agreement ≥0.85 and Cohen κ ≥0.70 (sensitivity analysis mandatory). **These are proposal thresholds, not R5.1 norms, not science-owner frozen.**
- If systematically poor independent agreement persists despite adequate Gold clarification, R5.1 §166 **RA2** allows reopening Program Architecture. No such test can be performed with solely reviewer-authored rules.

## Current evidence state

`WorkerA=NOT_EXECUTED`  
`WorkerB=NOT_EXECUTED`  
`Adjudicator=NOT_EXECUTED`  
`IndependentAgreement=UNAVAILABLE`  
`CandidateKey=AUTHOR_AUTHORED_NOT_GOLD`  
`BlankScoreCheck=REJECTED_INCOMPLETE_INPUT_AS_EXPECTED`  
`RealSystemExperiment=0`  
`G-O=NOT_EXECUTED`  
`G-E=NOT_EXECUTED`

Worker-only packet SHA-256: `784f8036b49908460f593f693897129fb7c03f8b40d7412531d374b0ce76bee8`, 12,569 bytes. Full controller local ZIP SHA-256: `326cdd20afe869df5f62ee000f5ad43e4b849bb4585d497eb7510ae87279db27`, 49,846 bytes. These file bytes exist in the conversation's active container; neither ZIP was pushed verbatim into this GitHub review branch.

**SAR-03-B remains a completed conceptual/formal work unit with the independent blind gate OPEN. SAR-03 remains IN_REVIEW/OPEN.**