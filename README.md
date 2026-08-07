# Airbnb-Data-Analysis-project
An end-to-end Python data analysis project analyzing Airbnb listings, availability, and reviews in Athens, Greece.

## Project Overview
This project processes raw Airbnb datasets to perform thorough data cleaning and extract meaningful business metrics regarding market revenue, host performance, and pricing efficiency.

## Tech Stack & Libraries
 * **Python**
 * **Pandas** (Data manipulation & cleaning)
 * **NumPy** (Numerical operations & conditional logic)

## Workflow & Features

### Part A: Data Pipeline & Cleansing
* **Multi-dataset Processing:** Merged and normalized `Listings`, `Calendar`, and `Reviews` DataFrames.
* **Type Conversion & Formatting:** Cleaned currency (`$`) and rate metrics (`%`) into numeric floats. Parsed dates into uniform datetime formats.
* **Data Imputation & Feature Engineering:** Imputed missing values (`Unknown` for text, `mode` for response metrics) and removed completely empty metadata columns.
* **Outlier Handling:** Applied boundary clips on minimum/maximum booking nights and filtered high-end listing price anomalies (< €2000 filter).

### Part B: Exploratory Data Analysis & Insights
* **Top Profitable Areas:** Computed total & average revenue per neighborhood to highlight top-earning zones in Athens (e.g., Σταθμός Λαρίσης, Πεδίο Άρεως, Θησείο).
* **Host Performance Analysis:** Aggregated overall reviews per listing to determine dominant market actors.
* **Pricing Efficiency Metric:** Evaluated active listings based on `Revenue per Available Day` to identify optimal pricing strategies.
