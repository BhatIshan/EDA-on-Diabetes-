# Diabetes Data Analysis Project

## Overview
This project is an **Exploratory Data Analysis (EDA) and statistical analysis** of a diabetes dataset (commonly known as the *Pima Indians Diabetes Dataset*). The goal is to understand the relationships between medical attributes (such as glucose, BMI, age, insulin, etc.) and the **diabetes outcome**, while applying real-world data cleaning, visualization, and basic statistical inference techniques.

This project focuses on **data understanding and insights**, not machine learning model building.

---

## Dataset Description
The dataset contains medical diagnostic measurements for individuals along with a binary outcome variable indicating diabetes presence.

### Key Features
- **Pregnancies** – Number of pregnancies
- **Glucose** – Plasma glucose concentration
- **BloodPressure** – Diastolic blood pressure (mm Hg)
- **SkinThickness** – Triceps skin fold thickness (mm)
- **Insulin** – 2-Hour serum insulin (mu U/ml)
- **BMI** – Body Mass Index
- **DiabetesPedigreeFunction** – Genetic influence score
- **Age** – Age in years
- **Outcome** – 0 (Non-diabetic), 1 (Diabetic)

---

## Project Workflow

### 1. Importing Required Libraries
- NumPy
- Pandas
- Matplotlib & Seaborn
- SciPy
- Plotly (for interactive visualizations)

---

### 2. Data Loading and Initial Exploration
- Loaded the dataset using `pandas.read_csv()`
- Viewed sample records
- Checked dataset shape, data types, and basic statistics

---

### 3. Descriptive Statistics
- Mean, median, standard deviation, minimum, and maximum values
- Helped identify unrealistic values (e.g., zeros in medical features)

---

### 4. Skewness Analysis
- Checked skewness of numerical features
- Identified features with non-normal distributions

---

### 5. Missing Value Identification
- Zero values in features like **Glucose, BloodPressure, SkinThickness, Insulin, and BMI** were treated as missing values

---

### 6. Handling Missing Values
- Applied **median imputation** to replace missing values
- Median chosen due to robustness against outliers

---

### 7. Outlier Detection and Handling
- Used **Interquartile Range (IQR)** method
- Identified and treated extreme values to reduce noise

---

### 8. Correlation Analysis & Feature Selection
- Created a **correlation heatmap**
- Identified strongly correlated features
- Observed that **BMI and SkinThickness** have a strong positive correlation
- Redundant features were considered for removal

---

### 9. Data Visualization

#### Distribution Analysis
- Histogram of **Glucose levels** grouped by diabetes outcome
- Diabetic individuals show higher glucose concentrations

#### Relationship Analysis
- **BMI vs Age (Scatter Plot)**
- **BMI vs Glucose by Outcome (Facet Grid)**

Key observations:
- Higher BMI and glucose levels are more common among diabetic individuals
- Age alone is not a sufficient predictor

---

### 10. Statistical Inference

#### Confidence Interval
- Constructed confidence intervals for glucose levels

#### Hypothesis Testing
- Performed **one-sample t-test**
- Tested whether mean glucose level significantly differs from zero
- Result: Null hypothesis rejected, indicating statistically significant glucose levels

---

## Key Insights
- Glucose is the strongest indicator of diabetes
- BMI and age contribute but are not decisive alone
- Data preprocessing (handling missing values & outliers) is critical before analysis
- Statistical tests support visual findings

---

## Technologies Used
- Python
- Jupyter Notebook
- Pandas, NumPy
- Matplotlib, Seaborn, Plotly
- SciPy

---

## How to Run the Project
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scipy plotly
   ```
3. Open the Jupyter Notebook
4. Run cells sequentially

---

## Project Type
**Exploratory Data Analysis (EDA) & Statistical Analysis**

---

## Author
Ishan Bhat

---

## Future Improvements
- Add machine learning models (Logistic Regression, Random Forest)
- Perform feature scaling and cross-validation
- Deploy insights using a dashboard
