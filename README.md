# 🧪 Environmental Health & Chronic Illness Analysis

This project explores how environmental and socioeconomic factors contribute to chronic illness rates across 100 counties in Eastern Tennessee. The analysis leverages R for statistical modeling and visualization, with insights communicated through an interactive Power BI dashboard and a comprehensive written report.

## 🎯 Objective

To evaluate whether indicators like air quality, water contamination, income, and education level are associated with chronic illness prevalence — and to translate these insights into actionable strategies for public health stakeholders.

## 🛠️ Tools & Technologies

- **R & R Markdown**: Statistical modeling, residual diagnostics, and regression analysis
- **Power BI**: Interactive dashboard for decision-makers
- **Key R packages**:
  - `ggplot2` — visualization
  - `car`, `broom`, `lmtest` — diagnostics
  - `dplyr`, `readr` — data manipulation

## 📈 Statistical Model

A multiple linear regression model was used:


### Key Results:
- 📌 **Adjusted R²:** 0.06 — model explains ~6% of the variance
- 📘 **Significant Predictor:** Education level (p = 0.039), suggesting a positive correlation with illness
- ⚠️ **Water Contamination:** Marginally significant (p = 0.066)
- 📉 AQI and income were not statistically significant

Diagnostics confirmed:
- No multicollinearity (VIF < 1.1)
- Residuals approximately normal (Shapiro-Wilk)
- Stable leverage across observations

## 📊 Power BI Dashboard

An interactive dashboard was developed with:
- KPIs for AQI, income, water contamination, and illness rate
- Bar chart: Illness rate by county
- Scatter plot: AQI vs illness rate (colored by education level)
- Slicers for filtering by AQI, income, and education level

📁 File: `/dashboard/Environmental_health_projectpowerbi.pbix`

## 🧾 Repository Structure

- `data/` — CSV dataset
- `analysis/` — Full R Markdown file (`.Rmd`) with code and commentary
- `visuals/` — Exported plots (e.g., residual plots, scatterplot)
- `report/` — Final Word report for academic/stakeholder delivery
- `dashboard/` — Power BI file for interactive visualization
