# Facebook Ads Campaign Performance Tracker (Power BI)
This project analyzes Facebook Ads performance data to uncover insights that help marketing teams improve engagement, conversions, and return on ad spend.
The dataset contains metrics such as impressions, clicks, conversions, and spend for multiple ad variations — enabling performance benchmarking across campaigns.

# Objective
To evaluate how well the ads performed and answer key business questions such as:
Which ads delivered the highest engagement?
What was the CTR (Click-Through Rate) and CPC (Cost per Click)?
Which campaigns achieved the best ROI?
Which audience segments responded best?

# Dataset
Columns used in this analysis include:
Field	Description
ad_id	Unique ad identifier
reporting_start / reporting_end	Date range for the ad
campaign_id / fb_campaign_id	Campaign identifiers
age / gender	Audience attributes
interest1 / interest2 / interest3	Facebook interests targeted
impressions	Number of views
clicks	Number of clicks received
spent	Total ad spend ($)
total_conversion	Number of conversions
approved_conversion	Number of conversions that were approved

# Metrics Calculated (DAX Measures)
CTR = DIVIDE(SUM(Table[clicks]), SUM(Table[impressions]))
CPC = DIVIDE(SUM(Table[spent]), SUM(Table[clicks]))
Conversion Rate = DIVIDE(SUM(Table[total_conversion]), SUM(Table[clicks]))
ROI = DIVIDE((SUM(Table[approved_conversion]) * 1.0) - SUM(Table[spent]), SUM(Table[spent]))

# Dashboard Features
The final Power BI dashboard includes:
Campaign KPI cards (CTR, CPC, Total Impressions, ROI)
Top performing ads chart (clicks / impressions)
Spend vs Conversions visualization
Audience performance breakdown
Filters (Age, Date, Gender)

# Insights (Summary)
The 45-49 age group generated the highest CTR(%).
The 30-34 age group generated the highest ROI(%).
Fb_Campaign 115615 had the strongest ROI performance.
Fb_Campaign 114532 showed the best engagement.

# Tools Used
Power BI	Dashboard & data modeling
Excel	Data cleaning / formatting
GitHub	Version control & sharing

# Author
Godwin Lang’at
Data Analyst — Kenya
