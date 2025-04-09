README: CREDIT FRAUD DETECTION

- PROJECT OVERVIEW
This project focuses on detecting fraudulent credit card transactions using machine learning. The dataset is highly imbalanced, so special care is taken during preprocessing and evaluation.

- DATASET
The dataset used is the Credit Card Fraud Detection dataset from Kaggle, which includes:
- Contains transactions made by European cardholders in September 2013.
- Features:
  - V1 to V28: PCA-transformed features
  - Amount, Time
  - Class: 0 (legit), 1 (fraud)

- TECHNOLOGIES USED
- Python
- Scikit-learn
- Pandas
- Matplotlib & Seaborn
- Imbalanced-learn (SMOTE)
- Joblib


- Exploratory Data Analysis
- Checked for duplicates and missing values
- Observed class imbalance (0: 99.8%, 1: 0.2%)

- Data Preprocessing
- Dropped duplicate rows
- Scaled Amount column using StandardScaler

- Handling Class Imbalance
- Used SMOTE to oversample the minority class (fraud)

- Model Building
- Random Forest Classifier was used as baseline
- RandomizedSearchCV used for hyperparameter tuning to reduce training time

-  Evaluation
- ROC AUC Score
- Precision-Recall Curve (AUPRC)
- Confusion Matrix & Classification Report

Due to class imbalance, AUPRC was the preferred metric.

- Performance Metrics
- ROC AUC Score: 0.91
- Precision-Recall AUC (AUPRC): 0.82

- DEPLOYMENT
- Joblib (Model Deployment)

- HOW TO RUN CODE
1. Clone the repository.
2. Install dependencies: pip install -r requirements.txt
3. Run python Credit_Fraud_Detection.ipynb to train the model.
4. Use python predict.py to make predictions.
...