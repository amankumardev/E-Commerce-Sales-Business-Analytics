# 🛒 E-Commerce Sales & Business Analytics

<p align="center">
  <b>Turning E-Commerce Data into Meaningful Business Insights 📊</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-Data%20Analysis-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-Data%20Querying-orange?style=for-the-badge&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-Data%20Cleaning-purple?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=for-the-badge&logo=powerbi&logoColor=black" />
</p>

<p align="center">
  <img src="https://img.shields.io/github/repo-size/amankumardev/E-Commerce-Sales-Business-Analytics" />
  <img src="https://img.shields.io/github/last-commit/amankumardev/E-Commerce-Sales-Business-Analytics" />
  <img src="https://img.shields.io/github/license/amankumardev/E-Commerce-Sales-Business-Analytics" />
</p>

---

## 📌 Project Overview

The **E-Commerce Sales & Business Analytics** project focuses on analyzing sales transactions to understand business performance, profitability, customer purchasing behavior, product performance, and regional sales trends.

The project uses Python, SQL, and data visualization techniques to transform raw sales data into meaningful insights that can support better business decisions.

The main objective is to identify sales patterns, evaluate profit margins, understand the impact of discounts, and discover top-performing products and regions.

## 🎯 Project Objectives

- Analyze overall sales, profit, and order performance.
- Understand product category-wise sales and profitability.
- Identify top-performing products and customers.
- Analyze regional sales and profit distribution.
- Explore monthly sales trends.
- Evaluate the relationship between discounts and profitability.
- Use SQL queries to perform business analysis.
- Prepare cleaned data for further visualization in Power BI.

## 🛠️ Tools & Technologies

| Technology | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| SQL | Business queries and analysis |
| SQLite | Database management |
| Jupyter Notebook | Analysis and documentation |
| Power BI | Dataset preparation for dashboard development |

## 📂 Project Structure

```text
E-Commerce-Sales-Business-Analytics/
│
├── Ecommerce_Sales_Practice_Dataset.csv
├── Ecommerce_Sales_Cleaned.csv
├── ecommerce_sales.db
├── Untitled.ipynb
├── LICENSE
└── README.md
```

## 📊 Dataset Description

The project uses an e-commerce sales dataset containing **1,000 records and 13 columns**.

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
| Product Name | Name of the product |
| Sales | Total sales amount |
| Quantity | Units sold |
| Discount | Discount applied |
| Profit | Profit earned |

**Product Categories:** Furniture, Technology, and Office Supplies.

## 🔍 Project Workflow

### 1. Data Loading & Exploration
- Imported datasets using Pandas.
- Explored dataset structure, rows, and columns.
- Checked data types and statistical summaries.
- Identified important business attributes.

### 2. Data Cleaning
- Checked missing values.
- Identified duplicate records and duplicate Order IDs.
- Converted Order Date into datetime format.
- Prepared the cleaned dataset for analysis.

### 3. Exploratory Data Analysis (EDA)
Performed multiple analyses to understand business performance:

- Overall Sales, Profit & Quantity Analysis
- Category-Wise Sales Analysis
- Category-Wise Profit Analysis
- Region-Wise Sales & Profit Analysis
- Monthly Sales Trend Analysis
- Top 10 Products by Sales
- Top 10 Customers by Sales
- Discount vs Profit Analysis
- Category-Wise Profit Margin Analysis

### 4. SQL Business Analysis

Converted the DataFrame into an SQLite database and performed SQL queries to analyze:

- Total sales and total profit.
- Category-wise sales and profit.
- Region-wise sales and order performance.
- Top five months by sales.
- Discount-wise profitability.

### 5. Data Visualization

Created visualizations using Matplotlib, including:

- Sales by Product Category
- Profit by Region
- Monthly Sales Trend
- Profit by Product Category
- Top 10 Products by Sales
- Top 10 Customers by Sales
- Profit by Discount Level
- Region-wise Sales and Profit Comparison

### 6. Power BI Preparation

Exported the cleaned dataset into CSV format for further analysis and dashboard development in Power BI.

## 📈 Key Business Metrics

The following KPIs were calculated from the dataset:

