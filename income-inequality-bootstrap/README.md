# Estimating Income Inequality in South Africa with Bootstrapping

A Python case study using historical 2017 South African survey data to estimate the **P90/P10 income ratio**, construct bootstrap uncertainty intervals, and compare inequality **within** population groups.

## Methods
- Data validation and missing-income filtering
- Quantile-based income inequality measurement
- 1,000 nonparametric bootstrap replications
- Percentile-based uncertainty intervals
- Exploratory comparison of within-group inequality

**Tools:** Python, pandas, NumPy, matplotlib.

## Reproduce

1. Obtain an authorised copy of `palms_clean.csv` from the original course/data provider. **The CSV is intentionally not included** pending confirmation of redistribution rights.
2. Place it in this folder alongside `analysis.ipynb`.
3. Install the repository dependencies (`pip install -r ../requirements.txt`).
4. Open `analysis.ipynb` in Jupyter and run all cells.

## Key observed results

After excluding missing incomes, the data contain **61,788 observations**. The overall P90/P10 ratio is approximately **23.41**. The observed within-group ratios are approximately **20.18** for African/Black respondents and **15.38** for Coloured respondents, a difference of **4.80**. Bootstrap interval estimates are recomputed in the notebook with a documented random seed.

## Caveats

This is an independently written portfolio adaptation of techniques practised in LSE PP422, not a reproduction of the original assessed questions. The data are historical and do not establish current conditions. The extract lacks survey weights and design variables, so simple bootstrap intervals should **not** be treated as survey-design-corrected population confidence intervals. The contrast between the most and least unequal observed groups was selected after inspecting the data and is exploratory. Findings are descriptive, not causal.
