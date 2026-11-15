# Artworks — Phillips

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Phillips artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 86 |
| `_v2` JSON files | 95 |
| Matched normal/v2 file pairs | 71 |
| v2-only files | 24 |
| Normal-only files | 15 |
| Rows in normal JSON files | 10,387 |
| Rows in v2 JSON files | 12,127 |
| Paired files with different row counts | 38 |
| CSV files available | 5 |
| CSV rows available | 564 |

## Findings

1. Phillips has incomplete and asymmetric v2 coverage: twenty-four files exist only in v2 and fifteen only in the normal dataset.
2. Among 71 matched pairs, 38 have different row counts. The v2 dataset contains 1,740 more rows overall than the normal dataset.
3. Using `lot_url`, `ID`, or sale/lot fallback keys, 8,578 records were common across the matched pairs and 7,471 changed in the selected comparison fields.
4. The largest changes are in `hammer_price_usd`, realized-price fields, and `subject_matter`. Medium, descriptions, titles, and estimate values also change substantially.
5. Five CSV exports are available with 564 rows. Their row counts match the normal JSON for all five covered stems but match the v2 JSON for only two, indicating that these CSVs are primarily aligned with the normal source version.

## Comparison rule for the next stage

Use the normalized record key for matched files, report coverage and row-count differences separately, and normalize numeric/null values before comparing CSV pricing outputs.

## Status

Completed for `Artworks → Phillips`. The next unit is `Artworks → Sothebys`.
