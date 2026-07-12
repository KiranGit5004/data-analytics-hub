# 📘 Solution – Lab 03: Date & Time Functions

## 🎯 Objective

This document contains the solutions for **Lab 03 – Date & Time Functions**. The formulas below are based on the **Employee_Dataset_Date_Time.xlsx** dataset.

> **Dataset Columns**

| Column | Field |
|---------|-------|
| A | Employee ID |
| B | Employee Name |
| C | Department |
| D | Date of Birth |
| E | Joining Date |
| F | Last Promotion Date |
| G | Project Start Date |
| H | Project End Date |
| I | Leave Start Date |
| J | Leave End Date |

---

# Part A – TODAY Function

## Solution 1 – Display Today's Date

### Formula

```excel
=TODAY()
```

### Explanation

Returns the current system date.

---

## Solution 2 – Days Since Joining

### Formula

```excel
=TODAY()-E2
```

### Explanation

Calculates the total number of days an employee has worked in the company.

---

## Solution 3 – Completed One Year?

### Formula

```excel
=IF(TODAY()>=EDATE(E2,12),"Yes","No")
```

### Explanation

Checks whether the employee has completed one year of service.

---

# Part B – NOW Function

## Solution 4 – Display Current Date & Time

### Formula

```excel
=NOW()
```

---

## Solution 5 – Report Timestamp

### Formula

```excel
=NOW()
```

### Explanation

Displays the current system date and time when the report is generated.

---

# Part C – DATE Function

## Solution 6 – Create Joining Date

### Formula

```excel
=DATE(2024,7,15)
```

---

## Solution 7 – Create Project Start Date

### Formula

```excel
=DATE(2025,1,1)
```

---

# Part D – DAY(), MONTH(), YEAR()

## Solution 8 – Extract Birth Day

### Formula

```excel
=DAY(D2)
```

---

## Solution 9 – Extract Joining Month

### Formula

```excel
=MONTH(E2)
```

---

## Solution 10 – Extract Joining Year

### Formula

```excel
=YEAR(E2)
```

---

# Part E – WEEKDAY()

## Solution 11 – Weekday Number

### Formula

```excel
=WEEKDAY(E2)
```

---

## Solution 12 – Weekend or Weekday

### Formula

```excel
=IF(OR(WEEKDAY(E2)=1,WEEKDAY(E2)=7),"Weekend","Weekday")
```

### Explanation

Returns **Weekend** if the joining date falls on Saturday or Sunday.

---

# Part F – WEEKNUM()

## Solution 13 – Week Number of Joining Date

### Formula

```excel
=WEEKNUM(E2)
```

---

## Solution 14 – Week Number of Project Start Date

### Formula

```excel
=WEEKNUM(G2)
```

---

# Part G – EDATE()

## Solution 15 – Confirmation Date

### Formula

```excel
=EDATE(E2,6)
```

### Explanation

Returns the employee confirmation date after six months.

---

## Solution 16 – Contract Expiry

### Formula

```excel
=EDATE(E2,12)
```

---

# Part H – EOMONTH()

## Solution 17 – Last Day of Joining Month

### Formula

```excel
=EOMONTH(E2,0)
```

---

## Solution 18 – Last Day of Current Month

### Formula

```excel
=EOMONTH(TODAY(),0)
```

---

# Part I – WORKDAY()

## Solution 19 – Project Completion Date

### Formula

```excel
=WORKDAY(G2,30)
```

### Explanation

Returns the date after 30 working days.

---

## Solution 20 – Next Review Date

### Formula

```excel
=WORKDAY(TODAY(),60)
```

---

# Part J – NETWORKDAYS()

## Solution 21 – Working Days Between Project Dates

### Formula

```excel
=NETWORKDAYS(G2,H2)
```

---

## Solution 22 – Employee Leave Working Days

### Formula

```excel
=NETWORKDAYS(I2,J2)
```

---

# Part K – DATEDIF()

## Solution 23 – Employee Age

### Formula

```excel
=DATEDIF(D2,TODAY(),"Y")
```

---

## Solution 24 – Employee Experience

### Formula

```excel
=DATEDIF(E2,TODAY(),"Y")
```

---

## Solution 25 – Experience in Months

### Formula

```excel
=DATEDIF(E2,TODAY(),"M")
```

---

## Solution 26 – Experience in Days

### Formula

```excel
=DATEDIF(E2,TODAY(),"D")
```

---

## Solution 27 – Remaining Months

### Formula

```excel
=DATEDIF(E2,TODAY(),"YM")
```

---

## Solution 28 – Remaining Days

### Formula

```excel
=DATEDIF(E2,TODAY(),"MD")
```

---

# ⭐ Challenge Solutions

## Challenge 1 – Age Category

### Formula

```excel
=IF(DATEDIF(D2,TODAY(),"Y")<25,"Young",
IF(DATEDIF(D2,TODAY(),"Y")<=35,"Adult",
IF(DATEDIF(D2,TODAY(),"Y")<=50,"Experienced","Senior")))
```

---

## Challenge 2 – Work Anniversary Month

### Formula

```excel
=IF(MONTH(E2)=MONTH(TODAY()),"Anniversary Month","Other Month")
```

---

## Challenge 3 – Old or New Employee

### Formula

```excel
=IF(E2<DATE(2020,1,1),"Old Employee","New Employee")
```

---

## Challenge 4 – Completing Five Years of Service

### Formula

```excel
=IF(DATEDIF(E2,TODAY(),"Y")>=5,"Eligible","Not Yet")
```

---

## Challenge 5 – Project Duration

### Years

```excel
=DATEDIF(G2,H2,"Y")
```

### Months

```excel
=DATEDIF(G2,H2,"M")
```

### Days

```excel
=DATEDIF(G2,H2,"D")
```

---

# 📌 Formula Summary

| Task | Function |
|------|----------|
| Current Date | TODAY |
| Current Date & Time | NOW |
| Create Date | DATE |
| Extract Day | DAY |
| Extract Month | MONTH |
| Extract Year | YEAR |
| Weekday Number | WEEKDAY |
| Week Number | WEEKNUM |
| Add Months | EDATE |
| Last Day of Month | EOMONTH |
| Future Working Date | WORKDAY |
| Working Days | NETWORKDAYS |
| Age & Experience | DATEDIF |

---

# ✅ Lab Completion Checklist

- [ ] Used TODAY() correctly
- [ ] Used NOW() correctly
- [ ] Created dates using DATE()
- [ ] Extracted day, month, and year
- [ ] Calculated weekday and week number
- [ ] Added months using EDATE()
- [ ] Calculated month-end dates
- [ ] Used WORKDAY() correctly
- [ ] Calculated working days using NETWORKDAYS()
- [ ] Calculated age and experience using DATEDIF()
- [ ] Completed all challenge questions

---
