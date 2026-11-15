# Daily Pricing Analysis Findings — Memorabilia / Sothebys

**Analysis date:** 2026-11-15  
**Status:** Completed

## File coverage

- Normal JSON files: 33
- V2 JSON files: 30
- Paired normal/V2 files: 27
- Normal-only files: 6 (`1AD`, `2AAC`, `3AHZ`, `3CAC`, `3JZV`, `4R`)
- V2-only files: 3 (`4GC`, `4EI`, `unknown`)
- Normal JSON rows: 3,005
- V2 JSON rows: 2,479
- Paired files with row-count mismatch: 9
- Matching CSV exports: 40
- CSV rows: 3,311

## Comparison findings

Across the 27 paired stems, 1,910 records matched by `lot_url` and 4,146 selected field changes were identified. The changes were concentrated in realized price and USD realized price, with 1,792 changes in each field. There were also 543 description changes and 19 title changes.

Nine paired stems have row-count mismatches. The largest population differences include `4BK` (223 normal vs 85 V2), `4DQ` (146 vs 117), `4DA` (156 vs 171), `4EF` (90 vs 93), and `3FHZ` (105 vs 96). The unpaired normal-only and V2-only files further indicate incomplete one-to-one coverage.

## Daily pricing conclusion

Sothebys Memorabilia has substantial V2 pricing impact, especially in realized prices and USD realized prices. Because of the row mismatches and unpaired files, the CSV outputs and auction-stem coverage should be reconciled before finalizing the daily pricing rerun.

## Next step

All Memorabilia auction houses in the current sequence are complete. Proceed to the next asset after confirmation.
