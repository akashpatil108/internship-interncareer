# Breast Cancer Wisconsin (Diagnostic) Dataset Analysis

## Overview

This repository contains an in-depth analysis of the Breast Cancer Wisconsin (Diagnostic) dataset. The dataset is commonly used for binary classification problems to diagnose whether a breast mass is malignant or benign.

## Dataset Description

- **Total Entries:** 569
- **Columns:** 33 columns
- **Column Types:** 1 integer, 1 object (diagnosis), and 31 float64
- **Missing Values:** Column "Unnamed: 32" has no non-null values (potentially irrelevant column)

The dataset comprises features computed from breast mass images, including mean, standard error, and worst values of attributes like radius, texture, perimeter, area, smoothness, compactness, concavity, symmetry, and fractal dimension.

## Key Observations

1. **Data Exploration:**
   - Explored the dataset structure, identifying 569 entries and 33 columns.
   - Cleaned the dataset by dropping the potentially irrelevant "Unnamed: 32" column.
   - Encoded the categorical variable "diagnosis" into numerical values (0 for 'B' - Benign, 1 for 'M' - Malignant).

2. **Data Preprocessing:**
   - Analyzed feature distributions and multicollinearity.
   - Identified and kept features that contribute to good classification (e.g., radius_mean, perimeter_mean).
   - Detected highly correlated features and considered dropping some to avoid multicollinearity.

3. **Model Building and Evaluation:**
   - Implemented machine learning models (Random Forest, SVM, etc.) for classification.
   - Evaluated model performance using accuracy, precision, recall, and F1-score.
   - Explored hyperparameter tuning to optimize model performance.

4. **Documentation:**
   - Created a comprehensive report documenting the approach, findings, and rationale behind model choices.

## Feature Selection

Two sets of features were selected and analyzed:

1. **Selected_Features_RF_SKB:**
   - Identified important features using Random Forest and SelectKBest.
   - Features selected based on both machine learning model importance and statistical analysis.

2. **Selected_Features_Good_Classified:**
   - Focused on features that showed good classification with respect to the target feature.
   - Addressed multicollinearity and selected features contributing to effective classification.

## Model Recommendations

- **For Selected_Features_RF_SKB:**
  - Best Model: Support Vector Machine (SVM) post hyperparameter tuning with an accuracy of 98.24%.

- **For Selected_Features_Good_Classified:**
  - Best Model: Support Vector Machine (SVM) post hyperparameter tuning with an accuracy of 99.12%.

## Conclusion

The internship project successfully explored the Breast Cancer Wisconsin dataset, leveraging AI for efficient data analysis and model building. The findings contribute to the understanding of breast cancer diagnosis and showcase the power of AI in healthcare applications.


