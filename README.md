# 🎓 Student Grade Classification using Machine Learning

This project uses machine learning techniques to classify students' performance levels (grades) based on various academic and behavioral indicators. The dataset contains multiple features and the goal is to predict the final `GRADE` of students.

---

## 📁 Dataset

- **Source:** `DATA (1).csv`
- **Target Variable:** `GRADE` (categorical)
- **Input Features:** Academic scores, attendance, assignment marks, etc.
- **Removed Columns:** `STUDENT ID` (irrelevant to prediction)

---

## 📊 Exploratory Data Analysis

- Checked for **missing values** and **data types**
- Analyzed **correlation** between features and the target (`GRADE`)
- Visualized important feature correlations using Seaborn bar plots

---

## 📉 Dimensionality Reduction

- **Standardized** features using `StandardScaler`
- Applied **PCA (Principal Component Analysis)** to reduce dimensionality
  - Retained components explaining **95% variance**
  - Visualized PCA results

---

## 🤖 Machine Learning Models

A total of **7 supervised classification models** were trained and compared:

| Model                | Description                    |
|---------------------|--------------------------------|
| Logistic Regression | Baseline linear model          |
| Decision Tree       | Tree-based model               |
| Random Forest       | Ensemble of decision trees     |
| SVC (SVM)           | Support Vector Classifier      |
| Gradient Boosting   | Boosted decision trees         |
| Bagging Classifier  | Bagging ensemble model         |
| Naive Bayes         | Probabilistic classifier       |

Each model was evaluated:
- On **original features**
- On **PCA-reduced features**

Metric used: **Accuracy Score**

---

## 📈 Results

- Accuracy scores were stored for both original and PCA-transformed datasets.
- Comparison reveals which model performs best and whether PCA improved classification.

---

## 📦 Requirements

Install the following Python packages before running:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
