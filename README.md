# Regression-Assignment-California-Housing
## Objective
This project aims to apply and evaluate various **regression algorithms** on the **California Housing dataset** using Python. The goal is to predict the **median house value** based on features like population, income, number of rooms, and more.

## Dataset
The dataset used is the **California Housing dataset** from `sklearn.datasets.fetch_california_housing`.  
It includes **8 input features** and **1 target variable** (median house price).

## Preprocessing Steps
-  **Conversion**: Loaded and converted to a Pandas DataFrame for ease of manipulation.
-  **Missing Values**: Checked and confirmed **no missing values**.
-  **Feature Scaling**: Applied `StandardScaler` for algorithms sensitive to feature magnitude (e.g., SVR, Linear Regression).

##  Implemented Regression Algorithms

| Model                  | Mean Squared Error (MSE) | Mean Absolute Error (MAE) | R² Score |
|------------------------|--------------------------|----------------------------|----------|
| **Random Forest**      | 0.2555                   | 0.3276                     | **0.8050** |
| **Gradient Boosting**  | 0.2940                   | 0.3717                     | 0.7756   |
| **Support Vector**     | 0.3552                   | 0.3978                     | 0.7289   |
| **Decision Tree**      | 0.4943                   | 0.4538                     | 0.6228   |
| **Linear Regression**  | 0.5559                   | 0.5332                     | 0.5758   |

---

##  Model Descriptions

- **Linear Regression**: Models a straight-line relationship; used as a baseline.
- **Decision Tree**: Tree structure-based splitting; good for capturing non-linearity.
- **Random Forest**: Ensemble of decision trees; reduces overfitting, performed best overall.
- **Gradient Boosting**: Sequentially optimizes predictions; good accuracy with controlled bias.
- **SVR (Support Vector Regressor)**: Margins around the best-fit curve; performs well but computationally heavier.

---

## Results Summary

-  **Best Model**: **Random Forest Regressor**  
  Justification: Highest R² score (**0.805**), lowest MSE and MAE.

-  **Worst Model**: **Linear Regression**  
  Justification: Lowest R² score (**0.575**), unable to model complex non-linear patterns in data.
