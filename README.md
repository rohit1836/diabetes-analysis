# diabetes-analysis

Diabetes Prediction using Random Forest
📄 Project Overview
This project focuses on predicting whether an individual is diabetic based on key health parameters such as HbA1c levels, fasting blood glucose, BMI, waist circumference, and blood pressure.
We utilized a Random Forest Classifier to build a robust and interpretable machine learning model for binary classification: Diabetic (Yes/No).

## 🗂️ Dataset
The dataset (diabetes_dataset.csv) contains various health and demographic features.
Key features:

- HbA1c (%)
- Fasting Blood Glucose (mg/dL)
- BMI (Body Mass Index)
- Waist Circumference (cm)
- Blood Pressure (Systolic and Diastolic)
- Sex
- Previous Gestational Diabetes
- Smoking and Alcohol Consumption Habits

#### Target Variable:
- Diabetic (0 = No, 1 = Yes)
- Derived based on health risk conditions (4 or more risk factors present = Diabetic).

## Methodology

### Data Cleaning
- Removed irrelevant columns (Unnamed: 0, Ethnicity).
- Filled missing values in Alcohol_Consumption with 'Unknown'.
- Converted categorical variables into numerical format using One-Hot Encoding.

### Feature Engineering
- Created a new binary target feature Diabetic based on health risk thresholds.

### Model Training
- Split data into training and testing sets.
- Trained a Random Forest Classifier on the processed data.

### Model Evaluation
#### Evaluated model performance using:
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)
- ROC-AUC Score

## 📈 Results
#### The Random Forest Classifier achieved strong performance metrics:
High Precision and Recall in detecting diabetic cases.
ROC-AUC Score indicating excellent model discrimination ability.

