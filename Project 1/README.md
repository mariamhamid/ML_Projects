Titanic Survival Prediction 🚢
🎯 Objective

Build, optimize, and compare machine learning models to predict whether a passenger survived the Titanic disaster based on their attributes. This project demonstrates feature engineering, pipeline creation, model training, hyperparameter tuning, and evaluation using multiple classifiers.

📊 Dataset

The project uses the Titanic Survival Dataset from Kaggle.

Dataset link: https://www.kaggle.com/competitions/titanic/data

Target variable: survived

1 → passenger survived

0 → passenger did not survive

Selected features:

pclass, sex, age, sibsp, parch, fare, class, who, adult_male, alone

🔑 Key Steps
1. Data Splitting

The dataset is split into training and testing sets

Stratification is applied to handle slight class imbalance in the target variable

2. Feature Preprocessing

Separate pipelines for numerical and categorical features

ColumnTransformer is used to combine the pipelines into a unified preprocessing step

3. Model Pipeline Creation

A Pipeline is created combining the preprocessor with a classifier

Initial classifier: RandomForestClassifier

4. Model Training & Optimization

GridSearchCV is used with Stratified K-Fold (cv=5)

Hyperparameters of the classifier are tuned for optimal performance

5. Evaluation

Performance metrics:

Accuracy

Precision

Recall

Confusion Matrix

Evaluated on unseen test data

6. Model Comparison

The classifier in the pipeline is replaced with LogisticRegression

Performance is compared to Random Forest to determine the most effective model

🛠️ Tech Stack

Programming Language: Python

Libraries: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib

✅ Outcome

Successfully built and optimized two classification models

Logistic Regression showed a slight performance edge over Random Forest

Demonstrates the importance of:

Feature preprocessing pipelines

Hyperparameter tuning

Understanding model predictions and performance comparison