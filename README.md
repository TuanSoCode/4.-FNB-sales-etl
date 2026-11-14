> Dataset attribution: Original dataset "Cafe Sales Dirty Data for Cleaning Training" authored by ahmedmohamed2003 (via Kaggle), licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). 📦

# Retail Sales Data Cleansing & Processing Script 🚀

A lightweight Python script designed to ingest, audit, and sanitize raw point-of-sale (POS) transactional records into business-ready analytical assets. 📊

## Project Overview 🎯
Real-world operational data often contains noise, formatting inconsistencies, and systemic errors. This repository demonstrates a pragmatic data cleaning workflow using Python and Pandas to transform a messy retail/F&B transactional dataset into a clean, reliable structure without manipulating or fabricating missing business records. ☕

## Data Cleansing Methodology & Workflow 🛠️

The cleaning pipeline processes 10,000 raw transactional records through strict systematic steps:
* **Ingestion & Audit:** Loaded raw POS data and inspected structural integrity, missing values, and statistical distributions (`df.info()`, `df.describe()`).
* **Noise Elimination:** Used regular expressions to hunt down and isolate corrupted tracking artifacts, system logs, and placeholder strings (`ERROR`, `UNKNOWN`), converting them into clean null values (`np.nan`).
* **Safe Type Casting:** Enforced robust numerical parsing on financial fields (`Price Per Unit`, `Total Spent`) via error-coercion (`pd.to_numeric(errors='coerce')`) and standardized transaction timestamps.
* 🔥 **The "No-Imputation" Principle :** Rows with missing values (`NaN`) or purged anomalies were **intentionally left blank**. *Why? Because in financial and business data analytics, artificially guessing, estimating, or filling missing values with mean/median or fake placeholders introduces synthetic bias. Preserving natural gaps protects the authentic integrity of the data and honors real-world auditing standards—we don't fake numbers!* 🛡️
* **Export & Persistence:** Compiled and exported the sanitized dataset into structured formats (`.xlsx` / CSV) via Google Drive integration.

## Tech Stack 💻
* **Language:** Python 3.x
* **Libraries:** Pandas, NumPy
* **Environment:** Google Colab, Google Drive
* 
