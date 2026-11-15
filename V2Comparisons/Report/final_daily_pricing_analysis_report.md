# Final Daily Pricing Analysis Report — V2 Comparison Rerun

**Report date:** 2026-11-15  
**Scope:** Artwork, Cars, and Memorabilia  
**Input:** V2 comparison outputs and merged files in `V2Comparisons/Combined`

## Executive summary

The normal-versus-V2 comparison review was completed for all available auction-house folders across the three planned assets. Individual findings reports were created under `V2Comparisons/Report/<Asset>/<AuctionHouse>/`, and the tracking Google Sheet was updated with file coverage, row counts, comparison findings, and report paths.

The final daily-pricing analysis was then rerun from the merged combined JSON files. The regenerated outputs are stored in `V2Comparisons/Report/DailyPricing_Rerun_2026-11-15/` and include analysis tables, CSV summaries, data-quality files, outlier lists, and charts.

## Final rerun results

| Asset | Source rows | Analysis lots | Low estimate median APE | Midpoint median APE | High estimate median APE |
|---|---:|---:|---:|---:|---:|
| Artwork | 139,442 | 18,967 | 32.89% | 34.38% | 41.73% |
| Cars | 12,531 | 151 | Event-specific | Gooding 37.38%; RM Abu Dhabi 11.11% | Event-specific |
| Memorabilia | 7,858 | 883 | 22.08% | 39.21% | 60.00% |

## Main findings

1. Artwork produced 18,967 eligible analysis lots. The low estimate performed better than the midpoint and high estimate on median absolute percentage error.
2. Cars produced 151 eligible lots across the Gooding Amelia Island and RM Abu Dhabi events. Cars were analyzed separately by event using buyer-premium inversion logic.
3. Memorabilia produced 883 eligible lots. The low estimate again had the lowest median absolute percentage error, while the high estimate had the largest error.
4. Several auction-house folders contain missing V2 files, unpaired stems, mismatched row populations, or misplaced files. These issues are documented in the individual auction-house reports.
5. No item-level Barkr, Local Pricer, Standard, or Llama predictions were present, so model-to-model accuracy and coverage comparisons could not be calculated.

## Deliverables

- Auction-house comparison reports: `V2Comparisons/Report/<Asset>/<AuctionHouse>/findings_report.md`
- Final rerun summary: `V2Comparisons/Report/DailyPricing_Rerun_2026-11-15/rerun_summary.md`
- Final rerun tables and charts: `V2Comparisons/Report/DailyPricing_Rerun_2026-11-15/Artwork/`, `Cars/`, and `Memorabilia/`
- Comparison tracking sheet: `V2 Comparebles`

## Outstanding validation items

- Obtain missing V2 files for auction houses where only normal JSON is available.
- Reconcile row mismatches and unpaired stems before treating every V2 output as complete.
- Validate title-based matching where V2 records lack `lot_url`.
- Confirm price-basis and currency assumptions before external publication.
- Supply item-level model prediction files if Barkr, Local Pricer, Standard, and Llama comparisons are required.
