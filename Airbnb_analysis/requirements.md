🧹 Part 1: Data Cleaning and Preparation

Tasks:
Review dataset and accompanying data dictionary.
Identify inconsistencies and anomalies in the data.
Clean and standardize:
Neighborhood labels: Correct inconsistent cases, remove trailing spaces.
Bedroom field: Convert missing/empty bedroom entries to 0 for studio apartments.
Filter data:
Exclude listings with no reviews in the past 12 months.
Exclude long-term rentals (minimum stay > 7 days).
Deliverables:
cleaning_steps_log.xlsx: All transformations documented with versions and justifications.
Cleaned dataset ready for analysis.
📊 Part 2: Aggregations and Pivot Table Analysis

Tasks:
Standardize studio apartments (bedrooms = 0).
Create a new column clean_bedroom_count.
Convert availability status into binary format:
0 = Not Available, 1 = Available.
Build pivot tables for:
Occupancy Rate by Neighborhood
Top 10 Vacation Rental Areas
Popular Property Sizes
Deliverables:
Pivot tables embedded in nyc_airbnb_analysis.xlsx.
📈 Part 3: Data Visualization

Tasks:
Generate bar charts to illustrate:
Occupancy rates by day of the week
Top neighborhoods for rentals
Most common property types and sizes
Use visual storytelling to highlight:
High-traffic rental days
Neighborhood-specific preferences
Deliverables:
Charts saved in /visualizations
Visuals embedded in final spreadsheet and presentation materials
📄 Part 4: Documentation & Presentation

Tasks:
Log all cleaning steps with version history and rationale.
Define and apply formatting guidelines:
Consistent font, color codes, table borders
Hide irrelevant columns
Executive summary with key insights
Table of Contents with internal navigation for the spreadsheet
Enable shareable, read-only access to stakeholders
Deliverables:
nyc_airbnb_analysis.xlsx: Finalized spreadsheet with TOC, visuals, and summaries
README.md: This documentation
Clear permissions for access & review
🧠 Assumptions & Notes

Reviews are used as a proxy for rental activity.
Luxury listings outliers are excluded to reduce skew.
Minimum stay threshold set at 7 days for filtering long-term rentals.
✅ Completion Criteria

Data integrity validated post-cleaning
Visualizations align with pivot analysis insights
Spreadsheet is polished, navigable, and presentation-ready
All steps and logic traceable via logs and documentation
📬 Feedback & Contributions

Pull requests and feedback are welcome. For major changes, please open an issue first to discuss potential updates.



