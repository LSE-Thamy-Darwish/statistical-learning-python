# Statistical Learning in Python

An evolving collection of independently documented statistical modelling and simulation projects, informed by methods studied in LSE's PP422 course.

## Projects

### [Predicting College Graduation Rates](college-graduation-prediction/)
A reproducible analysis of historical US college data comparing an eight-predictor OLS model, a simpler three-predictor model, and a mean-prediction baseline. Includes data validation, exploratory visualisation, and held-out RMSE/MAE evaluation.

**Tools:** Python, pandas, matplotlib, statsmodels, scikit-learn.

### [Estimating Income Inequality Using Bootstrapping](income-inequality-bootstrap/)

An applied statistical analysis of income inequality in South Africa using percentile-based measures and bootstrap resampling. Estimates the P90/P10 income ratio, constructs 95% bootstrap confidence intervals, and examines differences in income inequality across population groups.

**Tools:** Python, pandas, NumPy, matplotlib, statistical inference and bootstrapping.

## Run locally

```bash
pip install -r requirements.txt
cd college-graduation-prediction
jupyter notebook analysis.ipynb
```

## Academic and data attribution

This is an independently written portfolio analysis using techniques practised in PP422, not a copy of a graded submission or assignment questions. The `College` dataset is a historical educational dataset associated with *An Introduction to Statistical Learning* (ISLR/ISLP); credit remains with its original creators. It is included for reproducibility, not as contemporary institutional data.

## Limitations

Results describe predictive associations, not causal effects. The analysis excludes one graduation rate above 100%, so it does not exactly reproduce the original coursework results.
