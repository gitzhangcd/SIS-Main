# SAR-04-B｜Versioned Meta-Improver Prospective Causal Contract v0.1

> **SCIENTIFIC REVIEW / EXPERIMENT DESIGN CANDIDATE ONLY. NOT normative R5.1 / new schema field / demonstrated causal effect.**  
> `SAR-04=IN_REVIEW/OPEN`; `RA2=UNTESTED`, `G-O/G-E=NOT_EXECUTED`. Based on source R5.1 §§19–21, §24, §§25–33, §§40–44, §84, §§165–170, and SAR-04-A source-constrained *proposed* F0–F3 update loci.

## 1. Minimum scientific contrast and identities

- **Improvee `T_g`** is a frozen starting target system, with exact executable/configuration/starting-state identity, active components, effective graph, permissions and resources.
- **Improver `I_g`** is the *effective operator that proposes, selects, validates and authorizes/promotes future target modifications*, potentially comprising multiple modules and human authorization. Distinguish `I_g` from `T_g` and from the independent evaluator.
- **`I_(g+1)`** counts as *structural F3 candidate* only if a semantically relevant new updater version was actually installed and invoked with valid actor/authority/version/rollback receipts; a proposed/uninvoked patch does not suffice.
- **External evaluator `E*`**, sealed assessment opportunities `D_future`, upstream `D_dev/D_promote`, and evidence-time exposure ledger must be owned/protected outside the acting updater. No self-scored future outcome proof.
- **Primary experimental unit `j`** is the independent *future improvement opportunity*, not one sampled grading row on a task inside that opportunity.

Proposed claim estimand, conditional on task, information, risk and resources:

`theta_meta = E_{j~D_future}[U(Apply(I_(g+1),T_g,j),E*) - U(Apply(I_g,T_g,j),E*)]`.

`U` must be specified prospectively, accounting for future accepted/imperfect/rejected target updates, performance, compute/token/time/person cost, risk, no-change, failures and rollback.

**Crucial non-equivalence:** `T_(g+1)` with better endpoint score under unchanged `I_g` does **not** imply that the **improver** improved. New `I_(g+1)` structural installation does **not** imply `theta_meta>0`.

## 2. Protocol for a future *real* experiment — no such experiment executed

1. **Pre-register** clear estimand and falsifiers, legal selection/optimization dataset, all future opportunity sampling assumptions, risk and utility. Freeze exact `T_g`, both loaded I versions and external `E*` plus authority. Avoid "same name, different algorithm" or reverse errors.
2. **Separate** `D_dev`, `D_promote`, genuinely untouched future opportunities `D_future` and *opportunity-local* training vs external scoring. Freeze I versions *before* future evaluation and log all information exposure time. E* labels hidden.
3. **Randomize** future opportunities to installed I arms or pair two isolated cloned sandboxes on each opportunity; same `T_g` starting state, eligible tools, budget cap, task information, risks and evaluation process. Evaluate interference/carryover/positivity assumptions and stratification.
4. **Match and account for resources**: identical caps do not prove equal actual tokens/calls/time/energy. Record actual usage and net utility, identify cost/efficiency tradeoffs and avoid attributing pure extra search budget to I version.
5. **Independent frozen evaluator** scores future *target update outcomes*, not the operating agent's current self-report. ACL and checksum prevent I from modifying Gold/rubric. Third-party expert adjudication where scientific reference is multi-valued.
6. **Include all attempts** under ITT-like reporting: successful, failed, rejected, no-change, unauthorized, aborted or rolled-back patches and their real costs; report per-opportunity paired differences and clustered uncertainty. Do not treat repeated grading rows as independent randomized units.
7. **Negative/factorial contrasts**: prior fixed I, sham unchanged I, no-update, extra-retry/compute F0, human-made external SOP F1, target-model/policy F2, stronger pretrained model substitution, M1 known-pool activation vs M2 new-identity creation. Use source/creator rights as attribution criteria.
8. **Generalization and falsification**: independently sample heldout/OOD shifted future opportunities, report uncertainty/heterogeneity and harms; if real randomized/paired conditions cannot be established, downgrade causal claim to the appropriately supported descriptive association.

**Important limitations:** No universally normative alpha/CI threshold/sample size is established here; sample size and uncertainty must be pre-registered for the actual use case. No real experiment, independence verification, or estimate is contained in this contract.

## 3. Review-only minimum receipt fields (NOT required SIS Core schema)

`{focal_T_version_hash, pre/post_I_executable_hash, semantic_diff, creator, optimizer_owner, permission_authority, actually_installed, invoked, event_time, rollback_status, task_opportunity_id, opportunity_sampling, D_dev/D_promote/D_future_exposure, E*_hash_owner, allowed_information, resource_cap, actual_cost, risk, all_attempted_update_outcomes, U_definition, paired_design, estimand, M1M2_identity_map, intervention_correspondence}`.

These are **candidate research/provenance disclosures**, not owner-approved physical schema extensions. Source §84 retains one unified `ScientificExperimentContract`; Part VII-A `PROPOSED NORMATIVE PATCH` remains unadopted.

## 4. High-severity kill conditions / boundaries

**Abort or downgrade** strong F3 claim if: `I` version not effectively changed/installed; only target `T` changed; human external author misattributed as self-origin; E* modified or hidden future reference exposed; only evolve/test-tuned tasks improved; budget or permitted tools unequal; failed updates or rollback excluded; `do(Component)` unit mismatched across M1/M2; policy-only/no-change mislabeled learning; a single successful revision claimed as unbounded recursive intelligence.

**Evidence status:** `STRONG_F3_FUTURE_CAUSAL_EFFECT=NOT_ESTIMATED`; `RA2=UNTESTED`; `G-O=NOT_EXECUTED`; `G-E=NOT_EXECUTED`; `SAR-04-D_OWNER_DECISION=NOT_STARTED`; `normative_Master=UNCHANGED`.
