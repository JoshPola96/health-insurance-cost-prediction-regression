# Insurance Charges Prediction

This project aims to predict insurance charges using various regression techniques and evaluate their performance. The dataset used includes information such as age, sex, BMI, number of children, smoker status, and region, with the target variable being the insurance charges.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Modeling Techniques](#modeling-techniques)
- [Results](#results)
- [Conclusion](#conclusion)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Project Overview

This project involves predicting insurance charges based on several features using three different regression models: Linear Regression, Polynomial Regression, and K-Nearest Neighbors (KNN). The goal is to compare the performance of these models and determine the most effective approach for this prediction task.

## Dataset

The dataset used in this project is `insurance.csv`, which includes the following columns:
- `age`: Age of the individual
- `sex`: Gender of the individual
- `bmi`: Body Mass Index
- `children`: Number of children/dependents
- `smoker`: Whether the individual is a smoker or not
- `region`: The region where the individual lives
- `charges`: The insurance charges

## Modeling Techniques

The following models were implemented and evaluated:
1. **Linear Regression**: A basic regression technique used to establish a linear relationship between the features and the target variable.
2. **Polynomial Regression**: An extension of linear regression that captures non-linear relationships by adding polynomial terms.
3. **K-Nearest Neighbors (KNN)**: A non-parametric method used for classification and regression by comparing the target value with its nearest neighbors in the feature space.

## Results

### Linear Regression
- **R-squared (R²)**: 0.78
- **Mean Squared Error (MSE)**: 33,596,915.85
- **Mean Absolute Error (MAE)**: 4,181.19

### Polynomial Regression
- **Best Model Parameters**: {'model__fit_intercept': True, 'poly__degree': 2, 'poly__include_bias': True}
- **R-squared (R²)**: 0.87
- **Mean Squared Error (MSE)**: 20,712,805.99
- **Mean Absolute Error (MAE)**: 2,729.50

### K-Nearest Neighbors (KNN)
- **Best Model Parameters**: {'model__metric': 'manhattan', 'model__n_neighbors': 5, 'model__weights': 'distance'}
- **R-squared (R²)**: 0.76
- **Mean Squared Error (MSE)**: 37,984,876.27
- **Mean Absolute Error (MAE)**: 3,618.19

## Conclusion

In this analysis, Polynomial Regression outperforms the other models with the highest R-squared value of 0.87, indicating the best fit and predictive accuracy for this dataset. KNN offers moderate performance, while Linear Regression serves as a baseline model. Polynomial Regression is recommended for predicting insurance charges based on the evaluated metrics.

## Installation

To run this project locally, you will need Python and the following packages:
- `pandas`
- `numpy`
- `scikit-learn`
- `seaborn`
- `matplotlib`

You can install the necessary packages using pip:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/insurance-charges-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd insurance-charges-prediction
   ```
3. Place the `insurance.csv` file in the project directory.
4. Run the Jupyter notebook or Python script to execute the analysis:
   ```bash
   jupyter notebook analysis.ipynb
   ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
