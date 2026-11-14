# SAR-03-A｜Verification Receipt v1.0

> **2026-10-28 · INTERNAL SYNTHETIC FIXTURE/LOGIC VERIFICATION ONLY**  
> **SAR-03-A conceptually audited with open scientific gaps. NOT empirically or normatively verified.**

## Source and authority
- User-supplied R5.1 Candidate Full Master: **14,825 lines**, SHA-256 `92e7df596ac831e3185876cba814f9fa9a236d2331c2db14b55d317f9603684c`.
- Audit baselines: SAR-01-D `CONDITIONAL_ACCEPT_FOR_REVIEW_BASELINE`; SAR-02-D `CONDITIONAL_DUAL_VIEW_FOR_REVIEW_ONLY`; these are not source Master adoption.
- Source §22–33, §34–38, §40–50, §74–82, §91–94, §165–170; §84 `program_alignment`.

## Actual local execution summary
| Audit object | Count | Meaning |
|---|---:|---|
| Source line/heading assertions | **29 / 29 PASS** | Exact source anchors located in mounted R5.1 candidate |
| Five system families | **5 × 10 = 50** | Researcher-authored synthetic ScientificClaims |
| Claim routing expected/status consistency | **50 / 50 PASS** | Rules and review labels authored together; not independent Gold |
| Negative/invariance mutations | **30 / 30 PASS** | Deterministic reviewer-authored negative checks, not live model experiments |
| Same experiment → split SCF/SDR/ASR claim groups | **3 / 3 PASS** | Synthetic examples of §44 behavior |
| Canonical routing statuses represented | **4 / 4** | ROUTED, DESCRIPTIVE_ONLY, ROUTING_UNRESOLVED, SCIENTIFIC_NONCONFORMANT |
| Routed cases | **26** | SCF=13, SDR=6, ASR=7 **conditional on hypothetical evidence**, not actual measured effects |
| Nonrouted cases | **24** | DESCRIPTIVE_ONLY=9, ROUTING_UNRESOLVED=6, SCIENTIFIC_NONCONFORMANT=9 |
| Crosscutting illustration | **X1=1; X2=3** | Explicit focus; no independent causal proof |
| Directed non-regression review | **22** | 14 DESIGN_PRESERVED; 2 REVIEW_BASELINE_ONLY; 2 NOT_EXECUTED; 1 PROPOSAL_UNADOPTED; 1 OPEN_SEMANTIC_REVIEW; 1 OPEN_FUTURE_STRESS; 1 OPEN_DEFERRED |
| Real system experiments / measured causal effects | **0 / 0** | None performed |
| Independent blind second-coder review | **NOT_EXECUTED** | Needed for RA2 agreement validity |
| Formal ScientificExperimentContract runner | **NOT_EXECUTED** | G-O remains OPEN |

## Reproducible local package (not fully mirrored to GitHub)
- ZIP: `SIS-R5.1-SAR03-A_Review_Package_v1.0.zip` (43,962 bytes).
- ZIP SHA-256: `52540659c13c27f9b3176cf7fa3c1f993d25bb67e4860b36dea7dcef6afbff2b`; ZIP file integrity verified.
- Contains 11 files: full Chinese review, source-anchored English audit, source-anchor CSV, full 50-row fixture CSV/JSON, 30-row mutation CSV, 22-row nonregression CSV, negative routing contract, verification JSON, full local Python build/check source and SHA-256 manifest.
- GitHub review branch retains the **scientific audit summary, compact 50-row route index, 30-row negative test index, 22-row nonregression index, 16 open issues and this verification receipt**. These are not byte-for-byte assertions that the full ZIP was committed to GitHub.

## Interpretation and required boundaries
- `G-S=CONDITIONAL_REVIEW_WITH_OPEN_GAPS`
- `G-O=NOT_EXECUTED`
- `G-E=NOT_EXECUTED`
- `IndependentCoderReliability=UNTESTED`
- `OntologyRegimeComparability=OPEN`
- `RSI_MetaImproverExactContract=OPEN`
- `Part VII-A=PROPOSED_NORMATIVE_PATCH`
- `R5.1_Master=UNCHANGED`
- `SAR-03=IN_REVIEW/OPEN`

**Next unit:** SAR-03-B (Estimand Separation, Cross-View Identity & Blind Negative Routing Kill Audit). No normative Master updates, no new Primary Program, no schema expansion, no release/merge.
