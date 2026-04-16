# ❤️ Heart Disease Prediction using Machine Learning

<img src="https://i.postimg.cc/Vvbhnscg/Heart-Disease.png" width="300">

## 🧠 Problem Statement

The goal of this project is to develop a machine learning model that predicts whether a patient has heart disease based on medical attributes.

---

## 📊 Dataset

The dataset contains medical information of patients such as age, cholesterol level, chest pain type, etc.

* Target Variable:

  * `0` → No Heart Disease
  * `1` → Heart Disease

---

## 📂 Project Workflow

1. Data Loading
2. Data Understanding
3. Exploratory Data Analysis (EDA)
4. Data Splitting
5. Model Training (Decision Tree)
6. Model Evaluation
7. Cross Validation
8. Hyperparameter Tuning (GridSearchCV)
9. Final Model Selection
10. Feature Importance Analysis

---

## 📊 Exploratory Data Analysis

* Histogram analysis to understand feature distributions
* Countplot to check target balance
* Pairplot to analyze relationships between features
* Correlation heatmap to identify feature relationships

---

## ⚙️ Model Used

* Decision Tree Classifier

---

## 🔧 Hyperparameter Tuning

GridSearchCV was used with cross-validation to find the best parameters:

* max_depth
* min_samples_split
* min_samples_leaf

Multiple metrics were evaluated:

* Accuracy
* Precision
* Recall
* F1 Score

Final model was selected based on **Recall**.

---

## 📈 Model Evaluation

The model was evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

👉 Recall was prioritized to ensure correct detection of heart disease cases.

---

## 🌳 Decision Tree Visualization

The trained decision tree was visualized to understand how features influence predictions.

<img src="https://i.postimg.cc/0Qm5nwDY/Heart-Disease-Decision-Tree.png" width="300">

---

## 📊 Feature Importance

Feature importance was extracted to identify the most influential features in predicting heart disease.

---

## 🔤 Column Encoding Details

The dataset contains both numerical and encoded categorical features:

* `sex` → 0: Female, 1: Male

* `cp` (Chest Pain Type):

  * 0: Typical Angina
  * 1: Atypical Angina
  * 2: Non-anginal Pain
  * 3: Asymptomatic

* `fbs` (Fasting Blood Sugar):

  * 0: ≤ 120 mg/dl
  * 1: > 120 mg/dl

* `restecg` (ECG Results):

  * 0: Normal
  * 1: ST-T abnormality
  * 2: Left ventricular hypertrophy

* `exang` (Exercise-induced angina):

  * 0: No
  * 1: Yes

* `slope`:

  * 0: Upsloping
  * 1: Flat
  * 2: Downsloping

* `ca` → Number of major vessels (0–3)

* `thal`:

  * 1: Normal
  * 2: Fixed defect
  * 3: Reversible defect

---

## 💡 Key Insights

* Chest pain type and number of vessels are strong indicators of heart disease
* Age and cholesterol also influence predictions
* The dataset is balanced, enabling fair model learning
* Hyperparameter tuning improved model performance

---

## 🎯 Conclusion

A Decision Tree model was successfully built and optimized to predict heart disease.
The model performs well and prioritizes recall, making it suitable for medical prediction tasks where detecting disease cases is critical.

---

## 🚀 Future Improvements

* Try Random Forest and other ensemble models
* Perform feature engineering
* Deploy the model using Flask/Streamlit
* Use more advanced evaluation techniques