# Lab 01 - Basic Text Functions Exercises

---

# Objective

In this lab, you will practice the most commonly used Excel Text Functions by solving practical exercises using employee data.

By the end of this lab, you will be able to:

- Extract text
- Count characters
- Clean text
- Format text
- Combine text
- Convert text
- Search text
- Replace text

---

# Dataset

Open

```
Practice-Workbook.xlsx
```

Use the worksheet:

```
Basic_Practice
```

---

# Functions Covered

- LEFT()
- RIGHT()
- MID()
- LEN()
- TRIM()
- UPPER()
- LOWER()
- PROPER()
- CONCAT()
- TEXTJOIN()
- TEXT()
- VALUE()
- FIND()
- SEARCH()
- REPLACE()
- SUBSTITUTE()

---

# Exercise 1 - LEFT()

Extract the department prefix.

Example

```
EMP-1001
```

### Formula

``` excel
=LEFT(Basic_Practice!A2,3)
```

Expected Output

```
EMP
```

---

# Exercise 2 - RIGHT()

Extract the last four digits of every phone number.

### Formula

``` excel
=RIGHT(Basic_Practice!E2,4)
```

Expected Output

```
3210
6655
6789
```

---

# Exercise 3 - MID()

Extract the Employee Number.

Example

```
EMP-1001
```

Expected Output

```
1001
```

---

# Exercise 4 - LEN()

Find the total number of characters in every employee name.

### Formula

``` excel
=LEN(Basic_Practice!B2)
```

### Expected Output

    Character Count

---

# Exercise 5 - TRIM()

Remove unnecessary spaces from employee names.

Example

```
Rahul      Sharma
```

### Formula

``` excel
=TRIM(Basic_Practice!B2)
```

Expected

```
Rahul Sharma
```

---

# Exercise 6 - UPPER()

Convert every department into uppercase.

### Sample Value

    it

### Formula

``` excel
=UPPER(Basic_Practice!C2)
```

### Expected Output

    IT

---

# Exercise 7 - LOWER()

Convert all email addresses into lowercase.

### Sample Value

    RAHUL@GMAIL.COM

### Formula

``` excel
=LOWER(Basic_Practice!D2)
```

### Expected Output

    rahul@gmail.com

---

# Exercise 8 - PROPER()

Convert employee names into Proper Case.

### Sample Value

    rahul sharma

### Formula

``` excel
=PROPER(TRIM(Basic_Practice!B2))
```

### Expected Output

    Rahul Sharma

---

# Exercise 9 - CONCAT()

Create a Full Employee Label.

### Source Cell

`A2 & B2`

### Sample Value

    EMP-1001

### Formula

``` excel
=CONCAT(Basic_Practice!A2," - ",PROPER(TRIM(Basic_Practice!B2)))
```

### Expected Output

    EMP-1001 - Rahul Sharma

---

# Exercise 10 - TEXTJOIN()

Combine

City, Department, Employee ID using commas.

### Source Cell

`H2,C2,A2`

### Formula

``` excel
=TEXTJOIN(", ",TRUE,Basic_Practice!H2,UPPER(Basic_Practice!C2),Basic_Practice!A2)
```

Expected

```
Nashik, IT, EMP-1001
```

---

# Exercise 11 - TEXT()

Format Joining Date

### Source Cell

`Basic_Practice!F2`

### Sample Value

    01/07/2025

### Formula

``` excel
=TEXT(Basic_Practice!F2,"dd-mmm-yyyy")
```

### Expected Output

    01-Jul-2025

---

# Exercise 12 - VALUE()

Salary is stored as text.

Convert it into numbers.

### Source Cell

`Basic_Practice!G2`

### Sample Value

    45000

### Formula

``` excel
=VALUE(Basic_Practice!G2)
```

### Expected Output

    45000

---

# Exercise 13 - FIND()

Find the position of @ inside every email.

### Source Cell

`Basic_Practice!D2`

### Sample Value

    rahul@gmail.com

### Formula

``` excel
=FIND("@",Basic_Practice!D2)
```

### Expected Output

    6

---

# Exercise 14 - SEARCH()

Search for *gmail* inside every email.

### Source Cell

`Basic_Practice!D2`

### Formula

``` excel
=SEARCH("gmail",Basic_Practice!D2)
```

### Expected Output

    7

---

# Exercise 15 - REPLACE()

Mask the middle digits of every phone number.

Example

```
9876543210
```

### Formula

``` excel
=REPLACE(Basic_Practice!E2,3,8,"******")

Expected

```
98*****10
```

---

# Exercise 16 - SUBSTITUTE()

Replace EMP with Staff

### Source Cell

`Basic_Practice!A2`

### Sample Value

    EMP-1001

### Formula

``` excel
=SUBSTITUTE(Basic_Practice!A2,"EMP","STAFF")
```

### Expected Output

    STAFF-1001

---
