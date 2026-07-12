# 📘 Interview Questions & Answers – Date & Time Functions in Microsoft Excel

# 1. What are Date & Time Functions in Excel?

### Answer

Date & Time Functions are built-in Excel functions used to create, extract, calculate, and manipulate dates and times.

They are commonly used for:

- Employee Experience Calculation
- Attendance Tracking
- Payroll Processing
- Project Scheduling
- Invoice Management
- Sales Reporting
- Financial Analysis

---

# 2. What is the TODAY() function?

### Answer

The **TODAY()** function returns the current system date.

### Syntax

```excel
=TODAY()
```

### Example

```excel
=TODAY()
```

Output

```
12-Jul-2026
```

---

# 3. What is the NOW() function?

### Answer

The **NOW()** function returns the current date and current time.

### Syntax

```excel
=NOW()
```

### Example

```excel
=NOW()
```

Output

```
12-Jul-2026 10:45 AM
```

---

# 4. What is the difference between TODAY() and NOW()?

### Answer

| TODAY() | NOW() |
|----------|--------|
| Returns only the current date | Returns the current date and time |
| Time is not included | Time is included |

---

# 5. What is the DATE() function?

### Answer

The **DATE()** function creates a valid Excel date using year, month, and day values.

### Syntax

```excel
=DATE(year,month,day)
```

### Example

```excel
=DATE(2026,7,12)
```

Result

```
12-Jul-2026
```

---

# 6. What is the purpose of the DAY(), MONTH(), and YEAR() functions?

### Answer

These functions extract individual components from a date.

| Function | Returns |
|----------|----------|
| DAY() | Day |
| MONTH() | Month |
| YEAR() | Year |

### Example

```excel
=DAY(A2)
=MONTH(A2)
=YEAR(A2)
```

---

# 7. What does the WEEKDAY() function do?

### Answer

The **WEEKDAY()** function returns the day of the week as a number.

### Syntax

```excel
=WEEKDAY(date)
```

Example

| Date | Result |
|------|--------|
| Monday | 2 |
| Friday | 6 |

*(Default numbering where Sunday = 1)*

---

# 8. What is the WEEKNUM() function?

### Answer

The **WEEKNUM()** function returns the week number of a specified date.

### Syntax

```excel
=WEEKNUM(date)
```

### Example

```excel
=WEEKNUM(TODAY())
```

---

# 9. What is the EDATE() function?

### Answer

The **EDATE()** function adds or subtracts a specified number of months from a date.

### Syntax

```excel
=EDATE(start_date,months)
```

### Example

```excel
=EDATE(A2,6)
```

Returns the date six months after the date in A2.

---

# 10. What is the EOMONTH() function?

### Answer

The **EOMONTH()** function returns the last day of a month.

### Syntax

```excel
=EOMONTH(start_date,months)
```

### Example

```excel
=EOMONTH(A2,0)
```

---

# 11. What is the WORKDAY() function?

### Answer

The **WORKDAY()** function returns a future or past working day by excluding weekends.

### Syntax

```excel
=WORKDAY(start_date,days)
```

### Example

```excel
=WORKDAY(TODAY(),15)
```

Returns the date after 15 working days.

---

# 12. What is the NETWORKDAYS() function?

### Answer

The **NETWORKDAYS()** function calculates the number of working days between two dates.

### Syntax

```excel
=NETWORKDAYS(start_date,end_date)
```

### Example

```excel
=NETWORKDAYS(A2,B2)
```

---

# 13. What is DATEDIF()?

### Answer

The **DATEDIF()** function calculates the difference between two dates.

### Syntax

```excel
=DATEDIF(start_date,end_date,unit)
```

### Units

| Unit | Description |
|------|-------------|
| "Y" | Years |
| "M" | Months |
| "D" | Days |
| "YM" | Remaining Months |
| "MD" | Remaining Days |
| "YD" | Days excluding Years |

---

# 14. Why doesn't DATEDIF() appear in Formula AutoComplete?

### Answer

DATEDIF() is a hidden compatibility function.

Although it is supported by Excel, it does not appear in the Formula AutoComplete list.

---

# 15. How do you calculate an employee's age in Excel?

### Answer

Using DATEDIF()

```excel
=DATEDIF(A2,TODAY(),"Y")
```

Where A2 contains the employee's Date of Birth.

---

# 16. How do you calculate an employee's years of experience?

### Answer

```excel
=DATEDIF(A2,TODAY(),"Y")
```

Where A2 contains the Joining Date.

---

# 17. What is the difference between WORKDAY() and NETWORKDAYS()?

### Answer

| WORKDAY() | NETWORKDAYS() |
|------------|---------------|
| Returns a future or past working date | Counts working days between two dates |
| Output is a Date | Output is a Number |

---

# 18. What are common errors while working with dates?

### Answer

Common mistakes include:

- Dates stored as Text
- Invalid date formats
- Incorrect regional date settings
- Wrong date separators
- Using text instead of actual date values

---

# 19. What are common business applications of Date Functions?

### Answer

Date functions are used for:

- Employee Age Calculation
- Experience Calculation
- Payroll
- Leave Tracking
- Attendance Reports
- Project Timelines
- Invoice Due Dates
- Financial Reports
- Delivery Scheduling
- KPI Dashboards

---

# 20. Which Date Functions are most important for Data Analysts?

### Answer

The most frequently used Date Functions are:

- TODAY()
- NOW()
- DATE()
- YEAR()
- MONTH()
- DAY()
- DATEDIF()
- WORKDAY()
- NETWORKDAYS()
- EOMONTH()

These functions are commonly used in reporting, dashboards, and HR analytics.

---

# 💡 Interview Tips

- Always store dates as actual Excel dates, not text.
- Know the difference between TODAY() and NOW().
- Learn when to use WORKDAY() versus NETWORKDAYS().
- Practice calculating age and experience using DATEDIF().
- Understand how Excel internally stores dates as serial numbers.

---

# 📌 Quick Revision Table

| Function | Purpose |
|----------|---------|
| TODAY | Current Date |
| NOW | Current Date & Time |
| DATE | Create Date |
| DAY | Extract Day |
| MONTH | Extract Month |
| YEAR | Extract Year |
| WEEKDAY | Day Number |
| WEEKNUM | Week Number |
| EDATE | Add/Subtract Months |
| EOMONTH | Last Day of Month |
| WORKDAY | Next/Previous Working Date |
| NETWORKDAYS | Count Working Days |
| DATEDIF | Difference Between Dates |

---
