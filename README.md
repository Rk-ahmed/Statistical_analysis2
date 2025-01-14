# Boston Housing Price Analysis

## Description
This project analyzes the Boston Housing dataset to identify key factors influencing housing prices and build a predictive model for the median value of homes. The analysis involves exploratory data analysis, statistical tests, and regression modeling.

## Dataset
The dataset contains 506 observations of 14 features, including the target variable **MEDV** (Median value of owner-occupied homes in $1000s).

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

## Requirements
The following Python libraries are required to run the analysis:
```bash
pandas
numpy
matplotlib
seaborn
scipy
statsmodels
```

## Usage
1. Clone the repository.
2. Ensure all dependencies are installed.
3. Run the Jupyter notebook or Python script to reproduce the analysis.

## Results
Key insights from the analysis include:
- The number of rooms (**RM**) and socioeconomic status (**LSTAT**) are the most significant predictors of house prices.
- Homes near the Charles River tend to have higher values.

## License
This project is open-source and available under the MIT License.

