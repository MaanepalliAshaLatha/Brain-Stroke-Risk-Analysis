🧠 Brain Stroke Prediction Using Machine Learning (Explainable AI)<br>
<br>
Tools: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SMOTE, SHAP, CatBoost<br>
Dataset: Kaggle Stroke Prediction Dataset<br>
Goal: Build an end-to-end ML system to analyze key health factors, balance imbalanced data, compare algorithms, and deploy explainable prediction flow.<br>
<br>
📌 Project Overview<br>
<br>
Stroke occurs when blood flow to the brain stops. Early detection prevents disability and death. This project explores the Kaggle Stroke dataset using full EDA, data preprocessing, feature selection, model comparison, and explainable predictions. The workflow includes reading data, visualizing patterns, balancing classes using SMOTE, training multiple ML algorithms, and generating patient-level predictions (Normal or Stroke).<br>
<br>
📊 Exploratory Data Analysis (Based on Screens in DOCX)<br>
<br>
• Displayed dataset preview and all feature details<br>
• Visualized imbalance between "Normal" and "Stroke" cases (handled using SMOTE)<br>
• Correlation heatmap to identify highly correlated features (above 90%)<br>
• Age vs Stroke distribution<br>
• Gender differences in stroke counts<br>
• BMI vs Stroke patterns<br>
• Hypertension vs Stroke counts (1 = disease present)<br>
• Heart Disease vs Stroke counts (1 = disease present)<br>
• Glucose level charts for male/female stroke patients<br>
• Smoking status distribution among stroke cases<br>
• Residence Type (Urban / Rural) distribution<br>
<br>
🛠️ Data Preprocessing<br>
<br>
• Label Encoding for all categorical values<br>
• Normalizing numeric features<br>
• Applying SMOTE to balance Normal and Stroke classes<br>
• CHI-Square feature selection to identify important features<br>
• Splitting dataset into train and test sets<br>
<br>
🤖 Machine Learning Models Trained<br>
<br>
The following algorithms were implemented and evaluated (from screenshots in DOCX):<br>
<br>
• Random Forest — High accuracy, low misclassifications<br>
• SVM — (Used but accuracy not explicitly shown) <br>
• K-Nearest Neighbors — 92% accuracy<br>
• Naive Bayes — 77% accuracy<br>
• XGBoost — 89% accuracy<br>
• CatBoost (Extension Model) — ⭐ 95% accuracy (highest)<br>
<br>
📈 Explainable AI (XAI) with SHAP<br>
<br>
SHAP summary plot was generated to show which features contribute the most.  
Features with the highest SHAP influence:<br>
• Age<br>
• Glucose Level<br>
• Hypertension<br>
• Heart Disease<br>
• BMI<br>
<br>
🧪 Final Output (Prediction Flow)<br>
<br>
A test record is passed into the preprocessing pipeline (encoding + normalization).  
The chosen algorithm (CatBoost with 95% accuracy) predicts the label:<br>
• Output → “Normal” or “Stroke”<br>
<br>
📁 Files in This Repository<br>
<br>
• brain_stroke_analysis.ipynb — full Notebook with preprocessing, EDA, charts, and model training<br>
• healthcare-dataset-stroke-data.csv — Kaggle dataset used for analysis<br>
• README.md — documentation<br>
