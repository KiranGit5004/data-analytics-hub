# 📘 Solution – Lab 02: Logical Functions

## 🎯 Objective

This document contains the solutions for **Lab 02 – Logical Functions**. These solutions demonstrate how to use Excel Logical Functions to solve real-world business problems using the **Employee_Dataset_Logical_Functions_50.xlsx** dataset.

> **Note:** The formulas below assume the following column structure:

| Column | Field |
|--------|-------|
| A | Employee ID |
| B | Employee Name |
| C | Department |
| D | City |
| E | Salary |
| F | Bonus |
| G | Experience (Years) |
| H | Joining Date |
| I | Performance Rating |
| J | Attendance % |
| K | Department Code |

---

# Part A – IF Function

## Solution 1 – Bonus Eligibility

### Formula

```excel
=IF([@Salary]>=60000,"Eligible","Not Eligible")
```

### Explanation

Employees earning ₹60,000 or more are eligible for a bonus.

---

## Solution 2 – Salary Category

### Formula

```excel
=IF([@Salary]>=75000,"High Salary","Normal Salary")
```

---

## Solution 3 – Experience Level

### Formula

```excel
=IF([@[Experience (Years)]]>= 5,"Experienced","Fresher")
```

---

# Part B – Nested IF

## Solution 4 – Performance Grade

### Formula

```excel
=IF(E2>=90000,"A",
IF(E2>=70000,"B",
IF(E2>=50000,"C","D")))
```

---

## Solution 5 – Employee Level

### Formula

```excel
=IF(G2>=10,"Senior",
IF(G2>=5,"Mid-Level",
IF(G2>=2,"Junior","Trainee")))
```

---

# Part C – IFS Function

## Solution 6 – Salary Band

### Formula

```excel
=IFS(
E2>=100000,"Platinum",
E2>=80000,"Gold",
E2>=60000,"Silver",
E2>=40000,"Bronze",
TRUE,"Entry")
```

---

## Solution 7 – Bonus Rating

### Formula

```excel
=IFS(
F2>=15000,"Excellent",
F2>=10000,"Good",
F2>=5000,"Average",
TRUE,"Needs Improvement")
```

---

# Part D – AND Function

## Solution 8 – Promotion Eligibility

### Formula

```excel
=IF(AND(G2>=5,E2>=70000),"Eligible","Not Eligible")
```

### Explanation

Employee must satisfy **both** conditions.

---

## Solution 9 – Leadership Candidate

### Formula

```excel
=IF(AND(G2>=8,F2>=12000),"Yes","No")
```

---

# Part E – OR Function

## Solution 10 – Metro City Employee

### Formula

```excel
=IF(OR(D2="Mumbai",D2="Pune"),"Yes","No")
```

---

## Solution 11 – IT Support Team

### Formula

```excel
=IF(OR(C2="IT",C2="Support"),"Yes","No")
```

---

# Part F – NOT Function

## Solution 12 – Non-IT Employee

### Formula

```excel
=IF(NOT(C2="IT"),"Yes","No")
```

---

## Solution 13 – Non-HR Employee

### Formula

```excel
=IF(NOT(C2="HR"),"Yes","No")
```

---

# Part G – XOR Function

## Solution 14 – Exclusive Condition Check

### Formula

```excel
=XOR(E2>70000,F2>10000)
```

### Explanation

Returns **TRUE** only when exactly one of the two conditions is TRUE.

---

# Part H – IFERROR Function

## Solution 15 – Bonus Percentage

### Formula

```excel
=IFERROR(F2/E2,"Invalid")
```

---

## Solution 16 – Salary Per Year of Experience

### Formula

```excel
=IFERROR(E2/G2,"Invalid")
```

---

# Part I – IFNA Function

## Solution 17 – Department Code Lookup

Assume the following lookup table is created in **N2:O7**

| Department | Code |
|------------|------|
| IT | D001 |
| HR | D002 |
| Sales | D003 |
| Finance | D004 |
| Support | D005 |
| Marketing | D006 |

### Formula

```excel
=IFNA(VLOOKUP(C2,$N$2:$O$7,2,FALSE),"Department Not Found")
```

---

# ⭐ Challenge Solutions

## Challenge 1 – Employee Status

### Formula

```excel
=IF(AND(E2>=70000,G2>=5),
"Senior Employee",
IF(E2>=50000,
"Regular Employee",
"Junior Employee"))
```

---

## Challenge 2 – Special Bonus Eligibility

### Formula

```excel
=IF(AND(OR(C2="IT",C2="Finance"),E2>=75000),
"Eligible",
"Not Eligible")
```

---

## Challenge 3 – Old or New Employee

### Formula

```excel
=IF(H2<DATE(2021,1,1),
"Old Employee",
"New Employee")
```

---

## Challenge 4 – Bonus Category

### Formula

```excel
=IFS(
F2>=15000,"Excellent",
F2>=10000,"Good",
F2>=5000,"Average",
TRUE,"Low")
```

---

## Challenge 5 – HR Decision

### Formula

```excel
=IF(AND(G2>=5,E2>=70000),
"Promote",
IF(G2>=5,
"Review",
"Training Required"))
```

---

# ✅ Lab Completion Checklist

- [ ] Used IF function correctly
- [ ] Completed Nested IF exercises
- [ ] Applied IFS function
- [ ] Used AND and OR correctly
- [ ] Understood NOT and XOR
- [ ] Handled errors using IFERROR
- [ ] Used IFNA with VLOOKUP
- [ ] Completed all challenge questions

---

