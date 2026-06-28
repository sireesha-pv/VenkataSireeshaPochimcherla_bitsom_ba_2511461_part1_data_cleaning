# Cleaning Log

## List of issues found

-   Extra spaces, inconsistent casing, and inconsistent category/text
    values.
-   Missing values in region, ship_mode, discount, and date fields.
-   Invalid/unrecognized dates and ship dates before order dates.
-   Exact duplicate rows and duplicate order IDs with conflicting
    information.
-   Invalid discounts (negative or above allowed range).
-   Cancelled orders, failed payments, and refunded orders requiring
    special handling.

## Cleaning actions performed

-   Trimmed spaces and standardized text casing.
-   Standardized category, ship mode, segment, and status values.
-   Converted dates to a consistent format where possible.
-   Added shipping delay calculation.
-   Removed exact duplicate rows.
-   Flagged conflicting duplicate order IDs.
-   Filled missing region and ship_mode with "Unknown".
-   Replaced blank discounts with 0 only where applicable.
-   Added flag columns for data quality and business rule issues.

## Business rules applied

-   Missing region → filled with **Unknown** and flagged.
-   Missing ship_mode → filled with **Unknown** and flagged.
-   Missing discount → treated as 0 only when appropriate.
-   Negative discount → flagged as invalid.
-   Discount above allowed range → flagged as invalid.
-   Ship date before order date → flagged as invalid shipping record.
-   Cancelled orders and failed payments excluded from completed sales
    summaries.
-   Refunded orders retained for separate reporting.

## Assumptions made

-   Valid discount range is 0--1.
-   Blank discounts can be treated as 0 only when other sales fields are
    valid.
-   Existing sales/profit values were not recalculated unless explicitly
    required.

## Records removed

-   Exact duplicate rows only.

## Records flagged

-   Conflicting duplicate order IDs.
-   Invalid discounts.
-   Invalid shipping records.
-   Missing region/ship_mode filled with Unknown.

## Limitations

-   Sales/profit mismatches were not recalculated from source formulas.
-   Some business-specific validations may require domain rules not
    present in the dataset.
