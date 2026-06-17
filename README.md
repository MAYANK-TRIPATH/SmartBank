# BankSmart – Customer Spending & Churn Analysis

## DashBoard
<img width="802" height="453" alt="Screenshot 2026-06-17 at 10 09 20 AM" src="https://github.com/user-attachments/assets/be95051d-c83b-47a8-8241-17f43dfdfc04" />
<img width="892" height="498" alt="Screenshot 2026-06-17 at 10 08 43 AM" src="https://github.com/user-attachments/assets/d3560b3e-486e-426c-9139-6c2785ddc307" />



## Problem Overview

In today’s digital banking space, customer retention is becoming more challenging than ever. This project is based on a realistic scenario where a mid-sized bank is facing:

* Slow growth in savings accounts
* High customer churn
* Low engagement with digital banking channels

The goal was not just to analyze data, but to understand **why customers behave the way they do** and what the bank can do to improve.

---

## Business Objective

This analysis focuses on answering a few key business questions:

* How customers spend and save money
* What kind of customers are more likely to churn
* Whether income, age, or behavior impacts engagement
* How customers interact with different banking channels

The final aim was to generate **actionable insights** that can help the bank improve retention and customer engagement.

---

## Data Used

The dataset is synthetic but designed to simulate real banking data.

**Customers (~10K records):**

* Demographics (age, gender, income, occupation)
* City tier, join date
* Churn flag

**Transactions (~100K records):**

* Transaction amount and category
* Debit/Credit type
* Channel (UPI, App, ATM, Branch)
* Salary indicator

---

## Approach

### 1. Data Pipeline

Raw Data → Excel Cleaning → Pandas Transformation → SQL Analysis → Dashboard

---

### 2. Feature Engineering

To make the analysis meaningful, a few key metrics were created:

* **Total Spend** → Total debit transactions per customer
* **Total Salary** → Total credited salary
* **Transaction Count** → Number of transactions
* **Savings Ratio** → Salary / Spending
* **Spend Segment** → Low / Medium / High spenders

---

### 3. Analysis (SQL + Python)

The analysis focused on:

* Churn rate and its distribution
* Spending vs savings behavior
* Customer segmentation
* Channel usage patterns
* Category-wise spending

---

### 4. Visualization

Built a Power BI dashboard to present:

* Key KPIs (customers, spend, churn rate)
* Channel usage trends
* Customer segmentation
* Spending patterns

---

## Key Insights

* **Churn Rate:** ~19.4% customers have churned — a significant concern
* **Spending Behavior:** Average spend is around ₹16,000, with similar patterns across users
* **Customer Segments:** Majority are low spenders; high spenders are very few
* **Savings Behavior:** High spenders have the lowest savings ratio
* **Churn Pattern:** Higher churn observed in low-spend and low-engagement customers
* **Income Impact:** Income does not strongly influence spending or churn
* **Age Groups:** Mid-career and pre-retirement customers are most valuable
* **Channel Usage:** UPI and mobile apps dominate transactions
* **Spending Categories:** Fairly evenly distributed across categories

---

## Business Recommendations

Based on the analysis:

* Improve savings behavior through automated tools and nudges
* Increase engagement via targeted campaigns and rewards
* Focus on low-engagement customers to reduce churn
* Strengthen digital channels (UPI/app) further
* Target high-value segments for cross-selling products

---

## What This Project Shows

This project demonstrates:

* How to translate a business problem into data questions
* How to use SQL and Python for real-world analysis
* How to derive insights that actually matter for business decisions
* How to present findings in a simple and understandable way

---

## Tools Used

* Excel (data cleaning)
* Python (Pandas)
* PostgreSQL (analysis)
* Power BI (dashboard)

