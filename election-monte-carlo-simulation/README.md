# Monte Carlo Simulation of Election Outcomes

**Research question:** How does sample size affect the reliability of identifying the winner of a closely contested election?

## Overview
An independently written, reproducible simulation based on voting-table results from **Peru’s 2021 presidential runoff**. Using 1,000 random samples each of 5 and 100 voting tables, this project compares estimated vote margins, sampling variability and the frequency of identifying the population winner.

## Methods
- Inspect and validate voting-table counts; exclude rows with missing required counts or zero votes.
- Compute the complete-case population margin in **percentage points**.
- Simulate simple random samples of voting tables without replacement within each repetition.
- Compare the distribution of estimated margins for sample sizes 5 and 100.
- Illustrate approximate 90% confidence-interval coverage using a simulation-derived standard error.

## Run locally
Install dependencies using the repository-root `requirements.txt`. Place the source dataset named `Peru Election 2020.csv` in this folder, then run `jupyter notebook analysis.ipynb`.

**The CSV is not included** because its public redistribution permission has not been verified. The filename says 2020, but the election analysed was held in 2021.

## Interpretation
This is an educational **finite-population sampling simulation**, not a real-world election forecast or assessment of election integrity. Larger random samples reduce sampling variation on average, but even samples of 100 tables can suggest the wrong winner in a close contest.

## Attribution
Independent portfolio adaptation of simulation and statistical-inference techniques practised in **LSE PP422**. The original educational exercise credited its election question as developed in collaboration with Dan Levy. Election data was supplied for coursework; source provenance and sharing permissions should be verified before redistribution.
