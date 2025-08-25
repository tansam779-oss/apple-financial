# Apple Financials (FY2023–FY2024) — Power BI Dashboard

## Short Description / Purpose
Power BI project built from Apple’s quarterly Condensed Consolidated Statements of Operations (Unaudited) and Net Sales by Product Category. The model aggregates all quarterly data to show full-year results for 2023 and 2024, with % change comparing FY2024 to FY2023. (FY2022 not in scope.)

## Tech Stack
- Power BI Desktop — visuals and DAX measures  
- Power Query / PowerPivot — data cleaning and reshaping  
- Excel — PDF-to-Excel conversion and staging  
- DAX (Data Analysis Expressions) — KPIs and YoY logic  
- Data Modeling — Calendar dimension related to fact tables  
- File formats — README and PNG preview (PBIX optional and not included in repo)

## Data Source
Apple Inc. Investor Relations: quarterly PDFs for FY2023 and FY2024 — Condensed Consolidated Statements of Operations (Unaudited) and Net Sales by Product Category. Data extracted Q1–Q4 for each fiscal year and structured for analysis.

## Features / Highlights

### Business problem
Financial statements are published as PDFs, which are difficult to analyze directly. Stakeholders need a fast way to compare Apple’s full-year performance across 2023 and 2024 and see how product categories contribute to results.

### Goal of the dashboard
Transform quarterly PDF filings into an analysis-ready model and executive-friendly dashboard that aggregates to full-year numbers and clearly shows FY2024 vs FY2023 changes.

### Walkthrough of Key Visuals
- KPI cards: Revenue, Gross Profit, Net Income, Profit Margin%, Operating Expenses, COGS (FY 2023 & FY 2024).  
- Clustered column chart: Net Sales by Product Category (iPhone, Mac, iPad, Services, Wearables/Home/Accessories) for 2023 vs 2024.  
- YoY matrix: 2024 vs 2023 absolute and % change for key metrics (time intelligence over Calendar).  
- Expense mix: donut visuals for OpEx and COGS shares.  
- Slicer: Year only (2023, 2024). No other slicers are included by design for clarity.

### Business impact & Insights
Enables quick comparisons between fiscal years and across product categories, supports finance reviews and investor-style analysis, and reduces manual effort by standardizing the refresh path for each new quarter.

## Screenshots / Demos
![Dashboard preview](https://github.com/tansam779-oss/apple-financial/blob/main/screenshot%20BI.png)

## Problem Statements
Q1. What are the full-year totals for Revenue, Gross Profit, Net Income, Profit Margin%, Operating Expenses, and COGS in 2023 and 2024?  
Q2. How do quarterly results roll up to annual figures for each fiscal year?  
Q3. What are the Net Sales by Product Category (iPhone, Mac, iPad, Services, Wearables/Home/Accessories) for 2023 and 2024?  
Q4. What is the % change in 2024 compared to 2023 for the key financial metrics?  
Q5. How are Operating Expenses and Cost of Goods Sold distributed in each fiscal year?

## Approach - Project Planning & Aims Grid
### 1. Purpose
Convert quarterly PDF statements into a consistent, model-driven Power BI dashboard that summarizes full-year performance for FY2023 and FY2024 and surfaces FY2024 vs FY2023 changes.

### 2. Stake Holders
- Finance leadership (CFO/FP&A)  
- Investor Relations  
- Executive team  
- Data & Analytics

### 3. End Result
An interactive dashboard with validated totals, product category breakdowns, and documented steps for refreshing each new year.  
*(Single slicer: Year only — 2023 or 2024.)*

### 4. Success Criteria
- Annual totals reconcile to Apple’s published statements for 2023 and 2024.  
- FY2024 vs FY2023 % change is accurate and clearly displayed.  
- Minimal manual prep: repeatable PDF→Excel→Power BI pipeline.  
- Simple navigation with a Year slicer only (2023, 2024).

## Data Analysis - Approach
- Collect Q1–Q4 PDFs for FY2023 and FY2024 from Apple Investor Relations.  
- Convert PDFs to Excel; trim to Statement of Operations and Net Sales by Product Category tables.  
- Clean and normalize tables with Power Query/PowerPivot (tidy format).  
- Build a Calendar dimension (Date, Year, Quarter) and relate it to fact tables.  
- Create DAX measures for KPIs and YoY (2024 vs 2023).  
- Design visuals (KPI cards, category columns, expense donuts, YoY matrix) per Microsoft best practices.  
- Validate totals and YoY against the source tables; exclude 2022 from scope.

## Attachment
The financial statements used for analysis.

## Disclaimer
The information presented here is based on publicly available data and is provided solely for educational purposes. It must not be reproduced, distributed, or used for any other purpose.
