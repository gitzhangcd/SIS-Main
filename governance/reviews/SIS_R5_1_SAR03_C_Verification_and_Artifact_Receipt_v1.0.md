# SAR-03-C｜Verification & Artifact Receipt v1.0

> **2026-10-29 · REVIEW-ONLY AUDIT · NOT INDEPENDENT GOLD OR CONFORMANCE PASS.**  
> `SAR-03-C=REVIEW_CANDIDATE_COMPLETE`; `SAR-03-D=DECISION_PENDING`; `SAR-03=IN_REVIEW_OPEN`; `G-O/G-E=NOT_EXECUTED`.

## Source and actual local inputs

- Supplied `SIS-v0.3.1-R5.1-Candidate-Full-Master.md`, **14,825 lines**, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`.
- SAR-03-A source-read 50-row `SAR-03-A_Claim_Level_Routing_Fixtures_v1.0.csv`, 26 conditional expected routed (SCF13/SDR6/ASR7), 24 not routed (9 descriptive, 6 unresolved, 9 nonconformant).
- SAR-03-B source-read 48-row `Controller_Candidate_Key_v1.0.csv`, 24 triad + 12 cross-view + 12 negative, with 29 conditional routed, 5 descriptive, 6 unresolved, 8 nonconformant; candidate key is **author-authored and NOT Gold**.
- Worker A and B CSV both contain the same 48 anonymized tasks in different order and have five empty response fields per task. The separately verified Worker-only ZIP contains **only** protocol + two blank task files. No independent coder responses or adjudication.
- Inherited SAR-03-B finite-model index has 12 `PASS` labels for **bounded synthetic** counterexamples, not real-system evidence. SAR-03-C did not claim it independently re-executed the prior 512 known-universe trajectories.

## Executed SAR-03-C script — reproducible but not scientifically independent

The local script `SIS-R5.1-SAR03-C/build_sar03c.py` **executed 58/58 internal structural, source-anchor, linkage and blinding checks** without failure:
- SHA and exact line count of R5.1 source, plus **30 direct line/section anchor checks** against the supplied source;
- actual A=50, B=48, fixed expected-count/ID/label distribution and exact source linkage checks;
- B Worker A/B anonymous ID set equality, distinct order, empty response cells, worker ZIP integrity and absence of answer key;
- 12 previous finite-model PASS labels and 20 nonreg rows with official conformance `NOT_EXECUTED`;
- eight thematic question triads each contain SCF/SDR/ASR, and **S6/S8 mix original source system families**. This is flagged as an audit limitation, not misrepresented as within-experiment empirical control.
- Source/fixture structural checks share authorship with the expected labels and do **not** measure independent scientific discriminability.

**Actual independent reviewer A/B/adjudicator:** `NOT_EXECUTED` / `NOT_EXECUTED` / `NOT_EXECUTED`; **Cohen κ `UNAVAILABLE`**. `RA2=UNTESTED`. Actual Jev/LLM/SOP trials = 0. Formal `G-O` and empirical `G-E` remain `NOT_EXECUTED`.

## New local scientific review artifact inventory

| File | Content |
|---|---|
| `SAR-03-C_Scientific_Program_Synthesis_v1.0.md` | Full sourced Chinese/English scientific synthesis, strongest objections and evidence ceilings |
| `SAR-03-C_Minimum_Program_Separation_Contract_v0.1.md` | Candidate S0–S8 claim-level program/negative-route and cross-view contract |
| `SAR-03-C_Primary_Program_Minimum_Contract_v0.1.csv` | Three core scientific program definitions |
| `SAR-03-C_M1_M2_Claim_Comparability_v0.1.csv` | 12 cross-view criteria |
| `SAR-03-C_Negative_Routing_and_Abstention_Atlas_v0.1.csv` | 18 negative / abstention fixtures |
| `SAR-03-C_Triad_Source_Homogeneity_Audit_v1.0.csv` | 8 source-triad check results, S6/S8 marked cross-family |
| `SAR-03-C_Directed_NonRegression_v1.0.csv` | 24 review-only directed non-regression decisions |
| `SAR-03-C_Open_Decision_Gates_v1.0.csv` | 17 open scientific/validation/governance gates |
| `SAR-03-C_Source_Anchor_Check_v1.0.csv` | 30 checked exact R5.1 source heading line anchors |
| `SAR-03-C_Verification_Result_v1.0.json` | 58 complete check outcomes, input dimensions and evidence ceilings |
| `SAR-03-D_Science_Owner_Decision_Preview_v0.1.md` | Three options A/B/C, no decision presumed |
| `README.md`, `build_sar03c.py`, `SAR-03-C_SHA256SUMS.csv` | Reproducible script and file checksum manifest |

## Local package integrity and hashes

- Verified conversation-container ZIP: `/mnt/data/SIS-R5.1-SAR03-C_Review_Package_v1.0.zip`
- ZIP size **41,836 bytes**, SHA-256: `8c1edb36d2f9b1bc712f0dbdcc276959a667d9f8fa7f4c8f3962114899659d0f`; archive integrity and every manifest-file hash checked in build script.
- Full local science report SHA-256: `bcc7943000740eb7bd3d62244f25075dbfe03420815c56b2eb111748b741ea5e`.
- Local candidate contract SHA-256: `05d69d3bf847ea6005d98c6fcfa3c8222251a505b411787e7ace6abd3ee2ee98`.
- Reproducible local Python source SHA-256: `5f1d4959603687bcb4c24e3c1539b4bfbeb013a3020829854f2913654850ad5e`.
- **GitHub review branch has the scientific summary, candidate contract, 3/12/18/8/24/17 record indexes, decision preview and this receipt; the complete local ZIP including full Python is not claimed to be uploaded verbatim to GitHub.**

## Preservation of scientific non-regression

Three Primary Programs remain SCF/SDR/ASR; X1/X2 crosscutting; four canonical routing statuses unchanged; no newly adopted Core Primitive, Primary Program, enum, schema field, M2 `C_t` or §9 reinterpretation. `ScientificCoreDelta=0` is **not** certified by these checks. Part VII-A remains `PROPOSED NORMATIVE PATCH`.

**Review status:** SAR-03-C candidate complete, SAR-03-D science-owner decision pending, RA2 independent blind UNTESTED, R-01/R-02 HIGH OPEN, remaining G-O/G-E unexecuted. R5.1 Master and main branch unchanged.
