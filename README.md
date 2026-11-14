 > Dataset attribution: Original dataset "Cafe Sales Dirty Data for Cleaning Training" authored by ahmedmohamed2003 (via Kaggle), licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/). 📦

# Retail Sales Data Cleansing & Processing Script 🚀

A lightweight script designed to clean and prepare raw point-of-sale (POS) transactional records into reliable analytical assets. 📊

## Project Overview 🎯
Real-world operational data often contains noise, formatting inconsistencies, and errors. This repository demonstrates a practical data cleaning workflow to transform a messy retail and F&B transactional dataset into a clean structure without tampering with or fabricating missing business records. ☕

## Data Cleansing Methodology & Workflow 🛠️

The cleaning pipeline handles raw transactional records through clear, systematic steps:
* **Initial Audit:** Inspected the raw data structure, checked for missing values, and evaluated overall data quality to understand the baseline conditions.
* **Noise Elimination:** Identified and isolated corrupted tracking artifacts, system logs, and placeholder strings, clearing them out to prevent skewed results down the line.
* **Format & Type Refinement:** Standardized financial fields and transaction timestamps to ensure clean and consistent structures across all records.
* 🔥 **The "No-Imputation" Principle (Better missing than fabricated!):** Rows with missing values or purged anomalies were **intentionally left blank**. *Why? Because in business and financial analytics, guessing or faking missing numbers introduces artificial bias. We preserve natural gaps to protect real-world data integrity and accuracy—no fake numbers allowed!* 🛡️
* **Export & Persistence:** Compiled and exported the finalized dataset into structured formats via Google Drive for easy reporting and dashboard integration.

## Tech Stack 💻
* **Language:** Python
* **Environment:** Google Colab, Google Drive
* 
