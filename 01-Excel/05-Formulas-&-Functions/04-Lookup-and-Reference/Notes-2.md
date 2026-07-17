# 3. XLOOKUP Function

## What is XLOOKUP?

**XLOOKUP** is a modern lookup function introduced in Microsoft Excel 365 and Excel 2021.

It is designed to replace **VLOOKUP** and **HLOOKUP** by providing a more flexible and powerful way to retrieve data.

Unlike VLOOKUP, XLOOKUP can search:

- Left to Right
- Right to Left
- Top to Bottom
- Bottom to Top

It also supports custom error messages without requiring IFERROR().

---

# Purpose

Use XLOOKUP to:

- Retrieve employee information
- Search product prices
- Find customer records
- Return values from any direction
- Replace VLOOKUP and HLOOKUP

---

# Syntax

```excel
=XLOOKUP(lookup_value, lookup_array, return_array, [if_not_found], [match_mode], [search_mode])
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| lookup_value | Value to search |
| lookup_array | Column or row containing lookup values |
| return_array | Column or row containing return values |
| if_not_found | Value returned if no match is found |
| match_mode | Exact or approximate matching |
| search_mode | Search direction |

---

# Example 1

## Employee Dataset

| Employee ID | Name | Salary |
|--------------|------|---------|
| EMP001 | Rahul | 50000 |
| EMP002 | Sneha | 65000 |
| EMP003 | Amit | 70000 |

Find the salary of EMP002.

```excel
=XLOOKUP("EMP002",A2:A4,C2:C4)
```

Result

```
65000
```

---

# Example 2

Custom Error Message

```excel
=XLOOKUP(E2,A2:A100,C2:C100,"Employee Not Found")
```

Instead of returning **#N/A**, Excel displays:

```
Employee Not Found
```

---

# Example 3

Lookup from Right to Left

Suppose Employee ID is in Column C and Name is in Column A.

```excel
=XLOOKUP(C2,C2:C100,A2:A100)
```

Unlike VLOOKUP, XLOOKUP can retrieve values from the left.

---

# Advantages of XLOOKUP

- Replaces VLOOKUP and HLOOKUP
- Searches in any direction
- Supports custom error handling
- Does not require column index numbers
- More readable formulas
- Faster on large datasets

---

# Limitations

- Available only in Excel 365 and Excel 2021+
- Not supported in older Excel versions

---

# Best Practices

- Use XLOOKUP whenever available.
- Specify a custom **if_not_found** message.
- Use exact matching by default.

---
---

# 4. INDEX Function

## What is INDEX?

The **INDEX** function returns the value located at a specified row and column within a range.

Unlike lookup functions, INDEX does not search for values—it simply retrieves data based on position.

---

# Syntax

```excel
=INDEX(array,row_num,[column_num])
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| array | Data range |
| row_num | Row number |
| column_num | Column number |

---

# Example

| Name | Salary |
|------|---------|
| Rahul | 50000 |
| Sneha | 65000 |
| Amit | 70000 |

Formula

```excel
=INDEX(B2:B4,2)
```

Result

```
65000
```

---

# Two-Dimensional Example

| | A | B | C |
|---|---|---|---|
|1|Name|Department|Salary|
|2|Rahul|IT|50000|
|3|Sneha|HR|65000|

Formula

```excel
=INDEX(A2:C3,2,3)
```

Result

```
65000
```

---

# Advantages

- Fast
- Flexible
- Dynamic
- Does not depend on lookup direction

---

# Limitations

- Requires row and column numbers.
- Usually combined with MATCH for dynamic lookups.

---

# Best Practices

- Use INDEX with MATCH instead of VLOOKUP for advanced lookups.
- Lock ranges using absolute references.

---

# 5. MATCH Function

## What is MATCH?

The **MATCH** function returns the **position** of a value within a range.

It does **not** return the value itself.

---

# Purpose

Use MATCH to:

- Find row numbers
- Find column numbers
- Work with INDEX
- Build dynamic lookup formulas

---

# Syntax

```excel
=MATCH(lookup_value,lookup_array,[match_type])
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| lookup_value | Value to search |
| lookup_array | Search range |
| match_type | Match type |

---

# Match Types

| Value | Meaning |
|-------|----------|
| 0 | Exact Match |
| 1 | Less than |
| -1 | Greater than |

For most business scenarios, use:

```excel
0
```

---

# Example

| Employee ID |
|--------------|
| EMP001 |
| EMP002 |
| EMP003 |

Formula

```excel
=MATCH("EMP002",A2:A4,0)
```

Result

```
2
```

Meaning EMP002 is located in the **second position** of the range.

---

# Real-World Example

Suppose you need to know where an employee appears in a dataset before retrieving additional information.

MATCH identifies the row position, which can then be passed to INDEX.

---

# Advantages

- Dynamic
- Fast
- Works with INDEX
- Searches vertically or horizontally

---

# Limitations

- Returns only the position.
- Does not return actual values.

---

# Difference Between INDEX and MATCH

| INDEX | MATCH |
|--------|--------|
| Returns a value | Returns a position |
| Requires row/column numbers | Finds row/column numbers |
| Often combined with MATCH | Often combined with INDEX |

---

# Best Practices

- Always use **0** for exact matches unless approximate matching is required.
- Combine INDEX and MATCH for flexible lookups.
- Lock lookup ranges using absolute references.
- Use IFERROR() or XLOOKUP's built-in error handling for user-friendly results.

---

# Key Takeaways

- **XLOOKUP** is the modern replacement for VLOOKUP and HLOOKUP.
- **INDEX** retrieves a value based on row and column position.
- **MATCH** returns the position of a lookup value.
- INDEX and MATCH are commonly combined to create powerful, dynamic lookup solutions.
- These functions are widely used in Data Analysis, MIS reporting, dashboards, and business reporting.

---
