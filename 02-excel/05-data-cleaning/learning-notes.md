# Learning Notes: Basic Data Cleaning

## 1. What Is Data Cleaning?

Data cleaning is the process of identifying and handling inaccurate, incomplete, inconsistent, or duplicated data.

Clean data is important because poor-quality data can lead to incorrect calculations and misleading business decisions.

## 2. Duplicate Records

A duplicate record repeats information already present in a dataset.

For example:

| Product | Category | Quantity | Price |
|---|---|---:|---:|
| Notebook | Stationery | 10 | 50 |
| Notebook | Stationery | 10 | 50 |

These records appear identical. If they represent the same transaction entered twice, one is a duplicate.

However, identical-looking records are not always duplicates. Two separate legitimate transactions may contain the same values. Business context must be checked before deleting records.

### Removing Duplicates

In Microsoft Excel:

1. Select the dataset, including the headers.
2. Open the Data tab.
3. Choose Remove Duplicates.
4. Select the appropriate columns.
5. Confirm the operation.

In Google Sheets:

1. Select the dataset, including the headers.
2. Open Data.
3. Choose Data cleanup and then Remove duplicates.
4. Confirm the header-row setting.
5. Select the appropriate columns and confirm.

Always verify the remaining records after removing duplicates. If necessary, use Undo to reverse an accidental change.

## 3. Inconsistent Text

Text may contain inconsistent capitalization or unnecessary spaces.

Examples:

- `Stationery`
- `stationery`
- `Stationery `

These values may cause problems when filtering, grouping, or matching records.

Standardizing text helps improve consistency.

## 4. The TRIM() Function

The `TRIM()` function removes leading and trailing spaces and reduces repeated ordinary spaces between words to single spaces.

### Example

```excel
=TRIM(A2)
```

If A2 contains `  water bottle  `, the result is:

`water bottle`

TRIM works in Microsoft Excel and Google Sheets.

Note: TRIM does not remove every possible invisible character, such as certain nonbreaking spaces.

## 5. The PROPER() Function

The `PROPER()` function capitalizes the first letter of each word.

### Example

```excel
=PROPER(A2)
```

If A2 contains `water bottle`, the result is:

`Water Bottle`

### Combining TRIM() and PROPER()

These functions can be combined:

```excel
=PROPER(TRIM(A2))
```

If A2 contains ` water bottle `, the result is:

`Water Bottle`

TRIM removes unnecessary spaces, and PROPER standardizes capitalization.

Important: PROPER may not preserve special capitalization used in some names or abbreviations. Review the results before accepting them.

## 6. Missing Values

A missing value occurs when information is not available in a cell.

Example:

| Product | Quantity | Price |
|---|---:|---:|
| School Bag | | 800 |

The quantity is unknown, so total sales cannot be calculated reliably.

### How to Handle Missing Values

1. Check the original record or another reliable source.
2. Enter the verified value if it is available.
3. If the value cannot be verified, document the missing information.
4. Decide how to handle the missing value based on the analysis being performed.

### Missing Is Not the Same as Zero

A blank quantity does not mean that zero items were sold.

- Blank: the quantity is unknown or unrecorded.
- Zero: the confirmed quantity is zero.

Replacing a blank with zero without evidence can produce misleading results.

Missing values may affect different calculations in different ways, so their impact should be evaluated before analysis.

## 7. Preserve Original Data

It is safer to create cleaned values in new columns before replacing the original data.

Benefits include:

- Comparing original and cleaned values.
- Detecting formula errors.
- Preserving the original information.
- Reversing changes when necessary.

For example, keep the original product name in column A, use `=TRIM(A2)` in column B, and use `=PROPER(B2)` in column C.

## 8. Excel and Google Sheets

Both applications support the `TRIM()` and `PROPER()` functions and provide tools for removing duplicate records.

The menu layout may differ, but the underlying data-cleaning concepts are the same.

## Summary

Basic data cleaning involves identifying duplicates, correcting inconsistent text, removing unnecessary spaces, and handling missing information responsibly.

The goal is not simply to make a spreadsheet look neat. It is to improve data quality so that the resulting analysis is reliable and transparent.