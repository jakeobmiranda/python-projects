Introduction
This repository is a collection of Python projects designed for data exploration, with a primary focus on Pandas and NumPy. The exercises scale from foundational DataFrame operations to complex, multi-table workflows that resemble real-world business analysis scenarios. The intent is to build fluency in data cleaning, aggregation, joins, time-series logic, and KPI-style reporting.

The notebooks are presented as end-to-end business analysis projects implemented with Pandas and NumPy, covering multi-table data integration, missing data handling, time-series analysis, customer segmentation, and performance reporting across e-commerce, healthcare, retail, web analytics, and sales operations.

Projects
Transaction Analysis with Cumulative Logic and Customer Identification
- Analyzes customer transaction data including purchases and returns. Identifies top customers by spend, calculates cumulative spending patterns over time, and segments transaction types using conditional logic.
- Techniques: datetime conversion, lambda functions, boolean indexing, cumulative aggregation, Series combination, idxmax/idxmin for identification.

Web Traffic Clickstream Analysis and Conversion Rate Reporting
- Analyzes website session data to calculate conversion rates by device type, identify user navigation patterns, and measure session engagement.
- Techniques: boolean aggregation with .any() and .mean(), multi-step aggregation pipelines, drop_duplicates for top-N identification, transform for session-level metrics, conversion rate calculation.

Sales Team Performance Analysis with Quarter-over-Quarter Trends
- Evaluates sales representative performance across quarters including win rates, revenue ranking, and quarter-over-quarter revenue change analysis.
- Techniques: date arithmetic, .shift() for period-over-period comparison, .rank(), .agg() with named aggregations, nested conditional labeling.

Customer Support Ticket SLA Compliance Analysis
- Analyzes support ticket resolution times against SLA targets by priority level. Includes agent performance scoring, repeat customer identification, and compliance rate reporting.
- Techniques: timedelta calculations with .dt.total_seconds(), pivot tables, .map() with dictionary lookups, boolean indexing on aggregated results, SLA target mapping.

E-Commerce Order Analysis with Revenue Reporting and Growth Metrics
- Analyzes e-commerce order data including discount impact, shipping performance, customer tiering by spend, top product identification with percentage-of-total analysis, and month-over-month revenue growth tracking.
- Techniques: pivot tables with margins, percentage of total calculations, customer segmentation with lambdas, .nlargest(), month-over-month growth with .shift().

Multi-Store Retail Analysis with Data Integration and Performance Mapping
- Integrates sales transaction data with store master data, handles missing values with group-specific imputation, identifies unmatched records across datasets, and maps regional performance labels.
- Techniques: multi-file imports, left joins with unmatched record detection, .notna(), .copy(), cumulative calculations, .shift() for percentage change, .map() with dictionary comprehensions, .agg() with nunique, .isin() filtering.

Hospital Visit Analysis with Patient Segmentation and Cost Tracking
- Analyzes hospital visit data across departments and doctors, integrating patient visit records with physician data. Includes out-of-pocket cost analysis, SLA-style doctor performance scoring, repeat patient identification with diagnosis pattern analysis, and cumulative cost tracking.
- Techniques: two-file merges with missing data handling, inner vs left join comparison, pivot tables with margins, cumulative calculations, visit-over-visit percentage change, .agg() with nunique, .map() with dictionary comprehensions, boolean indexing on grouped results, .idxmax(), chaining merges, nested lambdas.

E-Commerce Repeat Customer Deep Dive with Regional Performance Benchmarking
- Deep analysis of repeat customer behavior including purchase patterns, cumulative revenue tracking, order-over-order revenue changes, and regional performance benchmarking with tier labeling.
- Techniques: repeat customer identification with boolean indexing, multi-step merges, .idxmax(), .cumsum() on transactional data, .shift() for sequential comparison, .agg() with nunique, .map() with dictionary comprehension, ranking, nested lambdas.

Technical Skills Demonstrated
- Data Integration & Quality: multi-source merging with various join types, missing value detection and group-specific imputation, unmatched record identification, data type conversion.
- Aggregation & Reporting: multi-level groupby with named aggregations, pivot tables with margins, percentage-of-total analysis, conversion rate calculation, compliance rate reporting.
- Time-Series & Sequential Analysis: period-over-period comparison using shift, cumulative calculations, date arithmetic, datetime component extraction, growth rate computation.
- Customer & Entity Segmentation: conditional labeling with multi-tier logic, dictionary-based mapping, ranking and top-N identification, repeat entity detection with behavioral analysis.
- Data Reshaping & Identification: pivot tables, drop_duplicates for mode identification, idxmax/idxmin for entity lookup, boolean indexing on aggregated results.

Tools & Libraries
- Python 3
- Pandas
- NumPy
- Jupyter Lab

About This Repository
This repository demonstrates end-to-end analytics workflows, from ingesting and integrating multiple data sources through cleaning, transformation, and feature engineering, to producing stakeholder-style summaries such as KPI reporting, segmentation outputs, conversion and compliance rates, and time-based performance trends.
