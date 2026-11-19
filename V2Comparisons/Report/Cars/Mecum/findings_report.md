# Daily Pricing Analysis Findings — Cars / Mecum

**Analysis date:** 2026-11-14  
**Status:** Completed

## File coverage

- Normal JSON files: 7
- V2 JSON files: 3
- Paired normal/V2 files by stem: 1 (`4D`)
- Normal-only files: 6
- V2-only files: 2 (`1B`, `4J`)
- Normal JSON rows: 4,301
- V2 JSON rows: 1,734
- Paired files with row-count mismatch: 1 (`4D`: 68 normal vs 40 V2)
- CSV exports: 3
- CSV rows: 8,826

## Comparison findings

The paired `4D` files share 40 records when matched by `lot_url`. No changes were found in the compared fields: description, estimates, sale price, USD sale price, or model. However, the normal file contains 68 rows while the V2 file contains 40, so 28 normal records are not represented in the V2 output.

The remaining files are not directly paired by stem: six normal-only files contribute 4,233 rows, and two V2-only files contribute 1,694 rows. The CSV output contains three exports totaling 8,826 rows and requires separate reconciliation to the source populations.

## Daily pricing conclusion

For the 40 records common to the paired `4D` files, V2 does not alter the selected pricing or descriptive fields. The row-population difference and multiple unpaired files should be resolved before treating the full Mecum dataset as a complete V2 pricing rerun.


