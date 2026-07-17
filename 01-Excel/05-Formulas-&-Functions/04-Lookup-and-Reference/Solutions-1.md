# 📘 Solution – Lab 04: Lookup & Reference Functions (Part 1)

## 🎯 Objective

This document contains the solutions for **Part 1** of the Lookup & Reference Functions Lab.

Functions Covered:

- VLOOKUP()
- HLOOKUP()

---

# Datasets Used

- Employees.xlsx
- Departments.xlsx
- Salaries.xlsx

---

# Assumptions

## Employees Sheet

| Column | Field |
|---------|-------|
| A | Employee ID |
| B | Employee Name |
| C | Department ID |
| D | Salary ID |
| E | City |

---

## Departments Sheet

| Column | Field |
|---------|-------|
| A | Department ID |
| B | Department Name |
| C | Manager |
| D | Extension |
| E | Floor |

---

## Salaries Sheet

| Column | Field |
|---------|-------|
| A | Salary ID |
| B | Basic Salary |
| C | HRA |
| D | Bonus |
| E | Other Allowance |
| F | Gross Salary |

---

# Part A – VLOOKUP

---

## Solution 1

### Task

Retrieve Employee Name using Employee ID.

### Formula

```excel
=VLOOKUP(A5,Employees!$A$2:$E$26,2,FALSE)
```

### Explanation

Searches the Employee ID and returns the Employee Name.

---

## Solution 2

### Task

Retrieve Department ID.

### Formula

```excel
=VLOOKUP(A9,Employees!$A$2:$E$26,3,FALSE)
```

### Explanation

Returns the Department ID associated with the employee.

---

## Solution 3

### Task

Retrieve Salary ID.

### Formula

```excel
=VLOOKUP(A2,Employees!$A$2:$E$26,4,FALSE)
```

---

## Solution 4

### Task

Retrieve Employee City.

### Formula

```excel
=VLOOKUP(A25,Employees!$A$2:$E$26,5,FALSE)
```

---

## Solution 5

### Task

Retrieve Department Name using Department ID.

### Formula

```excel
=VLOOKUP(C2,Departments!$A$2:$E$26,2,FALSE)
```

### Explanation

Looks up the Department ID and returns the Department Name.

---

## Solution 6

### Task

Retrieve Department Manager.

### Formula

```excel
=VLOOKUP(C5,Departments!$A$2:$E$26,3,FALSE)
```

---

## Solution 7

### Task

Retrieve Office Extension.

### Formula

```excel
=VLOOKUP(C2,Departments!$A$2:$E$26,4,FALSE)
```

---

## Solution 8

### Task

Retrieve Floor Number.

### Formula

```excel
=VLOOKUP(C8,Departments!$A$2:$E$26,5,FALSE)
```

---

## Solution 9

### Task

Retrieve Basic Salary using Salary ID.

### Formula

```excel
=VLOOKUP(D2,Salaries!$A$2:$F$26,2,FALSE)
```

---

## Solution 10

### Task

Retrieve HRA.

### Formula

```excel
=VLOOKUP(D2,Salaries!$A$2:$F$26,3,FALSE)
```

---

## Solution 11

### Task

Retrieve Bonus.

### Formula

```excel
=VLOOKUP(D2,Salaries!$A$2:$F$26,4,FALSE)
```

---

## Solution 12

### Task

Retrieve Gross Salary.

### Formula

```excel
=VLOOKUP(D2,Salaries!$A$2:$F$26,6,FALSE)
```

### Explanation

Returns the Gross Salary corresponding to the Salary ID.

---

# Part B – HLOOKUP

Create the following table in Excel.

| | A | B | C | D | E |
|---|---|---|---|---|---|
|1|Quarter|Q1|Q2|Q3|Q4|
|2|Sales|450000|520000|610000|700000|

---

## Solution 13

### Task

Retrieve Q2 Sales.

### Formula

```excel
=HLOOKUP("Q2",$A$1:$E$2,2,FALSE)
```

### Result

```
520000
```

---

## Solution 14

### Task

Retrieve Q4 Sales.

### Formula

```excel
=HLOOKUP("Q4",$A$1:$E$2,2,FALSE)
```

### Result

```
700000
```

---

## Solution 15

### Task

Retrieve Q1 Sales.

### Formula

```excel
=HLOOKUP("Q1",$A$1:$E$2,2,FALSE)
```

### Result

```
450000
```

---
