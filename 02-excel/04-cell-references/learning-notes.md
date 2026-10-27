# Learning Notes: Cell References

## 1. What Is a Cell Reference?

A cell reference identifies a cell in a spreadsheet.

For example:

- `A1` refers to column A, row 1.
- `B3` refers to column B, row 3.
- `F1` refers to column F, row 1.

Cell references allow formulas to use values stored in other cells.

## 2. Relative Cell References

A relative reference adjusts when a formula is copied to another location.

Example:

```excel
=B2*C2
```

If this formula is entered in D2 and copied to D3, it becomes:

```excel
=B3*C3
```

Both references adjust because the formula has moved down one row.

### When to Use Relative References

Use relative references when each row needs to calculate using values from that same row.

Examples include:

- Calculating sales for each product.
- Calculating total expenses for each transaction.
- Calculating revenue for each order.

## 3. Absolute Cell References

An absolute reference keeps both the column and row fixed when a formula is copied.

Example:

```excel
=B2*$F$1
```

Here:

- `B2` is a relative reference.
- `$F$1` is an absolute reference.

If the formula is copied from D2 to D3, it becomes:

```excel
=B3*$F$1
```

The product-price reference changes, but the reference to F1 remains fixed.

### Understanding the Dollar Signs

In `$F$1`:

- `$F` locks column F.
- `$1` locks row 1.

### When to Use Absolute References

Absolute references are useful when multiple formulas need to refer to the same cell.

Examples include:

- Applying a standard discount rate.
- Using a fixed tax rate.
- Applying a common commission percentage.
- Referring to a fixed assumption in a financial model.

## 4. Mixed Cell References

A mixed reference locks either the column or the row, but not both.

### Column Locked: `$F1`

The column stays fixed, while the row can change.

For example, copying a formula containing `$F1` down one row changes the reference to:

```excel
$F2
```

### Row Locked: `F$1`

The row stays fixed, while the column can change.

For example, copying a formula containing `F$1` one column to the right changes the reference to:

```excel
G$1
```

### When to Use Mixed References

Mixed references are useful when formulas need to move across rows or columns while keeping one part of a reference fixed.

For example, they can be used in tables that calculate values using different rates listed across a row or down a column.

## 5. Comparison of Cell References

| Reference | Column | Row | Behaviour |
|---|---|---|---|
| `F1` | Relative | Relative | Both can change |
| `$F$1` | Fixed | Fixed | Neither changes |
| `$F1` | Fixed | Relative | Only the row can change |
| `F$1` | Relative | Fixed | Only the column can change |

## 6. Practical Example: Product Discounts

Suppose a store has the following data:

| Product | Original Price | Discount Rate |
|---|---:|---:|
| Notebook | ₹100 | 10% |
| School Bag | ₹800 | 10% |
| Water Bottle | ₹200 | 10% |
| Calculator | ₹500 | 10% |

### Using Relative References

If the original price is in column B and the discount rate is in column C, enter this formula in D2:

```excel
=B2*C2
```

Copy the formula down to calculate discounts for the other products.

### Using Absolute References

Suppose the standard discount rate is stored in F1.

Enter this formula in D2:

```excel
=B2*$F$1
```

Copy it down the column.

The reference to F1 stays fixed, while the price reference changes for each product.

If F1 changes from 10% to 15%, the formulas recalculate automatically.

## 7. Important Lessons

- A cell reference identifies a spreadsheet cell.
- Relative references adjust when formulas are copied.
- Absolute references lock both the row and column.
- Mixed references lock either the row or the column.
- The dollar sign determines which part of a reference stays fixed.
- Absolute references lock the cell reference, not the value stored in the cell.
- Correct formulas still depend on using the correct cells and data.

## 8. Excel and Google Sheets

Relative, absolute, and mixed references work in both Microsoft Excel and Google Sheets.

The same reference syntax applies in both applications.

## Summary

Cell references help make spreadsheet formulas reusable and efficient.

Understanding how references behave when formulas are copied helps prevent calculation errors and makes it easier to build spreadsheets for business analysis.