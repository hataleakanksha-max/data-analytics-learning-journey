# Practice Exercises: Basic Data Cleaning

## Lesson Information

- **Lesson:** 6 — Basic Data Cleaning
- **Tools:** Microsoft Excel and Google Sheets
- **Status:** Practiced

## Exercise 1: Identify Data-Quality Problems

Consider this dataset:

| Product | Category | Quantity | Price |
|---|---|---:|---:|
| Notebook | Stationery | 10 | 50 |
| Notebook | Stationery | 10 | 50 |
| pen | stationery | 20 | 10 |
| School Bag | Accessories | | 800 |
| water bottle | Accessories | 5 | 150 |

Identify the following:

- A possible duplicate record.
- Inconsistent capitalization.
- A missing quantity.

### Learning Outcome

Recognize common data-quality problems before attempting to clean a dataset.

## Exercise 2: Remove Duplicates

### Task

Remove one confirmed duplicate Notebook record from the practice dataset.

### Expected Outcome

The dataset contains four data rows after removing one duplicate, excluding the header row.

### Important Consideration

Confirm that the repeated record is genuinely a duplicate before deleting it.

## Exercise 3: Remove Extra Spaces

### Formula

```excel
=TRIM(A2)
```

### Task

Enter the formula in a new column and copy it down for the remaining product names.

### Expected Outcome

Unnecessary leading and trailing spaces are removed, and repeated ordinary spaces between words are reduced to single spaces.

## Exercise 4: Standardize Capitalization

### Formula

```excel
=PROPER(B2)
```

### Task

Use the cleaned text from column B to standardize capitalization in column C.

### Expected Outcome

Examples include:

- `pen` becomes `Pen`.
- `water bottle` becomes `Water Bottle`.
- `school bag` becomes `School Bag`.

## Exercise 5: Combine Text-Cleaning Functions

### Formula

```excel
=PROPER(TRIM(A2))
```

### Task

Apply the formula to a product name containing extra spaces.

### Expected Outcome

The text is cleaned and its capitalization is standardized.

For example, ` water bottle ` becomes `Water Bottle`.

## Exercise 6: Handle Missing Values

### Scenario

A School Bag has a price of ₹800, but its quantity is missing.

Answer these questions:

1. Why can't total sales be calculated reliably?
2. What should be entered if the original record confirms that four bags were sold?
3. What should happen if the quantity cannot be verified?

### Learning Outcome

Understand the difference between missing information and a confirmed zero value.

## Exercise 7: Preserve Original Data

### Task

Create separate columns for original product names, cleaned text, and standardized text.

### Learning Outcome

Understand why original data should be preserved until cleaning results have been reviewed.

## Practical Reflection

Through this lesson, I practised identifying duplicates, cleaning text with `TRIM()` and `PROPER()`, and handling missing values without making unsupported assumptions.

I also learned that data cleaning must preserve legitimate records and that original data should be retained for verification.

## Completion Checklist

- [ ] Identified duplicate records.
- [ ] Removed a confirmed duplicate.
- [ ] Practised `TRIM()`.
- [ ] Practised `PROPER()`.
- [ ] Identified a missing value.
- [ ] Explained why missing values should not automatically be replaced with zero.
- [ ] Practised in Microsoft Excel and Google Sheets.

## Next Step

Continue to the next Excel topic after reviewing data-cleaning concepts and confirming that the practical exercises have been completed.