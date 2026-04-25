# Medicare Advantage: Star Ratings and Regression Discontinuity Analysis

This project analyzes the Medicare Advantage (MA) market from 2010 to 2015, focusing on the impact of "Star Ratings" on plan market share and enrollment. The analysis concludes with a Regression Discontinuity (RD) design to estimate the Average Treatment Effect (ATE) of receiving a marginally higher rating.

## Project Overview
The study explores how hospital star ratings influence consumer choice and plan performance.
### Key Components:
1.  **Summary Statistics:** Longitudinal tables (2010–2015) tracking mean star ratings, enrollment figures, and market shares, including a specific look at unrated plans.
2.  **Distributional Analysis:** Visualizations (bar graphs) of star rating distributions in 2010, 2012, and 2015 to identify industry-wide quality shifts.
3.  **Cross-Sectional Regressions:** A series of OLS regressions by year, estimating the correlation between specific star rating tiers (3.0, 3.5, 4.0, 4.5+) and market share.
4.  **Regression Discontinuity (RD) Design:** * Calculation of the "running variable" (the raw score before rounding into stars).
    * Estimation of the effect of crossing thresholds (e.g., 2.5 to 3.0 stars) on enrollments using specific bandwidths.
5.  **Robustness & Diagnostic Checks:**
    * **Bandwidth Sensitivity:** Testing estimates across multiple bandwidths (0.1 to 0.15) to ensure results aren't driven by arbitrary window choices.
    * **Manipulation Testing:** Graphical examination of the running variable distribution to check for "sorting" or manipulation around thresholds.
    * **Balance Tests:** Comparing plan characteristics (HMO and Part D status) just above and below thresholds to validate the RD assumptions.
