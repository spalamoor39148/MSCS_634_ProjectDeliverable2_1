# MSCS_634_ProjectDeliverable2_1

# Diabetes Prediction Project – Deliverable 1: Data Collection, Cleaning, and Exploration

## Dataset Summary

- **Dataset Name:** Pima Indians Diabetes Dataset  
- **Source:** [Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) / UCI Machine Learning Repository  
- **Records:** 768 patients  
- **Features:** 8 health-related attributes (Glucose, BMI, Insulin, Blood Pressure, Age, etc.)  
- **Target:** Outcome (0 = No Diabetes, 1 = Diabetes)  

This dataset contains clinical measurements used to predict diabetes onset. Its moderate size and relevant features make it suitable for demonstrating data preprocessing and predictive modeling techniques.

---

## Key Insights from Analysis

- Glucose levels and BMI have a strong positive correlation with diabetes diagnosis.
- Age and insulin levels also show distinctive patterns between diabetic and non-diabetic groups.
- The dataset shows moderate class imbalance favoring non-diabetic cases.
- Some features contained missing or invalid zero values, which were addressed through imputation.

---

## Data Cleaning and Exploration Steps

- **Missing Value Handling:** Replaced zero values (which are physiologically implausible) in key features with `NaN` and imputed using median values to preserve data distribution without biasing means.
- **Duplicate Removal:** Removed exact duplicate rows to ensure data integrity.
- **Outlier Detection:** Filtered extreme BMI values to avoid skewing model performance.
- **Exploratory Data Analysis:** Used visualizations including histograms, boxplots, pairplots, and correlation heatmaps to understand feature distributions, detect outliers, and assess relationships with the target variable.

---

## Challenges Encountered

- **Missing/Invalid Data:** Several features contained zeros where they were not valid (e.g., BMI=0), requiring careful replacement with medians.
- **Class Imbalance:** Though moderate, imbalance in diabetic vs. non-diabetic cases will require attention in future modeling steps (e.g., class weighting or oversampling).
- **Outliers:** Detecting and handling outliers needed domain knowledge to avoid removing valid but extreme health conditions.
- **Feature Scale Differences:** Wide variation in feature scales suggests need for normalization before modeling.

---

## Next Steps

The cleaned and explored dataset will be used for feature engineering, regression and classification modeling, and further pattern mining in subsequent project deliverables.

