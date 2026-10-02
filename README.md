# Advanced Empirical Finance

**Portfolio construction, financial data analysis and model uncertainty in Python.**

Selected academic group projects from Advanced Empirical Finance at the University of Copenhagen, 2026. Portfolio presented by Alexander Gjerum Fredbo-Nielsen.

**Course grade: 12**, the highest grade on the Danish grading scale. This is the course grade, not a separate grade for each report.

## Overview

When does a more sophisticated financial model actually produce a better decision?

These projects explore portfolio optimisation, risk estimation and backtesting. A recurring theme is that model complexity must be weighed against noisy inputs, unstable portfolio weights and trading costs.

**Start with Project 1** for a practical example of turning financial data into an analysis of investment choices and their limitations.

## 1. Portfolio optimisation and transaction costs

[Read the report](01_Portfolio_Optimisation_and_Transaction_Costs.pdf)

- Constructed an equity investment universe and compared portfolio strategies using factor-based covariance estimates, shrinkage and a trading penalty.
- Evaluated turnover and performance after assumed transaction costs, with checks across different universe sizes.
- **Finding:** Equal weighting had the highest reported Sharpe ratio in this study. More complex portfolios were sensitive to estimation uncertainty and trading costs.

## 2. High-frequency data and minimum-variance investing

[Read the report](02_High_Frequency_Data_and_Minimum_Variance.pdf)

- Processed intraday equity data and estimated realised covariance matrices.
- Compared minimum-variance portfolios using high-frequency information and daily-data shrinkage against equal weighting.
- **Finding:** Daily-data shrinkage produced lower reported volatility and more stable portfolios than the high-frequency approach in this sample.

## 3. Efficient portfolios and estimation uncertainty

[Read the report](03_Efficient_Portfolios_and_Estimation_Uncertainty.pdf)

- Used Monte Carlo simulation to compare portfolio strategies under known and estimated inputs.
- Examined efficient frontiers, minimum-variance portfolios and sensitivity to sample size.
- **Finding:** Estimation error can undermine theoretically optimal portfolios; simpler approaches can be more robust in the simulated settings.

## Tools and scope

Python, NumPy, pandas, numerical optimisation, statistical estimation and data visualisation.

This repository contains the reports, including code excerpts where present in the original documents. It does not provide a standalone runnable codebase or redistribute the underlying datasets.

## Limitations

These are academic simulations and historical analyses, not realised investment returns. Project 1 is not a fully recursive machine-learning backtest: signal training overlaps part of the evaluation period. Project 2 uses a survivor-based stock universe and reports performance before trading costs. Results should be read alongside the assumptions and limitations in each report.

## Authorship

All three reports are group work. Mandatory Assignment 1 was co-authored by Alexander Fredbo-Nielsen and Emil Kjeldgaard Leth. The exam reports retain their original contribution statements. This portfolio does not imply sole authorship of the analyses or code.
