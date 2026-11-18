# Predicting College Graduation Rates

**Question:** How well do institutional characteristics predict US college graduation rates?

## Approach
1. Inspect 777 records and identify one impossible graduation-rate value (118%).
2. Exclude that observation transparently.
3. Make a 70/30 train/test split.
4. Fit an eight-predictor OLS model and a pre-specified three-predictor model.
5. Compare both against a mean-prediction baseline using held-out RMSE and MAE.

## Files
- [`analysis.ipynb`](analysis.ipynb) — executable analysis, charts, and interpretation
- [`College.csv`](College.csv) — historical educational dataset

## Interpretation
Predictive performance is assessed on data not used for model fitting. The relationships are not causal, and one train/test split cannot establish generalisability.

## Attribution
Independently written portfolio adaptation of methods practised in LSE PP422. Dataset: `College`, distributed for educational use in the *Introduction to Statistical Learning* ecosystem.
