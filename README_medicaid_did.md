# Medicaid Expansion and Health Insurance Coverage

This project studies whether Medicaid expansion under the Affordable Care Act increased health insurance coverage and whether the effect differed between metro and non-metro populations.

## Research question

Did Medicaid expansion increase health insurance coverage, and were the gains different for metro and non-metro populations?

## Data

The analysis uses American Community Survey (ACS) data obtained through IPUMS. The sample is restricted to adults ages 19--64 in California and Texas for 2013 and 2015.

- California is treated as the Medicaid expansion state.
- Texas is used as the non-expansion comparison state.
- The outcome is whether an individual has any health insurance coverage.
- Metro status is used to test for geographic heterogeneity.

## Methods

The project uses a difference-in-differences design. The main model compares the change in insurance coverage in California before and after Medicaid expansion to the change in Texas over the same period.

A second model adds a triple interaction between expansion status, post period, and metro status to test whether the treatment effect differs between metro and non-metro populations.

## Files

- `medicaid_did_analysis.R`: Cleaned R script for data cleaning, summary statistics, plots, and regression models.
- `outputs/table1_summary.csv`: Summary statistics table.
- `outputs/coverage_trend_ca_tx.png`: Pre/post insurance coverage plot by state.
- `outputs/coverage_by_metro_status.png`: Pre/post insurance coverage plot by metro status.
- `outputs/regression_results.html`: Regression table.
- `outputs/regression_results.tex`: LaTeX regression table for Overleaf.

## Main findings

The difference-in-differences estimate suggests that insurance coverage increased more in California than in Texas after Medicaid expansion. The heterogeneity analysis does not show strong evidence that the expansion effect differed substantially between metro and non-metro populations.

## Notes

The analysis relies on the parallel trends assumption. Because the final project used only one pre-treatment year, this assumption should be discussed as a limitation rather than treated as fully testable.