| KPI | Result |
|---|---:|
| Total Revenue (Sales) | 114,850.80 |
| Total Profit | 7,537.47 |
| Total Orders | 1,000 |
| Total Quantity Sold | 2,091 |
| Average Order Sales | 114.85 |
| Overall Profit Margin | 6.56% |

## 💡 Key Business Insights

### 1. Category Performance

Furniture generated the highest revenue, contributing 85,640.70 in sales.

| Category | Sales | Profit | Profit Margin |
|---|---:|---:|---:|
| Furniture | 85,640.70 | 3,399.92 | 3.97% |
| Technology | 21,016.50 | 2,795.09 | 13.30% |
| Office Supplies | 8,193.60 | 1,342.46 | 16.38% |

**Insight:** Furniture drives the highest revenue, while Office Supplies has the highest profit margin.

### 2. Regional Performance

- East generated the highest regional profit of 1,920.08.
- North recorded the highest regional sales of 25,311.40.
- South recorded the highest number of orders at 216.

**Insight:** The East region leads in profitability, while North leads in sales revenue.

### 3. Top-Selling Products

The top-performing products by sales include:

1. Writing Desk – 25,883.00
2. Filing Cabinet – 21,519.00
3. Office Chair – 17,131.75
4. Bookshelf – 16,518.75

**Insight:** Furniture products dominate the top-selling product list.

### 4. Discount vs Profit Analysis

- 0% discount generated the highest total profit of 2,766.36.
- 25% discount resulted in a small overall loss.
- 30% discount resulted in a total loss of 456.62.

**Insight:** Higher discounts are associated with lower profitability in this dataset. Businesses should carefully evaluate discount strategies before offering large discounts.

### 5. Monthly Sales Performance

The highest monthly sales were recorded in August 2025, reaching 6,844.35.

**Insight:** Monthly analysis helps identify stronger sales periods and supports business planning.

## 💻 SQL Analysis Example

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

## 🚀 How to Run the Project

**Step 1:** Clone the repository.

```bash
git clone https://github.com/amankumardev/E-Commerce-Sales-Business-Analytics.git
```

**Step 2:** Navigate to the project directory.

```bash
cd E-Commerce-Sales-Business-Analytics
```

**Step 3:** Install the required Python libraries.

```bash
pip install pandas numpy matplotlib jupyter
```

**Step 4:** Launch Jupyter Notebook.

```bash
jupyter notebook
```

**Step 5:** Open `Untitled.ipynb` and execute the cells sequentially.

## 📸 Project Visualizations

Add your actual analysis charts or Power BI dashboard screenshots here.

<!-- Replace these placeholders with screenshots uploaded to your repository. -->

<!--
![Sales by Category](screenshots/category_sales.png)
![Monthly Sales Trend](screenshots/monthly_sales.png)
![Regional Analysis](screenshots/regional_analysis.png)
![Power BI Dashboard](screenshots/powerbi_dashboard.png)
-->

## 🎯 Skills Demonstrated

- Data Cleaning & Data Preprocessing
- Exploratory Data Analysis (EDA)
- Data Aggregation & Grouping
- SQL Query Writing
- Business KPI Analysis
- Data Visualization
- Profitability Analysis
- Analytical Thinking
- Business Intelligence Concepts

## 🔮 Future Improvements

- Develop an interactive Power BI dashboard.
- Add dynamic filters for region, category, and date.
- Perform customer segmentation analysis.
- Build sales forecasting models.
- Automate data updates and reporting.
- Create more advanced business performance KPIs.

## 👨‍💻 Author

**Aman Kumar**

Aspiring Data Analyst | Python | SQL | Excel | Power BI | Data Visualization

- GitHub: [@amankumardev](https://github.com/amankumardev)
- LinkedIn: [Aman Kumar](https://www.linkedin.com/in/aman-kumar-615b5a292/)
- Portfolio: [Visit My Portfolio](https://aman-portfolio-2.onrender.com/)

## ⭐ Support

If you find this project useful or interesting, consider giving it a ⭐ on GitHub!

---

<p align="center">
  <b>Thank you for visiting my project! 🚀</b>
</p>
