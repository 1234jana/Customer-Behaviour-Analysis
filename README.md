# Customer Purchase Behavior Analytics
Customer Behaviour Analysis using Python, SQL, Excel, and Power BI to uncover customer purchasing patterns, revenue trends, and business insights through data analysis and interactive dashboards.

## Overview

This project analyzes a customer shopping behavior dataset to understand purchasing patterns, customer segments, and revenue trends. The workflow covers the full data analysis pipeline — from raw data cleaning in Python to storing the processed data in a PostgreSQL database, and finally visualizing key insights through an interactive Power BI dashboard.

## Tech Stack

- **Python** (Pandas) — data cleaning, transformation, and feature engineering
- **SQL / PostgreSQL** — database storage for cleaned data
- **SQLAlchemy & psycopg2** — Python-to-PostgreSQL connectivity
- **Power BI** — interactive dashboards and visualizations
- **MS Excel** — data review and reporting

## Project Workflow

1. **Data Loading** — Imported the raw customer shopping behavior dataset using Pandas.
2. **Data Cleaning**
   - Checked and handled missing values (imputed `Review Rating` using category-wise median).
   - Standardized column names to snake_case for consistency.
   - Removed redundant columns (e.g., duplicate `promo_code_used` column).
3. **Feature Engineering**
   - Created an `age_group` column by binning customer ages into quartiles (Young Adult, Adult, Middle-aged, Senior).
   - Created a `purchase_frequency_days` column by mapping purchase frequency categories (e.g., "Weekly", "Monthly") to numeric day values.
4. **Database Integration**
   - Connected to a PostgreSQL database using SQLAlchemy and psycopg2.
   - Loaded the cleaned dataset into a `customer` table for further querying and use in BI tools.
5. **Dashboard & Visualization**
   - Built interactive Power BI dashboards to visualize customer behavior, sales trends, and key business insights.

## Key Insights

- Identified customer segments based on age groups and purchasing frequency.
- Uncovered revenue trends across product categories.
- Highlighted patterns in discount usage and review ratings by category.

## How to Run

1. Clone this repository.
2. Install the required Python packages:
```bash
   pip install pandas sqlalchemy psycopg2-binary
```
3. Update the PostgreSQL connection details (username, password, host, database) in the notebook.
4. Run the Jupyter notebook to clean the data and load it into PostgreSQL.
5. Open the Power BI dashboard file to explore the visualizations.

## Files

- `Customer_behavior.ipynb` — Python notebook for data cleaning, feature engineering, and database loading.
- Power BI dashboard (`.pbix`) — interactive visualizations of customer behavior and sales insights.

## Author

**Janarthanan K**
[LinkedIn](https://linkedin.com/in/janarthanan-k-1804ab236) | [GitHub](https://github.com/1234jana)
