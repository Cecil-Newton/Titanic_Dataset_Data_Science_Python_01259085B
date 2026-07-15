# Titanic Data Science Project — BCS 404

**Course:** BCS 404 — Introduction to Data Science with Python
**Institution:** Accra Technical University, Department of Computer Science
**Lecturer:** Dr. Joseph Dadzie
**Academic Year:** 2025/2026, Second Semester

## Project Overview

This project applies a full data science workflow — data acquisition, cleaning,
exploratory visualisation, statistical analysis, and machine learning — to the
Kaggle Titanic dataset, in order to explore and predict passenger survival aboard
the RMS Titanic.

## Repository Contents

| File | Description |
|---|---|
| `Titanic_Data_Science_Project.ipynb` | Main Jupyter Notebook containing all analysis code, outputs, and inline interpretations (Tasks 1–5). |
| `CPS_Data_Science_Project_Report.docx` / `.pdf` | Full written project report (cover page, ToC, introduction, methodology, results, discussion, conclusion, references, code appendix). |
| `titanic.csv` | Titanic passenger dataset (same schema as Kaggle's `train.csv`, 891 rows × 12 columns). |
| `figures/` | All exported chart images (histogram, bar chart, boxplot, scatter plot, correlation heatmap, pairplot, confusion matrix). |
| `README.md` | This file. |

## How to Run

1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
2. Launch Jupyter:
   ```bash
   jupyter notebook Titanic_Data_Science_Project.ipynb
   ```
3. Run all cells top to bottom (`Kernel > Restart & Run All`).

## Summary of Key Results

- **Dataset:** 891 passengers, 12 original columns; `Age` (19.9%), `Cabin` (77.1%),
  and `Embarked` (0.2%) contained missing values.
- **Cleaning:** `Age` imputed with median, `Embarked` imputed with mode, `Cabin`
  dropped due to excessive missingness. No duplicate rows found.
- **Strongest correlations with survival:** `Pclass` (-0.338, strongest negative),
  `Fare` (+0.257, strongest positive).
- **Machine Learning:** Logistic Regression classifier trained on 7 features
  (Pclass, Sex, Age, SibSp, Parch, Fare, Embarked) achieved **80.45% accuracy**
  on the test set (vs. a 61.6% baseline).

## Dataset Source

Kaggle — Titanic: Machine Learning from Disaster
https://www.kaggle.com/competitions/titanic/data

## Author

[Bright Newton Gawugah] — [01259085B]
