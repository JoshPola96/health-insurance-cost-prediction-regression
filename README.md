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

This project involves predicting insurance charges based on several features using different regression models: Linear Regression, Polynomial Regression, K-Nearest Neighbors (KNN), and Decision Tree Regression. The goal is to compare the performance of these models and determine the most effective approach for this prediction task.

## Dataset

The dataset used in this project is `insurance.csv`, which includes the following columns:

- **age**: Age of the individual
- **sex**: Gender of the individual
- **bmi**: Body Mass Index
- **children**: Number of children/dependents
- **smoker**: Whether the individual is a smoker or not
- **region**: The region where the individual lives
- **charges**: The insurance charges

The dataset can be found on Kaggle: [Insurance Charges Dataset](https://www.kaggle.com/datasets/teertha/ushealthinsurancedataset/code)

## Modeling Techniques

The following models were implemented and evaluated:

- **Linear Regression**: A basic regression technique used to establish a linear relationship between the features and the target variable.
- **Polynomial Regression**: An extension of linear regression that captures non-linear relationships by adding polynomial terms.
- **K-Nearest Neighbors (KNN)**: A non-parametric method used for classification and regression by comparing the target value with its nearest neighbors in the feature space.
- **Decision Tree Regression**: A model that uses a tree-like graph of decisions and their possible consequences for predicting values.

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

### Decision Tree Regression
- **Best Model Parameters**: {'model__criterion': 'poisson', 'model__max_depth': 10, 'model__max_features': None, 'model__max_leaf_nodes': 10, 'model__min_samples_leaf': 4, 'model__min_samples_split': 10}
- **Mean Squared Error (MSE)**: 22,508,600.27
- **Mean Absolute Error (MAE)**: 2,830.75
- **R-squared (R²)**: 0.855

## Conclusion

In this analysis, Polynomial Regression outperforms the other models with the highest R-squared value of 0.87, indicating the best fit and predictive accuracy for this dataset. Decision Tree Regression also shows promising performance with an R-squared value of 0.855. KNN offers moderate performance, while Linear Regression serves as a baseline model. Polynomial Regression is recommended for predicting insurance charges based on the evaluated metrics.

## Installation

To run this project locally, you will need Python and the following packages:

- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

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

This project is licensed under the MIT License.
