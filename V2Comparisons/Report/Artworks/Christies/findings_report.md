# Artworks — Christies

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Christies artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 224 |
| `_v2` JSON files | 235 |
| Matched normal/v2 file pairs | 200 |
| v2-only files | 35 |
| Normal-only files | 24 |
| Rows in normal JSON files | 24,147 |
| Rows in v2 JSON files | 26,688 |
| Paired files with different row counts | 99 |
| CSV files available | 28 |
| CSV rows available | 3,015 |

## Findings

1. The normal and v2 datasets do not have identical file coverage. Thirty-five files exist only in v2 and twenty-four exist only in the normal dataset.
2. Among 200 matched file pairs, 99 have different row counts. Across all files, v2 contains 2,541 more rows than the normal dataset.
3. Christies records do not retain stable generated `ID` values between versions. `lot_url` was therefore used as the primary record key, with sale and lot identifiers as fallback keys.
4. Using the normalized record key, 19,301 records were common to both versions and 18,238 had changes in the selected comparison fields.
5. The largest changes are in `subject_matter`, realized-price fields, and `hammer_price_usd`. Estimate values, descriptions, medium, and titles also change for subsets of records.
6. The available CSV exports cover 28 file stems and 3,015 rows. CSV counts match the normal JSON counts for 26 stems but match the v2 counts for only 13 stems. CSV values include additional pricing-model and market-index columns and require type/null normalization before equality checks.
7. Because the v2 dataset changes both coverage and record content, it should be treated as a revised extraction rather than a simple append or direct replacement.

## Comparison rule for the next stage

Use `lot_url` as the primary key for Christies, with sale number plus lot number as a fallback. Normalize numeric strings, URL formatting, and null markers before comparing fields. Keep file coverage, row-count, record additions/removals, field changes, and CSV pricing outputs as separate findings.

## Status

Completed for `Artworks → Christies`. The next unit is `Artworks → Freemans`.
