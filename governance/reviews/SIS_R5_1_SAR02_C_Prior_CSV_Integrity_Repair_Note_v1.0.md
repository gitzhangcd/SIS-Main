# SAR-02-C Data Integrity Note — Prior Issue Registry CSV Delimiters

> **REVIEW-ARTIFACT REPAIR ONLY, NOT A SCIENTIFIC DECISION.** 2026-10-28.

The existing `SIS_R5_1_SAR02_Open_Semantic_Issues_v1.0.csv` contained six malformed delimiters in G-01 through G-06 following the SAR-02-B status refresh: an adjacent quoted status value had been joined to the previous quoted field. This caused a CSV syntax/column-count fault; it did **not** indicate that six science decisions were approved.

For SAR-02-C, the six separators were repaired, with **12/12 issue records retained, 9/9 columns per row**, and all G-01 through G-06 scientific statuses kept **OPEN**. The source R5.1 Master was not touched. The repair was verified by parsing all 13 CSV lines (header plus 12 rows).

SAR-02 remains `IN_REVIEW/OPEN`, SAR-02-D owner choice `PENDING`, official executable and empirical gates `NOT_EXECUTED`.

Changed file: `governance/reviews/SIS_R5_1_SAR02_Open_Semantic_Issues_v1.0.csv`; repair commit `e4b606d9254996df28b74a6885648910bc22ebfb`.
