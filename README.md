
# 🚢 Titanic Dataset — Data Cleaning & Exploratory Data Analysis

**GEN AI Internship — Week 2 Assignment**

## 📋 Project Overview

This project performs comprehensive **data cleaning** and **exploratory data analysis (EDA)** on the classic Titanic dataset from Kaggle. The analysis explores relationships between variables and identifies key patterns and trends that influenced passenger survival.

## 📊 Dataset

- **Source**: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data)
- **Training Set**: 891 passengers with 12 features
- **Test Set**: 418 passengers with 11 features

### Features

| Feature | Description |
|---------|-------------|
| PassengerId | Unique identifier |
| Survived | Survival (0 = No, 1 = Yes) |
| Pclass | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name | Passenger name |
| Sex | Gender |
| Age | Age in years |
| SibSp | # of siblings/spouses aboard |
| Parch | # of parents/children aboard |
| Ticket | Ticket number |
| Fare | Passenger fare |
| Cabin | Cabin number |
| Embarked | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

## 🛠️ Setup & Installation

```bash
# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook titanic_eda.ipynb
```

## 📁 Project Structure

```
Analyser/
├── titanic/                  # Dataset
│   ├── train.csv
│   ├── test.csv
│   └── gender_submission.csv
├── titanic_eda.ipynb         # Main EDA Notebook
├── requirements.txt          # Python dependencies
└── README.md                 # This file
```

## 🔍 Analysis Sections

1. **Data Loading & Initial Inspection** — Understanding the dataset structure
2. **Missing Values Analysis** — Identifying and visualizing gaps in the data
3. **Data Cleaning** — Handling missing values with intelligent imputation
4. **Feature Engineering** — Creating new meaningful features (Title, FamilySize, AgeGroup, etc.)
5. **Univariate Analysis** — Distribution of individual variables
6. **Bivariate Analysis** — Survival rate across different categories
7. **Multivariate Analysis** — Complex relationships using heatmaps, pairplots, and faceted charts
8. **Key Findings** — Summary of discovered patterns and trends

## 📌 Key Findings

- **Gender**: Women had a significantly higher survival rate (~74%) compared to men (~19%)
- **Class**: 1st class passengers had the highest survival rate (~63%), followed by 2nd (~47%) and 3rd (~24%)
- **Age**: Children (under 10) had a higher survival rate than adults
- **Family Size**: Passengers traveling with 1-3 family members had better survival rates than those alone or in large families
- **Fare**: Higher fares strongly correlated with better survival chances
- **Embarkation**: Passengers from Cherbourg (C) had the highest survival rate

## 🧰 Technologies Used

- **Python 3.x**
- **Pandas** — Data manipulation
- **NumPy** — Numerical computing
- **Matplotlib** — Static visualizations
- **Seaborn** — Statistical visualizations
- **Jupyter Notebook** — Interactive analysis
