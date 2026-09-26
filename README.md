# Time-Series-Sales-Forecast

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-orange)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)

An end-to-end retail sales forecasting project that uses historical sales data, machine learning, and Power BI to predict future demand and translate the results into practical business insights.

## Project Overview

Accurate sales forecasting can help businesses anticipate demand, plan inventory, allocate resources, and make better operational decisions.

In this project, historical retail sales data was cleaned, explored, and transformed into features for machine learning models. Multiple forecasting approaches were evaluated before developing a 21-day sales forecast.

The final results were presented through an interactive Power BI dashboard designed to communicate expected demand, forecast variation, peak periods, and weekly demand patterns to business stakeholders.

---

## Business Problem

A retailer wants to better anticipate short-term sales demand using historical sales information.

The objective of this project was to:

- Understand historical sales patterns
- Identify relationships between sales and available business variables
- Prepare historical data for forecasting
- Develop machine learning forecasting models
- Compare forecasting approaches
- Generate a 21-day sales forecast
- Translate the forecast into actionable business insights
- Present the results through an interactive Power BI dashboard

---

## Objectives

1. Clean and prepare the historical sales dataset.
2. Explore sales trends and relationships between variables.
3. Engineer features that capture historical sales behaviour.
4. Develop machine learning models for sales forecasting.
5. Evaluate and compare forecasting approaches.
6. Generate a 21-day forecast.
7. Identify periods of relatively high and low expected demand.
8. Build a business-focused Power BI dashboard.

---

## Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Jupyter Notebook**
- **Power BI**
- **DAX**

---

## Project Workflow

### 1. Data Preparation

The historical sales data was inspected and prepared for analysis.

Key preparation steps included:

- Checking the structure and data types
- Handling missing or inconsistent values
- Standardizing column names
- Converting the date field into a usable datetime format
- Sorting observations chronologically
- Preparing the dataset for time-series modelling

---

### 2. Exploratory Data Analysis

Exploratory analysis was performed to understand the behaviour of sales over time and examine relationships between sales and other variables.

The analysis focused on:

- Sales trends
- Inventory behaviour
- Price behaviour
- Sales variability
- Relationships between sales and explanatory variables
- Historical demand patterns

---

### 3. Feature Engineering

Features were created to provide the forecasting models with information about recent sales behaviour.

The final forecasting features included:

- Sales lag 1
- Sales lag 7
- Sales lag 14
- Sales lag 28
- 7-day rolling sales
- 14-day rolling sales
- 30-day rolling sales
- Price
- Inventory
- Price change
- Inventory change

These features combine recent sales history with available business variables to provide information about short-term demand.

---

## Forecasting Approach

Multiple machine learning approaches were tested to determine how effectively they could forecast future sales.

The modelling process included regression-based and tree-based approaches, including:

- Linear Regression
- Decision Tree Regression
- Gradient Boosting Regression
- Random Forest Regression

The forecasting process was evaluated using metrics including:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)

The modelling process also compared recursive and direct multi-step forecasting approaches for the 21-day forecasting horizon.

---

## 21-Day Forecast

The final forecasting workflow generated predictions for the next 21 days.

The final forecast produced:

| Metric | Value |
|---|---:|
| Forecast Horizon | 21 days |
| Average Daily Forecast | 203.93 units |
| Minimum Daily Forecast | 142.41 units |
| Maximum Daily Forecast | 336.81 units |
| Total Forecasted Sales | 4.28K units |
| Forecast Standard Deviation | 42.61 units |

The forecast indicates variation in expected daily demand, with some days substantially above or below the overall forecast average.

---

## Power BI Dashboard

The forecast was transformed into an interactive Power BI dashboard designed for business users.

### Dashboard Features

- Total forecasted sales
- Average daily forecast
- Maximum daily forecast
- Minimum daily forecast
- Forecast volatility
- Actual vs forecasted sales
- Daily forecast breakdown
- Variance from overall average
- Demand distribution
- Peak demand periods
- Weekly forecasted demand

The dashboard allows users to interact with the weekly forecast and examine the corresponding daily forecast values.

### Dashboard Preview

![Retail Sales Forecast Dashboard](images/BI_Dashboard.png)

---

## Key Business Insights

The forecast can support short-term operational planning by helping the retailer identify:

### Demand Planning

Expected daily demand can be used as an input for short-term inventory and resource planning.

### Peak Demand

The forecast identifies specific days with substantially higher expected sales, allowing the business to prepare for periods of increased demand.

### Lower-Demand Periods

Days below the overall forecast average can be monitored for potential changes in inventory, promotions, or other operational factors.

### Weekly Planning

Aggregating the 21-day forecast by week provides a higher-level view of expected demand and can support short-term planning.

---

## Business Recommendations

Based on the forecasting analysis, the retailer can:

1. **Use the forecast as a short-term planning input**  
   Expected demand can support inventory, staffing, and operational planning over the 21-day horizon.

2. **Prepare for high-demand periods**  
   Days with substantially higher predicted sales should receive additional attention when planning stock and operational capacity.

3. **Monitor lower-demand periods**  
   Days below the overall forecast average can be monitored alongside pricing, inventory, and other business factors.

4. **Review forecasts regularly**  
   Forecasts should be updated as new sales data becomes available so that planning decisions reflect the latest information.

5. **Combine forecasts with business context**  
   Machine learning predictions should be considered alongside promotions, holidays, stock availability, pricing changes, and other factors that may influence actual demand.

## Skills Demonstrated

This project demonstrates practical experience in:

- Data cleaning
- Exploratory data analysis
- Time-series feature engineering
- Machine learning
- Regression modelling
- Forecast evaluation
- Python data analysis
- Scikit-learn
- Power BI
- DAX
- Data visualization
- Business intelligence
- Translating analytical results into business recommendations

## Author

### Mary Eniola Olalere

Data Analyst | AI & Machine Learning

Portfolio: [maryeniola](https://maryeniola.vercel.app)

GitHub: [eniolamary](https://github.com/eniolamary)

---

## Project Structure

```text
Retail-Sales-Forecast/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── retail_sales_forecast.ipynb
│
├── data/
│   └── ...
│
├── powerbi/
│   └── retail_sales_forecast.pbix
│
└── images/
    └── dashboard.png
