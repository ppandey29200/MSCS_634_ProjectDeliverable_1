# MSCS_634_ProjectDeliverable_1

## Project Overview
This project is part of a broader effort to explore key stages of the data mining process, including data collection, preprocessing, feature engineering, and exploratory data analysis. The dataset selected for this deliverable focuses on diagnosing heart disease based on various patient health metrics.

---

## Dataset Summary

- **Dataset Name**: Heart Disease UCI
- **Source**: [Kaggle] https://www.kaggle.com/datasets/ineubytes/heart-disease-dataset
- **Records**: 1026
- **Attributes**: 14 (including target)
- **Objective**: Predict the presence (1) or absence (0) of heart disease based on features like age, sex, cholesterol, resting blood pressure, maximum heart rate, and more.

The dataset is suitable for this project due to its moderate size, mix of categorical and continuous variables, and relevance to real-world healthcare analytics.

---

## Data Cleaning Steps

1. **Checked for missing values**:
   - No missing values found in any column.
2. **Removed duplicate records**:
   - Duplicate records removed.
3. **Verified valid ranges** for features:
   - All continuous variables were inspected using `.describe()` to detect anomalies.
   - Outlier thresholds will be further considered in later modeling steps.

---

## Exploratory Data Analysis Highlights

- **Class Balance**:
  - The dataset is relatively balanced: ~54% of records indicate presence of heart disease.
  
- **Key Correlated Features**:
  - `cp` (chest pain type), `thalach` (max heart rate), `oldpeak` (ST depression) show strong correlation with `target`.
  
- **Visualizations**:
  - Count plots for target variable.
  - Correlation heatmap for numeric features.
  - Pairplots to examine feature relationships.

---

## Challenges Encountered

- Interpreting domain-specific features (e.g., `slope`, `ca`, `thal`) required additional research.
- Mixed data types (categorical encoded numerically) required contextual clarification.
- Some features like `fbs` and `restecg` showed weak correlation, which may influence feature selection later.

---

## Tools & Libraries Used

- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Next Steps

- Perform feature scaling and encoding where necessary.
- Proceed with regression and classification modeling in Deliverable 2.
- Consider dimensionality reduction techniques (PCA) to improve performance.

---

## Author
Pawan Pandey  
Advanced Big Data and Data Mining (MSCS-634-B01)  
University of the Cumberlands  