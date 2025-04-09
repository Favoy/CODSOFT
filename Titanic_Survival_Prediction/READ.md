README: TITANIC SURVIVAL PREDICTION

- PROJECT OVERVIEW
This project aims to predict passenger survival on the Titanic using machine learning. The dataset includes passenger details such as age, **gender, class, and ticket fare. I applied data preprocessing, feature engineering, model training, and hyperparameter tuning to improve predictions.

- DATASET
The dataset used is the Titanic dataset from Kaggle, which includes:
- Passenger Details: Age, Sex, Class, Fare, etc.
- Target Variable: Survived (1 = Survived, 0 = Did Not Survive)

- TECHNOLOGIES USED
- Python
- Pandas, NumPy (Data Handling)
- Matplotlib, Seaborn (Visualization)
- Scikit-Learn (Machine Learning)
- XGBoost (Advanced Modeling)
- Joblib (Model Deployment)

- DATA PREPROCESSING
1. Handled missing values in Age and Embarked.
2. Encoded categorical variables (Sex, Embarked).
3. Scaled numerical features (Age, Fare).

- MODEL SELECTION AND TUNING
- These models were tested : Random Forest, Logistic Regression, SVM, and XGBoost.
- GridSearchCV was used for hyperparameter tuning.

- RESULT
- Best model: Random Forest with an accuracy of 82.12%.
- Feature importance shows Sex, Age and Fare are strong predictors.

- DEPLOYMENT
- Model saved using joblib.dump() for reuse.
- Can be deployed via a Flask API.

- HOW TO RUN CODE
1. Clone the repository.
2. Install dependencies: pip install -r Requirements File.txt
3. Run python Titanic_Survival_Prediction.ipynb to train the model.
4. Use python predict.py to make predictions.



