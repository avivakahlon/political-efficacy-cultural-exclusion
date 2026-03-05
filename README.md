# Perceived Cultural Exclusion & Political Efficacy Among Immigrants in Europe
Tools: R, tidyverse, ggplot2, dplyr, dagitty
Data: European Social Survey Round 10 — available at europeansocialsurvey.org

UMass Amherst — Fall 2025

# Overview
This project examines whether perceived cultural exclusion is associated with political efficacy among first-generation immigrants across 22 European countries, using data from the European Social Survey (n = 3,087).

# Methods
- Cleaned and filtered ESS Round 10 data to isolate first-generation immigrants using dplyr
- Engineered a composite cultural exclusion index by aggregating 5 discrimination variables and a reverse-coded belonging measure via rowMeans
- Fit 3 sequential OLS regression models — bivariate, demographic controls, and country fixed effects
- Validated model assumptions via residuals vs. fitted, Q-Q, Scale-Location, and Cook's distance diagnostics

# Key Finding
Higher perceived cultural exclusion is significantly associated with lower political efficacy (p < 0.001), even after controlling for age, gender, education, income, and country-level differences.

To run this analysis, download the ESS Round 10 dataset (https://www.europeansocialsurvey.org/news/article/round-10-data-now-available), save it as ESS10e03_2.csv in the same directory as analysis.qmd, and render using Quarto.
