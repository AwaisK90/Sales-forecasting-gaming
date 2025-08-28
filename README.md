# Sales Forecasting for Gaming Publisher

A professional, end-to-end portfolio project demonstrating time-series **sales forecasting** for a gaming publisher and executive-ready **dashboarding** for decision support.

## What this repo includes
- `/data` – sample (or anonymized) datasets used for exploration and modeling.
- `/notebooks` – reproducible analysis notebooks (EDA, feature engineering, forecasting).
- `/scripts` – modular Python scripts for training, evaluation, and exporting forecasts.
- `/dashboard` – Tableau/Power BI artifacts for visual storytelling.
- `/outputs` – exported charts, dashboards (.pdf/.png) and final reports.

## Business Problem
A gaming publisher needs to **forecast global and regional sales** to plan inventory, marketing spend, and release calendars. Historical title-level sales and review metrics are available (e.g., critic/user scores, platform, genre, release year).

## Goals
1. Build reliable monthly/annual forecasts for total sales and by **genre/platform**.
2. Identify **drivers** of sales using features (genre, platform, critic/user score).
3. Package results into an **executive dashboard** with clear recommendations.

## Methodology (brief)
- **EDA**: Missing value handling, outlier checks, seasonal patterns.
- **Modeling**: Baseline naive & moving-average models; classical **ARIMA**; gradient-boosted regression for tabular drivers (with time features).
- **Validation**: Time-series split; metrics: MAPE / sMAPE / RMSE.
- **Communication**: Forecast plots with confidence bands; “What this means” callouts.
- **Automation-ready**: Scripts structured for scheduled retraining and export to dashboard.

## Quickstart
1. Create a Python env and install packages:
   ```bash
   pip install -r requirements.txt
   ```
2. Open `notebooks/01_eda_and_forecasting.ipynb` to reproduce the analysis.
3. Open the Tableau/Power BI file in `/dashboard` and point it to `outputs/forecast_export.csv`.

## Project Artifacts
- `outputs/` contains **ready-to-share** images/PDFs for a portfolio or client proposal.
- `dashboard/` contains a Tableau/Power BI dashboard configured for forecasting KPIs.

## Notes on Data
If client data cannot be shared, a **synthetic** or public dataset with the *same schema* is provided so dashboards remain functional for demonstration.

---
**Author:** Awais Khan · [LinkedIn](https://www.linkedin.com/in/aawaismkhan) · [Email](mailto:awaiskhan90@outlook.com)
