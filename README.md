# Housing Price Prediction with Scikit-learn

## Project Overview
This project aims to predict median house values in California using various regression techniques. By analyzing 1990 Census data, we identify the key drivers of property value and compare the effectiveness of linear vs. non-linear machine learning models.

## The Dataset
I utilized the _**California Housing Dataset**_ (fetched via **_sklearn.datasets_**).

- **Target Variable**: Median House Value

- **Key Features**: Median Income, House Age, Average Rooms, Population, and Geographic Location (Latitude/Longitude).

## Model Workflow
The steps taken:

**1. Exploratory Data Analysis (EDA):** Viewed the data attributes.

**2. Preprocessing:** Built a _**Scikit-Learn Pipeline**_ involving _**StandardScaler**_ to prevent data leakage.

**3. Model Comparison:** Evaluated three distinct approaches:

- Linear Regression (Baseline)

- Random Forest (Ensemble)

- XGBoost (Gradient Boosting)

**4. Diagnostics:** Performed **_Residual Analysis_** and _**Feature Importance**_ mapping.

### Residual Analysis
<img width="1408" height="683" alt="image" src="https://github.com/user-attachments/assets/b5cbbc6f-b71e-4a67-9b37-16ad508cb416" />


### Feature Importance

<img width="687" height="493" alt="image" src="https://github.com/user-attachments/assets/7ed7a4cb-c5b9-4fe2-8522-ebeadf889390" />


## Results
After rigorous testing, **XGBoost** emerged as the **superior model**.

- Linear Regression ---> R2_Score = 0.60          MAE = 0.53
- Random Forest ---> R2_Score = 0.80              MAE = 0.33
- XGBoost ---> R2_Score = 0.83                    MAE = 0.29
