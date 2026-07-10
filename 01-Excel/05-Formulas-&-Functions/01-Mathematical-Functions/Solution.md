# 📘 Solution – Lab 01: Mathematical Functions

## 🎯 Objective

This document contains the solutions for **Lab 01 – Mathematical Functions**. Use it to verify your formulas and understand how each mathematical function works in Microsoft Excel.

> **Note:** Since your dataset contains randomly generated values, the final numeric results may differ. The formulas below will always produce the correct answers.

---

# Part A – Basic Calculations

## Q1. Calculate Total Salary

### Formula

```excel
=SUM(G2:G201)
```

### Description

Calculates the total salary of all employees. *Output is 13866000.00*

---

## Q2. Calculate Average Salary

### Formula

```excel
=AVERAGE(G2:G201)
```

### Description

Returns the average salary of all employees. *Output is 69330.00*

---

## Q3. Find Highest Salary

### Formula

```excel
=MAX(G2:G201)
```

### Description

Returns the highest salary in the dataset. *Output is 119000.00*

---

## Q4. Find Lowest Salary

### Formula

```excel
=MIN(G2:G201)
```

### Description

Returns the lowest salary in the dataset. *Output is 25000.00*

---

## Q5. Count Numeric Salary Records

### Formula

```excel
=COUNT(G2:G201)
```

### Description

Counts the number of cells containing numeric salary values. *Output is 200.00*

---

## Q6. Count Non-Empty Employee Names

### Formula

```excel
=COUNTA(B2:B201)
```

### Description

Counts all non-empty employee names. *Output is 200*

---

## Q7. Count Blank Cells in Bonus/City Column

### Formula

```excel
=COUNTBLANK(H1:H201)
```

### Description

Counts the number of blank cells in the City column. *Output is 0*

---

# Part B – Conditional Calculations

## Q8. Calculate Total Salary for IT Department

### Formula

```excel
=SUMIF(C2:C201,"IT",G2:G201)
```

### Description

Adds the salaries of employees working in the IT department. *Output is 20,17,000.00*

---

## Q9. Calculate Total Salary for IT Employees in Mumbai

### Formula

```excel
=SUMIFS(G2:G201,C2:C201,"IT",H2:H201,"Mumbai")
```

### Description

Returns the total salary of employees who belong to the IT department and work in Mumbai. *Output is 114,000.00*

---

# Part C – Rounding Functions

## Q10. Calculate Monthly Salary using ROUND()

### Formula

Monthly Salary = Salary/12 using ROUND().

```excel
=ROUND(G2/12,2)
```

### Description

Calculates the monthly salary rounded to two decimal places.

---

## Q11. Calculate Monthly Salary using ROUNDUP()

### Formula

```excel
=ROUNDUP(G2/12,2)
```

### Description

Rounds the monthly salary up to two decimal places.

---

## Q12. Calculate Monthly Salary using ROUNDDOWN()

### Formula

```excel
=ROUNDDOWN(G2/12,2)
```

### Description

Rounds the monthly salary down to two decimal places.

---

# Part D – Other Mathematical Functions

## Q13. Find Absolute Value of -250

### Formula

```excel
=ABS(-250)
```

### Output

```
250
```

### Description

Returns the absolute (positive) value of a number.

---

## Q14. Return Integer Value of 15.98

### Formula

```excel
=INT(15.98)
```

### Output

```
15
```

### Description

Returns only the integer portion of the number.

---

## Q15. Find the Remainder when Salary is Divided by 1000

### Formula

```excel
=MOD(G2,1000)
```

### Description

Returns the remainder after dividing Salary by 1000.

---

## Q16. Return Integer Division of Salary by 1000

### Formula

```excel
=QUOTIENT(E2,1000)
```

### Description

Returns the integer result of Salary divided by 1000.

---

## Q17. Round Salary Up to the Next 5000

### Formula

```excel
=CEILING(G2,5000)
```

### Description

Rounds the salary up to the nearest multiple of 5000.

---

## Q18. Round Salary Down to the Previous 5000

### Formula

```excel
=FLOOR(G2,5000)
```

### Description

Rounds the salary down to the nearest multiple of 5000.

---

# ⭐ Challenge Solutions

## Challenge 1 – Department-wise Total Salary

### Formula

```excel
=SUMIF($C$2:$C$201,H2,$G$2:$G$201)
```

---

## Challenge 2 – City-wise Average Bonus

### Formula

```excel
=AVERAGEIF($D$2:$D$201,H2,$F$2:$F$201)
```

> **H2** contains the city name.

---

## Challenge 3 – Find Employees Earning Above Average Salary

### Step 1 – Calculate Average Salary

```excel
=AVERAGE(G2:G201)
```

Store the result in **J2**.

### Step 2 – Compare Each Employee Salary

```excel
=IF(G2>$J$2,"Above Average","Below Average")
```

---

## Challenge 4 – Create a Summary Table

| Metric | Formula |
|---------|---------|
| Total Salary | `=SUM(E2:E201)` |
| Average Salary | `=AVERAGE(E2:E201)` |
| Highest Salary | `=MAX(E2:E201)` |
| Lowest Salary | `=MIN(E2:E201)` |
| Total Employees | `=COUNTA(A2:A201)` |

---

# 📌 Key Takeaways

- **SUM()** adds numeric values.
- **AVERAGE()** calculates the mean value.
- **MIN()** returns the smallest number.
- **MAX()** returns the largest number.
- **COUNT()** counts numeric cells.
- **COUNTA()** counts all non-empty cells.
- **COUNTBLANK()** counts empty cells.
- **SUMIF()** performs conditional summation.
- **SUMIFS()** performs summation using multiple conditions.
- **ROUND()**, **ROUNDUP()**, and **ROUNDDOWN()** control decimal precision.
- **ABS()** returns the positive value of a number.
- **MOD()** returns the remainder after division.
- **QUOTIENT()** returns only the integer portion of a division.
- **CEILING()** rounds up to the nearest specified multiple.
- **FLOOR()** rounds down to the nearest specified multiple.

---


