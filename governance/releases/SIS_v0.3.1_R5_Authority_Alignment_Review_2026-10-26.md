# SIS-GOV-P0-A1 — R5 Authority Baseline Alignment (DRAFT)

> **DRAFT NOT ADOPTED. This PR is an auditable release candidate, not a normative release.**

## Main and archived predecessor

- Repository: `gitzhangcd/SIS-Main`
- Base commit: `096593987a928517d7fce66a3907019c767e36b9`
- Previous normative path: `specs/System_Intelligence_Science_v0.3.1.md`
- Previous blob SHA-1: `2c99d87f2c3d5458dca254b1ece3eb9bb7097ce4` (117227 bytes; R0-R4).
- Archived unchanged: `specs/archive/System_Intelligence_Science_v0.3.1_R0-R4_Pre_R5.md` (same Git blob SHA).

## Two source-distinct R5 files and decision

**Selected baseline for this draft PR:** the 149590-byte Library `System-Intelligence-Science-v0.3.1-R5-Regenerated-Master-Specification.md`. Previous user decision on 2026-10-21 selected this as substitute R5 baseline; treat that selection as a recorded project choice, **not by itself as an independently signed release approval**.

- Selected R5 SHA-256: `f7dff71e2c5973f75a7f83c77f189b6d605c5f1ea50f738506e0d115a857c44d`
- Selected R5 Git blob SHA-1: `9a8365ad944402d1f37668b222e7c2c9f2d3250d`
- Selected R5 size: 149590 bytes, 12415 text lines.

**Non-selected extended R5 snapshot:** user-supplied 181565-byte `SIS-v0.3.1-R5-Regenerated-Master-Specification (1).md`.

- Extended R5 SHA-256: `3e1da79a14111d2ead7bc49d47665bc05c1879969b9233fdaa060c2f95436a82`
- Extended R5 Git blob SHA-1: `419aa8c841206a63e0bf6d7f067fa3331880d5a3`
- Difference: it inserts a contiguous Part VII-A block of approximately 2402 lines labeled **PROPOSED NORMATIVE PATCH** for Capability Localization; the rest of the original Library R5 lines are identical (sequence comparison; this is not formal semantic equivalence).
- This insert is **not adopted** by replacement of the normative Master. It remains a separate proposed overlay requiring science-owner review.
- The R5.1 candidate composite was constructed using the extended 181565-byte snapshot; its upstream prefix therefore requires explicit reconciliation/rebase before future normative consideration.

## Non-regression and approval blockers

1. SIS Core Owner / scientific governance must ratify the Library R5 substitution for the canonical GitHub normative path and resolve any historical contrary approval evidence.
2. Confirm R5 ScientificCoreDelta=0, ProgramArchitectureDelta=0, CoreExperimentSchemaDelta=0 through applicable scientific review; a text statement inside R5 is not independent execution proof.
3. Decide Capability Localization patch status explicitly; do not silently promote a proposal to FROZEN.
4. Confirm exact source Git blobs and preservation of the pre-R5 archive; check downstream SIS-MED R6 and NDSF source pins after approval.
5. Keep R5.1 Candidate, RSI experiment data, literature artifacts and schema changes **outside** this PR.
6. Confirm production and CI results separately; do not infer science evidence from documentation checks.

## Release / rollout after approval

- Approve and merge through standard code review only after blockers resolved.
- Record approved commit and immutable release tag in an ApprovedNormativeManifest.
- Propagate new source refs to SIS-MED and Nutrition Foundation by separate domain PRs.
- If not approved: close draft PR without merge. `main` remains unchanged.

**Current Gate:** `HOLD_PENDING_CORE_OWNER_APPROVAL_AND_NON_REGRESSION`.
