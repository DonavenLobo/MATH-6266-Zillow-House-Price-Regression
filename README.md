# MATH 6266: Zillow Housing Market Data Analysis

## Overview

This project involves analyzing housing market data using linear regression models to understand the relationship between various property features and their selling prices. The analysis focuses on single-family houses in specific neighborhoods and examines the impact of square footage and other variables on selling prices.

## Data Filtering

- **House Type**: Only single-family houses are included.
- **Neighborhoods**: Focused on ZIP codes 30310, 30309, and 94043.

## Analysis Steps

1. **Data Filtering**: The dataset is filtered to include only single-family houses in the specified ZIP codes.
2. **Scatter Plots**: Created scatter plots of selling price vs. square footage for each neighborhood.
3. **Regression Analysis**:
   - Calculated regression lines for price vs. square footage using the least squares method.
   - Analyzed the linearity of the relationship between price and square footage.
4. **Statistical Tests**:
   - Tested if the intercept of the regression line is statistically different from zero.
   - Evaluated the significance of adding the number of bathrooms as a variable.

## Key Findings

- **Linearity**: The relationship between price and square footage appears linear in the analyzed neighborhoods.
- **Intercept Significance**: The intercept of the regression line was not statistically different from zero.
- **Bathrooms Impact**: The number of bathrooms did not have a statistically significant effect on the selling price after accounting for square footage.

## Model Comparison

Two models were compared to assess the impact of including the number of bathrooms as a predictor:

1. **Model with Bathrooms**:
   - R-squared: 0.588
   - Adjusted R-squared: 0.520
   - AIC: 1034
   - Coefficient for bath: Not significant

2. **Model without Bathrooms**:
   - R-squared: 0.588
   - Adjusted R-squared: 0.535
   - AIC: 1032

### Conclusion

- Excluding the number of bathrooms did not reduce the model's explanatory power.
- The model without bathrooms is preferred due to a slightly improved adjusted R-squared and a lower AIC, indicating a more efficient model.
- The number of bathrooms is not a significant predictor of selling price in this dataset.

## Tools Used

- **Python Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels
- **Environment**: Jupyter Notebook

## Author

- Donaven Lobo