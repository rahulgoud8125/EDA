# Titanic Exploratory Data Analysis (EDA)
Overview
This project performs an exploratory data analysis (EDA) on the Titanic dataset. The main objectives are to summarize the data, visualize distributions and relationships, engineer new features, and extract actionable insights.

**Files**
Titanic-Dataset-1.csv — Raw Titanic passenger records

cleaned_data-1.csv — Cleaned dataset after preprocessing steps

code.py — Full Python EDA script

tit.ipynb — Jupyter/Colab notebook version

task-2.pdf — Task description and guidelines

**Steps Performed**
1. Data Loading and Cleaning

Loaded CSV using pandas

Checked column types, missing values

Dropped columns with many missing values (e.g., Cabin)

Imputed missing Age with median, filled missing Embarked

2. Summary Statistics

Calculated mean, median, standard deviation, quartiles with describe()

Used .info() for missing value summary and datatypes

3. Visualizations

Histograms and boxplots for Age, Fare, SibSp, Parch

Pairplot and correlation heatmap for numeric features

Barplots for categorical survival rates (Sex, Pclass, Embarked)

Missing value matrix (using missingno)

4. Feature Engineering

Created FamilySize = SibSp + Parch + 1

Defined IsAlone feature for passengers traveling solo

5. Pattern & Anomaly Analysis

Identified outliers (extreme values in Age and Fare)

Highlighted main data trends: right-skewed Fare, majority solo travelers, females and first class with higher survival

6. Insights

Women and first-class passengers show higher survival rates

Majority fares are low; few very high outliers

Most passengers had no relatives aboard

Weak correlations among numeric features
