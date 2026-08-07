## Table of Contents
- **python_notebook/**: Contains the Jupyter Notebook with the end-to-end data analysis pipeline.
- **presentation/**: Contains the technical PowerPoint presentation detailing the analysis results and the step-by-step methodology followed.

## Instructions / Usage
1. **Explore the Python Notebook**:
   - Open the notebook file (`airbnb-python-data-analytics.ipynb`) to review the steps followed during the analysis. Due to large file sizes, raw datasets are not uploaded to this repository.
2. **Tech Stack & Libraries**
* **Python**
* **Pandas** (Data manipulation & cleaning)
* **NumPy** (Numerical operations & conditional logic)

## About the Project
This project was created as part of the course ["Python & Pandas: Comprehensive Data Analysis"](https://datatutor.gr/courses/python-pandas-data-analysis) by Data Tutor, under the guidance of [Alexandra Athanasakou](https://datatutor.gr/your-data-tutor).

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

## Data Source
The data used in this project is sourced from Airbnb and can be accessed through the following link:
- [Inside Airbnb](https://insideairbnb.com/get-the-data/)

The data is made available by Inside Airbnb and is used here under the terms of their dataset access policy. Please refer to the [Inside Airbnb Data Terms](https://insideairbnb.com/get-the-data/) for more details about the dataset and its usage.
