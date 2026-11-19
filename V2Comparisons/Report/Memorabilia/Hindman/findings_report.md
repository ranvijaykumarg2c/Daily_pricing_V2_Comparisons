# Daily Pricing Analysis Findings — Memorabilia / Hindman

**Analysis date:** 2026-11-15  
**Status:** Completed

## File coverage

- Normal JSON files: 2
- V2 JSON files: 2
- Paired normal/V2 files: 2 (`3BL`, `4W`)
- Normal-only files: 0
- V2-only files: 0
- Normal JSON rows: 715
- V2 JSON rows: 715
- Paired files with row-count mismatch: 0
- Matching CSV exports: 2
- CSV rows: 5,068

## Comparison findings

All 715 records matched by `lot_url`, with 381 matching records in `3BL` and 334 in `4W`. No differences were found in the compared fields: descriptions, estimates, realized prices, USD realized prices, titles, or models.

## Daily pricing conclusion

Hindman’s normal and V2 JSON outputs are identical for the available paired records. The V2 output does not require pricing changes based on this comparison. The CSV exports should still be reconciled for row-level completeness because they contain 5,068 rows versus 715 JSON records.


