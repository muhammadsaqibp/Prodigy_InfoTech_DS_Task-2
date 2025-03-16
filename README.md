# Prodigy_InfoTech_DS_Task-2
## Titanic Data Exploration

## Overview
This project involves performing **data cleaning** and **exploratory data analysis (EDA)** on the Titanic dataset from [Kaggle](https://www.kaggle.com/c/titanic/data). The main objective is to uncover patterns and relationships between passenger attributes—such as age, gender, fare, and class—and their survival outcomes.

## Table of Contents
1. [Dataset](#dataset)  
2. [Project Steps](#project-steps)  
   - [Step 1: Importing Libraries and Loading the Dataset](#step-1-importing-libraries-and-loading-the-dataset)  
   - [Step 2: Data Exploration and Cleaning](#step-2-data-exploration-and-cleaning)  
   - [Step 3: Data Analysis](#step-3-data-analysis)  
   - [Step 4: Data Visualization](#step-4-data-visualization)  
3. [Conclusions](#conclusions)  
4. [References](#references)

---

## Dataset
- **Source**: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic/data)  
- **Description**: Contains passenger data including survival status, passenger class (Pclass), name, sex, age, number of siblings/spouses aboard (SibSp), number of parents/children aboard (Parch), ticket number, fare, cabin number, and port of embarkation.

---

## Project Steps

### Step 1: Importing Libraries and Loading the Dataset
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, etc.
- **Dataset**: Loaded the CSV file into a Pandas DataFrame.
- **Initial Inspection**: Used methods like `df.head()`, `df.info()`, and `df.describe()` to understand the data structure and identify potential data quality issues.

### Step 2: Data Exploration and Cleaning
1. **Check for Missing Data**  
   - Identified missing values in columns like `Age`, `Cabin`, and `Embarked`.
   - Summarized the count of missing data for each column.
2. **Handle Missing Data**  
   - Imputed `Age` using either the median or mean based on distribution.
   - Dropped `Cabin` or performed feature engineering if feasible.
   - Filled `Embarked` with the most common port or another appropriate strategy.
3. **Data Types and Outliers**  
   - Converted columns (e.g., `Survived`, `Pclass`) to categorical where appropriate.
   - Examined outliers in `Fare` and `Age`.

### Step 3: Data Analysis
1. **Survival Rate**  
   - Calculated the overall survival rate and examined the distribution of survivors vs. non-survivors.
2. **Passenger Class Analysis**  
   - Explored how survival rates vary across the three passenger classes.
   - Investigated how class correlates with fare and age.
3. **Gender Analysis**  
   - Compared survival rates between males and females.
   - Explored interactions between gender and passenger class.
4. **Age Analysis**  
   - Examined average age among survivors and non-survivors.
   - Checked whether children had a higher survival rate.

### Step 4: Data Visualization
1. **Age Distribution**  
   - Created histograms or KDE plots to show the distribution of passenger ages.
2. **Fare Distribution**  
   - Visualized fare data using histograms and box plots to detect skewness and outliers.
3. **Correlation Heatmap**  
   - Showed how features like `Age`, `Fare`, `Pclass`, and `Survived` correlate with one another.
4. **Bar Charts & Pie Charts**  
   - Demonstrated survival counts by gender, class, and embarkation point.

---

## Conclusions
- **Key Predictors**: Passenger class, gender, and age significantly impact survival chances.  
- **Data Quality**: Missing data in `Age` and `Cabin` required careful handling.  
- **Insights**:  
  - **Females** and **upper-class** passengers generally had better survival rates.  
  - **Younger passengers** (especially children) showed higher survival probabilities.  
- **EDA Outcome**: These findings can inform further predictive modeling or deeper investigations into passenger behavior and rescue operations.

---

## References
- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)  
- [Pandas Documentation](https://pandas.pydata.org/docs/)  
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)  
- [Seaborn Documentation](https://seaborn.pydata.org/)  

---

**Thank you for checking out this Titanic EDA project!**  
Feel free to explore the notebooks in this repository for more details on the code and analysis.
