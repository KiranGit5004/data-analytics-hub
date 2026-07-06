# Text Functions in Excel - Part 3

---

# Table of Contents

1. CONCAT()
2. TEXTJOIN()
3. TEXT()
4. VALUE()
5. Comparison Table
6. Real-World Business Scenario
7. Best Practices
8. Common Mistakes


---

# 1. CONCAT()

## Definition

The **CONCAT** function combines multiple text strings into a single text string.

It is the modern replacement for the **CONCATENATE** function and is available in Excel 2019 and Microsoft 365.

It is commonly used to create full names, employee IDs, email addresses, addresses, and custom labels.

---

## Syntax

```excel
=CONCAT(text1,[text2],...)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text1 | First text value |
| text2... | Additional text values (optional) |

---

## Return Value

Returns a single combined text string.

---

## Example 1

```excel
=CONCAT("Data"," ","Analytics")
```

Result

```
Data Analytics
```

---

## Example 2

| First Name | Last Name |
|------------|-----------|
| Rahul | Sharma |

Formula

```excel
=CONCAT(A2," ",B2)
```

Result

```
Rahul Sharma
```

---

## Real-World Data Analytics Example

Creating Email IDs

| First Name | Last Name |
|------------|-----------|
| Rahul | Sharma |

Formula

```excel
=LOWER(CONCAT(A2,".",B2,"@company.com"))
```

Result

```
rahul.sharma@company.com
```

---

## Tips

- CONCAT can join numbers and text.
- Spaces must be added manually.

Example

```excel
=CONCAT(A2," ",B2)
```

---

## Common Mistakes

Incorrect

```excel
=CONCAT(A2,B2)
```

Result

```
RahulSharma
```

No space is added.

---

# 2. TEXTJOIN()

## Definition

The **TEXTJOIN** function combines multiple text values using a specified delimiter.

Unlike CONCAT, TEXTJOIN automatically inserts separators such as commas, spaces, hyphens, or line breaks.

---

## Syntax

```excel
=TEXTJOIN(delimiter,ignore_empty,text1,[text2],...)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| delimiter | Character to insert between values |
| ignore_empty | TRUE or FALSE |
| text1 | First value |
| text2... | Additional values |

---

## Return Value

Returns combined text separated by the chosen delimiter.

---

## Example 1

Employee Address

| City | State | Country |
|------|-------|----------|
| Nashik | Maharashtra | India |

Formula

```excel
=TEXTJOIN(", ",TRUE,A2:C2)
```

Result

```
Nashik, Maharashtra, India
```

---

## Example 2

Ignore Empty Cells

| A | B | C |
|---|---|---|
| Rahul | | Sharma |

Formula

```excel
=TEXTJOIN(" ",TRUE,A2:C2)
```

Result

```
Rahul Sharma
```

---

## Real-World Data Analytics Example

Generate complete mailing addresses from multiple columns while ignoring blank values.

---

## Tips

TEXTJOIN is ideal when:

- Some cells may be blank
- Delimiters are required
- Combining large ranges

---

# 3. TEXT()

## Definition

The **TEXT** function converts a number into text while applying a custom format.

It is commonly used to display dates, currency, percentages, and numbers in a readable format.

---

## Syntax

```excel
=TEXT(value,format_text)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| value | Numeric value |
| format_text | Desired display format |

---

## Return Value

Returns formatted text.

---

## Example 1

Formula

```excel
=TEXT(1500,"₹#,##0")
```

Result

```
₹1,500
```

---

## Example 2

Percentage

Formula

```excel
=TEXT(0.875,"0%")
```

Result

```
88%
```

---

## Real-World Data Analytics Example

Dashboard reports often require dates in a specific format.

Instead of

```
45839
```

Display

```
01-Jul-2025
```

Formula

```excel
=TEXT(A2,"dd-mmm-yyyy")
```

---

## Tips

TEXT changes the number into **text**.

The formatted result cannot be used directly for calculations.

---

## Common Mistakes

Trying to perform arithmetic on TEXT results.

Example

```
"100"
```

is text, not a number.

---

# 4. VALUE()

## Definition

The **VALUE** function converts text that looks like a number into an actual numeric value.

It is especially useful when data is imported from websites, CSV files, PDFs, or ERP systems.

---

## Syntax

```excel
=VALUE(text)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | Numeric value stored as text |

---

## Return Value

Returns a numeric value.

---

## Example 1

Text

```
"500"
```

Formula

```excel
=VALUE(A2)
```

Result

```
500
```

(Number)

---

## Example 2

Imported Sales Data

| Sales |
|--------|
| '2500 |
| '4500 |
| '8000 |

Formula

```excel
=VALUE(A2)
```

Result

```
2500
4500
8000
```

---

## Real-World Data Analytics Example

Many website exports store numbers as text.

Before calculating totals or averages, convert them using VALUE.

---

## Example

Formula

```excel
=SUM(B2:B20)
```

If numbers are stored as text

Result

```
0
```

After using VALUE

Formula

```excel
=VALUE(B2)
```

Excel recognizes them as numbers.

---

## Tips

Use VALUE after importing data from:

- CSV Files
- PDFs
- Websites
- ERP Systems
- CRM Software

---

## Common Mistakes

Trying to convert non-numeric text.

Example

```excel
=VALUE("Excel")
```

Result

```
#VALUE!
```

---

# Comparison Table

| Function | Purpose | Common Use |
|-----------|----------|------------|
| CONCAT | Combine text | Full Name |
| TEXTJOIN | Combine with delimiter | Address |
| TEXT | Convert number to formatted text | Date, Currency |
| VALUE | Convert text to number | Imported Data |

---

# Which Function Should You Use?

| Situation | Function |
|-----------|----------|
| Join first and last names | CONCAT |
| Join address fields | TEXTJOIN |
| Display dates professionally | TEXT |
| Convert imported numbers | VALUE |

---

# Real-World Business Scenario

Employee Data

| First | Last | Joining Date | Salary |
|-------|------|--------------|---------|
| Rahul | Sharma | 45839 | '45000 |

Required Tasks

| Task | Function |
|------|----------|
| Create Full Name | CONCAT |
| Create Address | TEXTJOIN |
| Format Joining Date | TEXT |
| Convert Salary into Number | VALUE |

These functions are frequently used while preparing HR, Finance, Sales, and Customer datasets for reporting.

---

# Best Practices

- Use CONCAT instead of CONCATENATE in newer Excel versions.
- Use TEXTJOIN when separators are required.
- Apply TEXT only for presentation purposes.
- Convert imported numeric text using VALUE before calculations.
- Validate data types after importing datasets.

---
