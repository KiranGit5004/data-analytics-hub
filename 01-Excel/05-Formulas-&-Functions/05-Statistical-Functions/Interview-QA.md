# 📘 Interview Questions & Answers – Statistical Functions in Microsoft Excel

## 🎯 Objective

This document contains important **theory-based interview questions** on Statistical Functions in Microsoft Excel. These questions are commonly asked in **Data Analyst, Business Analyst, MIS Executive, Reporting Analyst, and Excel** interviews.

---

# 1. What are Statistical Functions in Excel?

### Answer

Statistical Functions are used to analyze, summarize, and interpret numerical data. They help measure central tendency, identify trends, rank values, calculate averages, and understand the distribution of data.

---

# 2. What is the purpose of Statistical Functions?

### Answer

Statistical Functions are used to:

- Analyze numerical datasets
- Summarize business data
- Compare performance
- Measure variation
- Rank values
- Generate reports
- Support business decision-making

---

# 3. What is the difference between AVERAGE and MEDIAN?

### Answer

| AVERAGE | MEDIAN |
|---------|---------|
| Returns the arithmetic mean | Returns the middle value |
| Affected by outliers | Less affected by outliers |
| Best for evenly distributed data | Best for skewed data |

---

# 4. What is MODE.SNGL used for?

### Answer

MODE.SNGL returns the value that appears most frequently in a dataset. It is useful for identifying the most common value in numerical data.

---

# 5. What is the difference between MEDIAN and MODE.SNGL?

### Answer

| MEDIAN | MODE.SNGL |
|---------|-----------|
| Returns the middle value | Returns the most frequent value |
| Based on sorted position | Based on frequency |
| Works even if all values are unique | Returns an error if no value repeats |

---

# 6. What is the LARGE function?

### Answer

The LARGE function returns the **nth largest value** from a dataset. It is commonly used to identify top-performing employees, highest sales, or largest profits.

---

# 7. What is the SMALL function?

### Answer

The SMALL function returns the **nth smallest value** from a dataset. It is useful for finding minimum values, lowest sales, or bottom-performing records.

---

# 8. What is the difference between MAX and LARGE?

### Answer

| MAX | LARGE |
|-----|--------|
| Returns only the largest value | Returns the nth largest value |
| No ranking option | Allows ranking using the k argument |

---

# 9. What is the difference between MIN and SMALL?

### Answer

| MIN | SMALL |
|-----|--------|
| Returns the smallest value | Returns the nth smallest value |
| Returns only one minimum value | Can return 1st, 2nd, 3rd smallest, etc. |

---

# 10. What is the RANK.EQ function?

### Answer

RANK.EQ returns the rank or position of a value within a list of numbers. It can rank values in ascending or descending order.

---

# 11. What happens if two values have the same rank in RANK.EQ?

### Answer

If duplicate values exist, Excel assigns the same rank to both values and skips the next rank.

Example:

```
Rank 1
Rank 2
Rank 2
Rank 4
```

---

# 12. What is PERCENTILE.INC?

### Answer

PERCENTILE.INC returns the value below which a specified percentage of observations fall. It is used to analyze the distribution of data and evaluate performance levels.

---

# 13. What is QUARTILE.INC?

### Answer

QUARTILE.INC divides a dataset into four equal parts and returns the specified quartile value.

It is commonly used for analyzing salary distributions, customer segmentation, and performance reporting.

---

# 14. What is STDEV.S?

### Answer

STDEV.S calculates the **sample standard deviation**, which measures how much the values in a sample vary from the sample mean.

A higher standard deviation indicates greater variation, while a lower value indicates that data points are closer to the average.

---

# 15. What is the difference between STDEV.S and STDEV.P?

### Answer

| STDEV.S | STDEV.P |
|----------|----------|
| Used for sample data | Used for the entire population |
| Divides by (n − 1) | Divides by n |
| Most common in business analysis | Used when complete population data is available |

---

# 16. What is the difference between PERCENTILE.INC and QUARTILE.INC?

### Answer

| PERCENTILE.INC | QUARTILE.INC |
|----------------|--------------|
| Returns any percentile value | Returns only quartile values |
| Supports values from 0 to 1 | Supports quartiles 0 to 4 |
| More flexible | Simpler for quartile analysis |

---

# 17. Which Statistical Functions are most commonly used by Data Analysts?

### Answer

The most frequently used Statistical Functions include:

- AVERAGE
- AVERAGEIF
- AVERAGEIFS
- MEDIAN
- MODE.SNGL
- LARGE
- SMALL
- RANK.EQ
- PERCENTILE.INC
- QUARTILE.INC
- STDEV.S

---

# 18. In which business scenarios are Statistical Functions commonly used?

### Answer

Statistical Functions are widely used in:

- HR Analytics
- Sales Analysis
- Financial Reporting
- Inventory Management
- Customer Analytics
- Business Intelligence
- Dashboard Development
- Performance Analysis

---

# 19. What are the best practices when using Statistical Functions?

### Answer

- Use AVERAGE for general analysis.
- Use MEDIAN when data contains outliers.
- Use MODE.SNGL to identify the most common value.
- Use LARGE and SMALL for Top-N and Bottom-N analysis.
- Use RANK.EQ for performance ranking.
- Use PERCENTILE.INC and QUARTILE.INC to understand data distribution.
- Use STDEV.S to measure variation in sample data.

---

# 20. Which Statistical Functions are most frequently asked in Excel interviews?

### Answer

The most commonly asked functions are:

- AVERAGE
- AVERAGEIF
- AVERAGEIFS
- MEDIAN
- MODE.SNGL
- LARGE
- SMALL
- RANK.EQ
- PERCENTILE.INC
- QUARTILE.INC
- STDEV.S

Candidates are often expected to explain:

- The purpose of each function.
- The differences between similar functions.
- When each function should be used in real-world business scenarios.

---

# 📌 Quick Revision

| Function | Purpose |
|----------|---------|
| AVERAGE | Calculates the arithmetic mean |
| AVERAGEIF | Average based on one condition |
| AVERAGEIFS | Average based on multiple conditions |
| MEDIAN | Returns the middle value |
| MODE.SNGL | Returns the most frequent value |
| LARGE | Returns the nth largest value |
| SMALL | Returns the nth smallest value |
| RANK.EQ | Returns the rank of a value |
| PERCENTILE.INC | Returns a specified percentile |
| QUARTILE.INC | Returns quartile values |
| STDEV.S | Calculates sample standard deviation |

---

# 🎯 Interview Tips

- Understand the purpose of every statistical function.
- Learn the differences between similar functions such as **AVERAGE vs MEDIAN**, **MAX vs LARGE**, and **MIN vs SMALL**.
- Know when to use **STDEV.S** instead of **STDEV.P**.
- Be prepared to explain real-world business applications of each function.
- Focus on concepts and use cases rather than memorizing formulas alone.