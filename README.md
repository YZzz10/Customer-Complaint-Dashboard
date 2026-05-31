# Bank Customer Complaint Analysis Dashboard
## Project Objective
The objective of this project is to explore bank complaint patterns across different product categories, submission channels, and geographic regions, and to understand how these trends change over time.

## Dataset Used
- <a href="https://github.com/YZzz10/Customer-Complaint-Dashboard/blob/main/Complaints%20Data.csv">Customer Complaint Dataset</a>  
- <a href="https://github.com/YZzz10/Customer-Complaint-Dashboard/blob/main/State%20Map%20Data.csv">State Mapping Dataset</a>

## KPI Metrics
- Total number of complaints (2011–2020)
- Complaint share by product category (2011–2020)

## Visualization Overview
- The **Complaints Per Year** chart shows the percentage of complaints for each category within each year, which is driven by the “Select Product” filter in the top-right corner.
- The **Request Type** chart shows the percentage distribution of complaints by submission channel across all complaints or within each category, expressed as percentages, and can be updated by the “Select Product” filter.
- The **State Wise Map / Tile Chart** visualizes the geographic distribution of total complaints or complaints by category across states through map or tile views, and can be updated by the “Select Product” and “Select Map” filters.
- The **Year Trend** chart shows the trend of complaints over time (2011–2020, annual level), either for all complaints or by category, and can be updated by the “Select Product” filter.

## View Dashboard
<a href="https://public.tableau.com/app/profile/yixin.zhu3122/viz/Book2_17786133419830/CustomerComplaintDashboard">View Dashboard</a> (Please use “See this in Full Screen” if the dashboard elements overlap.)

## Process
- The “Date Received” field was incorrectly interpreted by Tableau as a year-first format. This issue was resolved by converting the field to string and re-parsing it using DATEPARSE("dd-MMM-yy", [Date Received]) to ensure accurate time-series analysis.
- Missing values were handled within the dashboard by excluding null entries to ensure clarity and accuracy in the charts.

## Dashboard
<img width="1600" height="900" alt="Dashboard Screenshot" src="https://github.com/user-attachments/assets/c245314d-fdc7-45a3-8249-0824aa3fec47" />


## Project Insight
- A total of 72,431 complaints were recorded between Dec 2011 and Oct 2020, with product distribution concentrated in Other (27.23%) and Credit Card (26.11%), indicating a relatively high share of non-standardized or broad complaint categories.
- Complaints are geographically concentrated, with California (12,107) being the highest, followed by New York (6,841), Florida (6,750), and Texas (5,537), suggesting that a small number of states account for a large proportion of total complaints.
- Submission channels are heavily dominated by Web (52.07%), followed by Referral (29.51%) and Phone (9.84%), indicating strong reliance on digital submission platforms.
- Time series analysis shows that complaint volumes peaked in 2017–2019 (8,000–10,000 range), while other years remained relatively stable at approximately 6,000–7,000 complaints, suggesting a temporary increase in reporting activity during this period.

## Final Conclusion
-
-
-
