# Titanic Dataset - Exploratory Data Analysis (EDA)

## Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns and relationships that influenced passenger survival.  
We analyze **numerical and categorical variables**, clean missing data, and visualize trends.

---

## Dataset
The dataset is the Titanic **train.csv**

Key columns:
- `Survived` → Target variable (0 = No, 1 = Yes)
- `Pclass` → Passenger class (1 = First, 3 = Third)
- `Sex` → Gender
- `Age` → Age in years
- `SibSp` → Number of siblings/spouses aboard
- `Parch` → Number of parents/children aboard
- `Fare` → Ticket fare
- `Embarked` → Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

---

##  Steps Performed

### 1️⃣ Data Loading & Inspection
- Loaded CSV using `pandas`.
- Checked data structure, types, and missing values.

### 2️⃣ Data Cleaning
- Filled missing **Age** with **median** (less sensitive to outliers).
- Filled missing **Embarked** with **mode** (most common category).
- Dropped **Cabin** due to too many missing values.
- Converted `Sex`, `Embarked`, and `Pclass` to `category` type for efficiency.

### 3️⃣ Univariate Analysis
- **Histograms** for Age and Fare distributions.
- **Count plots** for categorical variables like Sex and Pclass.

### 4️⃣ Bivariate Analysis
- Survival rate comparisons by Sex, Pclass, Age groups, and Fare.
- **Boxplots** and **barplots** to visualize differences.
- **Correlation heatmap** for numerical variables.

### 5️⃣ Multivariate Analysis
- Grouped survival rates by multiple factors (e.g., Pclass + Sex).
- Used **pairplots** to see trends between numerical features.

---

##  Key Insights
- **Gender**: Females had a much higher survival rate than males.
- **Class**: 1st-class passengers survived more often than 3rd-class passengers.
- **Fare**: Higher fares were associated with higher survival rates.
- **Age**: Median ages were similar for survivors and non-survivors, but young children tended to have better odds.
- **Family Size**: Moderate family sizes had slightly better survival than passengers traveling alone or in very large groups.
