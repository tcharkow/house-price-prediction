# House Price Prediction — Ames Housing Dataset

Predicting residential home sale prices using multiple regression techniques on the Ames, Iowa housing dataset — from raw data cleaning through feature engineering to regularized regression modeling in R.

## Project Overview

Using real housing transaction data to understand which features drive sale price, build a progression of regression models (simple → multiple → regularized), and compare model performance using cross-validation.

## Dataset

Ames Housing Dataset via the `AmesHousing` R package — 2,930 residential home sales in Ames, Iowa between 2006 and 2010, with 82 variables describing lot, building, and sale characteristics.

No manual download required — the dataset loads directly via:
```r
install.packages("AmesHousing")
library(AmesHousing)
ames <- ames_raw
```

## Key Goals

- Showcase the full regression pipeline: cleaning → EDA → feature engineering → modeling
- Compare simple, multiple, and regularized regression (Ridge & Lasso)
- Identify the features that most strongly predict sale price
- Translate model findings into interpretable business insights

## Project Structure

- `analysis.Rmd` — Full analysis: data cleaning, descriptive statistics, feature engineering, and modeling

## Tech Stack

- R 4.6
- tidyverse
- janitor
- corrplot
- glmnet (Ridge & Lasso)
- FastAPI (coming)
- React (coming)

## Setup

1. Clone this repository
2. Open `house-price-prediction.Rproj` in RStudio
3. Install dependencies:
```r
install.packages(c("AmesHousing", "tidyverse", "janitor", "corrplot", "scales", "glmnet"))
```
4. Open and run `analysis.Rmd`