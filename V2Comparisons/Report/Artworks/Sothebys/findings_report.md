# Artworks — Sothebys

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Sothebys artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 234 |
| `_v2` JSON files | 235 |
| Matched normal/v2 file pairs | 221 |
| v2-only files | 14 |
| Normal-only files | 13 |
| Rows in normal JSON files | 21,359 |
| Rows in v2 JSON files | 22,157 |
| Paired files with different row counts | 98 |
| CSV files available | 22 |
| CSV rows available | 1,775 |

## Findings

1. Sothebys has broadly complete but asymmetric v2 coverage: fourteen files exist only in v2 and thirteen only in the normal dataset.
2. Among 221 matched pairs, 98 have different row counts. The v2 dataset contains 798 more rows overall than the normal dataset.
3. Using `lot_url`, `ID`, or sale/lot fallback keys, 18,533 records were common across the matched pairs and 15,651 changed in the selected comparison fields.
4. The largest changes are in realized-price fields (`ah_price`, `ah_price_usd`, and `hammer_price_usd`), followed by subject matter and description fields. Artwork titles, descriptions, medium, and estimates also change for subsets of records.
5. Twenty-two CSV exports are available with 1,775 rows. CSV counts match the normal JSON for 17 covered stems and the v2 JSON for 15, so the CSV layer is mixed and requires explicit version alignment before pricing conclusions are drawn.

## Comparison rule for the next stage

Use the normalized record key for matched files, keep coverage and row-count differences separate, and normalize numeric/null values before comparing CSV pricing outputs.

## Status

Completed for `Artworks → Sothebys`. The Artworks asset is complete; the next asset is Cars.
