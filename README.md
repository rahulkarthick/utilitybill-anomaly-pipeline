Automated Utility Bill Extraction & Anomaly Detection Pipeline

An end-to-end Applied AI and data science pipeline that parses unstructured utility bills, validates billing math, forecasts expected monthly expenses, and flags abnormal cost spikes.

## Key Features
* **Unstructured Data Extraction:** Parses raw utility invoice text into structured JSON records (`billing_date`, `usage_kwh`, `rate_per_kwh`, `total_billed`).
* **Automated Math & Baseline Auditing:** Validates `Usage × Rate` consistency and flags statistical anomalies using Z-score thresholds.
* **Time-Series Cost Forecasting:** Uses `scikit-learn` Linear Regression to predict upcoming monthly charges (`R² = 0.9979`) and establishes automated `±10%` tolerance bounds.
* **Visual Anomaly Reporting:** Generates `matplotlib` trend charts highlighting historical usage, predicted ranges, and flagged billing spikes.

## Tech Stack
* **Language:** Python 3
* **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Regex / Structured JSON Schemas
