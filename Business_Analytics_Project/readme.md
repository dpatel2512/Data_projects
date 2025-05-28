# 🛒 E-Commerce Business Analytics

## 📈 Project Overview

This project centers on cohort analysis for an e-commerce platform. The core objective was to transform raw transactional logs into strategic business insights. The analysis focused on constructing a **conversion funnel** to measure how efficiently the platform turns product page views into purchases, and building **monthly acquisition cohorts** based on users' first purchases to monitor their retention over time.

---

## 📁 Repository Structure

[E-Commerce Business](https://docs.google.com/spreadsheets/d/1p1xVITLMesCs7pC-9nCTq8OvBMJnwkY57m0tFNTSx2g/edit?usp=sharing)

---

## 📚 Table of Contents

| Tab            | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| `Data`         | Overview of the data source and schema                                      |
| `Description`  | Summary of project goals and deliverables                                   |
| `Assumptions`  | Assumptions made during the analysis process                                |
| `Process`      | Step-by-step methodology used for cleaning, analyzing, and visualizing data |
| `Findings`     | Key business insights and analytical conclusions                            |

---

## 📊 Data

The dataset tracks user behavior on an e-commerce site with the following columns:

- **`user_id`**: Unique identifier for each customer  
- **`event_type`**: Type of user activity (e.g., view, cart, purchase)  
- **`category_code`**: Product category classification  
- **`brand`**: Manufacturer or brand name  
- **`price`**: Product price in USD  
- **`event_date`**: Timestamp of the event (`YYYY-MM-DD` format)

---

## 🧾 Description

- Delivered an **8-tab Excel workbook** containing:
  - Data dictionary and organizational index
  - Cleaned raw data
  - Purchase activity logs
  - 3-stage conversion funnel analysis
  - Cohort-based retention model
  - Month-over-month retention rate visuals

---

## 🧠 Assumptions

- Only `user_id`, `event_type`, and `event_date` were leveraged for behavioral funnel and cohort modeling.
- The conversion funnel reflects **unique users** at each interaction stage, with natural attrition illustrated across steps.
- Monthly retention rates were calculated using cohort-based segmentation starting from the **first purchase date**.

---

## 🔍 Process

1. **Data Cleaning**:
   - Filtered irrelevant records and ensured schema integrity.
2. **Conversion Funnel Modeling**:
   - Built a 3-stage funnel: *View → Cart → Purchase*
   - Aggregated unique user counts and computed stage-to-stage conversion rates.
3. **Cohort Analysis**:
   - Identified users' first purchase dates to group monthly cohorts.
   - Calculated rolling retention rates over subsequent months.
4. **Data Visualization & Documentation**:
   - Created pivot tables, charts, and dashboards within the Excel workbook.
   - Structured spreadsheet for clarity and stakeholder usability.

---

## 📌 Key Findings

### 🔽 Conversion Funnel
- Roughly **10%** of product viewers proceed to purchase.
- Each step of the funnel experiences ~33% drop-off.
- Final purchase conversion is **1 in 10** from initial interest.

### 🔁 Retention Trends
- **September cohort** retained **13%** of users into the second month.
- Retention declines to **4%** by the fourth month.
- In the **January 2021 cohort**, retention after the first month was **7%**.

---

## 📎 Additional Notes

> This analysis informs strategic recommendations for optimizing user engagement, improving product conversion paths, and designing retention strategies tailored to cohort behaviors.

