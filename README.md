# World Layoffs Data Cleaning and Analysis (MySQL)

I cleaned a raw dataset of company layoffs, then explored it to find trends.
I built this by following Alex The Analyst's SQL tutorial, which also provided the dataset.

## Data cleaning
- Created staging tables to keep the raw data unchanged
- Removed duplicates using ROW_NUMBER() and a CTE
- Standardised company, industry and country names
- Converted dates from text to DATE format using STR_TO_DATE
- Filled in missing industries using a self join
- Removed rows with no useful layoff data and dropped a helper column

## Exploratory data analysis
- Total layoffs by company, industry, country and year
- Monthly layoffs with a rolling total, using a CTE and a window function
- Top companies by layoffs each year, using DENSE_RANK()

## Files
- `layoffs_data_cleaning.sql`: the cleaning script
- `layoffs_exploratory_analysis.sql`: the analysis script
- `layoffs_raw.csv`: the original data

## Tools
MySQL, MySQL Workbench
