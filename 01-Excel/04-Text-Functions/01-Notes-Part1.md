# Text Functions in Excel 

# Introduction

Text Functions are built-in Excel functions used to manipulate, extract, combine, clean, and analyze text values. They help transform raw data into meaningful information without manually editing each cell.

In Data Analytics, datasets often contain employee names, customer IDs, email addresses, phone numbers, product codes, invoice numbers, and many other text-based fields. Text Functions make it easy to clean and prepare this data before analysis.

Learning these functions is essential because data received from databases, websites, ERP systems, CRM software, and CSV files is rarely perfectly formatted.

---

# Why Text Functions Matter

A Data Analyst spends a significant amount of time cleaning data before performing any analysis.

Common tasks include:

- Extracting Employee IDs
- Splitting First and Last Names
- Removing unwanted spaces
- Counting characters
- Validating product codes
- Standardizing imported data
- Preparing datasets for Power Query and Power BI

Instead of editing thousands of rows manually, Text Functions automate these tasks in seconds.

---

# Categories of Text Functions

| Category | Functions |
|-----------|-----------|
| Text Extraction | LEFT, RIGHT, MID |
| Text Length | LEN |
| Text Formatting | UPPER, LOWER, PROPER |
| Text Cleaning | TRIM |
| Text Combining | CONCAT, TEXTJOIN |
| Text Conversion | TEXT, VALUE |
| Text Searching | FIND, SEARCH |
| Text Replacement | REPLACE, SUBSTITUTE |

> **Note**
>
> In this part, we will focus on the Text Extraction and Text Length functions.

---

# 1.LEFT()

## Definition

The **LEFT** function returns a specified number of characters from the beginning (left side) of a text string.

It is commonly used when important information appears at the beginning of a value.

---

## Syntax

```excel
=LEFT(text,[num_chars])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | The text string to extract characters from |
| num_chars | Number of characters to return from the left |

---

## Return Value

Returns the specified number of characters starting from the left side.

---

## Example 

Assume Cell A2 contains

```
EMP-1001
```

Formula

```excel
=LEFT(A2,3)
```

Result

```
EMP
```

---

## Real-World Data Analytics Example

Employee IDs

| Employee ID |
|-------------|
| EMP-1001 |
| HR-2025 |
| FIN-3010 |

Extract Department Code

```excel
=LEFT(A2,3)
```

Result

| Output |
|---------|
| EMP |
| HR- |
| FIN |

This can be used to categorize employees by department.

---

## Common Mistakes

Incorrect

```excel
=LEFT(A2)
```

Many users expect the entire text.

Actual Result

Only the first character.

---

# 2.RIGHT()

## Definition

The **RIGHT** function returns a specified number of characters from the end (right side) of a text string.

This function is useful when important information appears at the end of a value.

---

## Syntax

```excel
=RIGHT(text,[num_chars])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | Text string |
| num_chars | Number of characters to extract |

---

## Return Value

Returns characters from the right side.

---

## Example 

```excel
=RIGHT("Analytics",4)
```

Result

```
tics
```

---

## Real-World Example

Invoice Numbers

| Invoice |
|----------|
| INV-2025-001 |
| INV-2025-002 |
| INV-2025-003 |

Formula

```excel
=RIGHT(A2,3)
```

Output

```
001
002
003
```

Useful for extracting serial numbers.

---

## Common Mistakes

Forgetting that spaces count as characters.

Example

```
Excel 
```

contains an extra space after the word.

---

# 3.MID()

## Definition

The **MID** function extracts characters from the middle of a text string.

Unlike LEFT and RIGHT, MID allows you to specify both the starting position and the number of characters to extract.

---

## Syntax

```excel
=MID(text,start_num,num_chars)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | Text string |
| start_num | Starting position |
| num_chars | Number of characters to return |

---

## Return Value

Returns characters from any position within the text.

---

## Example 

```excel
=MID("Analytics",3,4)
```

Result

```
alyt
```

---

## Real-World Example

Order Number

```
ORD-2025-4589
```

Extract Year

```excel
=MID(A2,5,4)
```

Result

```
2025
```

---

## Tips

Character positions begin at **1**, not 0.

Example

```
H E L L O

1 2 3 4 5
```

---

# 4.LEN()

## Definition

The **LEN** function counts the total number of characters in a text string.

It counts:

- Letters
- Numbers
- Spaces
- Special Characters

---

## Syntax

```excel
=LEN(text)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | Text string whose length will be calculated |

---

## Return Value

Returns the total number of characters.

---

## Example 1

```excel
=LEN("Excel")
```

Result

```
5
```

---

## Example 2

```
John Smith
```

Formula

```excel
=LEN(A2)
```

Result

```
10
```

The space between John and Smith is counted.

---

## Real-World Example

Password Validation

Requirement

Password should contain at least 8 characters.

Formula

```excel
=LEN(A2)
```

If result is less than 8

Password is invalid.

---

## Common Mistakes

Many users believe LEN ignores spaces.

It does **not**.

To ignore extra spaces, combine LEN with TRIM.

Example

```excel
=LEN(TRIM(A2))
```

---

# Comparison Table

| Function | Purpose | Example |
|-----------|----------|---------|
| LEFT | Extract characters from the beginning | Employee Prefix |
| RIGHT | Extract characters from the end | Last 4 digits of Phone Number |
| MID | Extract characters from any position | Year from Invoice Number |
| LEN | Count total characters | Password Validation |

---

# Real-World Business Scenario

Imagine you receive employee information from an HR system.

| Employee ID | Employee Name | Phone |
|-------------|---------------|--------|
| EMP-1001 | Rahul Sharma | 9876543210 |
| EMP-1002 | Priya Singh | 9988776655 |
| EMP-1003 | Amit Patel | 9123456789 |

Using the functions learned in this chapter, you can:

| Task | Function |
|------|----------|
| Extract Employee Prefix | LEFT |
| Extract Employee Number | MID |
| Extract Last Four Digits of Phone | RIGHT |
| Count Characters in Employee Name | LEN |

These tasks are commonly performed while cleaning HR datasets before analysis.

---

# Best Practices

- Use descriptive formulas for better readability.
- Verify character positions before using MID.
- Remember that LEN counts spaces.
- Use LEFT and RIGHT only when the required data is consistently positioned.
- Test formulas with sample data before applying them to large datasets.

---

# Summary

In this chapter, you learned four essential Excel Text Functions used in data cleaning and preparation.

Functions Covered:

- LEFT()
- RIGHT()
- MID()
- LEN()

These functions are widely used in Data Analytics to extract meaningful information from raw text, validate datasets, and prepare data for reporting and visualization.

---
