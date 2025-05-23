# 📊Employee Analysis
This project performs a structured analysis of an HR dataset to uncover trends in employee turnover. Using Python and Jupyter Notebook, the analysis explores various factors such as education, city, job role, and experience in relation to employee retention.

## 📁 Dataset Overview

The dataset `Employee.csv` contains 4,653 rows and 9 columns with the following features:

- `EmployeeID`: Unique identifier for each employee
- `Education`: Employee’s educational qualification
- `City`: Geographic location of the employee
- `Gender`: Gender of the employee
- `EverBenched`: Indicates whether the employee was ever placed on bench (Yes/No)
- `ExperienceInCurrentDomain`: Number of years of experience in their current domain
- `LeaveOrNot`: Indicates if the employee stayed (0) or left (1)
- `JoiningYear`: The year the employee joined the company
- `PaymentTier`: Salary tier classification (e.g., 1 = Low, 2 = Medium, 3 = High)

## 🛠️ Tools & Libraries

- **Python** (Pandas, Matplotlib, Seaborn)
- **Jupyter Notebook** for interactive analysis
- **Visualization** with bar charts, count plots, and pie charts

## 🔍 Step-by-Step Analysis

1. **Loading and Inspecting the Dataset**
   - Loaded the CSV file using `pandas.read_csv()`
   - Checked the shape, column names, and data types
   - Used `.describe()` and `.unique()` to understand distribution and unique values

2. **Exploring Turnover Trends**
   - Grouped data by `LeaveOrNot` to compare retention vs attrition
   - Filtered and sorted to understand which segments had the highest turnover

3. **Education-Based Analysis**
   - Grouped by `Education` and `LeaveOrNot` to evaluate if education level affects attrition
   - Compared different education levels across the dataset

4. **City-Based Analysis**
   - Grouped by `City` to analyze turnover per location
   - Combined `City` and `Education` columns to understand if geography and qualification together influence turnover

5. **Bench Status and Experience Impact**
   - Analyzed how being ever benched (`EverBenched`) affects the likelihood of leaving
   - Explored the relationship between `ExperienceInCurrentDomain` and attrition

6. **Comprehensive Filtering**
   - Created filtered datasets to isolate employees who left, segmented by:
     - City
     - Education
     - Gender
     - Experience in current domain

7. **Final Visualization & Summary**
   - Summarized key findings using aggregated visual charts
   - Identified the most significant patterns influencing turnover

## 📊 Key Insights

- Turnover was higher among employees with certain education levels and from specific cities
- Employees with low domain experience or who had been benched were more likely to leave
- Geography and education combination showed interesting turnover patterns
- Gender and payment tier also provided nuanced insights into workforce stability
