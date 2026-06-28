# Raw Orders Data

**File:** raw_orders.xlsx  
**Status:** Active Data File  
**File Size:** 121.7 KB  
**Last Updated:** 2026-06-28

## Overview

This file contains the original, unprocessed order data in Excel format (.xlsx). The data has been uploaded and is ready for cleaning and analysis.

## File Information

- **Format:** Microsoft Excel (.xlsx)
- **Location:** `/data/raw_orders.xlsx`
- **Encoding:** Binary (Office Open XML)

## Expected Data Structure

Based on the data schema, the file should contain the following columns:

| Column | Data Type | Description |
|--------|-----------|-------------|
| order_id | Integer | Unique order identifier |
| order_date | Date | Date when order was placed |
| ship_date | Date | Date when order was shipped |
| customer_id | Integer | Unique customer identifier |
| customer_name | Text | Name of the customer |
| segment | Text | Customer segment |
| region | Text | Geographic region |
| state | Text | State/Province |
| city | Text | City name |
| category | Text | Product category |
| sub_category | Text | Product sub-category |
| product_name | Text | Name of the product |
| ship_mode | Text | Shipping method |
| quantity | Integer | Number of items ordered |
| unit_price | Decimal | Price per unit |
| discount | Decimal | Discount percentage or amount |
| sales | Decimal | Total sales amount |
| cost | Decimal | Cost of goods sold |
| profit | Decimal | Profit amount |
| payment_status | Text | Payment status (Pending, Completed, Failed, etc.) |
| order_status | Text | Order status (Pending, Completed, Cancelled, etc.) |

## Data Quality Notes

- The raw data may contain:
  - Missing or null values
  - Inconsistent formatting
  - Duplicate entries
  - Invalid data types
  - Outliers or anomalies

These issues should be identified and handled during the data cleaning process.

## Next Steps

1. **Data Exploration:** Load and examine the raw data to understand its structure and content
2. **Data Cleaning:** Remove duplicates, handle missing values, standardize formats
3. **Data Validation:** Verify data integrity and consistency
4. **Data Documentation:** Update this file with actual data schema and statistics once analysis is complete

## Related Files

- `cleaned_orders_placeholder.md` - Placeholder for cleaned data documentation
- `raw_orders_placeholder.md` - Original placeholder file

---

*Data File Activated: 2026-06-28*
