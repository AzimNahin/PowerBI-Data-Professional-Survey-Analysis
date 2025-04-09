# 📊 Data Professional Survey Analysis (Power BI + Excel)

This project explores survey responses from data professionals around the world. Built entirely in **Power BI**, the analysis provides insights into salary trends, career challenges, demographics, and programming preferences among individuals working in data-focused roles.
---

## 📌 Project Summary

The dataset includes responses from **630 individuals**, capturing:
- Job titles and salaries
- Career transition status
- Work satisfaction metrics
- Programming language preferences
- Perceptions on entering the data field
- Demographic info: age, gender, country, education, ethnicity

All data was cleaned and modeled using **Power Query** in Power BI before building the final dashboard.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Data Professional Survey.xlsx` | Raw dataset used for analysis |
| `Data Professional Survey Analysis.pbix` | Power BI file with queries, model, and visuals |
| `Data Professional Survey Dashboard.jpg` | Exported snapshot of the dashboard |

---

## 🧹 Data Processing in Power BI (Power Query)

The raw survey data was cleaned and transformed using Power Query in Power BI. The following steps were applied:

### 🗃️ Columns Removed
Only non-essential metadata fields were dropped to reduce clutter:
- `Browser`, `OS`, `City`, `Country`, `Referrer`

### 🔁 Column Transformations
- **Job Title**, **Programming Language**, **Industry**, and **Country** columns included extra text (e.g., in parentheses). These were split and simplified by removing text after the delimiter `"("`
- A new column **`Average Salary`** was derived from the raw salary range:
  - Split ranges like `"50k - 70k+"` into low and high parts
  - Removed suffixes like `k`, `+`, `-`
  - Converted to numeric and averaged both ends to estimate salary

### 🔢 Data Type Conversions
- Converted string-based numeric fields (`Age`, happiness ratings, salary values) into proper number formats for accurate aggregation
- Converted date and time fields but excluded them from visualizations

The resulting dataset contains **23 cleaned and analysis-ready columns**, optimized for dashboard reporting.

---

## 📊 Dashboard Features

The dashboard presents several key visualizations:

### 1. **Average Salary by Job Title**
- Highest: **Data Scientist**
- Lowest: **Student/Entry Roles**

### 2. **Favorite Programming Language**
- Top language: **Python**
- Others include R, SQL, C++, and JavaScript

### 3. **Respondent Demographics**
- Largest respondent base: **United States** and **India**
- Average respondent age: **29.87**

### 4. **Career Transition and Difficulty**
- Donut chart showing ease or difficulty of breaking into data

### 5. **Satisfaction Gauges**
- **Work-Life Balance**: 5.74 / 10
- **Salary Satisfaction**: 4.27 / 10

### 6. **Total Survey Stats**
- 630 total responses analyzed

---

## 🛠 Tools Used

- **Power BI Desktop (.pbix)** – Dashboard design and modeling
- **Power Query (M Language)** – Data cleaning and transformation
- **Excel (.xlsx)** – Original survey data source
- **DAX** – Measures for aggregations like average age and salary

---

## 👤 Contributor

- [Azim Nahin](https://github.com/AzimNahin)

---

## 📷 Dashboard Preview

![Dashboard Preview](Data%20Professional%20Survey%20Dashboard.jpg)
