# Amazon-India-Dashboard-2026


# 🇮🇳 Amazon India Sales & Profitability Intelligence Dashboard | Advanced Excel BI Project

## Project Overview

The **Amazon India Sales & Profitability Intelligence Dashboard** is an advanced Microsoft Excel Business Intelligence project designed to analyze e-commerce sales performance, profitability, customer order behavior, revenue leakage, geographical performance, and future business opportunities.

The project goes beyond traditional sales reporting by combining interactive dashboards, automated KPI calculations, business diagnostics, forecasting models, what-if analysis, and management recommendations.

The primary objective is to help business managers answer five important questions:

1. How is the business performing?
2. Which products, categories, payment methods, and fulfilment channels drive revenue and profit?
3. Where is the business losing revenue through returns and cancellations?
4. What are the future sales expectations?
5. Which business actions can improve revenue and profitability?

This project demonstrates how Microsoft Excel can be used as a powerful Business Intelligence and decision-support tool.

---

## Business Objectives

- Monitor overall sales, profit, orders, units sold, average order value, and profit margin.
- Identify high-performing and low-performing product categories.
- Discover products with strong sales but weak profitability.
- Analyze returns, cancellations, and lost revenue.
- Evaluate payment methods and fulfilment channels.
- Identify strong and weak geographical markets.
- Compare gross sales with net sales.
- Forecast sales for the next 3–6 months.
- Estimate potential revenue and profit recovery through reduced lost orders.
- Generate automated business insights and actionable recommendations.

---

##  Project Dataset

The analysis uses an Amazon India e-commerce order dataset containing 10,000 order records.

**Dataset Information**

| Attribute          | Details                    |
| ------------------ | -------------------------- |
| Total records      | 10,000                     |
| Date range         | January 2024 – August 2026 |
| Product categories | 5                          |
| Unique products    | 25                         |
| Payment methods    | 5                          |
| Fulfilment methods | 3                          |
| Order statuses     | 4                          |
| States             | 10                         |
| Currency           | Indian Rupees (INR)        |
| Data format        | Excel (.xlsx)              |

### Dataset Columns

| Column          | Description                                |
| --------------- | ------------------------------------------ |
| Order_ID        | Unique order identification                |
| Order_Date      | Date of the order                          |
| Category        | Product category                           |
| Product         | Product name                               |
| Quantity        | Units purchased                            |
| Unit_Price_INR  | Unit selling price                         |
| Discount_Pct    | Discount percentage                        |
| Total_Sales_INR | Order sales value                          |
| Profit_INR      | Profit generated                           |
| Payment_Method  | Customer payment method                    |
| Fulfillment     | Order fulfilment channel                   |
| Order_Status    | Delivered, Shipped, Returned, or Cancelled |
| Ship_State      | Customer shipping state                    |

---

##  Tools & Technologies

- **Microsoft Excel** – Dashboard development and business analysis.
- **Excel Formulas** – Dynamic KPI calculations and automated insights.
- **SUMIFS / COUNTIFS** – Conditional aggregations.
- **AVERAGEIFS** – Conditional average calculations.
- **INDEX / MATCH** – Dynamic rankings and lookups.
- **IF / IFERROR / ABS** – Business logic and error handling.
- **TEXT** – Automated narrative generation.
- **FORECAST.ETS** – Time-series sales forecasting.
- **Charts and Visualizations** – Business performance reporting.
- **What-if Analysis** – Scenario-based business impact estimation.
- **GitHub** – Project version control and portfolio presentation.

---

##  Dashboard Architecture

The workbook contains four main worksheets.

### 1. Dashboard

The main interactive management dashboard containing seven analytical sections.

### 2. Calc

The calculation engine responsible for:

- KPI calculations.
- Automatic category and product extraction.
- Dynamic ranking.
- Monthly and yearly trends.
- Forecast calculations.
- Backtesting.
- Automated insights.
- Management recommendations.
- What-if calculations.
- Data reconciliation checks.

### 3. Data

Contains the underlying Amazon India order-level dataset.

### 4. Data Quality Summary

Provides data validation and quality checks, including missing values, duplicate Order_IDs, negative sales, negative profit, invalid discounts, and date validation.

---

##  Key Dashboard Features

### 1. Overall Sales & Profit Performance

Provides a high-level overview of business performance.

**Key Performance Indicators (KPIs):**

- Total Sales
- Total Profit
- Total Orders
- Total Units Sold
- Average Order Value (AOV)
- Profit Margin %

