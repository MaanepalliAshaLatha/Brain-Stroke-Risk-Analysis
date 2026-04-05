🧠 Brain Stroke Risk Analysis & Prediction

Tools: Python · Pandas · NumPy · Matplotlib · Seaborn · Scikit-learn
Dataset: Healthcare patient dataset with stroke diagnosis labels
Goal: Identify key health factors associated with stroke risk and build a predictive model

📌 Business Problem

Stroke is a medical emergency. Early identification of high-risk patients enables preventive care. This project analyses patient health data to find which factors most strongly predict stroke risk — and builds a classification model to identify at-risk individuals.

🔍 Key Findings

Age, hypertension, and glucose level are the top 3 predictors of stroke risk
Patients over 65 with hypertension and glucose > 150 mg/dL represent the highest-risk segment
The dataset is heavily imbalanced (stroke cases are rare) — handled during modelling

🛠️ Techniques Used

Data Cleaning:

Handled missing values in bmi column using median imputation
Encoded categorical variables (gender, ever_married, work_type, smoking_status) using label encoding

EDA:

Age distribution by stroke status
Glucose level vs stroke — boxplot analysis
Correlation heatmap — identified multicollinear features
Bar charts — stroke rate by gender, work type, residence type

Modelling:

Logistic Regression (baseline)
Decision Tree Classifier
Evaluated using Accuracy, Precision, Recall, F1-Score
Feature importance analysis — ranked top predictors

📊 Top Risk Factors (by feature importance)

Age
Average glucose level
Hypertension status
Heart disease history
BMI

📁 Files in this repo

File	Description
brain_stroke_analysis.ipynb	Full Jupyter notebook with EDA + models
healthcare-dataset-stroke-data.csv	Dataset
README.md	This file
