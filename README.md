# Vendors-Performance-Analysis
Ingested raw sales data into a SQLite3 database for structured storage and efficient querying. Performed data cleaning and transformation using Python, and created a summary table combining key performance metrics. the top 10 and bottom 10 vendors and brands based on total sales volume and revenue contribution to support business decision-making.

🚀 Features
📥 Ingest raw sales CSV data into SQLite3

🧹 Clean and preprocess data using Pandas

🧾 Generate a summary table with total sales, units sold, and average performance per vendor and brand

🔍 Identify top 10 and bottom 10 vendors and brands

📊 Visualize insights using Matplotlib and Seaborn

🛠️ Tech Stack
Python

Pandas / NumPy

SQLite3

SQLAlchemy (optional)

Matplotlib / Seaborn

📂 Data Flow

Data Ingestion
Import CSV into SQLite3 using sqlite3 or SQLAlchemy.

Data Cleaning & Transformation
Handle missing values, remove duplicates, convert date formats.

Summary Table Creation
Generate new tables aggregating:

total_sales

units_sold

avg_sales_per_transaction

Ranking & Insights
Sort and rank vendors and brands to identify:

Top 10 performers

Bottom 10 underperformers

Visualization
Use bar charts, heatmaps, and trend lines to display results.

📁 Project Structure
kotlin
Copy
Edit
├── data/

│   └── raw_sales.csv

├── scripts/

│   ├── ingest_data.py

│   ├── clean_transform.py

│   └── analyze_performance.py

├── results/

│   └── vendor_summary_table.csv

│   └── visualizations/

│       └── top_vendors.png

├── vendor_analysis.db

├── README.md

📌 Sample SQL Query
sql
Copy
Edit
SELECT vendor_name, brand_name, SUM(sales) AS total_sales
FROM sales_data
GROUP BY vendor_name, brand_name
ORDER BY total_sales DESC
LIMIT 10;

📊 Sample Visual
Bar chart of top 10 vendors by total sales (generated using Matplotlib)

📈 Outcome
Identified performance gaps between vendors and brands

Enabled targeted business decisions for vendor optimization

Established a repeatable, scalable workflow for sales data analytics.

🤝 Contributions
Feel free to fork this repo, suggest improvements, or use the analysis structure for similar data challenges.
