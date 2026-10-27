# Learning Notes: Basic Formulas and Cell References

## 1. What Is a Formula?

A formula is an expression that instructs a spreadsheet to perform a calculation.

In Excel and Google Sheets, formulas generally begin with an equals sign (`=`).

Example:

`=10+20`

Result: `30`

Formulas can use numbers directly or refer to values stored in other cells.

## 2. Basic Arithmetic Operators

| Operation | Symbol | Example | Purpose |
|---|---|---|---|
| Addition | `+` | `=A1+B1` | Adds two values |
| Subtraction | `-` | `=A1-B1` | Subtracts one value from another |
| Multiplication | `*` | `=A1*B1` | Multiplies two values |
| Division | `/` | `=A1/B1` | Divides one value by another |

## 3. What Is a Cell Reference?

A cell reference identifies a cell using its column letter and row number.

Examples:

- `A1`: Column A, row 1
- `B2`: Column B, row 2
- `C3`: Column C, row 3

Cell references allow formulas to use existing data instead of requiring numbers to be typed directly into every calculation.

Example:

`=B2*C2`

This multiplies the values in cells B2 and C2.

## 4. Business Example: Calculating Sales

Suppose a store sells notebooks.

| Product | Quantity Sold | Price per Unit |
|---|---:|---:|
| Notebook | 12 | 50 |

The total sales value is calculated as:

**Total Sales = Quantity Sold × Price per Unit**

Spreadsheet formula:

`=B2*C2`

Result: 600

If the price is in rupees, the result represents ₹600 in sales.

## 5. Copying Formulas

Excel and Google Sheets allow formulas to be copied into other cells.

For example:

| Cell | Formula |
|---|---|
| F2 | `=C2*D2` |
| F3 | `=C3*D3` |
| F4 | `=C4*D4` |

When the formula is copied down, the row references adjust automatically.

The fill handle is a convenient way to copy a formula into adjacent cells.

## 6. Relative Cell References

A relative cell reference changes when a formula is copied to another location.

For example, copying `=B2*C2` down one row normally changes it to `=B3*C3`.

This allows the same calculation to be applied to multiple records without rewriting every formula.

## 7. Automatic Recalculation

When a value referenced by a formula changes, the spreadsheet recalculates the result.

Example:

Original formula:

`=B3*C3`

Original values:
- B3 = 20
- C3 = 10

Result: 200

After changing B3 to 25:

- B3 = 25
- C3 = 10

New result: 250

The formula remains the same, but its result changes because the input value changed.

## 8. Why Formulas Matter in Data Analytics

Formulas are useful for:

- Calculating sales revenue
- Calculating expenses and profit
- Comparing prices
- Automating repetitive calculations
- Reducing manual calculation errors
- Updating results when source data changes

## 9. Important Points to Remember

1. Formulas generally begin with `=`.
2. `+` means addition.
3. `-` means subtraction.
4. `*` means multiplication.
5. `/` means division.
6. Cell references identify the values used in a formula.
7. Relative references adjust when formulas are copied.
8. Formula results can update automatically when input values change.

## 10. Excel and Google Sheets

The basic formulas covered in this lesson work in both Microsoft Excel and Google Sheets.

The interface may differ slightly, but the formula syntax and core concepts are substantially the same.