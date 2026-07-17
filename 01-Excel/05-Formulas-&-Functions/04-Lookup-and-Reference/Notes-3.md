# 6. INDEX + MATCH

## What is INDEX + MATCH?

The **INDEX + MATCH** combination is one of the most powerful lookup techniques in Microsoft Excel.

Instead of relying on column numbers like VLOOKUP, INDEX + MATCH dynamically finds the correct row and retrieves the desired value.

It is considered the professional alternative to VLOOKUP.

---

# Why Use INDEX + MATCH?

Compared to VLOOKUP, INDEX + MATCH:

- Searches both left and right
- Doesn't break when columns are inserted
- Faster on large datasets
- More flexible
- Easier to maintain

---

# Syntax

```excel
=INDEX(return_array,MATCH(lookup_value,lookup_array,0))
```

---

# Example

## Employee Dataset

| Employee ID | Name | Salary |
|-------------|------|---------|
| EMP001 | Rahul | 50000 |
| EMP002 | Sneha | 65000 |
| EMP003 | Amit | 70000 |

Find Salary of EMP002

Formula

```excel
=INDEX(C2:C4,MATCH("EMP002",A2:A4,0))
```

Result

```
65000
```

---

# Real-World Example

Retrieve:

- Employee Salary
- Department
- Designation
- Manager Name

using Employee ID.

---

# Advantages

- Dynamic
- Fast
- Flexible
- Works in every direction
- Recommended by Microsoft

---

# INDEX + MATCH + MATCH (2D Lookup)

Sometimes data is arranged like this.

| Employee | Jan | Feb | Mar |
|-----------|-----|-----|-----|
| Rahul | 5000 | 5500 | 6000 |
| Sneha | 6000 | 6500 | 7000 |

Find Rahul's February Salary.

Formula

```excel
=INDEX(B2:D3,
MATCH("Rahul",A2:A3,0),
MATCH("Feb",B1:D1,0))
```

Result

```
5500
```

---

# 7. CHOOSE Function

## What is CHOOSE?

The CHOOSE function returns a value from a list based on an index number.

---

# Purpose

Useful for:

- Grades
- Categories
- Dynamic Reports
- Region Selection

---

# Syntax

```excel
=CHOOSE(index_num,value1,[value2],...)
```

---

# Example 

Suppose

A2 contains

```
3
```

Formula

```excel
=CHOOSE(A2,"Poor","Average","Good","Excellent")
```

Result

```
Good
```

---

# Advantages

- Easy to use
- Good for fixed lists
- Makes formulas shorter

---

# Limitations

- Not suitable for very large datasets
- Limited number of values

---

# 8. OFFSET Function

## What is OFFSET?

The OFFSET function returns a reference to a cell or range based on a starting point.

---

# Purpose

OFFSET is commonly used for:

- Dynamic Ranges
- Dashboards
- Charts
- Reports
- Moving References

---

# Syntax

```excel
=OFFSET(reference,rows,cols,[height],[width])
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| reference | Starting cell |
| rows | Move up/down |
| cols | Move left/right |
| height | Height of range |
| width | Width of range |

---

# Example

Suppose

```
A1 = Rahul
A2 = Sneha
A3 = Amit
```

Formula

```excel
=OFFSET(A1,2,0)
```

Result

```
Amit
```

---

# Example 2

Return a range

```excel
=SUM(OFFSET(A1,0,0,5,1))
```

Returns the sum of five cells starting from A1.

---

# Advantages

- Dynamic
- Powerful
- Excellent for dashboards
- Creates dynamic ranges

---

# Limitations

- Can slow down large workbooks
- Harder to understand for beginners

---

# Comparison Table

| Feature | VLOOKUP | XLOOKUP | INDEX+MATCH |
|----------|----------|----------|-------------|
| Left Lookup | ❌ | ✅ | ✅ |
| Right Lookup | ✅ | ✅ | ✅ |
| Dynamic | ❌ | ✅ | ✅ |
| Faster | Medium | Fast | Fast |
| Breaks After Column Insert | Yes | No | No |
| Excel Version | All | 365+ | All |

---

# Best Practices

- Prefer **XLOOKUP** over VLOOKUP if available.
- Use **INDEX + MATCH** for professional reporting.
- Avoid hardcoded column numbers.
- Lock lookup ranges using **absolute references**.
- Use **IFERROR()** for user-friendly output.
- Keep lookup tables clean and sorted when using approximate matches.

---

# Key Takeaways

- VLOOKUP is the traditional lookup function.
- HLOOKUP is used for horizontal tables.
- XLOOKUP is Microsoft's modern lookup function.
- INDEX returns values based on position.
- MATCH returns positions.
- INDEX + MATCH is the preferred solution for advanced lookups.
- CHOOSE returns values from a fixed list.
- OFFSET creates dynamic references.

---
