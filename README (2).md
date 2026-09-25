# HR Employee Attrition Analysis

A data analytics project analyzing employee attrition patterns using Python, Excel, and Power BI, built as part of a B.Tech Artificial Intelligence & Data internship submission.

## Problem Statement

Organizations lose valuable employees every year, and high attrition increases hiring and training costs. This project analyzes historical employee data — department, job role, salary, experience, satisfaction, and overtime — to identify where and why attrition happens, giving HR teams a clearer picture of workforce patterns.

## Objective

- Identify which employees are more likely to leave
- Compare attrition rates across departments and job roles
- Understand the impact of overtime, salary, experience, and satisfaction on attrition
- Build an interactive dashboard for HR decision-makers

## Tools Used

| Tool | Purpose |
|------|---------|
| Excel | Initial data check and formatting |
| Python (Pandas) | Data cleaning, feature engineering, exploratory analysis |
| Power BI | Interactive dashboard and visualization |

## Dataset

IBM HR Analytics Employee Attrition Dataset — 1,470 employees, 35 features including department, job role, income, satisfaction scores, and attrition status.

## Data Cleaning & Preparation

- Checked for missing values (none found)
- Removed constant/uninformative columns: `EmployeeCount`, `Over18`, `StandardHours`
- Converted categorical `Attrition` and `OverTime` columns into numeric flags for analysis
- Created grouped features: `AgeGroup`, `SalaryRange`, `ExperienceLevel` for clearer comparisons

## Key Findings

- **Overall attrition rate:** 16.1% (237 of 1,470 employees)
- **Overtime is the strongest driver:** employees working overtime leave at **30.5%** vs **10.4%** for those who don't — nearly 3x higher
- **Department differences:** Sales (20.6%) and HR (19.0%) show higher attrition than R&D (13.8%)
- **Job role risk:** Sales Representative has the highest attrition at **39.8%**, far above senior roles like Manager (4.9%) and Research Director (2.5%)
- **Age:** youngest employees (18–25) leave at **34.8%**, dropping steadily with age
- **Salary:** lowest salary band shows **28.6%** attrition vs **8.9%** in the highest band
- **Experience:** entry-level employees (0–5 years) leave at **28.8%** vs **8.7%** for veterans (16+ years)
- **Job satisfaction:** lowest satisfaction level shows **22.8%** attrition vs **11.3%** at the highest level

## Dashboard

![Dashboard](dashboard/screenshot.png)

The Power BI dashboard includes:
- KPI cards for total employees, attrition count, attrition rate, and average salary
- Department and job role comparisons with drill-down
- Breakdown by overtime, salary range, experience level, and satisfaction
- A scatter plot relating age, income, and attrition
- Interactive filters for department, job role, gender, and experience

## Repository Structure

```
├── data/            # Dataset (or source link if not included)
├── notebook/         # Python analysis (Jupyter/Colab notebook)
├── dashboard/        # Power BI file (.pbix) and dashboard screenshot
├── presentation/      # Project presentation (PPTX)
└── README.md
```

## Future Scope

Build a machine learning model (e.g., Logistic Regression or Decision Tree) to predict attrition risk for individual employees, using the features identified in this analysis as predictors.
