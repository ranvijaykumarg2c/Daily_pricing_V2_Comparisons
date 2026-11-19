# Daily Pricing Analysis Findings — Memorabilia / Freemans

**Analysis date:** 2026-11-15  
**Status:** Completed

## File coverage

- Normal JSON files: 1
- V2 JSON files: 1
- Paired normal/V2 files: 1 (`4W`)
- Normal-only files: 0
- V2-only files: 0
- Normal JSON rows: 412
- V2 JSON rows: 412
- Paired files with row-count mismatch: 0
- Matching CSV exports: 1
- CSV rows: 2,329

## Comparison findings

The normal and V2 files have equal row counts, but the V2 records do not contain `lot_url`, so URL matching is unavailable. Using title as a fallback key produced 385 common records. Across those records, 1,492 selected field changes were found: 385 low-estimate changes, 385 high-estimate changes, 361 sale-price changes, and 361 USD sale-price changes.

The V2 file also uses a different schema and includes lot numbers in `asset_number`, while the normal file contains auction and lot URL fields. This schema difference should be considered during CSV reconciliation.

## Daily pricing conclusion

Freemans V2 materially changes pricing fields for the title-matched records. Because the V2 data lacks lot URLs, title-based matching should be validated before the final daily pricing output is generated.


