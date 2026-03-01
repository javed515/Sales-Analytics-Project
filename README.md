📊 Strategic Sales & Product Analytics Dashboard. Executive-Level Insights using SQL Server & Power BI

🎯 Project Objective
This project was developed to fulfill a strategic "Request from Management" for a high-level Product Analytics Overview. As a Senior Executive in Global Business Development, I designed this solution to bridge the gap between raw transactional data and executive decision-making, leveraging my MBA in International Business to provide context-rich insights.

The dashboard transforms complex sales data into actionable intelligence, enabling stakeholders to monitor global revenue, track year-over-year growth, and refine pricing strategies.

🏢 Business Case & Requirements
Following a simulated brief from stakeholders, the dashboard addresses key business questions:

- Global Revenue Analysis: High-level identification of top-performing regions to guide expansion strategies.
- Comparative Growth Trends: Visualizing Revenue and Profit trajectories across 2022 and 2023.
- KPI Tracking (YoY): Dynamic Year-over-Year metrics for Profit and Units Sold to measure operational efficiency.
- Pricing Strategy Insights: Analyzing revenue distribution across Discount Bands to optimize margin vs. volume.
- Operational Detail: A granular table view for deep-dives into customer types and specific regional performance.

🛠️ Technical Implementation & Problem Solving
This project showcases an end-to-end data pipeline, moving from raw SQL extraction to advanced DAX modeling.

1. Data Extraction (SQL)
Extracted multi-table sales data from SQL Server.
Utilized optimized queries to join product details and regional performance tables, ensuring data consistency before ingestion.
2. Data Transformation (Power Query)
The Locale Challenge: Resolved a critical data integrity issue where DD-MM-YYYY dates were misinterpreted by Power BI’s default settings.
Solution: Utilized Locale-based transformations to ensure accurate time-series analysis and prevent reporting errors.
3. Data Modeling (DAX & Star Schema)
The "Contiguous Date" Solution: To overcome errors with standard Time Intelligence functions, I designed a custom DAX Calendar Table.
Relationships: Established a 1-to-many relationship between the Calendar Table and the Sales Table to enable robust YoY reporting and dynamic filtering.

🔍 Key Findings & Analytical Insights
The following metrics represent high-level growth captured through the dashboard's dynamic filtering system for top-performing product lines (e.g., Arctis 7P+, NTP1-A):

Metric	Insight	Impact
- Profitability	109% Profit YoY increase	Demonstrates the success of optimized regional sales strategies for flagship products.
- Volume 108% Growth in Units Sold. Validated through DAX-driven time-intelligence measures.
- Market Leadership	US & Mexico Dominance	Identified these regions as primary revenue drivers across multiple categories.
- Revenue Mix	"Medium" Discount = 34% Sales	Discovered that mid-tier discount bands are highly effective, suggesting a pricing strategy sweet spot.
- Scalability	Dynamic Category Selection	Engineered to process and visualize unique performance trends for all 6 product categories instantly.

📁 Repository Structure
├── 📂 Data/ # Raw CSV source files used for the analysis
├── 📂 Dashboard/ # The final .pbix Power BI file
├── 📂 Screenshots/ # Visual captures of the Dashboard and Data Model
├── 📄 extraction_query.sql # The SQL logic used for data retrieval
└── 📄 README.md # Project documentation

---

👤 About the Author

**Javed Ansari**

*   **Current Role:** Senior Executive, Global Business Development at Newgen Software.
*   **Education:** MBA in International Business (Jamia Millia Islamia) | B.Com Hons (Delhi University).
*   **Focus:** Leveraging Data Analytics (SQL, Power BI) to drive international business growth and strategic expansion.
