# Stroke Risk Factor Analysis
**Tool:** Microsoft Excel (Power Query · Pivot Table · Dashboard)  
**Domain:** Healthcare  
**Dataset:** [Stroke Prediction Dataset — Fedesoriano (Kaggle)](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)

---

## Overview

Stroke is a leading cause of disability and death worldwide. This project explores which demographic, medical, and lifestyle factors most strongly differentiate stroke risk — using exploratory data analysis (EDA) rather than predictive modeling.

The goal: **identify actionable risk signals from real patient data**, presented through an interactive Excel dashboard.

---

## Key Findings

| Factor | Insight |
|---|---|
| **Age** | Strongest differentiator. Stroke prevalence rises sharply after age 60, peaking in the 80+ group |
| **Hypertension** | Patients with hypertension show noticeably higher stroke prevalence vs. those without |
| **Heart Disease** | Positive association with stroke, though weaker than age |
| **Avg Glucose Level** | Higher glucose levels correlate with increased stroke risk |
| **Gender** | Minimal difference in stroke prevalence between male and female patients |

> Age is the single strongest risk factor in this dataset. Hypertension and high glucose are secondary signals worth monitoring in clinical screening.

---

## Dashboard

> 📸 *Screenshot dashboard menyusul — file Excel tersedia di folder `/reports`*

**Dashboard features:**
- KPI Cards: Total observations, overall stroke %, highest-risk age group, factor with largest risk gap
- Stroke prevalence by age group (column chart)
- Scatter plot: Age vs Stroke (with jitter for readability)
- Interactive slicers: Gender, Hypertension, Heart Disease, Age Group

---

## Process

**1. Data Understanding**
- Imported raw CSV, applied text-to-columns, converted to Excel Table
- Checked data types, identified missing BMI values and age anomalies

**2. Data Preparation (Power Query)**
- Removed duplicates
- Standardized data types and column names
- Cleaned invalid/missing BMI entries
- Created calculated columns: `Age Group`, `Glucose Level Group`

**3. Analysis (Pivot Table)**
- Calculated stroke prevalence (%) per factor group
- Gap analysis: identified factors with the largest difference in stroke rate between positive/negative groups
- Used column-based percentages for fair comparison across uneven group sizes

**4. Visualization**
- Single-page interactive dashboard
- Slicers for dynamic filtering across all charts

---

## Repo Structure

```
excel-stroke-risk-analysis/
├── data/
│   └── stroke_raw.csv          # Original dataset
├── reports/
│   └── stroke_analysis.xlsx    # Excel workbook (cleaned data + dashboard)
└── README.md
```

---

## Tools Used

`Microsoft Excel` `Power Query` `Pivot Table` `Pivot Chart` `Slicers`

---

## Notes

- This is an exploratory analysis — no predictive model was built
- Dataset is imbalanced (stroke cases are minority class); prevalence % is used instead of raw counts for fair comparison
- BMI missing values were removed rather than imputed to avoid introducing bias in a single-table EDA context

---

*Part of my [data portfolio](https://github.com/ramayogas/data-portofolio) — Rama Yogaswara*
