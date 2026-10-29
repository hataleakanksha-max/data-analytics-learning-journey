
# Lesson 8: Important Excel Functions — Learning Notes

## 1. IF()

The IF function checks a condition and returns one result when the condition is TRUE and another when it is FALSE.

### Syntax

`=IF(logical_test, value_if_true, value_if_false)`

### Example

`=IF(B2>=10000,"Achieved","Not Achieved")`

If B2 contains 12000, the result is Achieved. If B2 contains 8000, the result is Not Achieved.

### Key Learning

- `>` means greater than.
- `<` means less than.
- `>=` means greater than or equal to.
- `<=` means less than or equal to.
- Text results must be enclosed in double quotation marks.

## 2. COUNTIF()

COUNTIF counts cells that meet one condition.

### Syntax

`=COUNTIF(range, criteria)`

### Text Example

`=COUNTIF(B2:B9,"HR")`

Counts the cells containing HR in the specified range.

### Numeric Example

`=COUNTIF(B2:B9,">=10000")`

Counts values greater than or equal to 10000.

### Key Learning

COUNTIF counts matching cells. It does not add their numerical values.

## 3. SUMIF()

SUMIF adds values when one condition is satisfied.

### Syntax

`=SUMIF(range, criteria, sum_range)`

### Example

`=SUMIF(B2:B7,"Accessories",C2:C7)`

Checks the category in B2:B7 and adds the corresponding values in C2:C7 when the category is Accessories.

### Key Learning

- `range` contains the cells to check.
- `criteria` defines the condition.
- `sum_range` contains the numbers to add.

## 4. COUNTIFS()

COUNTIFS counts records satisfying multiple conditions.

### Syntax

`=COUNTIFS(criteria_range1, criteria1, criteria_range2, criteria2)`

### Example

`=COUNTIFS(B2:B7,"Electronics",C2:C7,">10000")`

Counts products belonging to Electronics with sales greater than 10000.

### Key Learning

COUNTIFS uses AND logic: all specified conditions must be satisfied.

## 5. SUMIFS()

SUMIFS adds values satisfying multiple conditions.

### Syntax

`=SUMIFS(sum_range, criteria_range1, criteria1, criteria_range2, criteria2)`

### Example

`=SUMIFS(C2:C7,B2:B7,"Electronics",C2:C7,">10000")`

Adds sales values for Electronics products whose sales exceed 10000.

### Important Difference

SUMIFS begins with the sum_range, unlike COUNTIFS.

## 6. Comparison of Functions

| Function | Purpose |
|---|---|
| IF | Returns one of two results based on a condition |
| COUNTIF | Counts cells matching one condition |
| SUMIF | Adds values matching one condition |
| COUNTIFS | Counts records matching multiple conditions |
| SUMIFS | Adds values matching multiple conditions |

## 7. Important Lessons Learned

1. Choose a function based on the business question.
2. Use matching range sizes in conditional calculations.
3. Pay attention to the difference between `>` and `>=`.
4. Put text criteria and comparison expressions in quotation marks.
5. Check whether the question requires counting records or adding values.
6. Verify formula results against the source data.
