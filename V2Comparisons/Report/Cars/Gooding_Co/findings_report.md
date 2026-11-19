# Daily Pricing Analysis Findings — Cars / Gooding Co

**Analysis date:** 2026-11-14  
**Status:** Completed

## File coverage

- Normal JSON files: 3
- V2 JSON files: 1
- Paired normal/V2 files: 1 (`4D`)
- Normal-only files: 2 (`1A`, `4A`)
- V2-only files: 0
- Normal JSON rows: 398
- V2 JSON rows: 133
- Paired files with row-count mismatch: 0
- CSV exports: 6
- Unique CSV stems: 3 (`1A`, `4A`, `4D`)
- CSV rows: 751

## Comparison findings

The paired `standardized_gooding_co_data_4D.json` and `standardized_gooding_co_data_4D_v2.json` files contain the same 133 records. No differences were found in the compared fields: description, estimates, sale price, USD sale price, or model.

The normal dataset also contains two unpaired files (`1A` and `4A`), contributing 265 additional normal rows. The CSV output contains six exports across three unique stems, indicating repeated exports for some auction periods/months.

## Daily pricing conclusion

For the available paired Gooding Co data, the V2 output does not change the pricing or selected descriptive fields. The existing normal values can be retained for the paired `4D` comparison, subject to the broader CSV reconciliation.


