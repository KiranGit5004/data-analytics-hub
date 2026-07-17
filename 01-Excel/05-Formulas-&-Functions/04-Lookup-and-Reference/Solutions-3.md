# 📘 Solution – Lab 04: Lookup & Reference Functions (Part 3)

## 🎯 Objective

This document contains the solutions for **Part 3** of the Lookup & Reference Functions Lab.

Functions Covered:

- INDEX + MATCH()
- CHOOSE()
- OFFSET()
- Challenge Questions

---

# Part F – INDEX + MATCH

---

## Solution 29

### Task

Retrieve Employee City.

### Formula

```excel
=INDEX(Employees!$E$2:$E$26,MATCH(A2,Employees!$A$2:$A$26,0))
```

### Explanation

MATCH finds the Employee ID position and INDEX returns the corresponding City.

---

## Solution 30

### Task

Retrieve Department Name.

### Formula

```excel
=INDEX(Departments!$B$2:$B$26,MATCH(C2,Departments!$A$2:$A$26,0))
```

---

## Solution 31

### Task

Retrieve Department Manager.

### Formula

```excel
=INDEX(Departments!$C$2:$C$26,MATCH(C2,Departments!$A$2:$A$26,0))
```

---

## Solution 32

### Task

Retrieve Gross Salary.

### Formula

```excel
=INDEX(Salaries!$F$2:$F$26,MATCH(D2,Salaries!$A$2:$A$26,0))
```

---

## Solution 33

### Task

Retrieve Product Category.

### Formula

```excel
=INDEX(Products!$C$2:$C$26,MATCH(A2,Products!$A$2:$A$26,0))
```

---

## Solution 34

### Task

Retrieve Product Stock.

### Formula

```excel
=INDEX(Products!$E$2:$E$26,MATCH(A2,Products!$A$2:$A$26,0))
```

---

# Part G – CHOOSE

---

## Solution 35

### Task

Create Employee Grades.

### Formula

```excel
=CHOOSE(A2,"A","B","C","D")
```

### Explanation

If A2 contains:

| Value | Output |
|-------|--------|
|1|A|
|2|B|
|3|C|
|4|D|

---

## Solution 36

### Task

Display Department Categories.

### Formula

```excel
=CHOOSE(A2,"Technical","Management","Business","Accounts")
```

### Explanation

Where A2 contains:

| Value | Department Category |
|------|----------------------|
|1|Technical|
|2|Management|
|3|Business|
|4|Accounts|

---

# Part H – OFFSET

---

## Solution 37

### Task

Return the employee located two rows below the first employee.

### Formula

```excel
=OFFSET(Employees!B2,2,0)
```

### Explanation

Starts from Employee Name in **B2** and moves **2 rows down**.

---

## Solution 38

### Task

Return the third product from the Products table.

### Formula

```excel
=OFFSET(Products!B2,2,0)
```

---

## Solution 39

### Task

Calculate the sum of the first five salaries.

### Formula

```excel
=SUM(OFFSET(Salaries!B2,0,0,5,1))
```

### Explanation

Creates a range of five salary cells starting from **B2** and sums them.

---

## Solution 40

### Task

Return a dynamic range of five employee names.

### Formula

```excel
=OFFSET(Employees!B2,0,0,5,1)
```

---

# ⭐ Challenge Solutions

---

## Challenge 1

### Retrieve Department Name using three methods.

### VLOOKUP

```excel
=VLOOKUP(C2,Departments!$A$2:$B$26,2,FALSE)
```

### XLOOKUP

```excel
=XLOOKUP(C2,Departments!$A$2:$A$26,Departments!$B$2:$B$26)
```

### INDEX + MATCH

```excel
=INDEX(Departments!$B$2:$B$26,MATCH(C2,Departments!$A$2:$A$26,0))
```

---

## Challenge 2

### Find Gross Salary of every employee.

### Formula

```excel
=INDEX(Salaries!$F$2:$F$26,MATCH(D2,Salaries!$A$2:$A$26,0))
```

---

## Challenge 3

### Retrieve Product Price.

```excel
=INDEX(Products!$D$2:$D$26,MATCH(A2,Products!$A$2:$A$26,0))
```

### Retrieve Supplier.

```excel
=INDEX(Products!$F$2:$F$26,MATCH(A2,Products!$A$2:$A$26,0))
```

---

## Challenge 4

### Find Manager Name of every employee.

### Step 1

Retrieve Department ID.

### Step 2

Lookup Manager.

### Formula

```excel
=INDEX(Departments!$C$2:$C$26,MATCH(C2,Departments!$A$2:$A$26,0))
```

---

## Challenge 5

### Sales Report

Retrieve:

- Employee Name

```excel
=INDEX(Employees!$B$2:$B$26,MATCH(C2,Employees!$A$2:$A$26,0))
```

Retrieve:

- Product Name

```excel
=INDEX(Products!$B$2:$B$26,MATCH(D2,Products!$A$2:$A$26,0))
```

Other columns come directly from **Sales.xlsx**.

---

## Challenge 6

### Product Report

Retrieve

- Product Name
- Category
- Stock
- Supplier

Use INDEX + MATCH or XLOOKUP.

---

## Challenge 7

### Employee handling highest-value order.

### Formula

```excel
=INDEX(Employees!$B$2:$B$26,
MATCH(MAX(Sales!G2:G26),Sales!G2:G26,0))
```

---

## Challenge 8

### Employees working in IT Department.

Filter employees whose Department ID corresponds to **IT** in Departments.xlsx.

This can be solved using:

- FILTER() (Excel 365)
- INDEX + MATCH
- XLOOKUP

---

## Challenge 9

### Products costing more than ₹20,000.

Filter Product Table where:

```
Unit Price > 20000
```

Functions like FILTER() or AutoFilter can be used.

---

# 📊 Formula Comparison

| Function | Best Use Case |
|----------|---------------|
| VLOOKUP | Simple vertical lookup |
| HLOOKUP | Horizontal lookup |
| XLOOKUP | Modern Excel lookups |
| INDEX | Return value by position |
| MATCH | Find row/column position |
| INDEX + MATCH | Dynamic lookups |
| CHOOSE | Fixed value selection |
| OFFSET | Dynamic ranges |

---

# 💡 Best Practices

- Prefer **XLOOKUP()** over VLOOKUP() when available.
- Use **INDEX + MATCH()** for dynamic and scalable reports.
- Avoid hardcoding row and column numbers.
- Always lock lookup ranges using **absolute references**.
- Use **IFERROR()** or XLOOKUP's **if_not_found** argument for cleaner reports.
- Keep lookup values unique to avoid incorrect results.
- Use named ranges for better readability in large workbooks.

---

# 📌 Final Summary

After completing this lab, you should be able to:

- Retrieve data from multiple worksheets.
- Connect related datasets.
- Use VLOOKUP, HLOOKUP, and XLOOKUP effectively.
- Build dynamic lookup formulas with INDEX + MATCH.
- Create flexible reports using CHOOSE and OFFSET.
- Solve real-world HR, Sales, Inventory, and Finance lookup problems.

---

