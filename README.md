# 🚨 Layoffs Data Cleaning & Analysis Project

## 📌 Overview
This project focuses on cleaning and preparing a real-world layoffs dataset using SQL.  
The goal is to transform raw data into a structured and analysis-ready format by removing duplicates, handling missing values, and standardizing inconsistent data.

---

## 🗂️ Dataset
The dataset contains global company layoff records including:
- Company name
- Location
- Industry
- Number of employees laid off
- Percentage of layoffs
- Date
- Funding information

---

## 🧹 Data Cleaning Process

### 1. Creating Staging Tables
- Created a staging table to preserve original data
- Copied raw data into working tables for transformation

### 2. Removing Duplicates
- Used `ROW_NUMBER()` window function
- Partitioned by all key columns
- Removed duplicate rows

### 3. Standardizing Data
- Trimmed whitespace from text fields
- Standardized industry names (e.g., "crypto")
- Cleaned country values (removed trailing dots)
- Converted date column to proper DATE format

### 4. Handling Missing Values
- Identified NULL values in key columns
- Filled missing industry values using self-join
- Removed rows where both key metrics were NULL

### 5. Final Cleanup
- Dropped helper columns used for transformation

---

## 🛠️ SQL Techniques Used
- CREATE TABLE AS SELECT
- INSERT INTO SELECT
- CTE (Common Table Expressions)
- ROW_NUMBER() Window Function
- JOIN operations
- UPDATE statements
- Data type conversion (STR_TO_DATE)
- DELETE operations
- ALTER TABLE

---

## 📊 Key Insights from Data Preparation
- Duplicate records were present and successfully removed
- Inconsistent text formatting was standardized
- Missing values were partially recovered using relational logic
- Dataset is now clean and ready for analysis or visualization

---

## 🎯 Purpose of This Project
This project demonstrates real-world data cleaning skills used in Data Analysis roles, including:
- Data preprocessing
- Data quality improvement
- SQL transformation techniques

---

## 🚀 Future Improvements
- Build dashboards using Power BI or Tableau
- Perform exploratory data analysis (EDA)
- Create predictive models for layoffs trends

---

## 👨‍💻 Tools Used
- SQL (MySQL / PostgreSQL compatible)
- Data Cleaning Techniques
- Window Functions
