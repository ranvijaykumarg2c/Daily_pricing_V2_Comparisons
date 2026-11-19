# Artworks — Freemans

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Freemans artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 19 |
| `_v2` JSON files | 10 |
| Matched normal/v2 file pairs | 7 |
| v2-only files | 3 |
| Normal-only files | 12 |
| Rows in normal JSON files | 3,139 |
| Rows in v2 JSON files | 823 |
| Paired files with different row counts | 1 |
| CSV files available | 0 |
| CSV rows available | 0 |

## Findings

1. Freemans has incomplete v2 coverage: twelve normal-only files and three v2-only files are present, with only seven matched file pairs.
2. The normal dataset contains 3,139 rows, while the v2 dataset contains 823 rows. This difference is primarily a coverage difference rather than a row-level change across all source files.
3. Using `lot_url`, `ID`, or sale/lot fallback keys, 375 records were common across the matched pairs and 296 changed in the selected comparison fields.
4. All 296 detected record changes affect `subject_matter`. Smaller changes occur in artwork title and medium. No price-field changes were detected in the selected common records.
5. No Freemans Artwork CSV exports are currently available under `V2Comparisons\Output`, so CSV-based pricing validation cannot be completed for this auction house.



