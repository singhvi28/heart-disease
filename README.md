# Heart Disease Analysis and Prediction

Dataset - https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction

The heart disease dataset contains medical information and patient attributes used for predicting the presence of heart disease. It includes 14 features, both categorical and numerical, representing patient demographics, medical history, and diagnostic information. Key features include:

- `Age`: The patient’s age in years.
- `Sex`: The gender of the patient (1 = male, 0 = female).
- **Chest Pain Type** `CP`: Indicates the type of chest pain experienced (e.g., typical angina, atypical angina, non-anginal pain, asymptomatic).
- **Resting Blood Pressure** `RestingBP`: Resting blood pressure in mm Hg.
- **Cholesterol** `Chol`: Serum cholesterol levels in mg/dl.
- **Fasting Blood Sugar** `FBS`: Whether the fasting blood sugar is above 120 mg/dl (1 = true; 0 = false).
- `RestingECG`: Results of the resting electrocardiographic test.
- **Max Heart Rate Achieved** `MaxHR`: Maximum heart rate reached during exercise.
- **Exercise Induced Angina** `ExerciseAngina`: Presence of exercise-induced angina (1 = yes, 0 = no).
- **ST Depression** `Oldpeak`: ST depression induced by exercise relative to rest.

The dataset also includes the target variable, `Heart Disease`, which indicates the presence or absence of heart disease (1 = presence, 0 = absence). This dataset is widely used for modeling, exploring relationships between features, and building machine learning models to predict heart disease risk.

## Overview

This project involves developing a heart disease prediction model using traditional machine learning algorithms. The goal is to predict whether a patient is likely to have heart disease based on various health metrics and patient attributes. The dataset includes categorical and numeric features such as age, sex, chest pain type, cholesterol levels, maximum heart rate, and the presence of heart disease.
The project applies Exploratory Data Analysis (EDA) and Statistical Analysis to uncover patterns, relationships, and insights that aid in building accurate models.

## Project Structure
- **Exploratory Data Analysis (EDA)**: Visualized the data distribution and relationships using histograms, box plots, and correlation heatmaps to understand the structure and identify patterns.
- **Statistical Analysis**: Used chi-square tests and t-tests to explore relationships between categorical and numerical variables to assess their significance in heart disease prediction.
- **Data Preprocessing**: Handled categorical variables using one-hot encoding and scaled numerical features when necessary. The dataset was split into training (80%) and testing (20%) sets to evaluate model performance.
- **Machine Learning Models**: Trained and evaluated multiple machine learning models, including:
  - Logistic Regression (Test Accuracy: 85.33%)
  - Support Vector Machine Classifier (Test Accuracy: 86.41%)
  - Random Forest Classifier (Test Accuracy: 85.33%)
  - XGBoost Classifier (Test Accuracy: 88.04%)

The models were tuned to address overfitting and improve generalization using techniques such as hyperparameter adjustment, cross-validation, and regularization.

## Results
The XGBoost Classifier achieved the highest accuracy (88.04%), while the SVM Classifier also performed well (86.41%). These results highlight the effectiveness of ensemble methods and regularization techniques in improving predictive accuracy. Detailed evaluation metrics and model comparisons are included in the notebook.

## Key Takeaways
- Gained insights into data analysis and visualization techniques for healthcare data using `matplotlib` and `seaborn`.
- Explored various statistical methods like chi-square tests and t-tests to establish relationships between variables.
- Implemented and fine-tuned multiple machine learning algorithms for accurate predictions, focusing on mitigating overfitting.
- Developed a scalable machine learning pipeline using Python libraries like `pandas`, `scikit-learn`, and `xgboost`.
