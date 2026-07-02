# 📘 Formatting Data for Analysis

## 🎯 Objective

Learn how to format data in Microsoft Excel to improve readability, consistency, and accuracy before performing data analysis.

---

# What is Data Formatting?

Data formatting is the process of changing the appearance of data without altering its actual value.

Proper formatting makes datasets:

- Easier to read
- More professional
- Consistent
- Ready for analysis

---

# Why is Formatting Important?

Well-formatted data helps you:

- Improve readability
- Identify important information quickly
- Reduce errors
- Maintain consistency
- Create professional reports and dashboards

---

# Common Formatting Options

## 1. Font Formatting

Used to customize the appearance of text.

### Options

- Font Style
- Font Size
- Bold
- Italic
- Underline
- Font Color

Example:

| Before | After |
|---------|--------|
| Sales Report | **Sales Report** |

---

## 2. Cell Fill Color

Changes the background color of cells.

Common Uses:

- Highlight important values
- Separate headers from data
- Improve readability

Example:

| Name | Salary |
|------|---------|
| Header | Blue Background |

---

## 3. Borders

Borders separate data visually.

Types:

- All Borders
- Outside Borders
- Thick Borders
- Bottom Border

Example:

```
-------------------------
| Name | Salary | City |
-------------------------
```

---

## 4. Text Alignment

Controls the position of text inside a cell.

### Horizontal Alignment

- Left
- Center
- Right

### Vertical Alignment

- Top
- Middle
- Bottom

---

## 5. Wrap Text

Wrap Text displays long text on multiple lines within the same cell.

### Without Wrap Text

```
This is a very long sentence...
```

### With Wrap Text

```
This is a very
long sentence...
```

---

## 6. Merge & Center

Combines multiple cells into one.

Example:

```
A1:D1

Monthly Sales Report
```

⚠️ **Best Practice:** Avoid merging cells in datasets used for analysis, sorting, filtering, or PivotTables. Use **Center Across Selection** if only visual alignment is needed.

---

## 7. Number Formatting

Excel supports different number formats.

### Common Formats

| Format | Example |
|----------|----------|
| General | 1200 |
| Number | 1,200.00 |
| Currency | ₹1,200.00 |
| Accounting | ₹ 1,200.00 |
| Percentage | 25% |
| Date | 01-Jan-2026 |
| Time | 10:30 AM |

---

## 8. Decimal Places

Increase or decrease decimal values.

Example

```
25.6789

↓

25.68
```

---

## 9. Cell Styles

Predefined formatting combinations.

Examples:

- Title
- Heading
- Total
- Good
- Bad
- Neutral

---

## 10. Format Painter

Copies formatting from one cell to another.

### Steps

1. Select the formatted cell.
2. Click **Format Painter**.
3. Click the destination cell.

Only formatting is copied—not the data.

---

## AutoFit Rows and Columns

Automatically adjusts row height and column width based on content.

### AutoFit Column Width

- Double-click the right edge of the column header.

### AutoFit Row Height

- Double-click the bottom edge of the row number.

---

# Best Practices for Formatting

- Use a single font throughout the worksheet.
- Keep font sizes consistent.
- Highlight headers with bold text and a fill color.
- Use borders sparingly.
- Avoid excessive colors.
- Use appropriate number formats.
- Ensure dates are stored as dates, not text.
- Do not merge cells within data tables.

---

# Common Formatting Mistakes

| Mistake | Solution |
|----------|----------|
| Different fonts | Use one consistent font |
| Random colors | Use a simple color scheme |
| Numbers stored as text | Convert to Number format |
| Merged cells in datasets | Avoid merging data tables |
| Uneven column widths | Use AutoFit |

---

# Real-World Example

A sales dataset contains:

- Different font sizes
- Mixed date formats
- Currency values without formatting
- Misaligned text

Before analysis, a Data Analyst:

- Formats headers
- Applies Currency format
- Standardizes dates
- Adjusts column widths
- Uses Wrap Text
- Aligns data consistently

This makes the dataset easier to analyze and present.

---

# Practice Exercise

Create the following table:

| Employee ID | Name | Department | Salary | Joining Date |
|--------------|------|------------|---------|--------------|
| E101 | Rahul | HR | 35000 | 12-Jan-2024 |
| E102 | Kiran | IT | 50000 | 20-Feb-2024 |
| E103 | Sneha | Finance | 42000 | 18-Mar-2024 |

Apply the following formatting:

- Bold the header row.
- Apply a background color to the headers.
- Center-align the headers.
- Format the **Salary** column as Currency.
- Format the **Joining Date** column as Date.
- Add borders to the table.
- Use AutoFit for all columns.
- Apply Wrap Text where necessary.

---

# Key Takeaways

- Formatting improves the appearance and usability of data.
- Use consistent fonts, colors, and alignment.
- Apply the correct number format for different data types.
- Use Wrap Text for long content.
- Use Format Painter to copy formatting efficiently.
- Avoid merged cells in analytical datasets.
- AutoFit improves readability by adjusting row and column sizes automatically.

---

Good formatting improves readability, consistency, and presentation, but the raw data should remain clean and structured. Avoid excessive formatting or merged cells in datasets because they can break sorting, filtering, formulas, and PivotTables.