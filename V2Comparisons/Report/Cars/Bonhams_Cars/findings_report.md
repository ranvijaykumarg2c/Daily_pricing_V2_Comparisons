# Cars — Bonhams Cars

## Scope

This report compares the normal standardized JSON files, matching `_v2` JSON files, and the Cars CSV exports for the Bonhams Cars source folder.

## Coverage

| Measure | Result |
|---|---:|
| Normal JSON files | 13 |
| `_v2` JSON files | 15 |
| Matched normal/v2 file pairs | 8 |
| v2-only files | 7 |
| Normal-only files | 5 |
| Rows in normal JSON files | 1,666 |
| Rows in v2 JSON files | 1,768 |
| Paired files with different row counts | 2 |
| Cars CSV files available | 5 |
| Cars CSV rows available | 797 |

## Findings

1. Bonhams Cars data is stored under `V2Comparisons\Cars\Bonhams_Cars`, separate from the empty `Cars\Bonhams` folder.
2. v2 coverage is incomplete and asymmetric: seven files exist only in v2 and five only in the normal dataset.
3. Eight file pairs are available; two have different row counts. Across all files, v2 contains 102 more rows than the normal dataset.
4. Using normalized URL, ID, or sale/lot fallback keys, 423 records were common across matched pairs and 159 changed in the selected comparison fields.
5. The main changes are in description blocks, realized-price fields, auction URLs, estimates, and titles. Model changes affect a smaller subset.
6. Five Cars CSV exports are available with 797 rows. Their counts align with the normal JSON files for all five stems; three align with the v2 counts. CSVs should therefore be treated as primarily base-version pricing outputs unless version provenance is confirmed.
7. Additional CSVs under the same bucket source are located in a `Memorabilia` path and were excluded from this Cars analysis.


