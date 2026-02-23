# 📊 Exploratory Data Analysis & Advanced Analytics Project

> A comprehensive SQL-based data analytics project built in **MySQL (Microsoft MySQL Workbench)**, covering the full analytics pipeline — from raw data exploration to advanced business insights.

---

## 🗺️ Project Roadmap

![Project Roadmap](https://github.com/user-attachments/assets/b6a0e8f2-2dd3-4804-aaca-58d31edd866c)

The project is structured around **two core analytics tracks**:

### 🔵 Exploratory Data Analysis (EDA)
Understanding the data before drawing conclusions — exploring databases, dimensions, dates, measures, magnitude, and rankings.

### 🟢 Advanced Analytics
Going deeper with performance metrics, trend analysis, segmentation, part-to-whole breakdowns, and business reporting.

---

## 📁 Repository Structure

```
📦 project-root/
├── 📂 datasets/                    # Raw and processed CSV data sources
│   ├── bronze.crm_cust_info.csv    # CRM customer information (raw)
│   ├── bronze.crm_prd_info.csv     # CRM product information (raw)
│   ├── bronze.crm_sales_details.csv
│   ├── bronze.erp_cust_az12.csv    # ERP customer data (raw)
│   ├── bronze.erp_loc_a101.csv     # ERP location data (raw)
│   ├── bronze.erp_px_cat_g1v2.csv  # ERP product category data (raw)
│   ├── silver.crm_cust_info.csv    # Cleaned/transformed CRM data
│   ├── silver.crm_prd_info.csv
│   ├── silver.crm_sales_details.csv
│   ├── gold.dim_customers.csv      # Final dimensional model
│   ├── gold.dim_products.csv
│   ├── gold.fact_sales.csv
│   ├── gold.report_customers.csv   # Ready-to-use business reports
│   └── gold.report_products.csv
│
└── 📂 scripts/                     # SQL scripts (MySQL)
    ├── 00_init_database.sql
    ├── 01_database_exploration.sql
    ├── 02_dimensions_exploration.sql
    ├── 03_date_range_exploration.sql
    ├── 04_measures_exploration.sql
    ├── 05_magnitude_analysis.sql
    ├── 06_ranking_analysis.sql
    ├── 07_change_over_time_analysis.sql
    ├── 08_cumulative_analysis.sql
    ├── 09_performance_analysis.sql
    ├── 10_data_segmentation.sql
    ├── 11_part_to_whole_analysis.sql
    ├── 12_report_customers.sql
    └── 13_report_products.sql
```

---

## 🔬 Analytics Modules

### Phase 1 — Exploratory Data Analysis (EDA)

| # | Module | Description |
|---|--------|-------------|
| 01 | **Database Exploration** | Inspect tables, schemas, row counts, and relationships |
| 02 | **Dimensions Exploration** | Analyze categorical columns — unique values, cardinality, distributions |
| 03 | **Date Range Exploration** | Understand temporal coverage — earliest/latest dates, gaps |
| 04 | **Measures Exploration** | Summarize numeric columns with min, max, avg, and nulls (Big Numbers) |
| 05 | **Magnitude Analysis** | Compare sizes across categories using bar-style aggregations |
| 06 | **Ranking Analysis** | Identify top-N and bottom-N performers across key metrics |

### Phase 2 — Advanced Analytics

| # | Module | Description |
|---|--------|-------------|
| 07 | **Change-Over-Time Analysis** | Trend detection across time periods (MoM, YoY, rolling) |
| 08 | **Cumulative Analysis** | Running totals and cumulative growth metrics |
| 09 | **Performance Analysis** | KPI benchmarking and target vs. actuals comparisons |
| 10 | **Data Segmentation** | Customer and product grouping using clustering logic |
| 11 | **Part-to-Whole Analysis** | Proportional breakdowns — share of revenue, category mix |
| 12 | **Report: Customers** | Consolidated customer report with key behavioral metrics |
| 13 | **Report: Products** | Consolidated product report with sales and category insights |

---

## 🗄️ Data Sources

The project uses data from two business systems, organized across three data layers:

| Layer | Description |
|-------|-------------|
| 🥉 **Bronze** | Raw, unprocessed source data from CRM and ERP systems |
| 🥈 **Silver** | Cleaned and standardized data after transformation |
| 🥇 **Gold** | Final dimensional model ready for analysis and reporting |

**Source Systems:**
- **CRM** — Customer relationship data including customer info, product catalog, and sales transactions
- **ERP** — Operational data including customer records, location hierarchies, and product categories

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **MySQL** | Primary database engine for all queries and analysis |
| **MySQL Workbench** | Query development, schema visualization, and result export |
| **CSV Files** | Data input/output format across all pipeline layers |

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```

2. **Set up the database**  
   Open MySQL Workbench, connect to your server, and run:
   ```sql
   source scripts/00_init_database.sql;
   ```

3. **Load datasets**  
   Import the CSV files from the `datasets/` folder into their corresponding tables, or use the init script if it handles loading.

4. **Run analyses in order**  
   Execute scripts sequentially from `01` through `13` for the full analytics flow:
   ```sql
   source scripts/01_database_exploration.sql;
   source scripts/02_dimensions_exploration.sql;
   -- ... continue through 13
   ```

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👤 About Me

I'm an aspiring **Data & AI Engineer** passionate about transforming raw data into meaningful business insights. This project reflects my hands-on approach to learning SQL analytics — from exploratory analysis to building structured reporting pipelines.

Feel free to reach out for collaboration, feedback, or inquiries related to this project!

---

> ⭐ *If you found this project useful, consider giving it a star!*
