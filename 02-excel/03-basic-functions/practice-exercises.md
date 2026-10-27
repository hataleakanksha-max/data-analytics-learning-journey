# Practice Exercises: Basic Spreadsheet Functions

## Exercise 1: Understanding Functions

### Q1. What is the difference between a formula and a function?

Answer: A formula is an expression that performs a calculation. A function is a predefined calculation that can be used within a formula.

### Q2. What does `=SUM(B2:B6)` do?

Answer: Adds the numerical values in the range B2:B6.

### Q3. Which function calculates the average?

Answer: `=AVERAGE(B2:B6)`

### Q4. Which function finds the lowest value?

Answer: `=MIN(B2:B6)`

### Q5. Which function finds the highest value?

Answer: `=MAX(B2:B6)`

### Q6. What does the colon mean?

Answer: It specifies a continuous range from the starting cell to the ending cell, including the cells in between.

### Q7. Why use SUM() for large datasets?

Answer: It reduces manual work, saves time, and avoids the repetitive errors that can occur when adding many values manually.

## Exercise 2: Stationery Store Sales

### Dataset

| Product | Quantity Sold | Price per Unit |
|---|---:|---:|
| Notebook | 20 | 50 |
| Pen | 50 | 10 |
| School Bag | 5 | 800 |
| Pencil Box | 15 | 100 |
| Water Bottle | 10 | 150 |

### Task 1: Calculate Individual Sales

Formula in D2:

`=B2*C2`

Formula in D6 after copying down:

`=B6*C6`

### Task 2: Calculate Total Revenue

Formula:

`=SUM(D2:D6)`

Result: ₹8,500

### Task 3: Calculate Average Sales

Formula:

`=AVERAGE(D2:D6)`

Result: ₹1,700

### Task 4: Find the Lowest Sales

Formula:

`=MIN(D2:D6)`

Result: ₹500

### Task 5: Find the Highest Sales

Formula:

`=MAX(D2:D6)`

Result: ₹4,000

## Skills Practiced

- Writing formulas using cell references
- Copying formulas down a column
- Using SUM()
- Using AVERAGE()
- Using MIN()
- Using MAX()
- Interpreting numerical summaries

## Practice Status

**Status: Completed**

**Tools:** Microsoft Excel and Google Sheets