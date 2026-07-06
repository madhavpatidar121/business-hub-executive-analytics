# Business Hub Executive Analytics Platform

A reusable executive analytics dashboard for sales, profitability, customer, product, and regional performance analysis. The dashboard is built as a self-contained HTML application and supports uploading future CSV/Excel files with the same schema.

## Live Demo

After enabling GitHub Pages, open:

```text
https://<your-github-username>.github.io/business-hub-executive-analytics/
```

## Project Objective

Business Hub is a hypothetical multinational company. This project simulates an executive BI dashboard for the CEO and CFO to monitor business performance, identify profitability drivers, analyze customers and products, and detect underperforming areas.

The goal is to demonstrate end-to-end business intelligence thinking: dataset design, KPI development, dashboard layout, interactive filtering, executive insights, and reusable upload-based analytics.

## Key Features

- Executive KPI cards for sales, profit, margin, orders, customers, and average order value
- Reusable file upload model for CSV and Excel files
- Built-in demo dataset for instant preview
- Dynamic filters and slicers
- Sales and profit trend analysis
- Region, category, product, and customer analytics
- Top customer and product rankings
- Profit margin analysis
- Pareto-style contribution analysis
- Product health and profitability analysis
- Export option for filtered data
- Responsive single-page dashboard design

## Dataset

The repository includes two datasets:

| File | Purpose |
|---|---|
| `BusinessHub_Executive_Dataset_2000Rows.csv` | Main demo dataset with 2,000 rows |
| `Dashboard_Model_Test_File.csv` | Independent test dataset to validate reusability |

Excel versions are also included for Power BI and Excel-based analysis.

## Expected Schema

The dashboard works best when uploaded files follow the same column structure:

- Order ID
- Order Date
- Invoice Date
- Ship Date
- Delivery Date
- Order Status
- Customer ID
- Customer Name
- Customer Segment
- Customer Status
- Country
- Region
- City
- Product SKU
- Product Category
- Product Subcategory
- Brand
- Sales Channel
- Sales Representative
- Shipping Mode
- Quantity Sold
- Unit Price
- Discount %
- Gross Sales
- Discount Amount
- Net Sales
- Unit Cost
- Total Cost
- Shipping Cost
- Gross Profit
- Profit Margin %
- Budget Sales
- Budget Profit
- Return Flag

## How to Use

### Option 1: Run Locally

1. Download or clone this repository.
2. Open `index.html` in a browser.
3. Use the built-in demo data or upload a CSV/Excel file with the same schema.
4. Apply filters and review KPIs, visuals, and insights.

### Option 2: Use GitHub Pages

1. Go to repository **Settings**.
2. Click **Pages**.
3. Under **Build and deployment**, select:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
4. Save.
5. GitHub will generate a live URL for the dashboard.

## Power BI Learning Extension

This project can also be replicated in Power BI to learn professional BI methodology:

1. Import the Excel dataset.
2. Clean data in Power Query.
3. Build a star schema with fact and dimension tables.
4. Create DAX measures for KPIs.
5. Build report pages for executive summary, sales, profitability, customer, and product analytics.
6. Add slicers, drill-through, tooltips, and conditional formatting.

## Suggested Power BI Measures

```DAX
Total Sales = SUM(Sales[Net Sales])

Total Profit = SUM(Sales[Gross Profit])

Profit Margin % = DIVIDE([Total Profit], [Total Sales])

Total Orders = DISTINCTCOUNT(Sales[Order ID])

Total Customers = DISTINCTCOUNT(Sales[Customer ID])

Average Order Value = DIVIDE([Total Sales], [Total Orders])
```

## Business Questions Answered

- What are total sales, profit, and profit margin?
- Which regions and categories drive the most revenue?
- Which customers contribute most to sales and profit?
- Which products have strong sales but weak margins?
- Which regions or categories require management attention?
- How does business performance change over time?

## Recommended Repository Description

Reusable executive analytics dashboard built with HTML, JavaScript, and interactive data visualization. Supports CSV/Excel uploads, dynamic KPIs, sales analysis, profitability analysis, customer analytics, and product performance insights.

## Resume Bullet

Built a reusable executive analytics dashboard for a hypothetical multinational company using HTML, JavaScript, and interactive data visualization, enabling CSV/Excel upload, dynamic KPI tracking, sales and profit analysis, customer segmentation, product performance review, and executive-level insights.

## Tech Stack

- HTML
- CSS
- JavaScript
- CSV/Excel file upload logic
- Browser-based analytics
- Power BI-ready dataset

## Project Status

Version 1 is complete and ready for portfolio use. Future enhancements may include true chart cross-filtering, map visualization, advanced forecasting, AI narrative insights, and Power BI replication.
