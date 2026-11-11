# E-Commerce Sales & Business Analytics

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Arial&weight=500&size=24&pause=1000&color=36BCF7&center=true&vCenter=true&width=650&lines=E-Commerce+Sales+Analytics;Turning+Data+into+Business+Insights;Python+%7C+SQL+%7C+Data+Analysis" alt="Typing SVG" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=3&section=header" width="100%" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Data%20Analysis-blue?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/SQL-Database-orange?style=flat-square&logo=sqlite" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Cleaning-purple?style=flat-square&logo=pandas" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter" />
  <img src="https://img.shields.io/badge/SQLite-Database-blue?style=flat-square&logo=sqlite" />
</p>

---

## Project Overview

This project focuses on analyzing e-commerce sales data to understand business performance, sales trends, product performance, customer behavior, and profitability.

Using Python, SQL, and data analysis techniques, this project transforms raw sales data into meaningful business insights that can support better decision-making.

The main objective is to identify sales patterns, evaluate profit margins, understand discount impacts, and analyze product and regional performance.

## Project Objectives

- Analyze overall sales, profit, and order performance.
- Understand category-wise sales and profitability.
- Identify top-performing products and customers.
- Analyze regional sales and profit distribution.
- Explore monthly sales trends.
- Evaluate the relationship between discounts and profitability.
- Perform business analysis using SQL queries.
- Prepare cleaned data for Power BI visualization.

## Tools & Technologies

| Technology | Purpose |
|---|---|
| Python | Data Analysis |
| Pandas | Data Cleaning & Manipulation |
| NumPy | Numerical Operations |
| Matplotlib | Data Visualization |
| SQL | Business Data Analysis |
| SQLite | Database Management |
| Jupyter Notebook | Analysis Environment |
| Power BI | Dashboard Preparation |

## Dataset Information

The dataset contains **1,000 records and 13 columns**.

| Column | Description |
|---|---|
| Order ID | Unique order identifier |
| Order Date | Date of purchase |
| Customer ID | Unique customer identifier |
| Customer Name | Customer name |
| Segment | Customer segment |
| Region | Sales region |
| Product ID | Unique product identifier |
| Category | Product category |
| Product Name | Product name |
| Sales | Total sales amount |
| Quantity | Units sold |
| Discount | Discount applied |
| Profit | Profit earned |

**Product Categories:** Furniture, Technology, and Office Supplies.

## Project Workflow

### 1. Data Collection & Exploration

- Imported datasets using Pandas.
- Explored rows, columns, and data types.
- Performed statistical analysis.
- Identified important business attributes.

### 2. Data Cleaning

- Checked missing values.
- Identified duplicate records.
- Checked duplicate Order IDs.
- Converted Order Date into datetime format.
- Prepared the dataset for analysis.

### 3. Exploratory Data Analysis (EDA)

- Overall Sales & Profit Analysis
- Category-Wise Sales Analysis
- Category-Wise Profit Analysis
- Region-Wise Sales & Profit Analysis
- Monthly Sales Trend Analysis
- Top 10 Products by Sales
- Top 10 Customers by Sales
- Discount vs Profit Analysis
- Category-Wise Profit Margin Analysis

### 4. SQL Business Analysis

- Created an SQLite database.
- Performed category-wise sales analysis.
- Analyzed regional sales and profit.
- Identified top-performing months.
- Evaluated discount-wise profitability.
- Calculated important business KPIs.

### 5. Data Visualization

Created charts using Matplotlib:

- Sales by Product Category
- Profit by Region
- Monthly Sales Trend
- Profit by Product Category
- Top 10 Products by Sales
- Top 10 Customers by Sales
- Profit by Discount Level
- Region-Wise Sales and Profit Comparison

## Key Performance Indicators (KPIs)

| Metric | Result |
|---|---:|
| Total Sales | 114,850.80 |
| Total Profit | 7,537.47 |
| Total Orders | 1,000 |
| Total Quantity Sold | 2,091 |
| Average Order Sales | 114.85 |
| Overall Profit Margin | 6.56% |

## Key Business Insights

**1. Category Performance**

- Furniture generated the highest sales of 85,640.70.
- Technology generated a profit of 2,795.09.
- Office Supplies achieved the highest profit margin of 16.38%.

**2. Regional Performance**

- East generated the highest profit of 1,920.08.
- North recorded the highest sales of 25,311.40.
- South recorded the highest number of orders at 216.

**3. Top-Selling Products**

- Writing Desk: 25,883.00
- Filing Cabinet: 21,519.00
- Office Chair: 17,131.75
- Bookshelf: 16,518.75

**4. Discount Analysis**

- 0% discount generated the highest total profit of 2,766.36.
- 25% discount resulted in a loss of 7.34.
- 30% discount resulted in a loss of 456.62.

**5. Monthly Sales Performance**

- August 2025 recorded the highest monthly sales of 6,844.35.

## SQL Query Example

```sql
SELECT
    Category,
    ROUND(SUM(Sales), 2) AS Total_Sales,
    ROUND(SUM(Profit), 2) AS Total_Profit,
    SUM(Quantity) AS Total_Quantity
FROM sales
GROUP BY Category
ORDER BY Total_Sales DESC;
```

This query calculates category-wise sales, profit, and quantity sold.

## Project Structure

```text
E-Commerce-Sales-Business-Analytics/
│
├── Ecommerce_Sales_Practice_Dataset.csv
├── Ecommerce_Sales_Cleaned.csv
├── ecommerce_sales.db
├── Ecommerce_Sales_Analysis.ipynb
├── LICENSE
└── README.md
```

## How to Run the Project

**Step 1: Clone the Repository**

```bash
git clone https://github.com/amankumardev/E-Commerce-Sales-Business-Analytics.git
```

**Step 2: Navigate to Project Directory**

```bash
cd E-Commerce-Sales-Business-Analytics
```

**Step 3: Install Required Libraries**

```bash
pip install pandas numpy matplotlib jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5:** Open `Ecommerce_Sales_Analysis.ipynb` and execute the cells.

## Future Improvements

- Develop an interactive Power BI dashboard.
- Add dynamic filters for region and category.
- Perform customer segmentation analysis.
- Implement sales forecasting.
- Automate data updates and reporting.

## Author

**Aman Kumar**

Aspiring Data Analyst

- GitHub: [amankumardev](https://github.com/amankumardev)
- LinkedIn: [Aman Kumar](https://www.linkedin.com/in/aman-kumar-615b5a292/)
- Portfolio: [Visit My Portfolio](https://aman-portfolio-2.onrender.com/)

## GitHub Contribution Activity

<p align="center">
  <img src="https://raw.githubusercontent.com/amankumardev/amankumardev/output/github-contribution-grid-snake-dark.svg" width="100%" alt="GitHub Contribution Snake" />
</p>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=3&section=footer" width="100%" />
</p>

<p align="center">
  **Thank You for Visiting My Project!**
</p>

<p align="center">
  If you find this project useful, please consider giving it a star.
</p>
