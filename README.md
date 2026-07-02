# Predicting Brazil's Municipal Human Development Index with Random Forest

[![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white)](https://www.r-project.org/)
[![HarvardX](https://img.shields.io/badge/HarvardX-Data%20Science%20Capstone-A51C30)](https://credentials.edx.org/credentials/74eb4ba5c6fe4e7a8ebb7937dab9d224/)
[![edX](https://img.shields.io/badge/edX-Professional%20Certificate-02262B)](https://credentials.edx.org/credentials/74eb4ba5c6fe4e7a8ebb7937dab9d224/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-green)](#modeling-approach)
[![Random Forest](https://img.shields.io/badge/Random%20Forest-Regression-2E7D32)](#results)

## Overview

This repository contains my capstone project for the **HarvardX Data Science Professional Certificate**, offered through edX.

The project applies machine learning techniques to predict Brazil's **Municipal Human Development Index (IDHM)** using socioeconomic indicators related to income, education, health, poverty, inequality and demographics.

This work is an adaptation of my undergraduate thesis in Economics at the Federal University of Mato Grosso do Sul (UFMS), redesigned as a data science capstone project using R, exploratory data analysis, data wrangling, visualization and Random Forest regression.

## Project Objective

The main objective is to evaluate whether a Random Forest model can accurately predict IDHM values for Brazil, the Brazilian states and the Federal District using socioeconomic variables from 2012 to 2021.

The project also shows how machine learning can support economic analysis and public policy by identifying important predictors of human development.

## Data

The dataset was built from public socioeconomic indicators from Atlas Brasil and related sources.

The final analytical dataset includes observations for Brazil, the 26 Brazilian states and the Federal District across the period 2012-2021.

Main variables include:

- Municipal Human Development Index (IDHM)
- Per capita income
- Life expectancy
- Infant mortality
- Poverty rate
- Total population
- Average years of schooling
- Education subindices
- School attendance subindex
- Illiteracy rates by age group
- Gini index
- Theil index

## Methodology

The project follows an end-to-end data science workflow:

```text
Data collection
-> Data cleaning and reshaping
-> Dataset joining
-> Exploratory Data Analysis
-> Correlation analysis
-> Train/test split
-> Random Forest regression
-> Hyperparameter comparison
-> RMSE evaluation
-> Variable importance analysis
```

## Modeling Approach

The main algorithm used was **Random Forest regression**, implemented in R with the `randomForest` and `caret` packages.

Two model configurations were tested:

- Model 1: Random Forest with 500 trees and `mtry = 3`
- Model 2: Random Forest with 500 trees and `mtry = 4`

The second model achieved slightly better performance and was selected as the preferred configuration.

## Results

The Random Forest model showed strong predictive performance for IDHM.

Key results:

| Model | Trees | mtry | Variance Explained | RMSE |
|---|---:|---:|---:|---:|
| Model 1 | 500 | 3 | 97.38% | 0.0087 |
| Model 2 | 500 | 4 | 97.58% | 0.0083 |

The most relevant predictors included:

- School attendance subindex
- Per capita income
- Life expectancy
- Education-related variables
- Infant mortality
- Poverty rate

These results suggest that Random Forest can capture important nonlinear relationships between socioeconomic indicators and human development outcomes.

## Repository Structure

Current structure:

```text
.
├── README.md
├── EDX IDHM.Rmd
├── EDX-IDHM.pdf
├── references.bib
├── *.xlsx
└── EDX Havard choose your own.Rproj
```

Recommended future structure:

```text
.
├── README.md
├── reports/
│   └── EDX-IDHM.pdf
├── notebooks/
│   └── EDX IDHM.Rmd
├── data/
│   └── raw/
├── src/
├── figures/
├── references.bib
└── EDX Havard choose your own.Rproj
```

The current RMarkdown file reads the Excel files from the repository root using relative paths, so the existing structure is kept to preserve reproducibility.

## Tools and Packages

The project was developed in R using:

- R
- RStudio
- RMarkdown
- `tidyverse`
- `dplyr`
- `tidyr`
- `ggplot2`
- `corrplot`
- `RColorBrewer`
- `ggpubr`
- `caret`
- `randomForest`
- `caTools`
- `readxl`

## Certificate

This project was developed as part of the **HarvardX Data Science Professional Certificate** on edX.

Credential:

```text
https://credentials.edx.org/credentials/74eb4ba5c6fe4e7a8ebb7937dab9d224/
```

## Report

The full project report is available here:

[EDX-IDHM.pdf](./EDX-IDHM.pdf)

## GitHub Repository Metadata

Suggested About description:

```text
HarvardX Data Science Capstone applying Random Forest regression in R to predict Brazil's Municipal Human Development Index using socioeconomic indicators.
```

Suggested topics:

```text
r
data-science
machine-learning
random-forest
harvardx
edx
capstone-project
human-development-index
idhm
socioeconomic-indicators
economics
caret
tidyverse
ggplot2
```

Repository name:

```text
harvardx-data-science-capstone-idhm
```

Alternative shorter name:

```text
idhm-random-forest-capstone
```

## Author

**Matheus Assis de Oliveira**

Economist | MSc Candidate in Applied Economics | Data Analysis & Data Science

- GitHub: https://github.com/matheusassiso
- LinkedIn: https://www.linkedin.com/in/matheus-assis-de-oliveira-086a4a178/
