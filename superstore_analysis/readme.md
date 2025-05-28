# 📊 SuperStore Operations Analysis with Tableau

## 🚀 Project Overview

This project presents a comprehensive data analysis of an e-commerce SuperStore to evaluate operational performance, diagnose profitability issues, and develop strategic recommendations to prevent financial decline. Conducted independently, the project culminates in an interactive Tableau workbook featuring advanced data visualizations and dashboards.

**Primary Objectives:**
- Analyze sales and returns data.
- Identify profit/loss trends across products, regions, and time.
- Deliver actionable insights for advertising and inventory optimization.
- Support data-driven decision-making to avoid potential bankruptcy risks.

📎 **Data Source**: `SuperStore.xls` (includes `Orders` and `Returns` sheets)

🌐 **Tableau Public Dashboard**: (Dashboard)[https://public.tableau.com/app/profile/dhruv.patel3653/viz/superstorestorytelling_17361154385740/Dashboard1?publish=yes](#)

---

## 📁 Files Included

| File Name        | Description                                |
|------------------|--------------------------------------------|
| `SuperStore.xls` | Raw dataset including order and return data|
| `README.md`      | Project documentation                      |

---

## 🧭 Table of Contents

| Tab Title                        | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| **Profit & Losses by Product**  | Profit overview by subcategory and region                                  |
| **Product Analysis**            | Profit/loss analysis by product subcategory (geography-independent)        |
| **Loss-makers Products**        | Top 10 loss-generating products                                            |
| **Profit per Month**            | Monthly profit trends segmented by state                                   |
| **Profit per State**            | Top 3 most profitable states based on average profits                      |
| **Advertising Dashboard**       | Suggested advertising strategy by month/state with budget recommendations  |
| **Returned Items**              | Return ratio by product subcategory                                        |
| **Customer Returns**            | Top 10 customers with the most return requests                             |
| **Returns vs Profit**           | Products to prioritize based on profit-to-return ratio                     |
| **Customer Returns & Profit Dashboard** | Consolidated view of returns, segment performance, and profit impact     |

---

## 🧠 Key Assumptions

- Certain product categories are consistently unprofitable.
- Losses are directly correlated with return frequency and poor sales performance.
- Not all products contribute positively to revenue.
- Seasonal variation impacts sales volume.
- Advertising strategy lacks data-driven targeting.

---

## 🔧 Process Workflow

1. **Data Integration**  
   - Merged `Orders` and `Returns` datasets using a left join on `Order ID`.

2. **Profitability Analysis**  
   - Identified top-performing and underperforming product subcategories and regions.

3. **Advertising Strategy Formulation**  
   - Isolated the most profitable timeframes and geographies to allocate marketing spend effectively.

4. **Returns Diagnosis**  
   - Pinpointed high-return products and customers.
   - Flagged products that should be discontinued based on return/profit ratios.

---

## 📈 Key Findings

### 💰 Profit & Loss Insights
- **Top Profit Centers**:
  - Copiers in the **West** region
  - Chairs in the **East** region
- **Major Loss Drivers**:
  - Binders in the **Central** region
  - Tables in the **East** region

### 📢 Advertising Recommendations
- Highest ROI advertising opportunities:
  - **Vermont** in **November**
  - **Rhode Island** in **December**
  - **Indiana** in **October**

> 🔍 Insight: Focus advertising in Q4 for maximum impact.

### 📦 Returns & Profitability
- **Best Performer**: Copiers – High profit, low returns.
- **Worst Performer**: Tables – Negative profit, highest return volume.

> ✅ Recommendation: **Discontinue Tables** to minimize losses.

---

## 📌 Conclusion

The SuperStore must pivot toward data-informed decision-making, focusing on high-performing products and regions while eliminating unprofitable segments. Optimized advertising and strategic discontinuation of loss-generating inventory can substantially improve the company’s financial trajectory.
