# Learning Notes: Basic Spreadsheet Functions

## 1. What Is a Function?

A function is a predefined calculation available in a spreadsheet application.

Functions can be used within formulas to perform calculations efficiently.

Examples:

- `=SUM(B2:B6)`
- `=AVERAGE(B2:B6)`
- `=MIN(B2:B6)`
- `=MAX(B2:B6)`

## 2. SUM()

The `SUM()` function adds numerical values in a specified range.

Example:

`=SUM(B2:B6)`

This adds the values in cells B2 through B6.

Business applications include:
- Total sales
- Total expenses
- Total units sold
- Total revenue

## 3. AVERAGE()

The `AVERAGE()` function calculates the arithmetic mean of the numerical values in a range.

Example:

`=AVERAGE(B2:B6)`

The average is calculated by dividing the sum of the included numeric values by the number of those values.

Business applications include:
- Average sales per product
- Average order value
- Average monthly expenses

## 4. MIN()

The `MIN()` function returns the smallest numerical value in a range.

Example:

`=MIN(B2:B6)`

Business applications include:
- Lowest sales
- Lowest product price
- Minimum expense

## 5. MAX()

The `MAX()` function returns the largest numerical value in a range.

Example:

`=MAX(B2:B6)`

Business applications include:
- Highest sales
- Highest product price
- Maximum expense

## 6. Understanding Cell Ranges

A range identifies a group of cells.

For example:

`B2:B6`

This range includes B2, B3, B4, B5, and B6.

The colon (`:`) separates the starting and ending cell references.

Using ranges makes formulas shorter and easier to maintain.

## 7. Formula Versus Function

A formula is an expression that performs a calculation.

A function is a predefined operation that can be used within a formula.

Examples:

- `=B2*C2` — formula using multiplication.
- `=SUM(B2:B6)` — formula using the SUM function.
- `=SUM(B2:B6)*10%` — formula combining a function and an arithmetic operation.

## 8. Business Example

A stationery store records sales for five products.

| Product | Quantity Sold | Price per Unit | Total Sales |
|---|---:|---:|---:|
| Notebook | 20 | ₹50 | ₹1,000 |
| Pen | 50 | ₹10 | ₹500 |
| School Bag | 5 | ₹800 | ₹4,000 |
| Pencil Box | 15 | ₹100 | ₹1,500 |
| Water Bottle | 10 | ₹150 | ₹1,500 |

Individual sales are calculated using:

`=B2*C2`

The formula is copied down for the remaining products.

Summary formulas:

- Total revenue: `=SUM(D2:D6)`
- Average sales: `=AVERAGE(D2:D6)`
- Lowest sales: `=MIN(D2:D6)`
- Highest sales: `=MAX(D2:D6)`

## 9. Results and Interpretation

| Metric | Result | Interpretation |
|---|---:|---|
| Total Revenue | ₹8,500 | Combined sales value of all five products |
| Average Sales | ₹1,700 | Mean sales value per product |
| Lowest Sales | ₹500 | Pen has the lowest sales value |
| Highest Sales | ₹4,000 | School Bag has the highest sales value |

These results describe this small fictional dataset. They do not establish profitability because product costs and other expenses have not been provided.

## 10. Important Points to Remember

1. `SUM()` adds numerical values.
2. `AVERAGE()` calculates the arithmetic mean.
3. `MIN()` finds the smallest numerical value.
4. `MAX()` finds the largest numerical value.
5. Cell ranges make formulas easier to read.
6. Functions reduce repetitive manual calculations.
7. Incorrect ranges or source data can still produce incorrect results.
8. Excel and Google Sheets support these basic functions.