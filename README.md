# DSA 2050 Week 6: Sales Prediction

## 1. Project Overview

This project focuses on predicting sales using machine learning techniques. It explores how business characteristics, including advertising expenditure, store visits, discount percentages, product categories, customer segments, and regions, can be used to estimate sales.

The project follows a data science workflow that includes data exploration, preprocessing, model development, evaluation, and interpretation. The aim is to identify a suitable predictive model that can support business planning and decision-making.

## 2. Project Objectives

The main objectives of this project are:

* To explore and understand the sales dataset.
* To identify missing values, duplicate records, and other data quality issues.
* To investigate the relationships between business characteristics and sales.
* To develop and compare different machine learning models for sales prediction.
* To evaluate model performance using appropriate regression metrics.
* To identify the best-performing model and assess its ability to predict sales.
* To examine prediction errors and potential limitations of the models.

## 3. Tools and Technologies

The following tools and libraries are used in this project:

* **Python:** Programming language used for data analysis and machine learning.
* **Jupyter Notebook:** Environment for writing code, performing analysis, and presenting results.
* **Pandas:** Used for data manipulation and analysis.
* **NumPy:** Used for numerical computations.
* **Matplotlib:** Used to create visualizations and examine sales patterns.
* **Scikit-learn:** Used for data preprocessing, model development, and evaluation.

## 4. Project Workflow

The project follows these steps:

1. **Data Loading:** Import the sales dataset into the Jupyter Notebook.
2. **Data Exploration:** Examine the dataset's structure, variables, and summary statistics.
3. **Data Quality Assessment:** Check for missing values, duplicate records, and unusual values.
4. **Problem Definition:** Define sales as the target variable and identify the features used for prediction.
5. **Data Preprocessing:** Handle missing values, standardize numerical features, and encode categorical variables.
6. **Data Splitting:** Divide the dataset into training and testing sets to evaluate model performance.
7. **Model Development:** Build baseline models, Linear Regression, Ridge Regression, and a Decision Tree Regressor.
8. **Model Evaluation:** Compare model performance using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R²).
9. **Cross-Validation:** Use five-fold cross-validation to assess model performance across different training subsets.
10. **Error Analysis:** Examine residuals, compare actual and predicted sales, and investigate prediction errors.
11. **Final Recommendation:** Identify the most promising model based on the evaluation results.

## 5. Dataset

The project uses a sales dataset named `DSA2050_Week6_Sales_Data.csv`.

The dataset contains the following variables:

* **Sales_KES:** Sales value in Kenyan shillings. This is the target variable.
* **AdvertisingSpend_KES:** Amount spent on advertising.
* **StoreVisits:** Number of store visits.
* **DiscountPercent:** Discount percentage offered.
* **ProductCategory:** Category of the product.
* **CustomerSegment:** Customer group, such as Retail, Corporate, or SME.
* **Region:** Geographical region associated with the observation.

The dataset is loaded and explored using Pandas. Data preprocessing is performed within a machine learning pipeline to ensure that preprocessing steps are learned from the training data rather than the test data.

## 6. Results and Evaluation

The project compares baseline models with Linear Regression, Ridge Regression, and a Decision Tree Regressor.

The models are evaluated using three main metrics:

* **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted sales. Lower values indicate better performance.
* **Root Mean Squared Error (RMSE):** Measures prediction errors while giving greater weight to larger errors. Lower values indicate better performance.
* **R-squared (R²):** Measures the proportion of variation in sales explained by the model. Values closer to 1 generally indicate better performance.

Based on the recorded evaluation results, Ridge Regression performed best among the candidate models on the test set, achieving:

* **MAE:** KES 13,714.40
* **RMSE:** KES 17,458.82
* **R²:** 0.8705

The five-fold cross-validation results also favored Ridge Regression, with an average MAE of KES 15,971.37, an average RMSE of KES 20,103.54, and an average R² of 0.8479.

These results suggest that Ridge Regression can explain a substantial proportion of the variation in sales and provides useful predictive performance on the available dataset.

Residual analysis and error inspection were also performed to examine prediction errors and identify areas where additional business information could improve the model.

## 7. Conclusion

This project demonstrates how machine learning can be applied to sales prediction using business-related data. Several regression models were developed and compared using appropriate evaluation metrics and cross-validation.

Ridge Regression achieved the strongest overall performance among the candidate models based on the recorded results. The findings suggest that advertising expenditure, store visits, discounts, product categories, customer segments, and regions can be useful features for estimating sales.

However, the predictions may be affected by limitations in the dataset and the absence of external factors such as seasonality, competitor activities, and inventory availability.

Further testing with additional data and continued monitoring would help determine how well the model performs in real-world business situations.

## 8. Author

**Cindy Mamang Kanga**

DSA 2050 — Data Science
