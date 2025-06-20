# 📊 Power BI E-Commerce Sales Analytics Dashboard 

This project presents an end-to-end interactive dashboard built using Power BI to analyze the performance of a fictional e-commerce business over a span of 3 years (2023–2025). The dataset contains over **30,000 transactions** and includes customer, product, sales, return, and operational details.

The dashboard was designed to help decision-makers explore key business questions related to customer behavior, sales growth, product performance, and operational efficiency — all through clear visual storytelling and dynamic filters.

---

##  Objective

To create a self-service analytics solution that enables:
- Fast, intuitive exploration of large-scale e-commerce data
- Performance tracking across customers, orders, and products
- Business insight discovery without needing to write queries

---

##  Data Modeling & Preparation

- Cleaned and enriched the data with custom fields: `Age Group`, `Order Time Buckets`, and `Month-Year`
- Built a **star schema model** with a separate `Date` dimension for time intelligence
- Ensured relationships supported context-aware DAX calculations
- Removed redundancy, filtered out nulls, and ensured granularity consistency

---

##  Dashboard Overview

The report is structured into **three dedicated pages**, each focused on a core aspect of the business:

###  Orders Page
Tracks overall order health and behavior:
- Monthly order trends with **MoM % change**
- Order status breakdown: Completed, Refunded, Failed
- Payment mode distribution (UPI, Card, COD, etc.)
- Peak order time analysis across weekdays and time slots

###  Product Page
Helps assess product-level performance and profitability:
- Top products by sales, quantity, and ratings
- **Return rate** by category
- Profit and margin calculations

###  Customer Page
Visualizes who the customers are and how they behave:
- Age group and gender segmentation
- Preferred payment modes by demographic
- Region-wise sales performance
- Order quantity and value trends by customer segment

---

##  KPIs & DAX Measures

Custom DAX measures were used to calculate key performance indicators:

- `Return_Rate = DIVIDE(Total_Returns, Total_Orders)`
- `MoM_Sales_Change` using `PREVIOUSMONTH()` and `DIVIDE()`
- `Avg_Profit_Per_Unit = SUM(Profit) / SUM(Quantity)`
- Additional KPIs:
  - Total Orders
  - Total Sales
  - Quantity Sold
  - Avg. Sales per Order
  - Refund Amounts
  - Profit & Margin

---

##  Visuals Used

The dashboard includes a mix of strategic and operational visuals:

- **Line & Clustered Column Charts** – Sales trends vs MoM growth
- **100% Stacked Bars** – Breakdown of payment and order status
- **Donut Charts** – Contribution by region or category
- **KPI Cards & Area Charts** – High-level metrics
- **Slicers & Tooltips** – Dynamic filters for years, regions, and platforms

---

##  Key Insights Uncovered

Here are just a few of the actionable insights surfaced by the dashboard:

- **UPI** is the most preferred payment method (~54% usage)
- Customers aged **25–34** show the highest purchase frequency and order value
- **Clothing & Electronics** are top-performing but also carry higher return rates
- Sales from **Asia and Europe** dominate, but **Australia** is growing rapidly YoY
- **Peak shopping hours** fall between **Evening and Night**, especially on weekends

---

##  Tools & Techniques Used

| Area                  | Tools / Concepts                          |
|-----------------------|-------------------------------------------|
| Data Cleaning         | Power Query                               |
| Data Modeling         | Star Schema, Relationships                |
| Calculations          | DAX (CALCULATE, FILTER, PREVIOUSMONTH)   |
| Interactions          | Slicers, Drill-through, Custom Tooltips   |
| Formatting            | Conditional Formatting, Data Labels       |

---

##  Why This Matters

This dashboard isn’t just about numbers — it's about enabling decisions.

Whether you're:
- A marketing manager looking to target the right age group,
- A product manager tracking returns and profitability,
- Or a business analyst spotting regional opportunities…

This dashboard brings the answers to your fingertips in a visual, filterable, and easily digestible format.

---

## 📷 Screenshots

*(Feel free to replace with your actual dashboard images)*

- Orders Performance & Payment Mode
- Product KPIs & Return Analysis
- Age vs Gender Trends

---

## 🙋 About Me

I'm passionate about turning raw data into clean, insightful dashboards that empower better business decisions. This project gave me the opportunity to bring together data modeling, analytical thinking, and UX-focused design to create something truly useful.

If you're into analytics, Power BI, or just want to chat dashboards — feel free to connect!

---

