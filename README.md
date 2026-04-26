<<<<<<< HEAD
# excel-stroke-risk-analysis
=======
# Excel – Exploratory Analysis of Stroke Risk Factors
**TL;DR:** 
This project analyzes stroke risk factors using Excel.
Age shows the strongest differentiation in stroke risk, with stroke prevalence increasing significantly among older age groups, especially individuals aged 80 and above. Other factors such as hypertension, heart disease, and glucose level show positive but weaker associations.

## Problem
Stroke is a major health issue influenced by multiple demographic, medical, and lifestyle factors.
This analysis aims to identify which factors differentiate stroke risk the most using exploratory data analysis (EDA), rather than building a predictive model.

## Data
- Source: [Stroke Prediction Dataset (by Fedesoriano)](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

## Business Understanding
1. Demographic Risk Factors
  <br> - Does age influence stroke risk?
  <br> - Which age groups have the highest stroke prevalence?
  <br> - Is there a difference in stroke risk by gender?
2. Medical Conditions
  <br> - Is hypertension strongly associated with stroke?
  <br> - Is heart disease associated with higher stroke risk?
3. Clinical Measurements 
  <br> - Is higher average glucose level associated with stroke?
    
## Data Understanding 
1. Imported raw CSV
2. Applied text to column
3. Converted dataset into an Excel Table
4. Checked data types and missing values
5. Identified invalid or missing BMI and age values

## Data Preparation
1. Remove Duplicates
2. Standardized data types
3. Cleaned data
4. Created calculated columns; Age Group; Glucose Level Group
5. Loaded cleaned table back to Excel

## Modelling
1. Tool: Power Query (ETL)
2. Built a single, clean analytical table
3. Standardized column names and formats
4. No Power Pivot relationships required (single-table model)

## Analysis
1. Pivot Table used to calculate: Stroke prevalence (%); Stroke distribution by age group and other factors
2. Pivot Chart
3. Slicers for dynamic filtering (gender, residence, work type, age group)
4. Column-based percentages used to compare stroke risk across groups
5. Gap analysis performed to identify factors with the largest risk difference

## Visualization
1. KPI Cards: Total Observations, % Stroke (Overall), Age Group with Highest Stroke Risk, Factor with Highest Risk Gap
2. Charts: Stroke prevalence by age group, Scatter plot (Age vs Stroke, with jitter)
3. Dashboard: Single-page Excel dashboard and Interactive slicers (Gender, Hypertension, Heart Disease)
>>>>>>> 0ee3efb (organizing folder)
