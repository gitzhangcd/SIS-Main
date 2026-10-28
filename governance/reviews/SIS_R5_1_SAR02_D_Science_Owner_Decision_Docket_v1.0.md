# SAR-02-D｜Minimal Ontology Science Owner Decision Docket v1.0

> **DECISION READY / OWNER CHOICE PENDING / SAR-02 IN_REVIEW OPEN / NON-NORMATIVE.**  
> No user choice has been made in this SAR-02-D round. Do not treat entering the decision work unit as approval of a default. **Do not edit or freeze the normative Master.**

## A. Source authority and precise decision object

Source: supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md` (SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`), especially §5 (Context); §6 `S_t=(C,R_t,X_t,O_t,π_t)`; §8 `A_t=Γ(C,R_t)`; §9 `X_t≠O_t`; §10 Control; §19 Dynamics; §20 Trajectory; §32 NO_CHANGE; §33 EvidenceTime; and existing `ScientificExperimentContract.context.time_horizon`.

The science owner already conditionally accepted SAR-01 Scientific Identity v0.8 **as a review-only baseline**, preserving O1/O2 and NR-13/14. SAR-02-A found 16 role definitions and five synthetic expressivity examples; SAR-02-B executed **24/24 finite toy-model checks**, including 512 three-step known-potential-universe traces and 16,739 finite *closed-slot* mappings. SAR-02-C developed six candidate semantic clarifications, 12 M1/M2 comparison dimensions and 22 design-level non-regression reviews. Its **new 25/25 source/toy-model checks** do not establish full ontology adequacy or real-world model success.

**Decision question:** May the existing five system-role tuple + external Dynamics be retained as the audit ontology, with G-01/G-03–G-06 minimal scientific interpretations and a conditional M1/M2 *representation review* policy for G-02, pending separate formal and normative authorization?

## B. Recommended option A — CONDITIONAL_DUAL_VIEW_FOR_REVIEW_ONLY

- **G-01:** Preserve distinct State and Observation epistemic roles/provenance; do not require their numeric payloads to differ under identity/full observation. §9 source's boxed `X_t≠O_t` is not silently rewritten.
- **G-03/G-04:** Distinguish permission/organization `R_t`, proposed selection `π(H_t)`, executed authorized action and transition `F`; distinguish context knowledge availability, runtime observations and legal decision-time history.
- **G-05/G-06:** Explicit evaluation horizon T using existing `context.time_horizon`; legal singleton, `R=∅`, fixed `π`, NO_CHANGE and identity dynamics.
- **G-02 conditional regime:** **M1** as audit representation when component identities are in a declared known/bounded `C*` and active/versioned members are reconstructible, including effective architecture `Γ(C_t^active,R_t^eff)`. **M2** (`C_t`) kept as a *separate proposed review representation* when open-world created/deleted identity is the scientific target. Neither is adopted as source §6/§8 notation merely by this decision.
- Both regimes need sufficient *identity, creator/source, generation, version, permissions and ordered lifecycle events* when such facts are relevant to the target claim. Equal output, current membership snapshot and equal final task score are insufficient evidence of identity/intervention equivalence.

**Condition for comparing claims across regimes (review criterion, not new Core schema):** disclose `ComponentBoundary`, `OntologyRegime`, `IdentityAndLineageMap`, `EffectiveRelations`, `ActionAuthority`, `InformationTimeCutoff`, `InterventionSet`, `TaskRiskResourceHorizon`, and whether the relevant scientific **estimand** is preserved. If no defensible mapping exists, report `REGIME_COMPARABILITY_UNRESOLVED` or bound the claim; do not invent equivalence or route by model label. These are review disclosures, **not** approved new physical fields.

### Strongest skeptical attack on A

A weak generative LLM writes code **P** executed by a fixed general-purpose interpreter **I**. In **M1**, `C*={I,...}` and P is internal state/program data. In **M2**, P may be modeled as a new capability-bearing component with its own identity, privileges and failure exposure. Both can yield the *same outputs*, while causal attribution ("Did the system create a new component?", "Did it acquire independent capability?", "Does disabling P or I identify the effect?"), CSCI localization and lineage can differ.

Consequently `BehavioralEquivalence ≠ ScientificIdentity/InterventionEquivalence`. The **same task** may receive non-equivalent ontology representations and therefore different target estimands. A two-regime policy with no explicit mapping would permit contradictory science even if both representations are internally coherent.

**Strong skeptic's alternative:** Adopt *one* canonical scientific membership identity convention now; encode all implementation differences behind it. The counterargument to this alternative is that adopting either a closed fixed set or universal dynamic member interpretation **now** would claim a level of sufficiency and formally approved meaning that SAR-02-B/C has not established.

