# Daily Pricing Analysis Findings — Memorabilia / Bonhams

**Analysis date:** 2026-11-14  
**Status:** Completed

## File coverage

- Normal JSON files: 3
- V2 JSON files: 3
- Paired normal/V2 files: 3 (`3ZA`, `4AR`, `4BB`)
- Normal-only files: 0
- V2-only files: 0
- Normal JSON rows: 362
- V2 JSON rows: 362
- Paired files with row-count mismatch: 0
- Matching Bonhams CSV exports: 5
- CSV rows: 2,281

## Comparison findings

All three normal/V2 file pairs have matching row counts and 362 common records when matched by `lot_url`. Changes were found in 297 selected field comparisons: 145 low-estimate changes, 145 high-estimate changes, and 7 title changes. No selected description, realized-price, or USD-realized-price changes were found.

The CSV count includes only exports under the Bonhams auction-house path. Similarly named `Bonhams_Cars` exports were excluded because they belong to a separate auction-house folder.

## Daily pricing conclusion

Bonhams V2 changes are concentrated in estimate values, while realized prices remain unchanged in the compared records. The V2 data is suitable for the pricing rerun after validating the estimate differences against the five matching CSV exports.

## Next step

Proceed to `Memorabilia → Broad Arrow` after confirmation.
