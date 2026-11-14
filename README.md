> Dataset attribution: Original dataset "Cafe Sales Dirty Data for Cleaning Training" authored by ahmedmohamed2003 (via Kaggle), licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). 📦

# Retail Sales Data Cleansing & Processing Script 🚀

A lightweight Python script designed to ingest, audit, and sanitize raw point-of-sale (POS) transactional records into business-ready analytical assets. 📊

## Project Overview 🎯
Real-world operational data often contains noise, formatting inconsistencies, and systemic errors. This repository demonstrates a pragmatic data cleaning workflow using Python and Pandas to transform a messy retail/F&B transactional dataset into a clean, reliable structure without manipulating or fabricating missing business records. ☕

## Data Cleansing Methodology & Workflow 🛠️

The data cleansing workflow is executed through a rigorous and sequential series of engineering steps. At the initial stage, the raw dataset comprising 10,000 raw point-of-sale records is ingested directly into the Python environment to inspect structural integrity, assess missing value distributions, and generate fundamental statistical summaries for a comprehensive baseline overview. Immediately following the audit, regular expressions are deployed to hunt down, isolate, and eliminate corrupted tracking strings, system error logs, and placeholder artifacts scattered across various columns. These irregular text markers are precisely converted into standardized null values to safeguard downstream analytical accuracy.

The subsequent phase focuses on robust type casting, where financial attributes such as unit prices and total expenditures are processed via error-coercion mechanisms to silently neutralize formatting conflicts. Simultaneously, quantity metrics and transaction timestamps are restructured into rigorous, standardized formats, routing any parsing discrepancies straight into safe null states. The core guiding principle throughout this entire process is an absolute commitment to preserving empirical truth: missing values are never artificially imputed, filled with averages, or fabricated with synthetic estimates. Maintaining these natural gaps preserves the authentic integrity of financial data and strictly adheres to rigorous corporate auditing standards. Ultimately, the finalized assets are compiled and exported into clean, structured formats via Google Drive integration, positioning them for immediate deployment in business intelligence and reporting dashboards.

## Tech Stack 💻
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy
* **Environment:** Google Colab, Google Drive
* 
