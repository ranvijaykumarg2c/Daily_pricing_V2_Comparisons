# Daily Pricing Analysis Findings — Memorabilia / Broad Arrow

**Analysis date:** 2026-11-15  
**Status:** Completed

## File coverage

- Normal JSON files: 2
- V2 JSON files: 1
- Paired normal/V2 files: 0
- Normal-only files: 2 (`4N`, `4O`)
- V2-only files: 1 (`4I`)
- Normal JSON rows: 388
- V2 JSON rows: 197
- Paired files with row-count mismatch: 0
- Matching CSV exports: 2
- CSV rows: 1,164

## Comparison findings

No normal/V2 file pair shares the same file stem, so no direct record-level comparison is available. The normal files contain 388 records in total, while the V2-only file contains 197 records.

The two matching CSV exports correspond to the normal-only `4N` and `4O` stems and contain 1,164 rows in total. The V2-only `4I` dataset has no matching CSV export in the local output folder.

## Daily pricing conclusion

Broad Arrow Memorabilia requires a data-lineage check before the V2 pricing rerun because the available V2 file is not paired with a normal JSON file by stem and has no corresponding CSV export.


