# 🫁 Lung Cancer Prediction using Ensemble Learning
This project focuses on predicting lung cancer risk based on lifestyle and health-related attributes. It leverages machine learning techniques, particularly ensemble models, to improve diagnostic accuracy and understand the significance of different features in lung cancer detection.

📂 Dataset
Source: Kaggle - Lung Cancer Dataset
Attributes: The dataset includes features such as age, smoking habits, fatigue, alcohol consumption, chronic diseases, and more.
Target: LUNG_CANCER (Yes/No - encoded as binary)

🔍 Project Workflow
1. Installation
bash
Copy
Edit
pip install kagglehub scikit-learn xgboost seaborn matplotlib

3. Data Loading
Dataset is downloaded using kagglehub and loaded into a pandas DataFrame.
Columns are cleaned and formatted for consistency.

4. Preprocessing
Categorical binary columns (Yes/No) are label-encoded.
All features are scaled using StandardScaler.

4. Exploratory Data Analysis
Heatmap to understand correlation between features.
Class distribution visualization to address any imbalance.

5. Model Building
Two classifiers used:
-RandomForestClassifier
-XGBClassifier
Combined using a Voting Classifier (soft voting strategy) for improved performance.

6. Evaluation Metrics
Classification Report (Precision, Recall, F1-score)
Confusion Matrix
Heatmap
ROC AUC Score
Probability Curve

7. Feature Importance
Feature importance extracted from the Random Forest model to highlight key predictors.

📊 Results
The ensemble model demonstrates strong predictive capability with competitive ROC AUC scores.

Top contributing features include Age, Smoking, Fatigue, and Wheezing.

🧠 Technologies Used
Python (Pandas, NumPy)
scikit-learn
XGBoost
seaborn, matplotlib
kagglehub

👩‍⚕️ Use Case
This tool can assist in early identification of individuals at high risk for lung cancer, helping in timely intervention and medical evaluation.
