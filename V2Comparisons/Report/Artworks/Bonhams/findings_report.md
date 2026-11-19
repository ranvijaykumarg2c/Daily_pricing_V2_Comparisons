# Artworks — Bonhams

## Scope

Comparison of normal standardized JSON files, matching `_v2` JSON files, and the available CSV exports for Bonhams artwork data.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 210 |
| `_v2` JSON files | 196 |
| Matched normal/v2 file pairs | 182 |
| v2-only files | 14 |
| Normal-only files | 28 |
| Rows in normal JSON files | 25,543 |
| Rows in v2 JSON files | 23,749 |
| Paired files with different row counts | 81 |
| CSV files available | 16 |
| CSV rows available | 1,595 |

## Findings

1. At the record level, 18,168 IDs were common to both versions. The selected comparison fields changed for 10,851 common records.
4. The largest changes are in descriptive fields (`description_block`, `medium`, and `subject_matter`) and realized-price fields (`ah_price`, `ah_bp_price`, and their USD equivalents). Auction URLs and artwork titles also change for a smaller subset.
5. The available CSV exports cover only 16 file stems and 1,595 rows. CSV row counts equal the normal JSON counts for all 16 covered stems, but v2 counts match only 11 of those stems. The CSVs also contain additional pricing-model and market-index columns, so comparisons must normalize numeric values and null representations before testing equality.
6. The v2 data appears to improve or restructure descriptive and price fields, but it should not be treated as a pure row-preserving replacement because records and schemas differ between versions.



