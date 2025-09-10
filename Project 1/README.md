<h1 style="font-size:55px; text-align:center; font-weight:bold;">🚢 Titanic Survival Prediction</h1>

---

<h2 style="font-size:35px; font-weight:bold;">🎯 Objective</h2>
<p style="font-size:25px;">
Build and optimize a machine learning model to predict whether a passenger survived the sinking of the Titanic based on their attributes.  
The project compares the performance of a <b>Random Forest Classifier</b> and a <b>Logistic Regression</b> model.
</p>

---

<h2 style="font-size:35px; font-weight:bold;">📊 Dataset</h2>
<p style="font-size:25px;">
<b>Source:</b> Titanic Survival Dataset (from the Seaborn library / Kaggle equivalent).  
<b>Target variable:</b> <code>survived</code>  
- <code>1</code> → Passenger survived  
- <code>0</code> → Passenger did not survive  
</p>

---

<h2 style="font-size:35px; font-weight:bold;">🔑 Key Steps</h2>

<h3 style="font-size:28px; font-weight:bold;">1. Select Features</h3>
<p style="font-size:25px;">
Features: <code>pclass</code>, <code>sex</code>, <code>age</code>, <code>sibsp</code>, <code>parch</code>, <code>fare</code>, <code>class</code>, <code>who</code>, <code>adult_male</code>, <code>alone</code>  
Target: <code>survived</code>  
</p>

<h3 style="font-size:28px; font-weight:bold;">2. Split Data</h3>
<p style="font-size:25px;">
Training & testing sets  
Stratification applied for class imbalance  
</p>

<h3 style="font-size:28px; font-weight:bold;">3. Define Preprocessing</h3>
<p style="font-size:25px;">
<b>Numerical pipeline:</b> imputation (median) + scaling  
<b>Categorical pipeline:</b> imputation (most frequent) + one-hot encoding  
Combined with <b>ColumnTransformer</b>  
</p>

<h3 style="font-size:28px; font-weight:bold;">4. Create Model Pipeline</h3>
<p style="font-size:25px;">
Preprocessor + classifier in a single pipeline  
Initial model: <b>RandomForestClassifier</b>  
</p>

<h3 style="font-size:28px; font-weight:bold;">5. Train & Optimize</h3>
<p style="font-size:25px;">
<b>GridSearchCV</b> with <b>StratifiedKFold (cv=5)</b> for hyperparameter tuning  
</p>

<h3 style="font-size:28px; font-weight:bold;">6. Evaluate Performance</h3>
<p style="font-size:25px;">
Metrics: precision, recall, F1, accuracy  
Confusion matrix visualization  
</p>

<h3 style="font-size:28px; font-weight:bold;">7. Compare Models</h3>
<p style="font-size:25px;">
Logistic Regression vs. Random Forest  
Performance compared side by side  
</p>

---

<h2 style="font-size:35px; font-weight:bold;">🛠️ Tech Stack</h2>
<p style="font-size:25px;">
- Python 🐍  
- Pandas  
- NumPy  
- Scikit-learn  
- Seaborn  
- Matplotlib  
</p>

---

<h2 style="font-size:35px; font-weight:bold;">✅ Outcome</h2>
<p style="font-size:20px;">
- Built & optimized <b>Random Forest</b> and <b>Logistic Regression</b> models  
- Logistic Regression showed a slight performance edge. 
 Project highlights:
  Importance of preprocessing pipelines,  
   Different model interpretations of features, 
   Value of hyperparameter tuning & evaluation metrics  
</p>

Feature preprocessing pipelines

Hyperparameter tuning

Understanding model predictions and performance comparison
