# HR-attrition-excel-dashboard
Excel-based HR analytics dashboard analysing attrition patterns across 1,470 employee records to identify key drivers of employee turnover and project cost-saving opportunities.

## Background

Project initiated in Power BI but migrated to Excel to leverage advanced analytical functions unavailable in the online version, including complex multi-condition logic,  custom charting configurations, and cross-sheet data modelling.

## Dataset

**Source:** IBM HR Analytics Employee Attrition & Performance dataset (publicly available via Kaggle)  
**Records:** 1,470 employees  
**Features:** 35 variables including demographics, job role, satisfaction scores, salary hike %, overtime, tenure, and attrition status

## What the Dashboard Covers

The workbook is structured across three sheets:

### Sheet 1 — KPI Summary & Trend Analysis
- Overall attrition rate: 16.12%
- Average tenure of leavers: 5.1 years
- Average job satisfaction score: 2.7
- Total headcount: 1,470 | Leavers: 237
- Attrition trend by years at company
- Attrition trend by salary hike percentage

### Sheet 2 — Departmental & Role Breakdown
- Department-wise attrition (HR, R&D, Sales)
- Job role-wise attrition breakdown
- Job level-wise attrition (levels 1–5)

### Sheet 3 — Multi-Variable Analysis
- Attrition, salary hike, and overtime trends by job role
- Departmental attrition risk segmented by job satisfaction level (Low/Medium/High/Very High)

## Key Findings

1. **Early tenure is the highest risk window** — 141 of 237 leavers had 0–4 years tenure; attrition drops sharply after 5 years
2. **Low salary hikes drive attrition** — employees receiving below 15% hike show significantly higher attrition; risk falls as hike percentage rises
3. **Sales roles carry the highest attrition rate** — Sales Representatives show the highest combined attrition rate (0.40) alongside elevated overtime exposure
4. **Job Level 1 accounts for 60% of all attrition** — entry-level employees are disproportionately at risk across all departments
5. **R&D has the largest volume but Sales has the worst rate** — 133 leavers from R&D vs 92 from Sales, but Sales is proportionally more exposed

## Methodology

- Data cleaning and transformation in Excel (Power Query)
- KPI calculation using Excel formulas and named ranges
- Logistic regression model achieving 87% accuracy to identify the 5 primary attrition drivers
- Multi-sheet dashboard with linked charts and cross-sheet references
- Visualisations: line charts, bar charts, treemap, pie chart, grouped bar chart

## Tools Used

- Microsoft Excel (Advanced — VBA, Power Query, cross-sheet modelling)
- Power BI (initial exploration)

## Files

| File | Description |
|------|-------------|
| `HR-Employee-Attrition-Final-Dashboard.xlsx` | Full dashboard workbook (3 sheets) |
