# Boston Housing Price Prediction Analysis

This project provides an in-depth analysis of the Boston Housing dataset with the goal of understanding the factors influencing house prices and building a predictive model to estimate median house values. The dataset is widely used in regression analysis, and this project employs statistical and machine learning techniques to extract actionable insights.

## Dataset Overview

The Boston Housing dataset consists of 506 observations with 13 features, representing key variables like crime rates, average number of rooms, property tax rates, and socio-economic factors, all contributing to the median house price (target variable).

| Feature   | Description                                                   |
|-----------|---------------------------------------------------------------|
| CRIM      | Per capita crime rate by town                                 |
| ZN        | Proportion of residential land zoned for large lots           |
| INDUS     | Proportion of non-retail business acres per town              |
| CHAS      | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| NOX       | Nitric oxide concentration (parts per 10 million)             |
| RM        | Average number of rooms per dwelling                          |
| AGE       | Proportion of owner-occupied units built before 1940          |
| DIS       | Weighted distances to five Boston employment centers          |
| RAD       | Index of accessibility to radial highways                     |
| TAX       | Full-value property tax rate per $10,000                      |
| PTRATIO   | Pupil-teacher ratio by town                                   |
| B         | Proportion of African-Americans by town                       |
| LSTAT     | % lower status of the population                              |
| MEDV      | Median value of owner-occupied homes in $1000s                |

- **Number of Observations**: 506
- **Number of Features**: 13 (Including predictors and target variable)
- **Target Variable**: MEDV (Median value of owner-occupied homes in $1000s)

## Project Objectives

- **Exploratory Data Analysis (EDA)**: To explore the distribution of key variables and their relationships with the target variable.
- **Statistical Analysis**: To conduct tests like T-tests and ANOVA for hypothesis testing on specific features.
- **Model Building**: To build a multiple linear regression model to predict the median house value using the available features.
- **Insight Generation**: To provide actionable insights on the factors affecting house prices in Boston.

## Exploratory Data Analysis (EDA)

### Key Findings:
- **Distribution of MEDV**: The target variable (MEDV) shows a slightly right-skewed distribution with a peak around $20,000.
- **Correlation Insights**:
  - **RM (average number of rooms)** has a strong positive correlation with **MEDV** (r = 0.7), suggesting that larger homes tend to have higher prices.
  - **LSTAT** (% lower status of the population) is negatively correlated with **MEDV** (r = -0.74), implying that areas with lower status populations tend to have lower house prices.
  - **NOX** and **DIS** show a moderate negative correlation, indicating that homes farther from employment centers tend to have better air quality.
- **Visualizations**:
  - **Correlation Heatmap**: Identifies relationships between variables.
  - **Boxplots & Histograms**: Provide deeper insights into distributions, especially regarding the influence of features like AGE, TAX, and PTRATIO.

## Statistical Analysis

### Key Statistical Tests:
- **T-Test for CHAS**: Conducted a two-sample T-test to check if there’s a significant difference in house prices for homes near and not near the Charles River. **Result**: Statistically significant (p < 0.05).
- **ANOVA for ZN Categories**: Performed ANOVA to check the effect of zoning on house prices. **Result**: Significant effect on house prices (p < 0.05).

## Multiple Linear Regression Model

A multiple linear regression model was built to predict **MEDV** based on all available predictors.

- **Adjusted R-squared**: 0.73, indicating that the model explains 73% of the variance in the target variable.
- **Significant Predictors**: RM, LSTAT, PTRATIO, and TAX.

## Findings and Insights

### Influence of Key Features:
- **RM** and **LSTAT** are the most significant predictors of house prices.
- Homes near the **Charles River (CHAS = 1)** tend to have higher median values.
- Higher accessibility to highways (higher RAD values) correlates with slightly lower house prices.

### Actionable Recommendations:
- Focus on developing larger homes with more rooms (**RM**).
- Improve socio-economic conditions in low-status areas (**LSTAT**) to boost house prices.
- Consider proximity to employment centers for future urban planning.

## Technologies Used

- **Python Libraries**:
  - Pandas, NumPy, Matplotlib, Seaborn (For data manipulation and visualization)
  - Scipy (For statistical testing)
  - Statsmodels (For regression modeling)

## Conclusion

This project demonstrates a thorough exploration of the Boston Housing dataset, providing both statistical and machine learning insights into factors influencing property prices. The findings have practical implications for urban planning, real estate development, and data-driven decision-making in the housing market.

## Files and Scripts

- **boston_housing.csv**: Dataset used for analysis.
- **EDA and Preprocessing**: Python code for data cleaning and exploration.
- **Statistical Tests**: Code for performing T-tests, ANOVA, and regression analysis.
- **Model Building**: Code for creating and evaluating the linear regression model.

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone <https://github.com/Rk-ahmed/Statistical-analysis/blob/main/online_retail.ipynb>
   ```
2. Open the Jupyter Notebook and run the cells in sequence.
3. Ensure the following libraries are installed:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

## License
This project is open-source and available under the MIT License.

