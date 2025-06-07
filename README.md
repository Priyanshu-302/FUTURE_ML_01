# FUTURE_ML_01
# AI-Powered Sales Forecasting Dashboard

This project involves developing a real-world **time series forecasting system** for retail sales using **Facebook Prophet** and visualizing actionable insights in **Power BI**. The goal is to help businesses forecast sales, identify trends, and make informed decisions.

---

## Project Overview

Retail businesses rely heavily on accurate forecasting to manage inventory and boost sales. This project combines **predictive analytics** and **interactive dashboarding** to deliver:

- Accurate 90-day **sales forecasts**
- Historical trend analysis
- Seasonal insight detection
- Business recommendations for planning

---

## 📊 Tools & Technologies

| Category             | Tools Used                   |
|----------------------|------------------------------|
| Language             | Python 3.x                   |
| Libraries            | Prophet, Pandas, Matplotlib  |
| Visualization        | Power BI Desktop             |
| Data Handling        | CSV, Excel, Jupyter Notebook |
| Forecasting Model    | Facebook Prophet             |

---

## Dataset Used

- `mock_kaggle.csv` – Simulated retail sales data  
  Columns:
  - `data`: Date of transaction
  - `venda`: Daily sales
  - `estoque`: Inventory
  - `preco`: Price

- `forecast.csv` – Output from Prophet model  
  Columns:
  - `ds`: Date
  - `yhat`: Forecasted sales
  - `yhat_lower`: Lower confidence bound
  - `yhat_upper`: Upper confidence bound

---

## Project Workflow

1. **Data Cleaning & Preprocessing**
   - Renamed columns for Prophet compatibility
   - Converted date strings to `datetime` objects

2. **Forecasting with Prophet**
   - Trained model on historical sales (`venda`)
   - Generated 90-day future forecast
   - Exported predictions to `forecast.csv`

3. **Dashboard in Power BI**
   - Merged `forecast.csv` and `mock_kaggle.csv`
   - Visualized:
     - Actual vs Forecasted Sales
     - Monthly & seasonal trends
     - Peak & low-performing dates
   - Added filters, tooltips, and KPIs
   - Wrote insights for business decisions

---

## Key Features in the Dashboard

Line chart: Actual vs Forecast  
Cards: Total Sales, Forecasted Sales, Growth Rate  
Filters: Date Range, Type (Actual/Forecast)  
Tooltips: Hover insights for each point  
Summary Page: Business Insights & Recommendations

---

## Insights & Recommendations

- **Sales expected to peak in mid-July** — plan inventory accordingly  
- **Forecast shows ~12% increase** in next quarter  
- **Late August shows low sales** — ideal for running promotions  
- Use insights to **optimize procurement and marketing**

---
