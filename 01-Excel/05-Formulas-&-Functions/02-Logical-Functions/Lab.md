# 📘 Lab 02 – Logical Functions

## 🎯 Objective

Practice Excel Logical Functions by solving real-world business scenarios using an employee dataset.

---

# Prerequisites

Before starting this lab, you should know:

- IF
- Nested IF
- IFS
- AND
- OR
- NOT
- XOR
- IFERROR
- IFNA

---

# Dataset

**File Name**

Employee_Dataset_200.xlsx

**Worksheet**

Employee_Data

---

# Dataset Columns

| Column | Description |
|----------|-------------|
| Employee ID | Unique employee ID |
| Employee Name | Employee Name |
| Department | Department Name |
| City | Employee Location |
| Salary | Monthly Salary |
| Bonus | Employee Bonus |
| Experience | Years of Experience |
| Joining Date | Employee Joining Date |

---

# Lab Scenario

You are working as a **Data Analyst** in an HR department.

Your manager has asked you to automate several HR decisions using Excel Logical Functions.

---

# Part A – IF Function

## Task 1

Create a new column named **Bonus Eligibility**.

Condition:

- Salary ≥ 60000 → Eligible
- Otherwise → Not Eligible

---

## Task 2

Create a column named **Salary Category**.

Condition:

- Salary ≥ 75000 → High Salary
- Otherwise → Normal Salary

---

## Task 3

Create a column named **Experience Level**.

Condition:

- Experience ≥ 5 years → Experienced
- Otherwise → Fresher

---

# Part B – Nested IF

## Task 4

Create a **Performance Grade** column.

Rules:

| Salary | Grade |
|----------|-------|
| ≥ 90000 | A |
| ≥ 70000 | B |
| ≥ 50000 | C |
| Otherwise | D |

---

## Task 5

Create an **Employee Level** column.

Rules:

| Experience | Level |
|-------------|-------|
| ≥10 | Senior |
| ≥5 | Mid-Level |
| ≥2 | Junior |
| Otherwise | Trainee |

---

# Part C – IFS Function

## Task 6

Using the **IFS** function, assign salary bands.

| Salary | Band |
|----------|------|
| ≥100000 | Platinum |
| ≥80000 | Gold |
| ≥60000 | Silver |
| ≥40000 | Bronze |
| Otherwise | Entry |

---

## Task 7

Assign employee grades using IFS.

| Bonus | Rating |
|--------|---------|
| ≥15000 | Excellent |
| ≥10000 | Good |
| ≥5000 | Average |
| Otherwise | Needs Improvement |

---

# Part D – AND Function

## Task 8

Create a **Promotion Eligibility** column.

Conditions:

- Experience ≥ 5 years
- Salary ≥ 70000

Both conditions must be TRUE.

---

## Task 9

Create a **Leadership Candidate** column.

Conditions:

- Experience ≥ 8 years
- Bonus ≥ 12000

---

# Part E – OR Function

## Task 10

Create a **Metro City Employee** column.

Condition:

Employee works in:

- Mumbai
- Pune

If either condition is TRUE, return **Yes**, otherwise **No**.

---

## Task 11

Create an **IT Support Team** column.

Condition:

Department is:

- IT
- Support

---

# Part F – NOT Function

## Task 12

Create a column named **Non-IT Employee**.

Return:

- Yes
- No

---

## Task 13

Display whether an employee does **NOT** belong to the HR department.

---

# Part G – XOR Function

## Task 14

Create a column to check whether **only one** of the following conditions is TRUE.

- Salary > 70000
- Bonus > 10000

If exactly one condition is TRUE, return TRUE.

---

# Part H – IFERROR Function

## Task 15

Calculate:

Bonus ÷ Salary

If an error occurs, display:

```
Invalid
```

---

## Task 16

Divide Salary by another column.

Use **IFERROR()** to prevent Excel errors.

---

# Part I – IFNA Function

## Task 17

Create a lookup table for Department Codes.

Example:

| Department | Code |
|------------|------|
| IT | D001 |
| HR | D002 |
| Sales | D003 |
| Finance | D004 |

Use **VLOOKUP()**.

If a department is missing, display:

```
Department Not Found
```

using **IFNA()**.

---

# Challenge Questions

## Challenge 1

Create an **Employee Status** column.

Rules:

- Salary ≥70000 AND Experience ≥5 → Senior Employee
- Salary ≥50000 → Regular Employee
- Otherwise → Junior Employee

---

## Challenge 2

Identify employees eligible for a **Special Bonus**.

Conditions:

- Department = IT OR Finance
- Salary ≥75000

---

## Challenge 3

Identify employees who joined before **01-Jan-2021**.

Return:

- Old Employee
- New Employee

---

## Challenge 4

Classify employees based on Bonus.

| Bonus | Category |
|--------|----------|
| ≥15000 | Excellent |
| ≥10000 | Good |
| ≥5000 | Average |
| Otherwise | Low |

---

## Challenge 5

Create a final **HR Decision** column.

Rules:

- Promotion Eligible → Promote
- Experienced but not eligible → Review
- Otherwise → Training Required

---
