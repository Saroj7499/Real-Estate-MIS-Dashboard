# Real-Estate-MIS-Dashboard
Designed and built a Real Estate MIS Dashboard to analyze 430+ booking records, identify revenue trends, and track pending payments. Improved decision-making by creating automated reports and an interactive Power BI dashboard.

# Real Estate MIS Dashboard

A self-initiated project built to practice end-to-end data analysis — from raw messy data to a live dashboard.

---

## Why I Built This

Real estate companies manage hundreds of bookings every month but rarely have one place to track sales performance, project status, and pending payments together. I built this system from scratch to solve that.

---

## Tools Used

- Microsoft Excel — data cleaning, formulas, pivot tables, MIS reports
- Power BI — interactive dashboard with DAX measures
- Power Query — automated data cleaning

---

## Dataset

- 430 flat booking records for year 2024
- 3 projects — across Adajan, Bopal, and Vesu
- Flat prices from 25 lakhs to 1.4 crore
- I intentionally added errors like extra spaces, wrong casing, and blank values to practice real data cleaning

---

## What I Did in Excel

**Data Cleaning**
- TRIM — removed extra spaces
- PROPER — fixed wrong casing in names and locations
- IF and IFERROR — handled blank and error cells
- Data Validation — restricted incorrect inputs on key columns
- Added Days Overdue column using TODAY() to flag delayed payments

**Formulas**
- VLOOKUP and INDEX-MATCH — both used to pull project details from a reference table
- SUMIFS — revenue by project, location, flat type, executive
- COUNTIFS — booking count by payment status
- Nested IF — performance rating per executive (Excellent / Good / Below Target)

**MIS Reports**
- Daily MIS — uses TODAY() to auto-update
- Monthly MIS — December data using DATE() filter
- Annual MIS — full year performance with conditional formatting

**Pivot Tables**
- Bookings by project and revenue by location
- Both connected to one slicer using Report Connections

**Power Query**
- Automated TRIM, capitalization, and null value replacement
- New data just needs a Refresh — no manual cleaning needed

---

## Power BI Dashboard

One page dashboard with 6 KPI cards at the top — Total Bookings, Total Revenue, Confirmed Bookings, Pending Payments, Confirmation Rate, and Average Deal Size. Last two are DAX measures.

Visuals — monthly booking trend, flat type split, revenue by location, executive performance table.

Three slicers — Project Name, Payment Status, Flat Type — all visuals update together on click.

---

## Key Insights

- 2BHK flats led bookings at 41% of total
- Bopal and Adajan drove 84% of total revenue
- 157 bookings have pending payments — flagged automatically
- Top executive — Pooja Desai with 106 bookings
- Best monthly performance — Meena Shah at 182% of target in December

---

## Project Files

- Real Estate MIS Dashboard.xlsx — raw data, cleaned data, formulas, pivot tables, MIS reports
- Real Estate MIS Dashboard.pbix — Power BI dashboard

---

## What I Learned

- Data cleaning is more important than the analysis itself
- INDEX-MATCH is safer than VLOOKUP in real projects
- Power Query saves a lot of time once set up
- A good dashboard answers questions before someone asks them