**Business Questions:**

- How much revenue is the business generating?
- How much profit is being earned?
- What is the average value of each order?
- Is the business generating healthy profit margins?

### 2. Category & Product Performance

Identifies the categories and products responsible for business performance.

**Analysis includes:**

- Top-performing product category.
- Category contribution to total sales.
- Best-selling products.
- Product-wise sales contribution.
- Category-wise profit margins.
- Products requiring management attention.
- Lowest-margin products.

**Business Value:**

Helps management identify high-performing products, protect important inventory, improve weak product profitability, and optimize product mix.

### 3. Order Status & Revenue Loss Analysis

Analyzes order fulfilment performance and revenue leakage.

**Key Metrics:**

- Delivered Orders
- Shipped Orders
- Returned Orders
- Cancelled Orders
- Return Rate
- Cancellation Rate
- Revenue Lost Through Returns and Cancellations

**Advanced Analysis:**

- Category-wise return rates.
- Category-wise cancellation rates.
- Lost-order contribution.
- Identification of categories with high order-loss rates.

**Business Value:**

Helps identify operational problems that affect revenue realization and highlights opportunities to reduce returns and cancellations.

### 4. Payment, Fulfilment & Geographic Performance

Evaluates business performance across payment methods, fulfilment channels, and geographical markets.

**Payment Analysis:**

- Top payment method.
- Payment-method sales contribution.
- Payment-method profitability.
- Loss rates by payment method.

**Fulfilment Analysis:**

- Top fulfilment channel.
- Fulfilment contribution to sales.
- Fulfilment-wise profit margins.
- Order-loss rates by fulfilment method.

**Geographic Analysis:**

- Top-performing states.
- State-wise sales contribution.
- State-wise order volume.
- Average order value by state.
- Identification of weaker geographical markets.

**Business Value:**

Helps management understand customer purchasing preferences, fulfilment performance, and regional business opportunities.

### 5. Sales Outlook & Forecasting

One of the most advanced components of this project.

The forecasting engine compares three forecasting approaches:

1. **Exponential Smoothing (ETS)** – Uses historical patterns and seasonality.
2. **Seasonal Naive** – Uses the corresponding historical seasonal period as a forecast.
3. **Three-Month Moving Average** – Uses the average of the latest three historical months.

#### Forecasting Approach

The project maintains separate forecasting analyses for:

- Gross Sales – All orders placed.
- Net Sales – Delivered and shipped orders only.

This distinction is important because gross sales do not necessarily represent revenue retained by the business.

#### Forecast Validation

The project uses two backtesting approaches:

- Fixed-origin backtesting: 6 test months.
- Rolling-origin backtesting: 8 test months.

A total of 14 backtests are used to compare the forecasting methods.

#### Model Evaluation Metrics

- MAPE – Mean Absolute Percentage Error.
- MAE – Mean Absolute Error.
- RMSE – Root Mean Squared Error.
- Forecast Bias.
- Number of backtest wins.
- Overall method ranking.

The method with the lowest MAPE across the 14 backtests is selected for the corresponding forecast series.

#### Forecast Outputs

- Next 3-month gross sales forecast.
- Next 6-month gross sales forecast.
- Next 3-month net sales forecast.
- Next 6-month net sales forecast.
- Expected profit.
- Forecast uncertainty ranges.
- Gross versus net sales comparison.

**Business Value:**

Helps management plan inventory, staffing, marketing activities, and business operations based on historical sales patterns and forecasted demand.

### 6. Automated Business Insights & Recommended Actions

The dashboard generates automated business insights using Excel formulas.

The insights cover:

- Sales and profit trends.
- Strongest and weakest months.
- Category performance.
- Product performance.
- Returns and cancellations.
- Payment and fulfilment performance.
- Geographical performance.
- Future sales outlook.

It also generates three priority management actions.

The objective is to convert numerical analysis into meaningful business recommendations.

### 7. Diagnostic Q&A – Business Decision Intelligence

This section is designed to work like an automated business analyst.

It contains 15 diagnostic business questions, each structured around three dimensions:

1. What happened?
2. Why might it have happened?
3. What should management do next?

Examples of diagnostic questions:

- Are sales and profit improving or declining over time?
- Is profitability keeping up with sales?
- Which months are weak and how big is the swing?
- Which category drives the business and how risky is that?
- Which categories earn good profit and which are weak?
- Which products sell most and which need attention?
- How much revenue is lost to returns and cancellations?
- Which category loses the most orders?
- Do some payment or fulfilment methods lose more orders?
- Which payment methods are profitable?
- How do fulfilment channels contribute?
- Which states are key markets and which are weak?
- Where are sales heading in the next 3–6 months?
- What is fixing lost orders worth in rupees?
- Which business improvement lever has the highest potential value?

