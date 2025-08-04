# Adventure Dashboard (Power BI)

### 📊 Dashboard Theme: Customer Demographics & Travel Trends

**Dashboard Link:** *(https://drive.google.com/file/d/11dgb6hfsrCT5k4s0MBrzb-56WD1okr8W/view?usp=drive_link)*

---

## 🧩 Problem Statement
This Power BI dashboard provides travel companies and executives with visual insights into customer behavior, preferences, and demographics. It is designed to enhance stakeholder decision-making by uncovering patterns such as average ratings, travel types, and customer segments.

---

## 🔧 Steps Followed

1. **Loaded dataset** (Excel or CSV) into Power BI Desktop.
2. Opened **Power Query Editor**:
   - Enabled: Column distribution, quality, profile.
   - Profiled data on the entire dataset.
3. Cleaned data:
   - Handled nulls and outliers.
   - Renamed columns and corrected datatypes.
4. Created calculated columns for:
   - Age group segmentation
   - Travel frequency classification
5. Built DAX measures for:
   - Average rating
   - Total number of passengers
   - % of repeat travelers
   - Revenue per customer
6. Designed visuals:
   - Slicers for Gender, Travel Type, Destination
   - Cards for KPIs (e.g., Total Customers, Avg Rating)
   - Bar chart: Travel type by age group
   - Donut chart: Customer segment distribution
7. Applied themes and branding:
   - Company logo, consistent color palette, and layout
8. Published report to Power BI Service.
 
---
9. Report Snipshot:
DAX formulas

- % of All Returns = 
    DIVIDE(
        [Total Returns],
        [All Returns]
    )   

- 10-day Rolling Revenue = 
    CALCULATE(
        [Total Revenue],
        DATESINPERIOD(
        'Calendar Lookup' [Date],
            MAX(
                'Calendar Lookup' [Date]
            ),
                -10,
                DAY
        )
    )
- YTD Revenue = 
    Calculate(
        [Total Revenue],
        DATESYTD(
            'Calendar Lookup'[Date]
        )
    )
- High Ticket Orders = 
    CALCULATE(
    [Total Orders],
    FILTER (
    'Product Lookup',
    'Product Lookup' [ProductPrice] > [Overall Average Price]
    ))

----
## Images 
## Dashboard Snapshot

![Adventure Dashboard1](https://github.com/user-attachments/assets/e522ca5b-97c3-4622-90dc-1e191083eddf)
![Adventure Dashboard2](https://github.com/user-attachments/assets/d81f97ef-d955-4222-a587-11bfa664a53f)


---

## 📈 Key Insights

- **Repeat Customers:** 65% of the users were return travelers.
- **Age Groups:** 40% users belonged to the 25-40 age segment.
- **Travel Type:** Business travel dominated at 68%.
- **Top Destination:** City X showed the highest travel frequency.
- **Revenue Trend:** Customers aged 30–45 contributed the highest average revenue.

---

## 💻 Tools Used
- Power BI Desktop (DAX, Power Query)
- Excel / CSV source files
- Power BI Service for publishing

---

## 🧠 Learnings
- Hands-on with DAX measures and custom visuals.
- Improved filtering and interactivity with slicers.
- Gained confidence in publishing and sharing dashboards via Power BI Service.

---

## 📎 Attachments
- PBIX File: [Adventure Dashfile.pbix](https://drive.google.com/file/d/11dgb6hfsrCT5k4s0MBrzb-56WD1okr8W/view?usp=drive_link) *(upload this file to GitHub or OneDrive and insert the link here)*
- GitHub Repo: [KKG78/Data-Analysis-Project](https://github.com/KKG78/Data-Analysis-Project)

---

> Feel free to explore the visuals and interact with slicers to derive personalized insights.

---

*Created by Kishan Kumar — Power BI | SQL | | Excel |Data Analytics*
