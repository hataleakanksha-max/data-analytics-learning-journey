# Practice Exercises: Basic Formulas and Cell References

## Exercise 1: Basic Formulas

### Questions and Answers

**Q1. What does `=A1+B1` do?**

Answer: It adds the values in cells A1 and B1.

Note: If the cells contain incompatible values, the formula may return an error such as `#VALUE!`.

**Q2. What does the `*` symbol mean?**

Answer: It multiplies the values referenced in the formula.

Example: `=C2*D2`

**Q3. Why use formulas instead of entering calculated results directly?**

Answer: Formulas save time, reduce repetitive manual calculations, and recalculate when referenced values change.

**Q4. What happens when `=C2*D2` is copied from F2 to F3?**

Answer: It normally changes to `=C3*D3` because the relative cell references adjust to the new row.

**Q5. How do you subtract B1 from A1?**

Answer: `=A1-B1`

**Q6. How do you divide A1 by B1?**

Answer: `=A1/B1`

## Exercise 2: Small Business Sales

### Dataset

| Product | Quantity Sold | Price per Unit |
|---|---:|---:|
| Notebook | 12 | 50 |
| Pen | 25 | 10 |
| School Bag | 3 | 800 |

### Task 1: Calculate Notebook Sales

Formula:

`=B2*C2`

Result: 600

### Task 2: Copy the Formula

After copying the formula down one row, the formula for Pen becomes:

`=B3*C3`

### Task 3: Update the Quantity

The quantity sold for Pen changed from 20 to 25.

The formula recalculated the sales value automatically.

Calculation:

25 × 10 = 250

Result: 250

### Task 4: Final Results

| Product | Quantity Sold | Price per Unit | Total Sales |
|---|---:|---:|---:|
| Notebook | 12 | 50 | 600 |
| Pen | 25 | 10 | 250 |
| School Bag | 3 | 800 | 2400 |

### What I Learned

- How to calculate sales using multiplication.
- How to copy formulas down a column.
- How relative cell references adjust automatically.
- How changing input data updates formula results.

## Practice Status

**Status:** Completed

**Tools:** Microsoft Excel and Google Sheets