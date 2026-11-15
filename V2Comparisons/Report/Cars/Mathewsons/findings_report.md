# Daily Pricing Analysis Findings — Cars / Mathewsons

**Analysis date:** 2026-11-14  
**Status:** Completed

## File coverage

- Normal JSON files: 1
- V2 JSON files: 3
- Paired normal/V2 files by stem: 1 (`1B`)
- Normal-only files: 0
- V2-only files: 2 (`1E`, `4A`)
- Normal JSON rows: 900
- V2 JSON rows: 811
- CSV exports: 1
- CSV rows: 1,394

## Comparison findings

The only paired stem, `1B`, has 900 records in the normal JSON and 599 records in the V2 JSON. The two versions have zero common records when matched by URL or ID, so no row-level field comparison or pricing-difference calculation is possible for this pair.

The V2-only files `1E` and `4A` contain 188 and 24 records respectively. The normal and V2 files therefore represent different record populations rather than a directly comparable revision of the same records.

The available CSV export contains 1,394 rows and should be reconciled separately against the appropriate source population before using it for daily pricing outputs.

## Daily pricing conclusion

Mathewsons requires a data-lineage check before final pricing rerun. The current normal/V2 pairing is nominally matched by filename stem but has no shared URLs or IDs, preventing a reliable record-level comparison.

## Next step

Proceed to `Cars → Mecum` after confirmation.
