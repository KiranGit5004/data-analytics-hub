# 📘 Date & Time Functions in Microsoft Excel

## 🎯 Objective

Learn how to use Date & Time Functions in Microsoft Excel to perform date calculations, manage schedules, track employee records, calculate project durations, and automate time-based analysis.

Date functions are widely used in **Data Analysis**, **Human Resources**, **Finance**, **Project Management**, **Sales Reporting**, and **Business Intelligence**.

---

# What are Date & Time Functions?

Date & Time Functions are built-in Excel formulas used to create, extract, calculate, and manipulate dates and times.

They help users perform calculations such as:

- Calculate employee age
- Calculate years of experience
- Determine project duration
- Find working days
- Calculate deadlines
- Generate today's date automatically
- Calculate month-end dates
- Analyze time-based business data

---

# Why Learn Date & Time Functions?

Date functions help you:

- Automate reports
- Calculate durations
- Reduce manual calculations
- Track employee experience
- Build attendance reports
- Create project timelines
- Perform time-based business analysis
- Improve dashboard automation

---

# Functions Covered

| Function | Purpose |
|----------|---------|
| TODAY | Returns today's date |
| NOW | Returns current date and time |
| DATE | Creates a valid date |
| DAY | Extracts the day |
| MONTH | Extracts the month |
| YEAR | Extracts the year |
| WEEKDAY | Returns the weekday number |
| WEEKNUM | Returns the week number |
| EDATE | Adds or subtracts months |
| EOMONTH | Returns the last day of a month |
| WORKDAY | Calculates the next working day |
| NETWORKDAYS | Counts working days |
| DATEDIF | Calculates the difference between two dates |

---

# Understanding Excel Dates

Excel stores dates as **serial numbers**.

Example:

| Date | Serial Number |
|------|---------------|
| 01-Jan-1900 | 1 |
| 01-Jan-2025 | 45658 (approx.) |

This allows Excel to perform mathematical operations on dates.

---

# Date Formats in Excel

| Format | Example |
|---------|----------|
| dd-mm-yyyy | 15-07-2026 |
| dd/mm/yyyy | 15/07/2026 |
| mmm-yyyy | Jul-2026 |
| dd-mmm-yyyy | 15-Jul-2026 |
| dddd | Tuesday |

---

# 1. TODAY Function

## Purpose

Returns the current system date.

### Syntax

```excel
=TODAY()
```

### Example

If today's date is **12-Jul-2026**

```excel
=TODAY()
```

Output

```
12-Jul-2027
```

### Real-World Uses

- Attendance reports
- Leave management
- Employee age
- Experience calculation
- Dashboard refresh date

---

# 2. NOW Function

## Purpose

Returns the current date and time.

### Syntax

```excel
=NOW()
```

### Example

```
12-Jul-2026 10:45 AM
```

### Real-World Uses

- Time stamping reports
- Logging transactions
- Dashboard refresh

---

# Difference Between TODAY and NOW

| TODAY | NOW |
|--------|-----|
| Returns only the date | Returns date and time |
| No time information | Includes current time |

---

# 3. DATE Function

## Purpose

Creates a valid date from year, month, and day.

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

### Real-World Example

Generate invoice dates, joining dates, or project start dates.

---

# 4. DAY Function

## Purpose

Extracts the day from a date.

### Syntax

```excel
=DAY(date)
```

### Example

```excel
=DAY("12-Jul-2026")
```

Result

```
12
```

---

# 5. MONTH Function

## Purpose

Returns the month number.

### Syntax

```excel
=MONTH(date)
```

### Example

```excel
=MONTH("12-Jul-2026")
```

Result

```
7
```

---

# 6. YEAR Function

## Purpose

Extracts the year from a date.

### Syntax

```excel
=YEAR(date)
```

### Example

```excel
=YEAR("12-Jul-2026")
```

Result

```
2026
```

---

# 7. WEEKDAY Function

## Purpose

Returns the day of the week as a number.

### Syntax

