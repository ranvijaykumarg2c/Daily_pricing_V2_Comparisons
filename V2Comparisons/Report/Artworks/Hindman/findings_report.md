# Artworks — Hindman

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Hindman artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 42 |
| `_v2` JSON files | 41 |
| Matched normal/v2 file pairs | 38 |
| v2-only files | 3 |
| Normal-only files | 4 |
| Rows in normal JSON files | 5,811 |
| Rows in v2 JSON files | 5,177 |
| Paired files with different row counts | 22 |
| CSV files available | 1 |
| CSV rows available | 106 |

## Findings

1. Hindman has near-complete but not identical v2 coverage. Three files exist only in v2 and four exist only in the normal dataset.
2. Among 38 matched pairs, 22 have different row counts. The v2 dataset contains 634 fewer rows overall than the normal dataset.
3. Using `lot_url`, `ID`, or sale/lot fallback keys, 4,350 records were common across the matched pairs and 4,047 changed in the selected comparison fields.
4. The largest changes are in `hammer_price_usd`, realized-price fields, and `subject_matter`. Titles, descriptions, medium, and estimate fields also change for subsets of records.
5. One CSV export is available with 106 rows. Its row count matches the normal JSON for its covered stem but not the v2 JSON, so it should be treated as a base-version pricing output unless the CSV generation rule is confirmed otherwise.

