# Statistical Learning in Python

An evolving collection of independently documented statistical modelling and simulation projects, informed by methods studied in LSE's PP422 course.

## Projects

### [Predicting College Graduation Rates](college-graduation-prediction/)
A reproducible analysis of historical US college data comparing an eight-predictor OLS model, a simpler three-predictor model, and a mean-prediction baseline. Includes data validation, exploratory visualisation, and held-out RMSE/MAE evaluation.

**Tools:** Python, pandas, matplotlib, statsmodels, scikit-learn.

### [Estimating Income Inequality Using Bootstrapping](income-inequality-bootstrap/)

An applied statistical analysis of income inequality in South Africa using percentile-based measures and bootstrap resampling. Estimates the P90/P10 income ratio, constructs 95% bootstrap confidence intervals, and examines differences in income inequality across population groups.

**Tools:** Python, pandas, NumPy, matplotlib, statistical inference and bootstrapping.

### [Monte Carlo Simulation of Election Outcomes](election-monte-carlo-simulation/)

A simulation-based analysis of Peru's 2021 presidential runoff election, examining how sample size affects the reliability of election outcome predictions. Uses 1,000 Monte Carlo simulations to compare samples of 5 and 100 voting tables, assess sampling variability, and illustrate the challenges of predicting outcomes in closely contested elections.

**Tools:** Python, pandas, NumPy, matplotlib, Monte Carlo simulation, statistical inference.

## Run locally

```bash
pip install -r requirements.txt
cd college-graduation-prediction
jupyter notebook analysis.ipynb
```

## Academic and data attribution

The projects in this repository are independently written portfolio analyses developed using statistical and computational techniques studied in PP422 at the London School of Economics and Political Science (LSE). They are not direct reproductions of graded submissions or assignment questions.

The analyses draw on the following datasets:

- **College Graduation Prediction:** The `College` dataset, associated with *An Introduction to Statistical Learning* (ISLR/ISLP), is used for educational and reproducibility purposes. Credit remains with its original creators.
- **Income Inequality and Bootstrapping:** South African income survey data from the Post-Apartheid Labour Market Series (PALMS). The original dataset is not redistributed in this repository.
- **Monte Carlo Simulation of Election Outcomes:** Voting-table data from Peru's 2021 presidential runoff election, used to examine sampling variability and electoral uncertainty. The original dataset is not redistributed in this repository.

All analyses, interpretations, and visualisations are presented for educational and portfolio purposes. Original data sources retain their respective attribution and usage rights.

## Limitations

Results describe predictive associations, not causal effects. The analysis excludes one graduation rate above 100%, so it does not exactly reproduce the original coursework results.
