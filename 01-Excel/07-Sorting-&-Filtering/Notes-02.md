# Part 3 – Filtering

## What is Filtering?

Filtering is an Excel feature that displays only the records that meet specific conditions while temporarily hiding the remaining data.

Unlike sorting, filtering **does not change the order of data**. It simply hides rows that do not match the selected criteria.

Filtering is one of the most frequently used features in Excel for analyzing large datasets.

---

# Why Use Filtering?

When working with thousands of records, manually searching for specific information is inefficient.

Filtering helps you:

- Display only relevant records.
- Analyze specific categories.
- Compare selected data.
- Find information quickly.
- Generate reports efficiently.

---

# Where to Find Filter

```
Data
   ↓
Filter
```

or

```
Home
   ↓
Sort & Filter
   ↓
Filter
```

Shortcut:

```
Ctrl + Shift + L
```

This shortcut enables or disables filters on the selected dataset.

---

# Types of Filtering

Excel supports several filtering methods:

- Auto Filter
- Text Filter
- Number Filter
- Date Filter
- Filter by Color
- Advanced Filter

---

# 1. Auto Filter

## What is Auto Filter?

Auto Filter is the default filtering feature in Excel.

When enabled, a drop-down arrow appears beside every column header.

Users can filter records using these drop-down menus.

---

## Steps

1. Select the dataset.
2. Go to **Data** tab.
3. Click **Filter**.
4. Drop-down arrows appear in each header.

---

## Business Use Cases

- Display one department.
- Show one city.
- View completed projects.
- Filter sales by region.

---

## Advantages

- Quick filtering.
- Easy to use.
- No formulas required.
- Supports multiple columns.

---

# 2. Text Filters

## What are Text Filters?

Text Filters allow users to filter records containing specific text values.

Available options include:

- Equals
- Does Not Equal
- Begins With
- Ends With
- Contains
- Does Not Contain

---

### Equals

Displays records exactly matching the specified text.

Example:

```
Department = IT
```

---

### Does Not Equal

Displays records excluding the specified text.

Example:

```
Department ≠ HR
```

---

### Begins With

Displays records starting with specific text.

Example:

```
Employee Name begins with A
```

---

### Ends With

Displays records ending with specific text.

Example:

```
Email ends with .com
```

---

### Contains

Displays records containing specified text anywhere.

Example:

```
Name contains Rahul
```

---

### Does Not Contain

Displays records that do not contain specified text.

Example:

```
Status does not contain Pending
```

---

## Business Use Cases

- Filter IT department.
- Display completed projects.
- Search customer names.
- Find products by category.

---

# 3. Number Filters

## What are Number Filters?

Number Filters allow filtering numeric values using mathematical conditions.

Available options include:

- Equals
- Does Not Equal
- Greater Than
- Greater Than or Equal To
- Less Than
- Less Than or Equal To
- Between
- Top 10
- Above Average
- Below Average

---

### Greater Than

Displays values greater than the specified number.

Example:

```
Salary > 70000
```

---

### Less Than

Displays values lower than the specified number.

Example:

```
Attendance < 90
```

---

### Between

Displays values between two numbers.

Example:

```
Salary between 50000 and 70000
```

---

### Top 10

Displays the top values in a dataset.

The number can be changed.

---

### Above Average

Displays values greater than the average.

---

### Below Average

Displays values below the average.

---

### Business Use Cases

- High salaries
- Low stock
- Top sales
- Above-average revenue

---

# 4. Date Filters

## What are Date Filters?

Date Filters allow records to be filtered based on dates.

Available options include:

- Today
- Yesterday
- Tomorrow
- This Week
- Last Week
- Next Week
- This Month
- Last Month
- Next Month
- This Year
- Last Year
- Between

---

## Business Use Cases

- Recent employees
- Current month sales
- Pending invoices
- Upcoming deliveries

---

## Advantages

- Easy timeline analysis.
- Monthly reporting.
- Financial reporting.
- HR reporting.

---

# 5. Filter by Color

## What is Filter by Color?

Excel allows users to filter records based on:

- Cell Color
- Font Color
- Cell Icon

This feature is especially useful when Conditional Formatting has been applied.

---

## Business Use Cases

- Show high-priority tasks.
- Display overdue invoices.
- Show high-performing employees.
- Filter warning records.

---

# 6. Advanced Filter

## What is Advanced Filter?

Advanced Filter provides more powerful filtering than Auto Filter.

It allows users to:

- Filter using multiple criteria.
- Copy filtered records to another location.
- Extract unique records.

---

## Features

- Criteria Range
- Copy to Another Location
- Unique Records Only

---

## Criteria Range

A Criteria Range contains the conditions used for filtering.

Excel uses this range to determine which records to display.

---

## Copy to Another Location

Instead of hiding records, Advanced Filter can copy matching records to a new location.

---

## Unique Records Only

This option removes duplicate values and displays only unique records.

---

# Comparison: Sort vs Filter

| Sort | Filter |
|------|--------|
| Rearranges data | Hides unwanted rows |
| Changes record order | Preserves record order |
| Used for organization | Used for analysis |
| Displays all records | Displays matching records only |

---

# Best Practices

- Keep one header row.
- Avoid blank rows and blank columns.
- Ensure data types are consistent.
- Apply filters only to complete datasets.
- Clear filters after analysis.
- Convert datasets into Excel Tables for easier filtering.

---

# Common Mistakes

- Filtering only one column without considering related data.
- Leaving blank rows inside the dataset.
- Forgetting that filters hide rows rather than deleting them.
- Applying filters to incomplete ranges.
- Forgetting to clear old filters before applying new ones.

---

# Performance Tips

For large datasets:

- Use Excel Tables.
- Keep column headers unique.
- Avoid unnecessary blank rows.
- Use Advanced Filter for complex criteria.
- Remove filters when exporting or printing reports.

---

# 📌 Key Takeaways

- Filtering displays only records that meet specific conditions.
- Auto Filter is the most commonly used filtering method.
- Text, Number, and Date Filters help analyze specific data quickly.
- Filter by Color works well with Conditional Formatting.
- Advanced Filter supports complex criteria, unique records, and copying filtered results.
- Filtering is an essential skill for Data Analysts, Business Analysts, and MIS Executives.

---
