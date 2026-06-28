# Part 1: Data Cleaning Project

This project focuses on data cleaning and quality assessment for order data.

## Project Structure

```
part1_data_cleaning/
├── data/
│   ├── raw_orders.xlsx          # Original order data
│   └── cleaned_orders.xlsx      # Cleaned and processed order data
├── outputs/
│   ├── data_quality_report.xlsx # Quality metrics and assessment
│   ├── pivot_summary.xlsx       # Summary pivot tables
│   └── cleaning_log.md          # Detailed cleaning steps and transformations
├── screenshots/
│   ├── raw_data_preview.png     # Preview of raw data
│   ├── cleaned_data_preview.png # Preview of cleaned data
│   ├── pivot_summary_1.png      # Pivot table visualization 1
│   └── pivot_summary_2.png      # Pivot table visualization 2
└── README.md                    # This file
```

## Overview

This repository contains the first part of a data cleaning workflow that includes:
- Raw order data in Excel format
- Cleaned and processed data
- Quality reports and summaries
- Visual documentation of the process

## Files Description

### Data Files
- **raw_orders.xlsx**: Original unprocessed order data
- **cleaned_orders.xlsx**: Data after cleaning, transformation, and validation

### Output Files
- **data_quality_report.xlsx**: Quality metrics, validation results, and data assessment
- **pivot_summary.xlsx**: Summary tables and pivot analysis
- **cleaning_log.md**: Detailed documentation of all cleaning steps and transformations applied

### Screenshots
Visual documentation showing before and after states of the data, including pivot table summaries.

## Getting Started

1. Review the raw data in `data/raw_orders.xlsx`
2. Check the cleaning log in `outputs/cleaning_log.md` for transformation details
3. View the cleaned data in `data/cleaned_orders.xlsx`
4. Examine quality reports and summaries in `outputs/`
5. Refer to screenshots for visual reference

---

*Project created on 2026-06-28*

# Data Cleaning & Quality Assessment Project

## Problem Summary

This project cleans, validates, and summarizes an order dataset for
reporting.

## Dataset Description

The dataset contains customer, order, shipping, product, sales, profit,
payment, and status fields.

## Tools Used

-   Microsoft Excel
-   Python (OpenPyXL)
-   Markdown

## Cleaning Steps Performed

-   Standardized text fields.
-   Standardized dates.
-   Added shipping delay.
-   Identified and handled duplicates.
-   Applied business rules.
-   Created quality reports and pivot summaries.

## Business Rules Applied

-   Missing region/ship_mode filled as Unknown.
-   Blank discount treated as 0 where applicable.
-   Invalid discounts flagged.
-   Ship date before order date flagged.
-   Cancelled and failed payments excluded from completed sales.
-   Refunded orders summarized separately.

## Summary of Data Quality Issues Found

-   Missing values
-   Duplicate records
-   Invalid discounts
-   Date issues
-   Order/payment status issues

## Summary of Final Pivot Reports

-   Sales & profit by region
-   Sales & profit by category/sub-category
-   Ship mode order counts
-   Profit margin by segment
-   Status by region
-   Monthly sales trend

## Key Business Insights

-   Regional performance varies.
-   Category profitability differs.
-   Shipping preferences are visible.
-   Monthly trends support planning.

## Assumptions and Limitations

-   Discount range assumed 0-1.
-   Domain-specific validation may require additional rules.

## Screenshots Included

-   Cleaned dataset
-   Data quality report
-   Pivot summary report
-   Cleaning log

