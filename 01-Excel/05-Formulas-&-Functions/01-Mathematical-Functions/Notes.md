# What are Mathematical Functions?

Mathematical functions are built-in Excel formulas used to perform calculations on numbers.

These functions help users:

Perform arithmetic operations
Summarize data
Round numbers
Find minimum and maximum values
Count records
Calculate totals and averages

They are widely used in finance, sales, HR, inventory management, and data analytics.

# Functions Covered

| Function   | Purpose                                  |
| ---------- | ---------------------------------------- |
| SUM        | Adds numbers                             |
| AVERAGE    | Calculates average                       |
| MIN        | Finds smallest value                     |
| MAX        | Finds largest value                      |
| COUNT      | Counts numeric cells                     |
| COUNTA     | Counts non-empty cells                   |
| COUNTBLANK | Counts empty cells                       |
| SUMIF      | Adds values based on one condition       |
| SUMIFS     | Adds values based on multiple conditions |
| PRODUCT    | Multiplies numbers                       |
| ROUND      | Rounds to specified digits               |
| ROUNDUP    | Always rounds up                         |
| ROUNDDOWN  | Always rounds down                       |
| INT        | Returns integer portion                  |
| ABS        | Returns absolute value                   |
| MOD        | Returns remainder after division         |
| FLOOR      | Rounds down to nearest multiple          |

--- 

## 1. SUM Function

### Purpose

Adds multiple numbers together.

### Syntax

```excel
=SUM(number1, number2, ...)
```

### Result

Returns the total of all numbers in the range.

### Real-World Example

Calculate total monthly sales.

---

## 2. AVERAGE Function

### Purpose

Calculates the average (mean) of numbers.

### Syntax

```excel
=AVERAGE(B2:B10)
```

### Example

Find the average employee salary.

---

## 3. MIN Function

### Purpose

Returns the smallest value.

### Syntax

```excel
=MIN(B2:B10)
```

### Example

Find the lowest product price.

---

## 4. MAX Function

### Purpose

Returns the largest value.

### Syntax

```excel
=MAX(B2:B10)
```

### Example

Find the highest sales amount.

---

## 5. COUNT Function

### Purpose

Counts cells containing numbers.

### Syntax

```excel
=COUNT(B2:B20)
```

### Example

Count how many employees have salary values.

---

## 6. COUNTA Function

### Purpose

Counts all non-empty cells.

### Syntax

```excel
=COUNTA(A2:A20)
```

### Example

Count total employee records.

---

## 7. COUNTBLANK Function

### Purpose

Counts blank cells.

### Syntax

```excel
=COUNTBLANK(B2:B20)
```

### Example

Find missing salary values.

---

## 8. SUMIF Function

### Purpose

Adds values based on one condition.

### Syntax

```excel
=SUMIF(range, criteria, sum_range)
```

### Example

```excel
=SUMIF(C2:C20,"IT",D2:D20)
```
Returns the total salary of IT employees.

---

## 9. SUMIFS Function

### Purpose

Adds values based on multiple conditions.

### Syntax

```excel
=SUMIFS(sum_range,criteria_range1,criteria1,criteria_range2,criteria2)
```

### Example

```excel
=SUMIFS(D2:D20,C2:C20,"IT",E2:E20,"Mumbai")
```
Returns the total salary of IT employees in Mumbai.

---

## 10. PRODUCT Function

### Purpose

Multiplies numbers.

### Syntax

```excel
=PRODUCT(A2:A5)
```

### Example

Calculate total units × price.

---

## 11. ROUND Function

### Purpose

Rounds a number to a specified number of digits.

### Syntax

```excel
=ROUND(number,num_digits)
```

### Example

```excel
=ROUND(15.6789,2)
```

### Result

```excel
15.68
``` 

---

## 12. ROUNDUP Function

Always rounds away from zero.

### Example

```excel
=ROUNDUP(15.123,2)
```

### Result

```excel
15.13
```

---

## 13. ROUNDDOWN Function

Always rounds toward zero.

### Example

```excel
=ROUNDDOWN(15.987,2)
```

### Result

```excel
15.98
```

---

## 14. INT Function

Returns only the integer part.

### Example

```excel
=INT(15.98)
```

### Result

```excel
15
```

---

## 15. ABS Function

Returns the absolute (positive) value.

### Example

```excel
=ABS(-250)
```

### Result

```excel
250
```

---

## 16. MOD Function

Returns the remainder after division.

### Example

```excel
=MOD(17,5)
```

### Result

```excel
2
```

---

## 17. FLOOR Function

Rounds a number down to the nearest multiple.

### Example

```excel
=FLOOR(17,5)
```

### Result

```excel
15
```

---

# Best Practices

Use cell references instead of hardcoded values.
Verify data types before calculations.
Use ranges instead of individual cells where possible.
Keep formulas simple and readable.
Test formulas with sample data.
Use Excel Tables for dynamic ranges.