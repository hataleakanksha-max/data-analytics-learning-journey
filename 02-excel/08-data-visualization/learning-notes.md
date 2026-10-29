# Lesson 9: Data Visualization — Learning Notes

## 1. What Is Data Visualization?

Data visualization represents information through charts and graphs to make comparisons, trends, and patterns easier to understand.

Data analysts use visualization to communicate findings and support business decisions.

## 2. Common Chart Types

### Column and Bar Charts

Used to compare values across categories.

Example: Comparing sales across products.

### Line Charts

Used to show changes over time.

Example: Tracking monthly sales or daily website visitors.

### Pie Charts

Used to show how a small number of categories contribute to a whole.

Example: Showing the percentage contribution of product categories to total sales.

Pie charts can become difficult to interpret when there are many categories or similarly sized slices.

### Scatter Plots

Used to explore the relationship between two numerical variables.

Example: Examining the relationship between advertising expenditure and sales revenue.

A scatter plot may reveal an association, but it does not by itself prove causation.

## 3. Selecting the Right Chart

| Business Question | Suitable Starting Chart |
|---|---|
| Which product has the highest sales? | Bar or column chart |
| How did sales change over 12 months? | Line chart |
| What share of sales comes from each category? | Pie chart or bar chart |
| Are advertising expenditure and sales associated? | Scatter plot |

The chart should be selected according to the question, audience, and type of data.

## 4. Interpreting Sales Data

Sample dataset:

| Product | Category | Quantity | Sales (₹) |
|---|---|---:|---:|
| Laptop | Electronics | 2 | 45000 |
| Mouse | Accessories | 10 | 2000 |
| Keyboard | Accessories | 5 | 3000 |
| Monitor | Electronics | 3 | 20000 |
| Headphones | Electronics | 4 | 5000 |
| Notebook | Stationery | 20 | 1000 |

### Key Metrics

- Total sales: ₹76,000
- Electronics sales: ₹70,000
- Accessories sales: ₹5,000
- Stationery sales: ₹1,000
- Number of products listed: 6
- Highest sales value by product: Laptop, ₹45,000
- Highest quantity sold: Notebook, 20 units

### Percentage Contribution

Percentage contribution is calculated as:

Percentage contribution = Category sales / Total sales × 100

Electronics:

70000 / 76000 × 100 ≈ 92.1%

Accessories:

5000 / 76000 × 100 ≈ 6.6%

Stationery:

1000 / 76000 × 100 ≈ 1.3%

The percentages total approximately 100%, allowing for rounding.

## 5. Dashboard Metrics and Formulas

Assuming the source worksheet is named Sales Data:

### Total Sales

`=SUM('Sales Data'!D2:D7)`

### Number of Products

`=COUNTA('Sales Data'!A2:A7)`

### Electronics Sales

`=SUMIF('Sales Data'!B2:B7,"Electronics",'Sales Data'!D2:D7)`

### Accessories Sales

`=SUMIF('Sales Data'!B2:B7,"Accessories",'Sales Data'!D2:D7)`

### Stationery Sales

`=SUMIF('Sales Data'!B2:B7,"Stationery",'Sales Data'!D2:D7)`

## 6. Dashboard Design Principles

1. Give the dashboard a clear title.
2. Place key metrics where they are easy to find.
3. Use meaningful chart titles and labels.
4. Format monetary values consistently.
5. Avoid unnecessary visual decoration.
6. Check that charts use the correct data ranges.
7. Verify calculated results before communicating findings.

## 7. Important Analytical Distinction

Sales value and quantity sold are different metrics.

Laptop has the highest sales value at ₹45,000, but Notebook has the highest quantity sold at 20 units. Analysts should identify which metric answers the business question.

Sales value does not equal profit. Profitability requires cost information.

## 8. Key Takeaways

Data visualization makes information easier to interpret, but the chart must be appropriate for the question. Good analysts verify calculations, distinguish facts from assumptions, and communicate insights clearly.
