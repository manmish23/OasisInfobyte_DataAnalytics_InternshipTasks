# Task 2: Data Cleaning - Airbnb NYC Dataset

## Objective
Clean raw Airbnb dataset by handling missing values, outliers, duplicates and standardizing formats.

## Dataset
**Source**: Kaggle - New York City Airbnb Open Data  
**Original Size**: 48,895 rows × 16 columns

## Problems Found
1. 10,068 missing values in `last_review`
2. 10,052 missing values in `reviews_per_month` 
3. Price outliers: $0 and >$10,000 listings
4. Inconsistent text formatting

## Cleaning Steps Performed
1. Filled missing prices with median value
2. Filled `reviews_per_month` nulls with 0
3. Removed 25 outlier records with price < $10 or > $10,000
4. Converted `last_review` to datetime
5. Standardized text columns to lowercase

## Results
| Metric | Before | After |
| --- | --- | --- |
| Total Rows | 48,895 | 48,870 |
| Missing Values | 20,120+ | 0 |
| Memory Usage | 6.3 MB | 6.3 MB |

## Tools & Libraries
Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## Files
- `Task4_DataCleaning_AB_NYC.ipynb` - Main notebook with all code
- `AB_NYC_2019_CLEANED.csv` - Final cleaned dataset