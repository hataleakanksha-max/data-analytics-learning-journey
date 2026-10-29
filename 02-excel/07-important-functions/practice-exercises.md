
# Lesson 8: Important Excel Functions — Practice Exercises

## Practice 1: IF()

### Scenario

An employee meets the sales target if sales are at least 20000.

| Employee | Sales |
|---|---:|
| Asha | 25000 |
| Rahul | 15000 |
| Priya | 20000 |

### Exercise

Write a formula to display Target Met or Target Not Met.

### Answer

`=IF(B2>=20000,"Target Met","Target Not Met")`

Results:
- Asha: Target Met
- Rahul: Target Not Met
- Priya: Target Met

## Practice 2: COUNTIF()

### Scenario

| Employee | Department |
|---|---|
| Asha | IT |
| Rahul | HR |
| Priya | IT |
| Amit | Finance |
| Sneha | IT |
| Rohan | HR |
| Neha | Finance |
| Kiran | IT |

### Exercises and Answers

1. Count employees in IT.

   `=COUNTIF(B2:B9,"IT")`

   Result: 4

2. Count employees in HR.

   `=COUNTIF(B2:B9,"HR")`

   Result: 2

## Practice 3: SUMIF()

### Scenario

| Product | Category | Sales |
|---|---|---:|
| Laptop | Electronics | 45000 |
| Mouse | Accessories | 2000 |
| Keyboard | Accessories | 3000 |
| Monitor | Electronics | 20000 |
| Headphones | Electronics | 5000 |
| Notebook | Stationery | 1000 |

### Exercises and Answers

1. Calculate Accessories sales.

   `=SUMIF(B2:B7,"Accessories",C2:C7)`

   Result: 5000

2. Calculate Stationery sales.

   `=SUMIF(B2:B7,"Stationery",C2:C7)`

   Result: 1000

## Practice 4: COUNTIFS()

Using the product dataset above:

1. Count Electronics products with sales greater than 10000.

   `=COUNTIFS(B2:B7,"Electronics",C2:C7,">10000")`

   Result: 2

2. Count Accessories products with sales greater than 2000.

   `=COUNTIFS(B2:B7,"Accessories",C2:C7,">2000")`

   Result: 1

## Practice 5: SUMIFS()

Using the product dataset above:

1. Calculate Electronics sales greater than 10000.

   `=SUMIFS(C2:C7,B2:B7,"Electronics",C2:C7,">10000")`

   Result: 65000

2. Calculate Electronics sales below 10000.

   `=SUMIFS(C2:C7,B2:B7,"Electronics",C2:C7,"<10000")`

   Result: 5000

## Practice 6: Final Review

Use this dataset:

| Product | Category | Quantity | Sales |
|---|---|---:|---:|
| Laptop | Electronics | 2 | 45000 |
| Mouse | Accessories | 10 | 2000 |
| Keyboard | Accessories | 5 | 3000 |
| Monitor | Electronics | 3 | 20000 |
| Headphones | Electronics | 4 | 5000 |
| Notebook | Stationery | 20 | 1000 |

### Questions and Answers

1. Which function counts products in Electronics?

   COUNTIF()

2. What are total Electronics sales?

   70000

3. How many Electronics products have quantity greater than 3?

   1

4. Calculate Accessories sales.

   `=SUMIF(B2:B7,"Accessories",D2:D7)`

   Result: 5000

5. Count products with sales greater than 10000.

   `=COUNTIF(D2:D7,">10000")`

   Result: 2

## Reflection

I practised conditional formulas, single-condition counting and summation, and multiple-condition analysis. These skills help automate business reporting and support data-driven decisions.