```excel
=WEEKDAY(date,[return_type])
```

### Example

```excel
=WEEKDAY("12-Jul-2026")
```

Result

```
1–7
```

Depending on the `return_type`, Sunday or Monday can be treated as the first day of the week.

### Real-World Uses

- Attendance tracking
- Weekend identification
- Shift scheduling

---

# 8. WEEKNUM Function

## Purpose

Returns the week number of a date.

### Syntax

```excel
=WEEKNUM(date)
```

### Example

```excel
=WEEKNUM(TODAY())
```

### Real-World Uses

- Weekly sales reports
- Weekly project tracking
- KPI dashboards

---

# 9. EDATE Function

## Purpose

Adds or subtracts months from a date.

### Syntax

```excel
=EDATE(start_date,months)
```

### Example

```excel
=EDATE("12-Jul-2026",6)
```

Result

```
12-Jan-2027
```

### Real-World Uses

- Contract expiry dates
- EMI schedules
- Renewal reminders

---

# 10. EOMONTH Function

## Purpose

Returns the last day of a month.

### Syntax

```excel
=EOMONTH(start_date,months)
```

### Example

```excel
=EOMONTH("12-Jul-2026",0)
```

Result

```
31-Jul-2026
```

### Real-World Uses

- Month-end reporting
- Financial closing
- Payroll processing

---

# 11. WORKDAY Function

## Purpose

Calculates a future or past working day, excluding weekends.

### Syntax

```excel
=WORKDAY(start_date,days)
```

### Example

```excel
=WORKDAY(TODAY(),10)
```

Returns the date after 10 working days.

### Real-World Uses

- Project deadlines
- Delivery schedules
- Leave planning

---

# 12. NETWORKDAYS Function

## Purpose

Counts the number of working days between two dates.

### Syntax

```excel
=NETWORKDAYS(start_date,end_date)
```

### Example

```excel
=NETWORKDAYS(A2,B2)
```

### Real-World Uses

- Employee attendance
- Payroll calculations
- Project duration
- Leave management

---

# 13. DATEDIF Function

## Purpose

Calculates the difference between two dates.

> **Note:** `DATEDIF` exists in Excel but does not appear in Formula AutoComplete.

### Syntax

```excel
=DATEDIF(start_date,end_date,unit)
```

### Units

| Unit | Meaning |
|------|---------|
| "Y" | Years |
| "M" | Months |
| "D" | Days |
| "YM" | Remaining Months |
| "MD" | Remaining Days |
| "YD" | Days excluding years |

### Example

```excel
=DATEDIF(A2,TODAY(),"Y")
```

Returns employee experience in years.

### Real-World Uses

- Employee age
- Experience calculation
- Contract duration
- Service anniversary

---

# Common Errors

| Error | Reason |
|--------|--------|
| #VALUE! | Invalid date or incorrect data type |
| #NUM! | Invalid date calculation |
| ##### | Column width too small to display the date |
| #NAME? | Incorrect function name |

---

# Best Practices

- Store dates as real Excel dates instead of text.
- Use `TODAY()` for dynamic reports.
- Use `DATE()` instead of manually typing dates in formulas.
- Apply consistent date formatting throughout the workbook.
- Use `NETWORKDAYS()` when calculating business days.
- Use absolute references where appropriate.

---

# Key Takeaways

- TODAY() returns the current date.
- NOW() returns the current date and time.
- DATE() creates valid dates.
- DAY(), MONTH(), and YEAR() extract components from a date.
- WORKDAY() calculates future or past working dates.
- NETWORKDAYS() counts working days between dates.
- DATEDIF() calculates differences between dates.
- EOMONTH() returns the last day of a month.

---

# Summary

After completing this lesson, you should be able to:

- Work confidently with Excel dates and times.
- Calculate employee age and experience.
- Build project schedules and timelines.
- Determine working days and deadlines.
- Create dynamic date-based reports and dashboards.
- Solve real-world business problems using Date & Time Functions.

---
