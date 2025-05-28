# 🏙️ NYC Airbnb Data Analysis Project

## Overview

This project conducts a comprehensive analysis of the NYC Airbnb dataset, focusing on data cleaning, transformation, aggregation, and visualization to uncover rental trends and occupancy insights. The final deliverable is a structured Excel spreadsheet and an executive summary for business stakeholders.

---

## 📁 Project Structure

- `Data_Cleaning_Log`: Tab documenting all cleaning steps and version updates
- `Pivot_Analysis`: Aggregation and trend identification via pivot tables
- `Visualizations`: Bar charts and graphs for key insights
- `Summary`: Executive summary, assumptions, and table of contents
- `Final_Spreadsheet.xlsx`: Cleaned, styled, and documented workbook

---

## ✅ Part 1 – Data Cleaning and Preparation

### Objectives:
- Explore raw NYC Airbnb dataset and review associated data dictionary.
- Identify and resolve data inconsistencies and cleanliness issues.

### Tasks:
- Standardize **neighborhood labels**:
  - Fix inconsistent capitalization (e.g., `brooklyn` → `Brooklyn`)
  - Trim leading/trailing whitespaces

- **Filter irrelevant listings**:
  - Exclude listings with **no reviews in the past 12 months**
  - Remove **long-term rentals** (minimum stay > 7 days)

- **Document changes** in a dedicated cleaning log tab:
  - Timestamp each cleaning operation
  - Record assumptions and data dictionary updates

---

## 📊 Part 2 – Aggregations and Pivot Table Analysis

### Objectives:
Generate summary metrics and trend insights from cleaned data.

### Tasks:
- Create pivot tables for:
  - **Occupancy rates**
  - **Top 10 neighborhoods** for vacation rentals
  - **Popular property sizes** by bedroom count

- Standardize bedroom field:
  - Replace blank/NaN with `0` for studio apartments
  - Create new column: `clean_bedroom_count`

- Calculate **average occupancy rate**:
  - Convert availability to binary:
    - `1` = available
    - `0` = not available

---

## 📈 Part 3 – Data Visualization

### Objectives:
Highlight key patterns in rental activity and guest preferences.

### Visuals:
- **Bar charts** of occupancy by day of the week
- **Trend charts** for:
  - Most active rental days
  - Property preferences by neighborhood

---

## 🧾 Part 4 – Documentation and Presentation

### Deliverables:
- **Data Cleaning Tab**: Logs all cleaning actions with version history
- **Executive Summary**: Key insights, business implications, and assumptions
- **Formatted Spreadsheet**:
  - Consistent font, color scheme, borders
  - Hidden helper columns for clarity
- **Table of Contents**: Internal links for navigation within spreadsheet

### Assumptions:
- **Luxury listings** excluded as outliers
- **Review count** used as proxy for booking activity
- **Studio units** defined as `0` bedrooms

---

## 📤 Sharing Guidelines

- Share final spreadsheet with **view-only** or **comment** access for reviewers.
- Use a shared drive or cloud service with clear naming conventions:
  - `NYC_Airbnb_Analysis_vFinal.xlsx`

---

## 🧠 Summary

This project empowers stakeholders to make data-driven decisions about NYC short-term rental trends, providing a clean, interactive, and insightful view of Airbnb performance across neighborhoods and property types.

---


