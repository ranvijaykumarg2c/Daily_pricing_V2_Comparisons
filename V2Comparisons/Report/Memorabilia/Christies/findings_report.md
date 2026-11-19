# Daily Pricing Analysis Findings — Memorabilia / Christies

**Analysis date:** 2026-11-15  
**Status:** Completed

## File coverage

- Normal JSON files: 8
- V2 JSON files: 7
- Paired normal/V2 files: 7
- Normal-only files: 1 (`4BZ`)
- V2-only files: 0
- Normal JSON rows: 837
- V2 JSON rows: 787
- Paired files with row-count mismatch: 3 (`3CO`, `3EH`, `4V`)
- Matching CSV exports: 6
- CSV rows: 2,182

## Comparison findings

Across the seven paired stems, 757 records matched by `lot_url` and 485 selected field changes were identified. Changes were found in realized price (284), USD realized price (81), descriptions (33), low estimates (32), high estimates (32), and titles (23).

Pair-level results were: `3CN` 252/252 rows with 13 changes; `3CO` 174/168 with 3 changes; `3EH` 32/62 with 123 changes; `4DA` 44/44 with 2 changes; `4DB` 78/78 with 75 changes; `4U` 102/102 with 105 changes; and `4V` 111/81 with 164 changes. The normal-only `4BZ` file contributes 44 additional normal rows.

## Daily pricing conclusion

Christies Memorabilia has substantial V2 impact, particularly on realized prices and the `3EH`, `4DB`, `4U`, and `4V` comparisons. The row-count mismatches and the normal-only `4BZ` file should be reconciled against the six CSV exports before finalizing the daily pricing output.


