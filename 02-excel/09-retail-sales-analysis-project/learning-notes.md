# Learning Notes — Retail Sales Data Analysis

## 1. Understanding the Dataset

A row represents one transaction. Each column represents an attribute, such as order ID, date, region, product, quantity, or price.

The dataset contains 15 transactions.

## 2. Data Validation

Before performing calculations, I checked:

- Whether the expected column headers were present.
- Whether any values were missing.
- Whether Order IDs were duplicated.
- Whether dates were recognised as dates.
- Whether quantity and unit price were numeric.

The checks reported no missing values or duplicate Order IDs. The date and numeric columns were also recognised correctly.

**Important lesson:** Data validation should happen before analysis. Missing or duplicated records can affect results, and suspected issues should be investigated before changing the data.

## 3. Calculating Transaction Revenue

Formula:

`=F2*G2`

Where:
- Column F contains Quantity.
- Column G contains Unit Price.

Example:

2 laptops × ₹45,000 = ₹90,000.

The formula was filled down through all 15 transactions. Excel adjusted the row references automatically.

## 4. Calculating Grand Total Revenue

Formula:

`=SUM(H2:H16)`

Result: ₹2,85,750.

The grand total represents the sales revenue from all 15 transactions combined.

## 5. Analysing Product Revenue with SUMIF

Syntax:

`=SUMIF(criteria_range, criteria, sum_range)`

Example for the product summary on the Sales Analysis worksheet:

`=SUMIF('Sales Data'!$D$2:$D$16,A2,'Sales Data'!$H$2:$H$16)`

This formula adds the Total Sales values for the product named in cell A2.

### Product Revenue Results

| Product | Revenue |
|---|---:|
| Laptop | ₹1,80,000 |
| Mouse | ₹9,200 |
| Keyboard | ₹10,800 |
| Monitor | ₹72,000 |
| Notebook | ₹1,750 |
| Headphones | ₹12,000 |

Laptop generated the highest revenue, while Notebook generated the lowest.

## 6. Analysing Regional Revenue with SUMIF

Example formula for the regional summary:

`=SUMIF('Sales Data'!$C$2:$C$16,D2,'Sales Data'!$H$2:$H$16)`

This formula adds revenue for the region named in cell D2.

### Regional Revenue Results

| Region | Revenue |
|---|---:|
| West | ₹1,67,000 |
| North | ₹87,000 |
| South | ₹19,550 |
| East | ₹12,200 |

West generated the highest revenue. East generated the lowest.

West–North difference:

₹1,67,000 − ₹87,000 = ₹80,000.

## 7. Charts and Dashboard

I created:
- A product revenue chart.
- A regional revenue chart.
- Four KPIs: total revenue, transaction count, top-revenue product, and top-revenue region.
- A key business insights section.

Charts help communicate comparisons visually. A chart title should clearly describe the measure and grouping being displayed.

## 8. Important Analytical Distinctions

- Revenue is not profit.
- Transaction count is not the same as units sold.
- Units sold are not the same as revenue.
- High revenue does not automatically mean high profitability.
- A single period of data cannot establish a long-term trend.

## 9. What I Learned

This project helped me practise data validation, calculated columns, `SUM()`, `SUMIF()`, relative references, summary tables, charts, dashboard layout, and evidence-based business interpretation.