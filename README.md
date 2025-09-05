# ITBIN-2211-0106_data_cleaning

## Data Cleaning Functions
##  Overview

This project provides reusable data cleaning functions for handling missing values, duplicates, outliers, inconsistencies, and validating datasets. The cleaned data can then be exported for analysis or modeling.

## Functions

load_dataset(file_path) → Load CSV file into a pandas DataFrame.

handle_missing_values(df) → Fill missing values (rules for children, country, agent, company).

remove_duplicates(df) → Remove exact duplicate rows.

detect_outliers_iqr(df, column) → Identify outliers using IQR method.

treat_outliers(df, column) → Cap outliers within IQR bounds.

fix_inconsistencies(df) → Fix guest count, country code, and categorical inconsistencies.

validate_data(df) → Final integrity checks (guests > 0, valid years, ADR non-negative, valid categories).

export_clean_data(df, path) → Save cleaned dataset to CSV file.

## Requirements

Python 

pandas
