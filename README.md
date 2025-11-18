// ...existing code...
# Titanic Exploratory Data Analysis (EDA) 🛳️

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)](https://jupyter.org/)

---

## Project Overview
This project performs a **comprehensive Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns related to passenger survival. Using statistical summaries and visualizations, the analysis identifies key factors that influenced survival probability.

**Dataset:** [Titanic Dataset (Data Science Dojo GitHub)](https://raw.githubusercontent.com/datasciencedojo/datasets/refs/heads/master/titanic.csv)

---

## Dataset Description

| Column      | Description |
|------------|-------------|
| PassengerId | Unique identifier for each passenger |
| Survived    | Survival status (0 = No, 1 = Yes) |
| Pclass      | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name        | Passenger name |
| Sex         | Passenger gender |
| Age         | Passenger age in years |
| SibSp       | Number of siblings/spouses aboard |
| Parch       | Number of parents/children aboard |
| Ticket      | Ticket number |
| Fare        | Passenger fare |
| Cabin       | Cabin number (dropped due to missing values) |
| Embarked    | Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## Project Tasks

### Task 1: Data Loading and Inspection
- Loaded the dataset using `pandas`.
- Checked the first 5 rows, column types, descriptive statistics, and missing values.

### Task 2: Handling Missing Values
- **Cabin:** Dropped (>75% missing).  
- **Embarked:** Imputed missing values with mode (most frequent port).  
- **Age:** Imputed missing values with median age.

### Task 3: Univariate Analysis
- **Survived:** ~38% of passengers survived.  
- **Pclass:** 3rd class had the most passengers.  
- **Age:** Histogram shows a right-skewed distribution.

### Task 4: Bivariate and Multivariate Analysis
- **Survival by Sex:** Females had a higher survival rate.  
- **Survival by Pclass:** Higher classes had better survival chances.  
- **Survival by Age:** Children survived more often; elderly less often.  
- **Survival by Embarked:** Cherbourg passengers slightly favored survival.

### Task 5: Conclusions and Insights
- **Top Predictors of Survival:** Sex, Pclass, and Age.
- Females, first-class passengers, and children had higher survival probabilities.
- Port of Embarkation (Cherbourg) had a minor influence.
- Social hierarchy, gender, and age were the strongest factors influencing survival.

---

## Methodology
1. **Data Cleaning:** Handled missing values and removed irrelevant columns.  
2. **Exploratory Analysis:** Performed univariate, bivariate, and multivariate analysis using `pandas`, `matplotlib`, and `seaborn`.  
3. **Visualization:** Count plots, bar charts, histograms, and KDE plots were used to interpret patterns.

---

## Libraries Used
- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  

---

## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/Rezaul33/Titanic-Exploratory-Data-Analysis-EDA
```
2. Use the following command in Terminal:
```
pip install -r requirements.txt
```
3. Open the Jupyter Notebook:
```bash
jupyter notebook Titanic_EDA.ipynb
```
4. Run all cells sequentially to reproduce the analysis and visualizations.

---

## Folder Structure
```
Titanic-Exploratory-Data-Analysis-EDA
├── Titanic_EDA.ipynb
├── README.md
├── requirments.txt
└── plots/
    ├── survival_count_plot.png
    ├── pclass_distribution.png
    ├── age_histogram.png
    ├── survival_by_sex.png
    ├── survival_by_pclass.png
    ├── survival_by_age.png
    └── survival_by_embarked.png

```

---