**Business Value:**

Instead of requiring managers to interpret every chart manually, the dashboard provides automated explanations and suggested actions.

---

##  Advanced Business Intelligence Features

### A. Dynamic Year Selection

The dashboard includes a Year dropdown that controls the selected-period analysis.

The calculation sheet automatically updates the relevant KPIs and analytical summaries when the selected year changes.

Some historical trend, forecasting, and diagnostic analyses intentionally use all available years rather than the selected-year filter.

### B. Gross Sales vs Net Sales

A key distinction in this project:

- Gross Sales: Value of all orders placed.
- Net Sales: Value of delivered and shipped orders only.

Returned and cancelled orders are excluded from net sales.

This helps management distinguish order-booking value from sales value retained after accounting for unsuccessful orders.

### C. Revenue Recovery What-if Analysis

The dashboard includes a scenario-based revenue recovery model.

Management can change the percentage reduction in returned and cancelled orders to estimate:

- Potential revenue recovery.
- Additional profit.
- Total sales after recovery.

It also compares alternative reduction scenarios.

### D. Business Improvement Lever Analysis

The dashboard compares three potential improvement opportunities:

- Lever A: Reduce lost orders.
- Lever B: Improve profit margin.
- Lever C: Increase sales.

The objective is to estimate which improvement opportunity could generate the greatest additional profit under the assumptions used in the model.

### E. Automated Data Reconciliation

The calculation sheet includes reconciliation checks for:

- Category sales.
- Product sales.
- Payment-method sales.
- Fulfilment sales.
- State-wise sales.
- Order-status counts.
- Monthly sales totals.

These checks help ensure that the analytical breakdowns reconcile with the overall business totals.

---

##  Key Business Findings

The following figures represent the workbook's currently calculated all-years snapshot. They may change when the underlying data or formulas are updated.

| KPI                                          | Current Workbook Result |
| -------------------------------------------- | ----------------------- |
| Total Sales                                  | ₹1,557.90 lakh          |
| Net Sales                                    | ₹1,401.41 lakh          |
| Total Profit                                 | ₹331.67 lakh            |
| Total Orders                                 | 10,000                  |
| Units Sold                                   | 24,926                  |
| Average Order Value                          | ₹15,579                 |
| Profit Margin on Net Sales                   | 23.67%                  |
| Revenue Lost Through Returns & Cancellations | ₹156.49 lakh            |
| Lost Revenue as % of Total Sales             | 10.04%                  |

### Important Business Observation

The workbook indicates a meaningful gap between gross sales and net sales.

Returns and cancellations represent a potential revenue-recovery opportunity.

The business can investigate:

- Product quality.
- Product descriptions and images.
- Packaging.
- Stock availability.
- Order confirmation.
- Delivery performance.
- Discounting and product profitability.

These areas should be investigated further before finalizing operational decisions.

---

##  Data Quality & Validation

The workbook includes a dedicated Data Quality Summary.

The current dataset checks report:

- 10,000 records.
- No missing values detected by the missing-value check.
- No duplicate Order_IDs detected.
- No negative sales values.
- No negative profit values.
- No invalid discount values.
- No missing order dates.
- All 10,000 dates recognized as valid Excel dates.
- No text or invalid dates detected.

Repeated order dates are expected because multiple orders can occur on the same date. They should not be confused with duplicate Order_IDs.

---

##  Important KPI Definitions

| KPI                 | Calculation                                  |
| ------------------- | -------------------------------------------- |
| Total Sales         | Sum of Total_Sales_INR                       |
| Net Sales           | Sales from Delivered and Shipped orders      |
| Total Profit        | Sum of Profit_INR                            |
| Average Order Value | Total Sales / Total Orders                   |
| Profit Margin       | Total Profit / Net Sales                     |
| Return Rate         | Returned Orders / Total Orders               |
| Cancellation Rate   | Cancelled Orders / Total Orders              |
| Lost-Order Rate     | (Returned + Cancelled Orders) / Total Orders |
| Sales Growth        | (Current Sales / Previous Sales) - 1         |
| Profit Growth       | (Current Profit / Previous Profit) - 1       |

All monetary calculations are based on Indian Rupees, with selected dashboard summaries displayed in lakh.

---
