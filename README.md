## Honest vs. Misleading Visualizations

**Objective:** This project investigates how routine charting choices—axis truncation, scale selection, and series selection—can distort the perceived magnitude of economic change, using classical statistical pitfalls and real-world FRED and World Bank data as case studies.

**Methodology:**
- Reconstructed Anscombe's Quartet to demonstrate that identical summary statistics (mean, variance, correlation) can underlie four datasets with fundamentally different distributions and relationships, reinforcing the necessity of visual inspection before trusting descriptive statistics alone
- Quantified the distortion of a truncated-axis revenue chart using Tufte's Lie Factor metric (ratio of depicted effect size to actual effect size in the data), computing an initial value of 49 before redesigning the chart to accurately represent the underlying trend
- Sourced average hourly earnings data (FRED series AHETPI), deflated to real 2020 dollars, and produced four distinct chart variants of the same series to illustrate how axis scaling and baseline choices can each support a different narrative from identical data
- Executed a structured four-step exploratory data analysis (EDA) checklist—structure, distributions, relationships, and anomalies—on a World Bank GDP panel spanning 262 countries and 64 years
- Developed an interactive visualization tool enabling real-time toggling between chart configurations (axis floor, linear/log scale, nominal/real series, time window), with a live-updating Lie Factor readout to quantify distortion under each configuration

**Key Findings:**
- Summary statistics alone are insufficient for data validation; visually dissimilar datasets can produce numerically indistinguishable descriptive statistics, underscoring the value of exploratory visualization as a diagnostic step
- Axis truncation can inflate the perceived magnitude of change by an order of magnitude or more—the revenue chart's Lie Factor of 49 indicated the depicted change was roughly 49 times larger than the change actually present in the data
- Deflating nominal earnings to real (inflation-adjusted) terms is essential for cross-decade wage comparisons; nominal series systematically overstate purchasing-power gains by conflating price-level growth with genuine wage growth
- Chart design choices—not just underlying data—materially shape narrative interpretation, reinforcing the need for standardized, transparent visualization practices in applied economic communication
