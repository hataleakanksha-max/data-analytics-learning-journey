# Practice Exercises — Retail Sales Data Analysis

## Project Dataset

The exercises use a sample retail dataset with 15 transactions and the following fields:

Order ID, Date, Region, Product, Category, Quantity, Unit Price, and Total Sales.

## Exercise 1: Understand the Data

1. How many transactions are in the dataset?
2. Which column identifies the number of units sold?
3. Which formula calculates transaction revenue?
4. Why is revenue more useful than quantity alone when comparing products with different prices?

### Results

1. 15 transactions.
2. Quantity.
3. `=F2*G2`
4. Revenue considers both the quantity sold and the unit price.

## Exercise 2: Validate the Data

1. Check whether any values are missing.
2. Check whether Order IDs are duplicated.
3. Verify that dates are recognised correctly.
4. Confirm that quantity and unit price are numeric.

### Reported Results

- No missing values found.
- No duplicate Order IDs found.
- Dates recognised correctly.
- Quantity and unit price contain numeric values.

## Exercise 3: Calculate Revenue

1. Add a Total Sales column.
2. Calculate revenue for each transaction.
3. Fill the formula down for all 15 orders.
4. Calculate the grand total using `SUM()`.

### Results

- First transaction: ₹90,000.
- Second transaction: ₹2,000.
- Grand total revenue: ₹2,85,750.

## Exercise 4: Analyse Product Revenue

1. Create a product summary for all six products.
2. Use `SUMIF()` to calculate each product's revenue.
3. Identify the highest-revenue product.
4. Identify the lowest-revenue product.

### Results

- Highest: Laptop — ₹1,80,000.
- Lowest: Notebook — ₹1,750.

## Exercise 5: Analyse Regional Revenue

1. Create a summary for West, North, South, and East.
2. Use `SUMIF()` to calculate each region's revenue.
3. Identify the highest- and lowest-revenue regions.
4. Calculate the revenue difference between West and North.

### Results

- Highest: West — ₹1,67,000.
- Lowest: East — ₹12,200.
- West–North difference: ₹80,000.

## Exercise 6: Build a Dashboard

1. Create a worksheet named Sales Dashboard.
2. Display total revenue and transaction count.
3. Display the highest-revenue product and region.
4. Add a product revenue chart.
5. Add a regional revenue chart.
6. Add a short business insights section.
7. Check that chart titles, labels, and currency values are readable.

## Exercise 7: Business Interpretation

**Question 1:** Does the highest-revenue product necessarily sell the most units?

**Answer:** No. A product can generate high revenue because of its higher unit price, even if its quantity sold is lower.

**Question 2:** Does the highest-revenue region necessarily have the most transactions?

**Answer:** No. Regional revenue depends on the products sold, their prices, and quantities—not just the number of transactions.

**Question 3:** Can we conclude that Laptop is the most profitable product?

**Answer:** No. Profit cannot be determined without product costs and other relevant expenses.

**Question 4:** Can this dataset prove that sales are increasing over time?

**Answer:** No. It covers only one month. More historical data and time-based analysis would be required.

## Reflection

After completing this project, reflect on these questions:

- Which Excel function was most useful, and why?
- What did data validation help you confirm?
- Which business insight was most useful?
- What additional data would improve the analysis?
- What would you add if you continued this project using SQL or Python?

## Completion Checklist

- [ ] Dataset organised and validated.
- [ ] Transaction-level revenue calculated.
- [ ] Grand total calculated.
- [ ] Product revenue summary completed.
- [ ] Regional revenue summary completed.
- [ ] Both charts added to the dashboard.
- [ ] Dashboard KPIs and insights checked.
- [ ] Project documentation saved to GitHub.