# Property Value Prediction for Cook County

<!-- BADGE ROW -->
![R](https://img.shields.io/badge/Language-R-276DC3?logo=r&logoColor=white)
![Random Forest](https://img.shields.io/badge/Model-Random%20Forest-brightgreen)
![Data Cleaning](https://img.shields.io/badge/Process-Data%20Cleaning-blue)
![Feature Engineering](https://img.shields.io/badge/Process-Feature%20Engineering-orange)
![Machine Learning](https://img.shields.io/badge/Category-Machine%20Learning-yellow)
![Cook County](https://img.shields.io/badge/Dataset-Cook%20County%20Properties-red)

This project focuses on developing a predictive model to estimate residential property values in Cook County. By leveraging historical property data and machine learning methods, the model aims to support more consistent and equitable tax assessments.

---

## Business Problem

Cook County faces ongoing challenges with **uneven property valuations**, which directly influence taxation fairness and regional planning.  
Traditional assessment methods often struggle with:

- Missing or inconsistent property data  
- Large variations in property characteristics  
- Difficulty identifying key drivers of sale price  

These gaps create uncertainty for both residents and county planners.

---

## Business Solution

Our team built a **Random Forest Regression model** that uses historical property characteristics to predict sale prices more accurately.  
The model:

- Addresses missing values and redundant features  
- Identifies the strongest predictors of property value  
- Generates consistent estimates for new properties  
- Provides data-driven support for equitable tax assessment and planning  

This solution helps improve valuation accuracy while offering transparency in what drives property prices.

---

## Project Overview

To create a fairer and more consistent valuation process, we processed the Cook County dataset, engineered meaningful features, and trained a Random Forest model to produce reliable value predictions.  
The workflow included data cleaning, handling multi-collinearity, encoding variables, and validating model performance.

---

## Key Objectives

1. Build a dependable predictive model for property valuations.  
2. Improve data quality by handling missing and redundant fields.  
3. Generate insights that assist Cook County’s taxation and planning decisions.

---

## Data Sources

- **Historic Property Dataset:** Includes structural attributes, geographic location, and previous sale prices.  
- **Prediction Dataset:** Contains new property entries requiring sale price estimates.

---

## Methodology

### 1. Data Cleaning & Preprocessing
- Treated missing values using median (numeric) and mode (categorical) imputation.  
- Removed columns with weak correlation to the target variable.  
- Addressed multi-collinearity by eliminating highly correlated predictors.

### 2. Feature Engineering
- Encoded categorical attributes into numeric form.  
- Standardized selected features for consistent scale.  
- Examined feature importance to refine model performance.

### 3. Model Training
- Implemented a **Random Forest Regression** model in R.  
- Used an 80/20 train–validation split.  
- Achieved a validation **MSE of 0.1217049**, demonstrating stable model performance.

### 4. Prediction & Evaluation
- Generated sale price predictions for the new property dataset.  
- Reversed scaling to return interpretable results.  
- Summary of sale price characteristics:
  - **Average:** \$350,000  
  - **Standard Deviation:** \$75,000  
  - **Range:** \$200,000 – \$1,500,000  
 
---

## Model Implementation

The model was developed entirely in **R**, with scripts covering:

- Data import and exploration  
- Missing value treatment  
- Feature transformation and encoding  
- Random Forest model training  
- Prediction generation and output export  

---

## Results

- A final predictions file (`predict_data_with_predictions.csv`) was produced.  
- The Random Forest model offered strong performance with low error metrics.  
- Feature importance analysis highlighted the property attributes most influential in determining sale price.

---

## Visualizations

- **Histogram:** Distribution of historic sale prices  
- **Boxplot:** Identification of outliers  
- **Feature Importance Graph:** Ranking of predictive features  

---

## Technologies Used

- **Language:** R  
- **Model:** Random Forest Regression  
- **Libraries:** `randomForest`, `caret`, `Metrics`, `readr`  

---

## My Contribution (Lasya)

As a member of the project team, I contributed to:

- Cleaning and preparing the historical dataset  
- Performing feature engineering and exploratory analysis  
- Supporting model training and validation  
- Reviewing outputs and helping structure the final insights  

---

## Future Improvements

- Incorporate economic and neighborhood-level indicators.  
- Experiment with Gradient Boosting, XGBoost, or Neural Networks.  
- Apply hyperparameter optimization and cross-validation for further model enhancement.

---