**Response within A:** representation neutrality must not mean attribution neutrality. Use component-identity/authority/events/intervention mapping **only when justified**; record unidentifiable or representation-dependent claims explicitly. Do not assert M1 and M2 are generally equivalent.

## C. Four Science Owner options

| Choice | Review-only consequence *after explicit approval* | Scientific cost and unresolved gate |
|---|---|---|
| **A · CONDITIONAL_DUAL_VIEW_FOR_REVIEW_ONLY (recommended)** | Keep all current Core object roles; conditionally accept G-01/G-03–G-06 as audit interpretations. M1 for known bounded membership; M2 for open-ID as separate **unadopted candidate**. Require declared regime and claim-level comparability/lineage audit. Mark `SAR-02 REVIEW_ACCEPTED_WITH_OPEN_GATES` and permit SAR-03 readiness. | Strongest objection: two representations can cause claim-dependent component identity and incomparable causal estimands. Normative core delta remains OPEN. |
| **B · M1_ONLY_DEFER_M2** | Maintain only fixed potential-universe/state representation for the review; open-ID systems unresolved. | May exclude or misattribute dynamic capabilities if finite closed universe is not defensible. |
| **C · M2_PRIMARY_PROPOSAL** | Adopt `C_t` as preferred *revision candidate*, not actual normative text; start expanded §6/§8/§19/§20/Schema semantic-impact analysis. | More extensive upstream scientific semantic delta; no automatic lineage. |
| **D · DEFER_OWNER_DECISION** | Keep SAR-02 IN_REVIEW; first perform stronger independent identity/intervention-preserving formal comparisons and blind review. | More evidence before a review baseline, delays SAR-03 by review-plan dependency. |

A choice to enter SAR-02-D **does not** imply selection of A.

## D. Six clauses and their approval boundaries

| Issue | Approval requested for scientific *review interpretation* | What is not automatically approved |
|---|---|---|
| G-01 | StateRole≠ObservationRole; payload equality allowed under full observation | A normative rewrite of §9's frozen formula |
| G-02 | Conditional M1 known-universe / M2 open-identity review candidate | Formal adoption of `C_t`, global M1↔M2 equivalence, dynamic-component ontology freeze |
| G-03 | Authority/Policy/Execution separated | New permission Primitive or run-log Schema |
| G-04 | Context Information/Observation/Legal history with provenance and cutoff | Unchecked post-hoc or hidden evaluator input |
| G-05 | Evaluation horizon T declared using existing contract | New Core time Primitive |
| G-06 | Singleton/empty R/no-op/identity F valid instantiations | Automatic SIS mechanism discovery from routine automation |

## E. Required evidence and non-regression safeguards

- `NR-13`: scientific identity v0.8 owner **review** accepted only. `ScientificCoreDelta=0` is **not certified**.
- `G-01`: source §9 semantic amendment remains open until later normative owner approval.
- `G-02`: M2 affects §6/§8 and potentially §19/§20; even M1's effective-architecture convention needs scientific scrutiny. Formal non-regression (G-O) not run.
- R5.1's five measured Properties, five tuple roles plus external Dynamics, derived architecture, SCF/SDR/ASR, CSCI/X2, CL0–CL7, independent Reference/Evaluator and estimand-first routing remain **design preserved**, not formally conformance-PASS.
- `O1/O2` of SAR-01 remain OPEN; `NR-14` strong RSI and F0–F3 meta-improver revisions remain for SAR-04.
- `G-S=CONDITIONAL`; `G-O=NOT_EXECUTED`; `G-E=NOT_EXECUTED`. No Jev/LLM/SOP system efficacy, causal compensation or recursive improvement laws are proven.
- R5.1 Part VII-A stays a `PROPOSED NORMATIVE PATCH`.

## F. Decision receipt placeholder (no decision recorded)

`decision_id: SAR-02-D-DEC-001`  
`decision_owner: SCIENCE_OWNER_USER`  
`owner_choice: PENDING`  
`review_status: SAR-02_IN_REVIEW_OPEN`  
`normative_master: UNCHANGED`  
`pr: #4 DRAFT OPEN`  
`next_action: AWAIT_EXPLICIT_A_B_C_D_CHOICE`

**After a choice only:** create `Science_Owner_Decision_Receipt_v1.0.md`, update decision register/progress, preserve open gates, and prepare SAR-03 if decision allows. Never merge or change the authoritative Master without a separate explicit approval.
