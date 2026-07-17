# 📘 Solution – Lab 04: Lookup & Reference Functions (Part 2)

## 🎯 Objective

This document contains the solutions for **Part 2** of the Lookup & Reference Functions Lab.

Functions Covered:

- XLOOKUP()
- MATCH()
- INDEX()

---

# Datasets Used

- Employees.xlsx
- Departments.xlsx
- Salaries.xlsx
- Products.xlsx

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

## Products Sheet

| Column | Field |
|---------|-------|
| A | Product ID |
| B | Product Name |
| C | Category |
| D | Unit Price |
| E | Stock |
| F | Supplier |

---

# Part C – XLOOKUP

---

## Solution 16

### Task

Retrieve Employee Name using Employee ID.

### Formula

```excel
=XLOOKUP(A2,Employees!$A$2:$A$26,Employees!$B$2:$B$26)
```

### Explanation & O/P

Searches Employee ID and returns the Employee Name. The O/P is **Rahul Sharma**

---

## Solution 17

### Task

Retrieve Department Name using Department ID.

### Formula

```excel
=XLOOKUP(C2,Departments!$A$2:$A$26,Departments!$B$2:$B$26)
```

---

## Solution 18

### Task

Retrieve Gross Salary using Salary ID.

### Formula

```excel
=XLOOKUP(D2,Salaries!$A$2:$A$26,Salaries!$F$2:$F$26)
```

---

## Solution 19

### Task

Display "Employee Not Found" if Employee ID does not exist.

### Formula

```excel
=XLOOKUP(A2,Employees!$A$2:$A$26,Employees!$B$2:$B$26,"Employee Not Found")
```

---

## Solution 20

### Task

Retrieve Product Price using Product ID.

### Formula

```excel
=XLOOKUP(A2,Products!$A$2:$A$26,Products!$D$2:$D$26)
```

---

# Part D – MATCH

---

## Solution 21

### Task

Find the position of Employee ID.

### Formula

```excel
=MATCH(A2,Employees!$A$2:$A$26,0)
```

### Explanation

Returns the row position of the Employee ID.

---

## Solution 22

### Task

Find the position of Product ID.

### Formula

```excel
=MATCH(A2,Products!$A$2:$A$26,0)
```

---

## Solution 23

### Task

Find the position of Department ID.

### Formula

```excel
=MATCH(A2,Departments!$A$2:$A$26,0)
```

---

## Solution 24

### Task

Find the position of Salary ID.

### Formula

```excel
=MATCH(A2,Salaries!$A$2:$A$26,0)
```

---

# Part E – INDEX

---

## Solution 25

### Task

Retrieve Employee Name using row number.

### Formula

```excel
=INDEX(Employees!$B$2:$B$26,5)
```

### Explanation

Returns the 5th employee from the Employee Name column.

---

## Solution 26

### Task

Retrieve Product Name.

### Formula

```excel
=INDEX(Products!$B$2:$B$26,8)
```

---

## Solution 27

### Task

Retrieve Department Manager.

### Formula

```excel
=INDEX(Departments!$C$2:$C$26,4)
```

---

## Solution 28

### Task

Retrieve Gross Salary.

### Formula

```excel
=INDEX(Salaries!$F$2:$F$26,10)
```

---

# 💡 Best Practices

- Use **XLOOKUP()** instead of VLOOKUP() whenever available.
- Always use **MATCH()** with `0` for exact matches.
- INDEX() retrieves data based on position and works best when combined with MATCH().
- Use absolute references (`$`) for lookup ranges.
- Add custom error messages with XLOOKUP instead of displaying `#N/A`.

Example:

```excel
=XLOOKUP(A2,Employees!$A$2:$A$26,Employees!$B$2:$B$26,"Not Found")
```

---
