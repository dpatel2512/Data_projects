### NYC Airbnb Data Analysis Project Plan

## Part 1: Data Cleaning & Preparation

# Objective: Ensure dataset integrity and relevance through systematic cleaning and filtering.

* Initial Exploration:

* Review the NYC Airbnb dataset and its accompanying data dictionary.
* Identify data quality issues such as inconsistent formatting, missing values, or irrelevant records.
Data Cleaning Actions:
Normalize neighborhood names: standardize text case, remove extra spaces, and unify label variations.
Filter out irrelevant listings:
Remove properties with no reviews in the past 12 months.
Exclude long-term rentals with a minimum stay requirement exceeding 7 days.
Version Control:
Maintain a separate "Data Cleaning Log" tab to document:
All cleaning steps
Rationales behind each decision
Dataset versions and update timestamps
Part 2: Aggregation & Pivot Table Analysis

Objective: Generate insights through calculated metrics and structured summaries.

Transformations:
Standardize empty bedroom entries:
Assign 0 bedrooms to listings labeled as studios.
Create a Clean Bedroom Count column.
Occupancy Analysis:
Derive an occupancy metric from availability and review data.
Convert availability fields to binary (1 = available, 0 = unavailable).
Pivot Table Development:
Identify the Top 10 neighborhoods for short-term rentals by occupancy.
Highlight the most common property sizes and their average performance.
Part 3: Data Visualization

Objective: Translate analytical outputs into actionable insights using visuals.

Visual Dashboards:
Build bar charts to depict:
Occupancy rates by day of the week
Neighborhood-specific rental popularity
Preferences by property type or size
Key Insight Visualization:
Showcase peak rental days, optimal listing types, and high-performing neighborhoods.
Part 4: Documentation & Executive Presentation

Objective: Ensure transparency, professionalism, and accessibility in project deliverables.

Cleaning Documentation:
Clearly outline all assumptions (e.g., using reviews as proxies for activity, excluding ultra-luxury listings).
Spreadsheet Formatting:
Apply consistent font styles, color schemes, and cell borders.
Use hidden columns for technical fields not needed by end users.
Navigation & Access:
Create a Table of Contents for ease of navigation.
Draft a concise Executive Summary highlighting major findings.
Ensure the final spreadsheet is shareable with defined access permissions for stakeholders.
