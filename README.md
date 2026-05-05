# synent-task1-datacleaning-kwanele
Data cleaning and preprocessing of the Titanic dataset - Synent Technologies Data Science Internship

# Task 1 - Data Cleaning & Preprocessing

## Problem Statement
Raw datasets often contain missing values, duplicates, inconsistent data types,
and poorly named columns that make analysis unreliable. This project cleans and
prepares the Titanic dataset so it is ready for accurate analysis or modeling.

## Dataset
- **Name:** Titanic Dataset
- **File:** `train.csv`
- **Records:** 891 passengers
  

## Approach
1. **Loaded** the raw CSV using pandas
2. **Handled missing values:**
   - Filled missing `Age` values with the median age
   - Filled missing `Embarked` values with the mode
   - Dropped the `Cabin` column due to excessive missing data (77%)
3. **Removed duplicates** — checked and dropped any duplicate rows
4. **Converted data types:**
   - `Survived` and `Pclass` converted to category type
   - `Sex` and `Embarked` encoded as category
5. **Renamed columns** for clarity (e.g. `SibSp` → `siblings_spouses`)

## Results
- Reduced missing values from 866 to 0
- Dataset went from 12 to 11 columns (Cabin dropped)
- Clean, analysis-ready CSV exported as `titanic_cleaned.csv`
