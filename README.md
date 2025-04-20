# Health Insurance Cost Prediction

## Project Overview
This project analyzes a health insurance dataset to predict medical costs based on various customer attributes. The analysis employs multiple regression models to determine which factors most significantly influence insurance charges and which modeling approach provides the most accurate predictions.

## Dataset Description
The dataset contains information about health insurance beneficiaries, including:
- **age**: Age of the insured individual
- **sex**: Gender of the insured (Male/Female)
- **bmi**: Body Mass Index of the insured
- **children**: Number of children/dependents covered by the insurance
- **smoker**: Whether the insured is a smoker (Yes/No)
- **region**: Geographical region of the insured (Northwest, Southeast, Southwest, or Northeast)
- **charges**: Insurance charges billed to the individual (target variable)

## Project Structure
1. **Data Loading and Exploration**
   - Loading the insurance dataset
   - Examining basic statistics and distributions
   - Visualizing relationships between features

2. **Data Preprocessing**
   - Encoding categorical variables
   - Feature scaling
   - Creating training and testing splits

3. **Model Implementation and Evaluation**
   - Linear Regression
   - Polynomial Regression
   - K-Nearest Neighbors (KNN)
   - Decision Tree Regression

4. **Model Comparison**
   - Performance metrics calculation (MSE, MAE, R²)
   - Visualization of predictions vs. actual values
   - Analysis of residuals

## Key Findings
The analysis reveals that:
- Polynomial Regression performs best with R² of 0.87, effectively capturing non-linear relationships in the data
- Decision Tree Regression follows closely with R² of 0.85, demonstrating strong capabilities in handling complex interactions
- Linear Regression (R² of 0.78) provides a good baseline but misses some non-linear patterns
- KNN (R² of 0.76) offers reasonable predictions but less accuracy than other models

## Technologies Used
- **Python**: Primary programming language
- **Pandas & NumPy**: Data manipulation and numerical operations
- **Scikit-learn**: Machine learning models and evaluation metrics
- **Matplotlib & Seaborn**: Data visualization
- **Pipeline & GridSearchCV**: Model construction and hyperparameter tuning

## Model Performance Summary

| Model | MSE | MAE | R² |
|-------|-----|-----|------|
| Linear Regression | 33,596,915.85 | 4,181.19 | 0.78 |
| Polynomial Regression | 20,712,805.99 | 2,729.50 | 0.87 |
| K-Nearest Neighbors | 37,984,876.27 | 3,618.19 | 0.76 |
| Decision Tree Regression | 22,508,600.27 | 2,830.75 | 0.85 |

## Usage
To run this project:
1. Clone the repository
2. Install required dependencies
3. Run the Jupyter notebook or Python script
