# Practice Exercises: Cell References

## Lesson Overview

**Topic:** Relative, Absolute, and Mixed Cell References

**Tools:** Microsoft Excel and Google Sheets

**Status:** Practiced

## Exercise 1: Relative References

### Objective

Understand how cell references change when a formula is copied.

### Formula

```excel
=B2*C2
```

### Task

Enter the formula in D2 and copy it down to D3.

### Expected Learning Outcome

The formula in D3 becomes:

```excel
=B3*C3
```

Both relative references adjust to the next row.

---

## Exercise 2: Absolute References

### Objective

Use an absolute reference to keep a standard discount rate fixed.

### Scenario

A store keeps its standard discount rate in cell F1.

### Formula

```excel
=B2*$F$1
```

### Task

Copy the formula down the column.

### Expected Learning Outcome

When the formula is copied to D3, it becomes:

```excel
=B3*$F$1
```

The price reference changes, but the reference to F1 remains fixed.

---

## Exercise 3: Changing the Discount Rate

### Objective

Understand how formulas recalculate when input values change.

### Task

1. Enter 10% in F1.
2. Calculate product discounts using `$F$1`.
3. Change F1 to 15%.
4. Observe the updated discount amounts.

### Expected Learning Outcome

The discount amounts recalculate automatically because the formulas refer to F1.

---

## Exercise 4: Mixed References

### Objective

Identify the difference between column-locked and row-locked references.

### Task A

Copy a formula containing `$F1` down one row.

**Expected result:**

```excel
$F2
```

The column remains fixed, while the row changes.

### Task B

Copy a formula containing `F$1` one column to the right.

**Expected result:**

```excel
G$1
```

The row remains fixed, while the column changes.

---

## Exercise 5: Final Understanding Check

### Question 1

What formula appears when `=B2*$F$1` is copied from D2 to D4?

**Answer:**

```excel
=B4*$F$1
```

### Question 2

If B4 contains ₹2,000 and F1 contains 15%, what discount amount is calculated?

**Answer:** ₹300

### Question 3

What formula appears when `=B2*C$1` is copied from D2 to D3?

**Answer:**

```excel
=B3*C$1
```

### Question 4

Which reference locks both the column and the row?

**Answer:** `$F$1`

### Question 5

What is the main difference between relative, absolute, and mixed references?

**Answer:**

- Relative references allow the row and column to adjust.
- Absolute references keep both the row and column fixed.
- Mixed references keep either the row or the column fixed.

## Reflection

Through these exercises, I practised using relative, absolute, and mixed cell references in Microsoft Excel and Google Sheets.

I learned how to apply a standard discount rate across multiple products and how formulas respond when references or input values change.

## Next Step

Continue to the next Excel lesson after reviewing cell references and confirming that the practical exercises have been completed in both spreadsheet applications.