# Student Performance Analysis

This project processes and analyzes various academic and personal factors to understand their impact on student exam scores.

## Dataset

The analysis is based on the **[Student Performance Factors](https://www.kaggle.com/datasets/lainguyn123/student-performance-factors)** dataset, available on Kaggle.

## Project Workflow

* **Feature Engineering:** Creates a comprehensive `Total_Study_Hours` metric by combining `Hours_Studied` and `Tutoring_Sessions`.
* **Data Cleaning:** Isolates key features (including `Attendance` and `Previous_Scores`), converts `Access_to_Resources` to numeric values using `LabelEncoder`, and drops 178 duplicate rows to ensure data quality.
* **Outlier Handling & Scaling:** Removes numerical outliers using the Interquartile Range (IQR) method and standardizes the features with `StandardScaler`.
* **Data Splitting:** Separates the dataset into an 80% training set and a 20% testing set, with `Exam_Score` as the target variable.
* **Exploratory Data Analysis (EDA):** Utilizes bar charts, boxplots, and grouped data to analyze the relationships between exam scores, average attendance, study hours, gender, and motivation levels.
