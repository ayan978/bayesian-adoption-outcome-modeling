# Bayesian Logistic Regression for Animal Shelter Adoption Outcomes

This project applies Bayesian logistic regression to animal shelter intake and outcome records from Long Beach Animal Shelter. The goal is to estimate how animal and intake characteristics are associated with the probability that a shelter record results in adoption.

The project is designed as a reproducible Bayesian analytics workflow using R, Quarto, JAGS, and MCMC diagnostics.

## Project Objective

Animal shelters collect detailed intake and outcome data, but these records are only useful when they can support practical decision-making. This project investigates whether observable characteristics such as animal type, recorded sex/status, intake condition, intake type, and age at intake are associated with adoption outcomes.

The analysis focuses on association, not causation.

## Research Question

**Which animal and intake characteristics are associated with the probability of adoption among common adoptable pets at Long Beach Animal Shelter?**

## Data Source

The dataset comes from TidyTuesday 2025 Week 9 and is based on Long Beach Animal Care Services shelter data.

Dataset page:  
https://github.com/rfordatascience/tidytuesday/tree/main/data/2025/2025-03-04

The raw dataset used in this project is stored in:

```text
data/raw/longbeach.csv
```

## Methods

The analysis uses a Bayesian logistic regression model:

- Response variable: adoption outcome
- Model type: Bayesian logistic regression
- Software: R, Quarto, JAGS
- Estimation: Markov Chain Monte Carlo
- Diagnostics: trace plots, effective sample size, Gelman-Rubin Rhat
- Outputs: posterior intervals and predicted adoption probabilities

## Repository Structure

```text
bayesian-animal-shelter-adoption/
├── analysis/
│   └── bayesian_logistic_adoption_analysis.qmd
├── data/
│   ├── raw/
│   │   └── longbeach.csv
│   └── processed/
├── outputs/
│   ├── figures/
│   └── tables/
├── presentation/
├── docs/
├── README.md
└── .gitignore
```

## Planned Outputs

This repository will include:

- cleaned and documented analysis workflow
- exploratory visualisations
- Bayesian model specification
- MCMC convergence diagnostics
- posterior coefficient interpretation
- predicted adoption probability visualisations
- rendered PDF report from the Quarto analysis

## Tools Used

- R
- Quarto
- tidyverse
- lubridate
- rjags
- coda
- ggplot2

## Project Status

Work in progress. The core dataset and project structure have been set up. The next stage is to polish the Quarto analysis, improve visualisations, add interpretation, and render the final professional report.