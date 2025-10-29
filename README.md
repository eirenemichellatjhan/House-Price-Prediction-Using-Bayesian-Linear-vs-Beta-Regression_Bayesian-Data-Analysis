# House-Price-Prediction-Using-Bayesian-Linear-vs-Beta-Regression_Bayesian-Data-Analysis

This project applies Bayesian regression methods to predict house prices based on key property and location features from the kc_house_data dataset. After sampling 5,000 entries and selecting 11 predictors through correlation analysis, the goal was to identify which housing attributes most strongly influence price.

**Tools**: R, rstanarm, Bayesian Linear Regression, Bayesian Beta Regression, DIC & WAIC Evaluation

**Approach**: Two Bayesian models were built — Linear Regression and Beta Regression. The Linear model was applied directly to the price variable, while the Beta model used a scaled price (0–1) for proportional estimation. Both models were compared using Deviance Information Criterion (DIC) and Widely Applicable Information Criterion (WAIC) to evaluate performance and model fit.

**Results**:
* Bayesian Linear Regression achieved lower DIC (1112.35) and WAIC (397.51), indicating better predictive accuracy than Bayesian Beta Regression (DIC = 2467.76, WAIC = 548.13).
* Posterior predictive checks showed that the model closely matched observed data, confirming a good fit.

**Key Insight**:
Bayesian Linear Regression provided more accurate and stable predictions of house prices. Variables such as floors, waterfront, view, grade, and latitude showed strong positive influence on price, while bedrooms, bathrooms, and living area had limited impact.
