# Multiple Linear Regression - Multi-Channel Marketing Analysis

This repository contains a data science project focused on evaluating the simultaneous impact of multiple marketing channels (TV, Radio, and Social Media) on overall sales performance using Multiple Linear Regression.

## Project Overview
The goal of this analysis is to model real-world multi-channel marketing spend, detect and address multicollinearity among predictors, and provide clear, evidence-based budget allocation recommendations to optimize business ROI.

## Step-by-Step Methodology
1. **Exploratory Data Analysis (EDA):** Analyzed descriptive statistics and inspected data structures to understand the distribution of variables.
2. **Multicollinearity Diagnostic:** Built a correlation matrix heatmap and calculated the Variance Inflation Factor (VIF) for independent variables (`TV`, `Radio`, `Social Media`) to ensure model stability.
3. **Model Implementation:** Fitted a multivariate Ordinary Least Squares (OLS) regression model using `statsmodels` to predict `Sales`.
4. **Assumption Checking & Diagnostics:** Evaluated the model’s assumptions using key visual diagnostic plots:
   * **Linearity & Fit:** Predicted vs. Actual Sales scatter plot.
   * **Homoscedasticity:** Residuals vs. Fitted values plot.
   * **Normality:** Normal Q-Q plot and a Residuals Distribution Histogram (validated formally with the Shapiro-Wilk test).
5. **Business Interpretation:** Interpreted the model's Adjusted $R^2$, individual predictor p-values, and regression coefficients in a business context.

## Technologies Used
* Python 3
* Pandas & NumPy (Data Cleaning and Transformation)
* Matplotlib & Seaborn (Advanced Statistical Visualizations)
* Statsmodels (OLS Regression & VIF Diagnostics)
* SciPy (Hypothesis Testing)

## Key Business Insights & Requirements Met
* **Multicollinearity Checked:** Addressed dependency issues among variables via VIF tracking.
* **Model Justification:** Evaluated variable inclusion using individual p-values and overall model fit via Adjusted $R^2$.
* **Actionable Recommendations:** Coefficients clearly demonstrate the effect of a one-unit increase in a single channel's budget while holding all other marketing channels constant, allowing for a prioritized budget allocation strategy.
*
