# Customer Satisfaction Factor and Sentiment Analysis at San Francisco International Airport (SFO)

This project analyzes customer satisfaction at San Francisco International Airport (SFO) using factor analysis (EFA/CFA) to uncover latent dimensions behind survey responses. The analysis also incorporates model refinement using modification indices and evaluates model fit through industry-standard metrics. The goal is to understand key drivers of satisfaction and produce a valid, interpretable factor structure suitable for reporting and future analysis.

## Project Overview
- Exploratory Factor Analysis (EFA)
- Confirmatory Factor Analysis (CFA)
- Model fit evaluation (CFI, TLI, RMSEA)
- Model refinement using modification indices
- Interpretation of latent satisfaction dimensions
- Integration of qualitative insights through sentiment analysis

## Dataset
The dataset includes:
- 14 survey items measuring customer satisfaction
- Likert-scale responses from SFO passengers
- Complementary open-text feedback used for qualitative insights

## Exploratory Factor Analysis (EFA)
Key steps:
- Conducted EFA to identify underlying factor structure across 14 survey items.
- Assessed dimensionality through eigenvalues, scree plot, and parallel analysis.
- Applied rotations (varimax and promax) to improve factor interpretability.
- Initial results suggested a multi-factor solution rather than a single generalized satisfaction factor.

## Confirmatory Factor Analysis (CFA)
A series of CFA models were tested to validate the structure found in EFA.

Initial findings:
- A 4-factor structure provided the strongest conceptual and statistical foundation.
- Baseline CFA model performance:
  - CFI: 0.964
  - TLI: 0.954
  - RMSEA: 0.053

## Model Refinement Using Modification Indices
To improve model accuracy and reflect realistic relationships between survey items:
- Added theoretically justified correlated residuals between closely related items.
- Refined item–factor relationships based on modification indices.
- Adjusted factor loadings where necessary to reduce model error.

Improved fit after refinements:
- CFI increased to 0.981
- TLI increased to 0.973
- RMSEA decreased to 0.041

These improvements indicate a substantially better-fitting and more interpretable factor structure.

## Final Model
The final selected model includes:
- 4 latent satisfaction factors
- Strong factor loadings across most items
- Minimal cross-loading
- Improved model fit and reduced error variance
- A structure that aligns with real-world themes in airport customer experience


## Technologies Used
- R
- lavaan
- psych
- tidyverse
- sentimentr (or other sentiment analysis package)


## Results Summary
- Identified a valid and interpretable 4-factor model for SFO customer satisfaction.
- Achieved strong final model fit (CFI = 0.981, TLI = 0.973, RMSEA = 0.041).
- Enhanced insights by combining factor analysis with sentiment analysis of passenger feedback.

## Repository Structure
- `data/` (optional) - survey datasets
- `scripts/` - R scripts for EFA, CFA, diagnostics, and sentiment analysis
- `results/` - output tables, fit statistics, and plots
- `README.md` - project overview and instructions

Links: 
- [Code and Report](https://github.com/Brianwitarsa/Customer-Satisfaction-Sentiment-Analysis-at-SFO/blob/main/Brian_Witarsa_Final_Project.html)
