# SIS-R5.1-REV-P0｜Authority Baseline, Exact Delta & Review Contract Freeze

> **REVIEW-ONLY / NON-NORMATIVE.** 2026-10-27 检查快照。此记录不批准 R5 替换、不采纳 R5.1、不修改 `main` 的规范正文，也不等同于 Scientific Non-Regression PASS。

## P0 Verifiable Authority Ledger

| Evidence object | SHA / size / status |
|---|---|
| GitHub `main` authoritative path | `specs/System_Intelligence_Science_v0.3.1.md`; Git blob `2c99d87f2c3d5458dca254b1ece3eb9bb7097ce4`; 117227 bytes; pre-R5 R0–R4 |
| Selected Library R5 | SHA-256 `f7dff71e2c5973f75a7f83c77f189b6d605c5f1ea50f738506e0d115a857c44d`; blob `9a8365ad944402d1f37668b222e7c2c9f2d3250d`; 149590 bytes / 12415 lines; proposed via PR #2, **not merged** |
| Non-selected extended R5 | SHA-256 `3e1da79a14111d2ead7bc49d47665bc05c1879969b9233fdaa060c2f95436a82`; blob `419aa8c841206a63e0bf6d7f067fa3331880d5a3`; 181565 bytes / 14817 lines; **PROPOSED NORMATIVE PATCH** |
| R5.1 reading copy | SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`; 182173 bytes / 14825 lines; 8-line explanation + byte-identical extended R5 |

Source governance: [SIS-Main PR #2](https://github.com/gitzhangcd/SIS-Main/pull/2) and its `governance/releases/SIS_v0.3.1_R5_Authority_Alignment_Review_2026-10-26.md`.

## Exact Delta Proof

- A Python byte-and-line audit reconstructed the selected 149590-byte Library R5 by removing the single Part VII-A insertion from the uploaded 181565-byte R5 extended file. Reconstructed SHA-256 and Git blob SHA-1 match PR #2's selected baseline **exactly**.
- Full line comparison with `SequenceMatcher(autojunk=False)` yielded **three and only three** operations: equal R5 lines 1–1671; insert extended lines 1672–4073; equal R5 lines 1672–12415.
- Therefore **2402 inserted lines, 0 deleted R5 lines, 0 replaced R5 lines**. The added part contains 32 candidate clauses (`39A–39AF`) and 10 proposed kill tests (`CL-KT1–CL-KT10`).
- The text equality does **not** prove semantic non-regression. `ScientificCoreDelta=0`, `ProgramArchitectureDelta=0`, and `CoreExperimentSchemaDelta=0` remain candidate claims requiring independent validation.
- Local reproducibility evidence includes the exact unified patch, 32-clause CSV, blocker registry, frozen review contract, and machine-readable manifest. The larger local evidence package has not been uploaded in this PR.

## Review Coverage Contract (P0-FROZEN FOR REVIEW ONLY)

1. **Scope:** Reuse 12415 R5 baseline lines as a lineage-verified source; perform intensive scientific review on the 2402 inserted lines, cross-layer non-regression, and authority resolution. The 8-line reading-copy header is not normative.
2. **Clause coverage:** Every one of the 32 `39A–39AF` candidate clauses requires an explicit `KEEP | MODIFY | MERGE | REMOVE | DEFER` disposition, owner, scientific necessity, existing SIS owner, construct, measurability, estimand, falsification, domain impact and citation.
3. **Kill tests:** `CL-KT1–10` must become executed positive/negative fixtures with expected and actual outcomes, code/runner version, evaluator independence and failure provenance. Written test statements are not test results.
4. **Program non-regression:** Preserve SCF / SDR / ASR; preserve CSCI and X2 cross-cutting status; use estimand-first routing, not frameworks/labels. Test Core primitives, experiment contract, CL0–CL7 and evidence-role separation.
5. **Identification controls:** Compare internalized capability, runtime information, scaffold/mechanism, resource use, human roles and evaluator reference distinctly. Never elevate performance differences to causal claims without identification.
6. **Domain pins:** SIS-MED R6 P0.4 and Nutrition Foundation v0.1 still cite SIS R5. Proposed localization must not silently become a mandatory domain schema or evidence/reference input.
7. **RSI stress test:** Check whether recursive self-improvement can be expressed through the existing science programs; lack of an RSI section is a coverage concern, not proof of new-primitive necessity.
8. **Human authority:** AI can audit and prepare evidence, but the SIS Core Owner retains normative approval. CI PASS or document similarity does not imply scientific validation.

## Blockers and Gates

| Gate / issue | Result |
|---|---|
| Source hashes and candidate provenance | **PASS** |
| Exact text Delta | **PASS** |
| P0 review contract definition | **PASS / REVIEW FROZEN** |
| R5 canonical baseline release (PR #2) | **HOLD**; Core Owner approval and non-regression outstanding |
| R5.1 candidate Part VII-A normative admission | **NOT ADOPTED** |
| Patch internal proposed/frozen language conflict | **HOLD**; external proposal status takes precedence |
| Capability/causal semantics review (32/32) | **NOT EXECUTED — P1** |
| Kill Tests / core/domain non-regression | **NOT EXECUTED — P2/P3** |
| Immutable normative release manifest/tag | **NOT CREATED** |
| Downstream normative adoption | **NOT AUTHORIZED** |

## Forward Actions

**P1:** review 39A–39AF with first-principles science, minimality, existing-semantic overlap, RSI expressivity and explicit dispositions.  
**P2:** run CL-KT1–10, program-routing, information/resource-control and SIS-MED/NDSF non-regression fixtures.  
**P3:** reconcile affected engineering/reference contracts and preserve historical records.  
**P4:** only after approved R5 base, science-owner adoption and pass evidence may a new Master be regenerated, tagged and downstream adopted.

**P0 final:** `SOURCE_INTEGRITY=PASS; EXACT_DELTA=PASS; REVIEW_CONTRACT=FROZEN_FOR_REVIEW; R5_NORMATIVE=HOLD; R5.1_NORMATIVE=NOT_ADOPTED`.
