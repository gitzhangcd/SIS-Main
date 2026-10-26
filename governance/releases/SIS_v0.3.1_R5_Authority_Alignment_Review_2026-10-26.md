# SIS-GOV-P0-A1 — R5 Authority Baseline Alignment (DRAFT)

> **This branch and PR are a review proposal, not an adopted release. Do not merge until SIS Core Owner / Scientific Governance approves.**

## Base snapshot

- Repository: `gitzhangcd/SIS-Main`
- Base main commit when branch created: `096593987a928517d7fce66a3907019c767e36b9`
- Previous normative path: `specs/System_Intelligence_Science_v0.3.1.md`
- Previous Git blob SHA-1: `2c99d87f2c3d5458dca254b1ece3eb9bb7097ce4`
- Exact previous content archived as `specs/archive/System_Intelligence_Science_v0.3.1_R0-R4_Pre_R5.md`.

## Candidate R5 source

- Source: user-provided `SIS-v0.3.1-R5-Regenerated-Master-Specification (1).md`
- Bytes: `181565`
- Source SHA-256: `3e1da79a14111d2ead7bc49d47665bc05c1879969b9233fdaa060c2f95436a82`
- Git blob SHA-1 expected: `419aa8c841206a63e0bf6d7f067fa3331880d5a3`
- Update mode: **verbatim complete Master**, no edits, no appended R5.1 candidate.

## Known review blockers

1. **Approval evidence:** local R5 text self-describes its R5 freeze and non-regression decisions, but an independently verifiable historical adoption signature, tag or approved PR was not located in the audited SIS-Main branch. A Core Owner decision is still required.
2. **Capability Localization semantic status:** Part VII-A labels itself `PROPOSED NORMATIVE PATCH` but later uses freeze-like wording. Resolve normative precedence expressly without retroactively rewriting the source snapshot.
3. **Domain adoption:** SIS-MED R6 and Nutrition Foundation cite SIS R5 but need immutable upstream tag/commit pin after release; do not update other projects in this PR.
4. **Regression:** historical claims, literature registry, program routing and exact engineering schemas have not been independently re-executed in this PR. Static identical-source verification is not sufficient for adoption.
5. **R5.1 exclusion:** R5.1 RSI/scientific-positioning revision stays `CANDIDATE / NOT_ADOPTED`; the RSI pilot and expert utility evidence remain separate.

## Required review checks before merge

- [ ] SIS Core Owner confirms normative R5 adoption and accepts exact upstream file fingerprint.
- [ ] Reviewers compare R0–R4 vs R5 at clause level and check Core/Program/Experiment non-regression.
- [ ] Confirm proposed-patch status interpretation (without silent semantic upgrades).
- [ ] Confirm old file archive SHA equals original Git blob.
- [ ] Confirm new R5 Git blob equals the supplied source.
- [ ] Decide release tag, manifest authority status, rollback path, downstream notifications.
- [ ] Applicable CI / domain conformance passes or each unresolved item is explicitly handled.

## Rollback

Revert this PR if merged or restore normative file from archived exact pre-R5 blob; never delete original revision, annotation or claim evidence. Versioned downstream adoption must be a separate PR.

**Current Gate: HOLD_PENDING_SIS_CORE_OWNER_APPROVAL_AND_NON_REGRESSION.**
