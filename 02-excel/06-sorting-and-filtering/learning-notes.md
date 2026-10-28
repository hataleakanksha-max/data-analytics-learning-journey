# Learning Notes: Sorting and Filtering Data

## 1. What Is Sorting?

Sorting arranges records in a particular order.

Examples include:

- Product names from A to Z.
- Prices from smallest to largest.
- Sales from largest to smallest.
- Dates from oldest to newest.

### Example

Suppose a store records the following sales:

| Product | Total Sales |
|---|---:|
| Notebook | ₹1,000 |
| School Bag | ₹4,000 |
| Headphones | ₹24,000 |

Sorting Total Sales from largest to smallest produces:

| Product | Total Sales |
|---|---:|
| Headphones | ₹24,000 |
| School Bag | ₹4,000 |
| Notebook | ₹1,000 |

The records are reordered, but their associated values remain together.

## 2. Sorting in Microsoft Excel

1. Select a cell within the dataset.
2. Open the Data tab.
3. Choose Sort.
4. Select the column to sort by.
5. Choose the required order.
6. Confirm that the dataset has headers and apply the sort.

For a simple ascending or descending sort, the relevant options may also be available directly on the Data tab.

## 3. Sorting in Google Sheets

1. Select the complete dataset.
2. Open Data.
3. Choose Sort range and, if needed, Advanced range sorting options.
4. Confirm that the data has a header row.
5. Select the sorting column and the required order.
6. Apply the sort.

Menu labels may differ slightly between application versions.

## 4. Why Sort the Complete Table?

Sorting only one column can separate values from their corresponding records.

For example, if sales amounts are sorted without moving the product names, a product could appear to have another product's sales.

Always sort the complete dataset or use the spreadsheet's sort feature so that entire records stay together.

## 5. What Is Filtering?

Filtering displays only records that meet selected conditions. Other records are temporarily hidden, not deleted.

Examples:

- Show only Accessories products.
- Display products priced above ₹500.
- Show products with more than 10 units sold.
- Display only Electronics products.

## 6. Filtering in Microsoft Excel

1. Select the dataset.
2. Open Data and select Filter.
3. Open the dropdown in the required column.
4. Select the values or conditions to display.
5. Apply the filter.

## 7. Filtering in Google Sheets

1. Select the dataset.
2. Open Data and select Create a filter.
3. Open the filter dropdown in the relevant column.
4. Choose the values or conditions.
5. Apply the filter.

Both applications allow filtering by selected text values and numerical conditions.

## 8. Numerical Filtering

Numerical filters help answer business questions.

Common conditions include:

- Greater than: `> 10`
- Greater than or equal to: `>= 10`
- Less than: `< 15`
- Less than or equal to: `<= 15`
- Equal to: `= 500`

For example, a filter for Quantity Sold greater than 10 excludes records with a quantity of exactly 10.

## 9. Filtering Multiple Columns

Filters can be applied to multiple columns simultaneously.

For example:

- Category = Accessories
- Quantity Sold > 10

A record must meet both selected column filters to remain visible.

From the practice dataset, Mouse is the only Accessories product with a quantity sold greater than 10.

## 10. Understanding AND and OR

### AND

AND requires every specified condition to be true.

Example:

- Price > ₹100 AND Quantity Sold > 10.

A product must satisfy both conditions.

### OR

OR requires at least one specified condition to be true.

Example:

- Category = Electronics OR Price > ₹500.

A product qualifies if it belongs to Electronics, has a price above ₹500, or satisfies both conditions.

Multiple ordinary spreadsheet column filters generally combine as AND across columns. To express more complex OR logic, use suitable filter options, helper columns, or formulas as appropriate.

## 11. Clearing Filters

Clear filters when you want to see the full dataset again.

This matters because someone viewing a filtered spreadsheet may mistakenly believe that the visible records represent all available data.

Clearing filters does not delete the records that were hidden.

## 12. Practical Dataset

The lesson used this fictional dataset:

| Product | Category | Quantity Sold | Price (₹) | Total Sales (₹) |
|---|---|---:|---:|---:|
| Notebook | Stationery | 20 | 50 | 1,000 |
| Pen | Stationery | 50 | 10 | 500 |
| School Bag | Accessories | 5 | 800 | 4,000 |
| Water Bottle | Accessories | 10 | 150 | 1,500 |
| Pencil Box | Stationery | 15 | 100 | 1,500 |
| Calculator | Electronics | 8 | 500 | 4,000 |
| Headphones | Electronics | 12 | 2,000 | 24,000 |
| Mouse | Accessories | 25 | 400 | 10,000 |

## 13. Important Results

- Highest total sales: Headphones, ₹24,000.
- Accessories products: School Bag, Water Bottle, and Mouse.
- Electronics products: Calculator and Headphones.
- Products with Quantity Sold greater than 10: Notebook, Pen, Pencil Box, Headphones, and Mouse.
- Products with Price greater than ₹500: School Bag and Headphones.
- Products with Quantity Sold less than 15: School Bag, Water Bottle, Calculator, and Headphones.
- Accessories with Quantity Sold greater than 10: Mouse.
- Products with Price greater than ₹100 AND Quantity Sold greater than 10: Headphones and Mouse.

## Summary

Sorting organizes records into a chosen order. Filtering displays records that meet specified conditions. Both techniques are essential for exploring datasets and answering business questions efficiently.