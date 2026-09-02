# Data Cleaning and Preprocessing – DataX Labs Task 1

## 📌 Project Overview

This project focuses on cleaning and preprocessing a raw marketing campaign dataset using Python and Pandas. The objective was to identify and resolve common data quality issues such as missing values, duplicate records, inconsistent formats, and incorrect data types.

## 🎯 Objective

To clean and prepare a raw dataset for further data analysis and visualization.

## 🛠️ Tools Used

* Python
* Pandas
* Jupyter Notebook

## 📂 Dataset

The project uses the Marketing Campaign dataset, which contains customer demographic information, purchasing behavior, campaign responses, and other marketing-related attributes.

## 🔄 Data Cleaning Steps

The following preprocessing steps were performed:

* Loaded and inspected the dataset.
* Checked the dataset structure and data types using `df.info()`.
* Identified missing values using `df.isnull().sum()`.
* Found 24 missing values in the `Income` column.
* Filled missing income values using the median income.
* Checked for duplicate records.
* Found no duplicate rows in the dataset.
* Standardized column names by converting them to lowercase.
* Standardized categorical text values by removing unnecessary spaces and converting text to lowercase.
* Converted the `dt_customer` column to datetime format.
* Checked for invalid date values and found none.
* Checked numerical columns for negative values and found none.
* Identified unrealistic birth year records and removed records with `year_birth` before 1920.
* Identified potential outliers, including an unusually high income value, but retained them because they were not confirmed as invalid.
* Exported the cleaned dataset as a CSV file.

## 📊 Final Results

* Original Dataset: **2,240 rows × 29 columns**
* Missing Income Values: **24**
* Duplicate Rows: **0**
* Invalid Birth Year Records Removed: **3**
* Final Dataset: **2,237 rows × 29 columns**
* Final Missing Values: **0**
* Final Duplicate Rows: **0**

## 📁 Project Files

```text
DataX-Labs-Task-1-Data-Cleaning/
│
├── marketing_campaign.csv
├── cleaned_marketing_campaign.csv
├── data_cleaning_task1.ipynb
└── README.md
```

## ✅ Conclusion

The dataset was successfully cleaned and preprocessed using Pandas. Missing values were handled, data formats were standardized, invalid records were removed, and data quality checks were performed. The final cleaned dataset is structured and ready for further analysis, visualization, or machine learning.
