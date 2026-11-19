# Cars — Broad Arrow

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the available Cars CSV exports for Broad Arrow.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 8 |
| `_v2` JSON files | 8 |
| Matched normal/v2 file pairs | 6 |
| v2-only files | 2 |
| Normal-only files | 2 |
| Rows in normal JSON files | 692 |
| Rows in v2 JSON files | 705 |
| Paired files with different row counts | 2 |
| CSV exports available | 9 |
| CSV stems represented | 8 |
| CSV rows available | 863 |

## Findings

1. Broad Arrow has eight normal JSON files and eight v2 files, but only six matched file pairs. Two files exist only in each version.
2. The v2 dataset contains 13 more rows overall, and two matched pairs have different row counts.
3. Using normalized URL, ID, or sale/lot fallback keys, 369 records were common across matched pairs and 368 changed in the selected comparison fields.
4. The largest changes are in description blocks and estimate fields. Realized-price fields and model also change for subsets of records.
5. Nine CSV exports represent eight stems because one stem appears in more than one output month. They contain 863 rows; seven represented stems align with normal JSON counts and three align with v2 counts.


