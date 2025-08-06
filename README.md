# 🧠 HR Analytics - Employee Attrition Prediction

This project explores an HR dataset to predict whether an employee is likely to leave the company using supervised machine learning models.

---

## 📌 Problem Statement

The goal is to analyze employee data and predict whether they will leave the organization (`left = 1`) or stay (`left = 0`), based on features like:
- Satisfaction level
- Last evaluation
- Number of projects
- Average monthly hours
- Time spent at the company
- Work accident history
- Promotions
- Department and salary

---

## 🧹 Steps Performed

### 1. **Exploratory Data Analysis (EDA)**
- Data inspection (`.info()`, `.describe()`, missing/duplicates check)
- Boxplots and histograms by "left" to visualize distributions
- Correlation heatmap

### 2. **Outlier Handling**
- Used 3σ (mean ± 3×std) method to cap outliers in `average_monthly_hours`, etc.

### 3. **Feature Engineering**
- Encoded categorical variables using OneHotEncoder
- Scaled numerical features using StandardScaler

### 4. **Model Building**
Tried multiple models:
- Decision Tree Classifier ✅
- Random Forest Classifier
- Logistic Regression

👉 **Final model selected:** `DecisionTreeClassifier` (best accuracy & interpretability)

### 5. **Model Evaluation**
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix
- Classification Report

---

## ✅ Results

| Metric        | Value       |
|---------------|-------------|
| Accuracy      | ~XX%        |
| Precision     | XX%         |
| Recall        | XX%         |
| F1-Score      | XX%         |

(*Replace XX with actual values*)

---

## 📁 Folder Structure

├── HR_dataset.ipynb # Main notebook
├── HR_comma_sep.csv # Dataset
└── README.md # Project summary

yaml
Copy
Edit

---

## 🛠️ Tools Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn

---

## 📈 Future Improvements
- Try ensemble models: XGBoost, CatBoost
- Add hyperparameter tuning (GridSearchCV)
- Deploy the model via Flask or Streamlit
