# 📊 Finance Analytics Power BI Dashboard

## 📝 Project Overview
The **Finance Analytics Dashboard** is an interactive Power BI solution designed for a financial organization to monitor and analyze overall financial transactions, customer behavior, fees, taxes, and transaction performance across various business segments and regions. 

This project provides stakeholders with a centralized analytical tool to track real-time KPIs, uncover transaction patterns, and drive data-backed financial decision-making.

---

## 🎯 Business Objectives
The management team required a solution to address challenges in tracking overall transaction growth, monthly trends, successful vs. failed transactions, and regional performance. This dashboard was built to:
* Monitor core financial KPIs in real-time.
* Identify high-performing customer segments and geographical states.
* Analyze historical transaction patterns and emerging seasonality trends.
* Track operational fees and tax revenue.
* Understand customer demographics (Gender, Occupation).
* Measure Year-over-Year (YoY) performance changes.

---

## 🛠️ Key Features & Interactive Filters
The dashboard empowers users with dynamic deep-dive capabilities using the following filters:
* **Year:** Isolate specific temporal performance.
* **Dynamic Measure:** Seamlessly swap chart values between core metrics (e.g., Amount, Transactions, Fees, Taxes) using Power BI Field Parameters.
* **Occupation:** Filter by specific professional demographics.
* **Category:** Isolate specific transaction or product groupings.

---

## 📈 Key Performance Indicators (KPIs)
The primary dashboard prominently displays the following metrics:
1. **Total Amount:** Total transaction amount processed (includes YoY growth comparison).
2. **Total Transactions:** Total volume of transactions performed (includes YoY volume changes).
3. **Average Transaction Value:** Average monetary amount per transaction.
4. **Total Fees:** Total operational fees collected.
5. **Total Tax:** Total tax generated from transactions.

---

## 📊 Visualizations Included

### Dashboard 1: High-Level Analytics
* **Total Amount by Month (Line/Area Chart):** Analyzes monthly transaction trends and seasonal spikes.
* **Total Amount by Transaction Status (Donut Chart):** Compares Success, Failed, and Pending transactions to measure operational efficiency.
* **Total Amount by Customer Segment (Horizontal Bar Chart):** Highlights contributions from Retail, Premium, SME, Corporate, and Wealth segments.
* **Total Amount by State (Horizontal Bar Chart):** Identifies top-performing regional markets.
* **Transaction Type Analysis (Matrix Table):** Evaluates profitability (Amount, Fees, Tax, Count) across types like Bill Payment, Card Payment, Loan EMI, Transfer, etc.
* **Total Amount by Gender (Donut Chart):** Analyzes transaction contributions between demographic groups.

### Dashboard 2: Granular Details & Drill-Through
* **Transaction Details Grid:** A comprehensive table view containing underlying transactional records (Transaction ID, Date, Customer Name, Segment, State, Type, Amount, Status, Fees, Tax).
* **Drill-Through Capability:** Users can right-click any visual element (e.g., a specific state or customer segment) on Dashboard 1 and drill through to Dashboard 2 to view the exact transactions making up that data point.

---

## 💻 Technical Implementation
* **Tool:** Power BI Desktop
* **Data Modeling:** Star Schema design with a central Fact Table (Transactions) and surrounding Dimension Tables (Date, Customer, Geography, Transaction Type).
* **Time Intelligence:** Custom DAX measures for Year-over-Year (YoY) percentage calculations.
* **Dynamic Interactivity:** Implemented **Field Parameters** to allow users to dynamically change the measure (Amount vs. Fees vs. Tax) displayed across all visuals simultaneously.

---

## 🚀 How to Open and Use
1. Ensure you have [Power BI Desktop](https://powerbi.microsoft.com/desktop/) installed.
2. Clone or download this repository to your local machine.
3. Open the `Finance_Analytics_Dashboard.pbix` file.
4. Use the slicers on the left/top panel to interact with the data. 
5. To test the drill-through, right-click on any bar or donut slice, hover over **Drill through**, and select **Transaction Details**.
