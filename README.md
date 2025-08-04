Adventure Dashboard (Power BI)
📊 Dashboard Theme: Customer Demographics & Travel Trends
Dashboard Link: (https://drive.google.com/file/d/11dgb6hfsrCT5k4s0MBrzb-56WD1okr8W/view?usp=drive_link)

🧩 Problem Statement
This Power BI dashboard provides travel companies and executives with visual insights into customer behavior, preferences, and demographics. It is designed to enhance stakeholder decision-making by uncovering patterns such as average ratings, travel types, and customer segments.

🔧 Steps Followed
Loaded dataset (Excel or CSV) into Power BI Desktop.
Opened Power Query Editor:
Enabled: Column distribution, quality, profile.
Profiled data on the entire dataset.
Cleaned data:
Handled nulls and outliers.
Renamed columns and corrected datatypes.
Created calculated columns for:
Age group segmentation
Travel frequency classification
Built DAX measures for:
Average rating
Total number of passengers
% of repeat travelers
Revenue per customer
Designed visuals:
Slicers for Gender, Travel Type, Destination
Cards for KPIs (e.g., Total Customers, Avg Rating)
Bar chart: Travel type by age group
Donut chart: Customer segment distribution
Applied themes and branding:
Company logo, consistent color palette, and layout
Published report to Power BI Service.
Report Snipshot:
DAX formulas

% of All Returns = DIVIDE( [Total Returns], [All Returns] )

10-day Rolling Revenue = CALCULATE( [Total Revenue], DATESINPERIOD( 'Calendar Lookup' [Date], MAX( 'Calendar Lookup' [Date] ), -10, DAY ) )

YTD Revenue = Calculate( [Total Revenue], DATESYTD( 'Calendar Lookup'[Date] ) )

High Ticket Orders = CALCULATE( [Total Orders], FILTER ( 'Product Lookup', 'Product Lookup' [ProductPrice] > [Overall Average Price] ))

Images

<img width="614" height="335" alt="image" src="https://github.com/user-attachments/assets/09ff4342-e54d-4262-bc08-a261375c072e" />


📈 Key Insights
Repeat Customers: 65% of the users were return travelers.
Age Groups: 40% users belonged to the 25-40 age segment.
Travel Type: Business travel dominated at 68%.
Top Destination: City X showed the highest travel frequency.
Revenue Trend: Customers aged 30–45 contributed the highest average revenue.
💻 Tools Used
Power BI Desktop (DAX, Power Query)
Excel / CSV source files
Power BI Service for publishing
🧠 Learnings
Hands-on with DAX measures and custom visuals.
Improved filtering and interactivity with slicers.
Gained confidence in publishing and sharing dashboards via Power BI Service.
📎 Attachments
PBIX File: Adventure Dashfile.pbix (upload this file to GitHub or OneDrive and insert the link here)
GitHub Repo: KKG78/Data-Analysis-Project
Feel free to explore the visuals and interact with slicers to derive personalized insights.

Created by Kishan Kumar — Power BI | SQL | | Excel |Data Analytics
