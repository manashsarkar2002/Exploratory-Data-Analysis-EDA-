# 🚢 Titanic Dataset - Exploratory Data Analysis & Feature Insights

This project explores the Titanic dataset to understand patterns in passenger survival using statistical summaries, visualizations, and feature-level inferences.

---

## 📁 Dataset

- Dataset: `Titanic-Dataset.csv`
- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data) *(classic ML classification problem)*

---

## 🛠️ Tasks Performed

### 1. Summary Statistics
- Computed **mean, median, std, min, max, quartiles** for numerical columns.
- Identified **missing values**, skewed distributions, and outliers.

### 2. Visualizations
- **Histograms & Boxplots** for numeric features: `Age`, `Fare`, `SibSp`, `Parch`
- **Correlation heatmap** to understand relationships between features
- **Survival analysis by Pclass, Sex, Age, Fare**
- Used `Seaborn` and `Matplotlib` for visuals

### 3. Patterns & Trends
- **Survival rate ≈ 38%**; Imbalanced target.
- **Women and children** had higher survival.
- **Higher class** (1st class) passengers survived more.
- **Fare** and **Pclass** are inversely related; higher fare → better survival.
- **Small families** (1–3 members) had higher survival than solo or large groups.

---

## 🔎 Feature-Level Inferences

| Feature     | Insight |
|-------------|---------|
| `Sex`       | Strong predictor. Females had higher survival. |
| `Pclass`    | 1st class survived most; 3rd class the least. |
| `Age`       | Children had high survival. Missing values need treatment. |
| `Fare`      | Higher fares → better survival. Strong outliers. |
| `SibSp` / `Parch` | Small families helped survival; large ones didn’t. |
| `Embarked`  | Mostly 'S', with few missing. Slight influence on survival. |

---

## ⚠️ Anomalies & Issues

- `Age` has ~20% missing values.
- `Cabin` is mostly missing — can be dropped or bucketed.
- `Fare` has outliers and some passengers paid 0 — worth further inspection.

---

## 📦 Requirements

- Python 3.8+
- Libraries:
  - pandas
  - matplotlib
  - seaborn

Install them using:
```bash
pip install pandas matplotlib seaborn
