# Daily Pricing Analysis Rerun — V2 Combined Outputs

**Run date:** 2026-11-15  
**Input folder:** `V2Comparisons/Combined`  
**Output folder:** `V2Comparisons/Report/DailyPricing_Rerun_2026-11-15`

## Results

### Artwork

- Combined source rows: 139,442
- Unique lots: 73,555
- Analysis lots: 18,967
- Low estimate median absolute percentage error: 32.89%
- Midpoint median absolute percentage error: 34.38%
- High estimate median absolute percentage error: 41.73%
- Midpoint within ±20%: 30.71%

### Cars

- Combined source rows: 12,531
- Matched lots: 442
- Analysis lots: 151
- Gooding Amelia Island 2025 midpoint median absolute percentage error: 37.38% (N=128)
- RM Abu Dhabi 2025 midpoint median absolute percentage error: 11.11% (N=23)
- Cars were analyzed by event using the existing buyer-premium inversion logic.

### Memorabilia

- Combined source rows: 7,858
- Unique matched lots used for analysis: 883
- Low estimate median absolute percentage error: 22.08%
- Midpoint median absolute percentage error: 39.21%
- High estimate median absolute percentage error: 60.00%
- Midpoint within ±20%: 22.99%
- Dollar-error sample: 675 lots

## Output contents

The `Artwork`, `Cars`, and `Memorabilia` subfolders contain the regenerated analysis tables, CSV summaries, and charts from the existing daily pricing analysis pipelines. These outputs were written to the new dated folder and did not overwrite the previous `daily_sales` reports.

## Important interpretation note

These are auction-house estimate benchmarks generated from the combined V2 comparison outputs. No Barkr, Local Pricer, Standard, or Llama item-level prediction values were present in the combined inputs, so model-to-model pricing accuracy could not be calculated.
