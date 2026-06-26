# Mental Health Care Data Analysis

## Overview

Mental Health Care Data Analysis is an end-to-end data analytics project that explores the relationship between lifestyle, social, and demographic factors and their impact on mental well-being. The project combines SQL for data cleaning and analysis with Power BI for interactive dashboard development, enabling users to identify patterns in anxiety, depression, stress, self-esteem, and life satisfaction.

The objective is to transform raw healthcare data into meaningful insights that support data-driven decision-making in mental health research and policy.

---

## Business Problem

Mental health is influenced by multiple interconnected factors including physical activity, sleep, financial stress, social support, and age. Organizations and healthcare professionals require analytical tools to identify these patterns and understand which factors contribute most significantly to mental well-being.

This project addresses these challenges by integrating SQL-based data preparation with Power BI dashboards for interactive analysis.

---

## Dataset Overview

The dataset contains mental health indicators collected across different demographic groups.

### Dataset Features

* Age
* Gender
* Physical Activity Hours
* Sleep Hours
* Social Support Score
* Anxiety Score
* Depression Score
* Stress Score
* Work Stress Level
* Financial Stress Level
* Self-Esteem Score
* Life Satisfaction Score
* Loneliness Score

---

## Project Objectives

* Analyze the relationship between physical activity and mental health.
* Measure the impact of work and financial stress across age groups.
* Study how social support influences anxiety and depression.
* Examine trends in self-esteem and life satisfaction.
* Build an interactive dashboard for exploratory analysis.

---

## SQL Data Preparation

The dataset was cleaned and transformed using SQL before visualization.

### Data Cleaning

* Removed unnecessary columns
* Identified duplicate records
* Checked for missing values
* Validated data types
* Standardized categorical fields
* Prepared the dataset for reporting

### Feature Engineering

Created derived columns including:

* Age Groups
* Overall Mental Health Categories
* KPI Measures
* Aggregated statistical summaries

### SQL Operations Performed

* Data Cleaning
* Filtering
* Aggregations
* CASE Statements
* GROUP BY Analysis
* HAVING Clause
* Window Functions
* KPI Calculations

---

## Sample SQL Queries

### Detect Duplicate Records

```sql
SELECT name,
       city,
       cuisine,
       COUNT(*)
FROM restaurants
GROUP BY name, city, cuisine
HAVING COUNT(*) > 1;
```

### Check Missing Values

```sql
SELECT column_name,
       COUNT(*) AS Null_Count
FROM table_name
WHERE column_name IS NULL
GROUP BY column_name;
```

### Categorize Age Groups

```sql
CASE
    WHEN age BETWEEN 18 AND 30 THEN 'Young Adults'
    WHEN age BETWEEN 31 AND 50 THEN 'Middle-aged'
    ELSE 'Seniors'
END AS Age_Group;
```

---

## Power BI Dashboard

The Power BI dashboard provides interactive visualizations for exploring mental health trends.

### Dashboard Components

* KPI Cards
* Box Plot
* Ribbon Chart
* Bar Chart
* Line Chart
* Interactive Filters
* Drill-through Analysis
* Dynamic Slicers

---

## Dashboard Insights

The dashboard allows users to analyze:

### Lifestyle Analysis

* Physical Activity vs Mental Health
* Sleep Duration vs Anxiety
* Sleep Duration vs Depression

### Stress Analysis

* Work Stress by Age Group
* Financial Stress Distribution
* Overall Stress Levels

### Psychological Well-being

* Self-Esteem Trends
* Life Satisfaction Analysis
* Loneliness Impact

### Demographic Analysis

* Age Group Comparison
* Gender-based Insights
* Mental Health Distribution

---

## Key Findings

* Individuals with higher physical activity generally reported better mental health scores.
* Strong social support was associated with lower anxiety and depression levels.
* Work and financial stress were highest among middle-aged individuals.
* Increased loneliness negatively affected self-esteem and life satisfaction.
* Mental health indicators varied significantly across demographic groups.

---

## Tools and Technologies

### Data Analysis

* SQL
* Power BI

### Data Processing

* SQL Queries
* Data Cleaning
* Feature Engineering
* Data Modeling

### Visualization

* KPI Cards
* Bar Charts
* Line Charts
* Ribbon Charts
* Box Plots
* Interactive Slicers

---

## Project Workflow

```
Dataset
     │
     ▼
SQL Data Cleaning
     │
     ▼
Feature Engineering
     │
     ▼
KPI Calculations
     │
     ▼
Power BI Data Modeling
     │
     ▼
Dashboard Development
     │
     ▼
Interactive Insights
```

---

## Repository Structure

```
Mental-Health-Care-Analysis/
│
├── Mental_Health_Care_Data.sql
├── Mental_Health.pbix
├── Dataset.csv
├── Dashboard.png
└── README.md
```

---

## Learning Outcomes

Through this project, I gained practical experience in:

* SQL Data Cleaning
* Data Validation
* Feature Engineering
* KPI Development
* Power BI Dashboard Design
* Interactive Reporting
* Data Storytelling
* Business Intelligence
* Exploratory Data Analysis

---

## Future Improvements

* Predictive Machine Learning Models
* Mental Health Risk Prediction
* Time-Series Trend Analysis
* Healthcare Recommendation Dashboard
* Real-time Data Integration

---

## Author

Mohd Anas Javed Khan

GitHub:
https://github.com/Anas-Javed362

LinkedIn:
https://www.linkedin.com/in/anas-javed-khan-4019262b6
