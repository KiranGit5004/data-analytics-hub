# 📘 Statistical Functions in Microsoft Excel

## 🎯 Objective

Statistical Functions in Microsoft Excel are used to analyze, summarize, and interpret numerical data. These functions help identify trends, measure central tendency, rank values, and analyze data distribution.

This module focuses on the most commonly used Statistical Functions required for Data Analysts and Excel interviews.

---

# Why Learn Statistical Functions?

Statistical Functions help you to:

- Analyze large datasets
- Find the middle value of data
- Identify the most common value
- Find top and bottom performers
- Rank employees or products
- Analyze salary distribution
- Measure variation in data
- Generate business reports

---

# Understanding Statistical Functions

Suppose a company has employee salaries.

| Employee | Salary |
|-----------|---------|
| Rahul | 35000 |
| Sneha | 42000 |
| Amit | 39000 |
| Neha | 60000 |
| Priya | 42000 |

Using Statistical Functions, Excel can answer questions like:

- What is the middle salary?
- Which salary appears most often?
- Who has the highest salary?
- What is the third highest salary?
- Which employee ranks first?
- How much variation exists in salaries?

These functions make business analysis faster and more accurate.

---

# 1. MEDIAN Function

## What is MEDIAN?

The **MEDIAN** function returns the middle value of a dataset after sorting the numbers in ascending order.

Unlike the average (mean), the median is **not heavily affected by extremely high or low values (outliers)**.

---

## Syntax

```excel
=MEDIAN(number1,[number2],...)
```

or

```excel
=MEDIAN(A2:A20)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| number1 | First number or range |
| number2 | Optional additional numbers or ranges |

---

## Example 1

Dataset

| Salary |
|---------|
| 25000 |
| 30000 |
| 35000 |
| 40000 |
| 80000 |

Formula

```excel
=MEDIAN(A2:A6)
```

Result

```
35000
```

---

## Real-World Example

An HR department wants to know the **typical salary** of employees.

Instead of using AVERAGE(), which may be affected by very high executive salaries, they use MEDIAN() to find the middle salary.

---

## Best Practices

- Use MEDIAN when data contains extreme values.
- Compare MEDIAN with AVERAGE for better insights.
- Ensure blank cells do not represent missing data incorrectly.

---

# 2. MODE.SNGL Function

## What is MODE.SNGL?

The **MODE.SNGL** function returns the value that appears most frequently in a dataset.

If multiple values have the same highest frequency, MODE.SNGL returns only the first one.

---

## Purpose

Use MODE.SNGL to:

- Find the most common salary
- Identify the most purchased product
- Analyze customer preferences
- Find frequently occurring values

---

## Syntax

```excel
=MODE.SNGL(number1,[number2],...)
```

or

```excel
=MODE.SNGL(A2:A20)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| number1 | First value or range |
| number2 | Optional values or ranges |

---

## Example

Dataset

```
10
20
20
30
40
40
40
50
```

Formula

```excel
=MODE.SNGL(A2:A9)
```

Result

```
40
```

---

## Real-World Example

A retail company wants to know which product price occurs most often.

MODE.SNGL quickly identifies the most frequent selling price.

---

## Best Practices

- Use MODE.SNGL for datasets with repeated values.
- Verify data quality before calculating the mode.

---

# Difference Between AVERAGE and MEDIAN and MODE

| Function | Returns |
|----------|----------|
| AVERAGE | Arithmetic Mean |
| MEDIAN | Middle Value |
| MODE.SNGL | Most Frequent Value |

---

# 3. LARGE Function

## What is LARGE?

The **LARGE** function returns the **nth largest value** from a dataset.

It is useful when finding top-performing employees, highest sales, or largest profits.

---

## Purpose

Use LARGE to:

- Find the highest salary
- Identify top sales
- Retrieve top profits
- Rank business performance

---

## Syntax

```excel
=LARGE(array,k)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| array | Data range |
| k | Position of largest value |

---

## Example

Dataset

```
12
25
30
50
70
90
```

Formula

```excel
=LARGE(A2:A7,1)
```

Result

```
90
```

---

Second Highest

```excel
=LARGE(A2:A7,2)
```

Result

```
70
```

---

Third Highest

```excel
=LARGE(A2:A7,3)
```

Result

```
50
```

---

## Real-World Example

A sales manager wants to identify the **Top 5 Sales Performers** without sorting the data.

LARGE() returns the required values instantly.

---

## Best Practices

- Combine LARGE with INDEX and MATCH to identify corresponding records.
- Validate that **k** is within the dataset size.

---

# 4. SMALL Function

## What is SMALL?

The **SMALL** function returns the **nth smallest value** from a dataset.

It is commonly used to identify minimum values, lowest sales, or bottom performers.

---

## Purpose

Use SMALL to:

- Find lowest salary
- Find cheapest product
- Identify minimum sales
- Analyze bottom-performing employees

---

## Syntax

```excel
=SMALL(array,k)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| array | Data range |
| k | Position of smallest value |

---

## Example

Dataset

```
12
25
30
50
70
90
```

Formula

```excel
=SMALL(A2:A7,1)
```

Result

```
12
```

---

Second Smallest

```excel
=SMALL(A2:A7,2)
```

Result

```
25
```

---

Third Smallest

```excel
=SMALL(A2:A7,3)
```

Result

```
30
```

---

## Real-World Example

An inventory manager wants to identify the **five products with the lowest stock levels**.

Instead of sorting the data manually, SMALL() returns the required values directly.

---

## Best Practices

- Combine SMALL with INDEX + MATCH or XLOOKUP for complete reports.
- Ensure the value of **k** does not exceed the number of records.

---

# 📌 Key Takeaways

- **MEDIAN()** returns the middle value in a dataset.
- **MODE.SNGL()** returns the most frequently occurring value.
- **LARGE()** returns the nth largest value.
- **SMALL()** returns the nth smallest value.
- These functions are widely used in Data Analysis, HR Analytics, Sales Reporting, Financial Analysis, and Business Intelligence.

---

# 5. RANK.EQ Function

## What is RANK.EQ?

The **RANK.EQ** function returns the **rank (position)** of a number within a list of numbers.

It is commonly used to rank:

- Employees
- Students
- Sales Representatives
- Products
- Branch Performance

If two or more values are the same, Excel assigns them the **same rank**.

---

## Purpose

Use RANK.EQ to:

- Rank employee salaries
- Rank student marks
- Find top salespersons
- Rank branch performance
- Identify best-performing products

---

## Syntax

```excel
=RANK.EQ(number,ref,[order])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| number | Number to rank |
| ref | Range containing all numbers |
| order | Optional (0 = Descending, 1 = Ascending) |

---

## Descending Order (Default)

Largest value receives Rank 1.

```excel
=RANK.EQ(B2,$B$2:$B$10,0)
```

---

## Ascending Order

Smallest value receives Rank 1.

```excel
=RANK.EQ(B2,$B$2:$B$10,1)
```

---

## Example

| Employee | Salary |
|-----------|---------|
| Rahul | 60000 |
| Sneha | 45000 |
| Amit | 70000 |
| Neha | 55000 |

Formula

```excel
=RANK.EQ(B2,$B$2:$B$5,0)
```

Result

| Salary | Rank |
|---------|------|
|70000|1|
|60000|2|
|55000|3|
|45000|4|

---

## Example with Duplicate Values

| Salary |
|---------|
|60000|
|70000|
|60000|
|45000|

Ranks

```
70000 → 1
60000 → 2
60000 → 2
45000 → 4
```

Notice Rank **3** is skipped.

---

## Real-World Example

A company wants to reward the **Top 10 Sales Employees**.

Instead of sorting the data manually, RANK.EQ instantly assigns ranks.

---

## Advantages

- Easy to rank data
- Supports ascending and descending order
- Uidely used in business reporting
seful in dashboards
- W
---

## Limitations

- Duplicate values receive the same rank.
- Next rank is skipped.

---

## Best Practices

- Use descending order for marks, salaries, and sales.
- Use ascending order for expenses or delivery time.
- Lock the reference range using absolute references.

---

# 6. PERCENTILE.INC Function

## What is PERCENTILE.INC?

The **PERCENTILE.INC** function returns the value below which a specified percentage of observations fall.

It helps divide data into percentages.

---

## Purpose

Use PERCENTILE.INC to:

- Analyze salaries
- Evaluate exam scores
- Study customer spending
- Measure business performance
- Financial analysis

---

## Syntax

```excel
=PERCENTILE.INC(array,k)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| array | Data range |
| k | Percentile between 0 and 1 |

---

## Common Percentiles

| Percentile | k Value |
|------------|---------|
|25th|0.25|
|50th|0.50|
|75th|0.75|
|90th|0.90|
|95th|0.95|

---

## Example

Dataset

```
20
25
30
35
40
45
50
55
60
```

Formula

```excel
=PERCENTILE.INC(A2:A10,0.75)
```

Result

```
50
```

---

## Real-World Example

An HR department wants to know the salary below which **75% of employees** fall.

Using PERCENTILE.INC provides the answer instantly.

---

## Best Practices

- Use values between **0** and **1**.
- Compare percentiles with quartiles for better insights.

---

## Difference Between Percentage and Percentile

| Percentage | Percentile |
|------------|------------|
|Part of 100|Position within a dataset|
|Example: 75% Marks|75th Percentile|

---

# 7. QUARTILE.INC Function

## What is QUARTILE.INC?

The **QUARTILE.INC** function divides a dataset into **four equal parts**.

Quartiles are commonly used in statistics, finance, and business reporting.

---

## Purpose

Use QUARTILE.INC to:

- Analyze salary distribution
- Study sales performance
- Detect outliers
- Compare employee performance
- Financial reporting

---

## Syntax

```excel
=QUARTILE.INC(array,quart)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| array | Data range |
| quart | Quartile number |

---

## Quartile Numbers

| Quart | Meaning |
|--------|----------|
|0|Minimum|
|1|First Quartile (Q1)|
|2|Median (Q2)|
|3|Third Quartile (Q3)|
|4|Maximum|

---

## Example

Dataset

```
10
20
30
40
50
60
70
80
90
```

Formula

First Quartile

```excel
=QUARTILE.INC(A2:A10,1)
```

Second Quartile

```excel
=QUARTILE.INC(A2:A10,2)
```

Third Quartile

```excel
=QUARTILE.INC(A2:A10,3)
```

---

## Real-World Example

A business analyst wants to divide customers into four spending groups:

- Low Spenders
- Medium Spenders
- High Spenders
- Premium Customers

Quartiles make this segmentation easy.

---

## Advantages

- Divides data into four equal parts
- Useful for detecting outliers
- Helps understand data distribution
- Common in HR and Finance

---

## Limitations

- Requires sorted numerical data internally.
- Less meaningful for very small datasets.

---

## Best Practices

- Compare quartiles with median.
- Use quartiles to identify unusual values.
- Combine with box plots for data visualization.

---

# Difference Between MEDIAN, PERCENTILE, and QUARTILE

| Function | Returns |
|----------|----------|
|MEDIAN|Middle Value|
|PERCENTILE.INC|Specified Percentile|
|QUARTILE.INC|Specified Quartile|

---

# 📌 Key Takeaways

- **RANK.EQ()** assigns a rank to a value.
- **PERCENTILE.INC()** finds the value at a specified percentile.
- **QUARTILE.INC()** divides data into four equal parts.
- These functions are widely used in HR Analytics, Financial Reporting, Sales Analysis, Business Intelligence, and Data Analytics.

---

# What is an Average?

The **Average (Arithmetic Mean)** is the sum of all values divided by the number of values.

Example

| Numbers |
|---------|
|10|
|20|
|30|
|40|
|50|

Formula

```excel
=AVERAGE(A2:A6)
```

Result

```
30
```

Because

```
(10+20+30+40+50)/5 = 30
```

---

# 1. AVERAGE Function

## What is AVERAGE?

The **AVERAGE** function calculates the arithmetic mean of a group of numbers.

It ignores blank cells but includes cells containing zero.

---

## Purpose

Use AVERAGE to:

- Calculate average salary
- Average sales
- Average marks
- Average monthly revenue
- Average customer spending

---

## Syntax

```excel
=AVERAGE(number1,[number2],...)
```

or

```excel
=AVERAGE(A2:A20)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| number1 | First number or range |
| number2 | Optional additional numbers or ranges |

---

## Example 1

| Marks |
|--------|
|80|
|75|
|90|
|85|
|70|

Formula

```excel
=AVERAGE(A2:A6)
```

Result

```
80
```

---

## Real-World Example

A company wants to know the **average salary** of all employees.

Instead of manually calculating the mean, Excel provides the result instantly using AVERAGE().

---

## Best Practices

- Use MEDIAN() if your dataset contains significant outliers.
- Ensure all cells contain numeric values.
- Remove unnecessary zeros if they should not be included.

---

# 2. AVERAGEIF Function

## What is AVERAGEIF?

The **AVERAGEIF** function calculates the average of cells that meet **one specific condition**.

---

## Purpose

Use AVERAGEIF to:

- Calculate average salary of one department.
- Average sales of one region.
- Average marks above a passing score.
- Average orders from one customer.

---

## Syntax

```excel
=AVERAGEIF(range,criteria,[average_range])
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| range | Range to evaluate |
| criteria | Condition to apply |
| average_range | Cells to average (optional) |

---

## Example 1

| Department | Salary |
|------------|--------|
|IT|50000|
|HR|40000|
|IT|60000|
|Sales|45000|
|IT|55000|

Formula

```excel
=AVERAGEIF(A2:A6,"IT",B2:B6)
```

Result

```
55000
```

---

## Example 2

Average Marks Greater Than 70

| Marks |
|--------|
|60|
|70|
|80|
|90|
|75|

Formula

```excel
=AVERAGEIF(A2:A6,">70")
```

Result

```
81.67
```

---

## Common Criteria Examples

| Criteria | Meaning |
|----------|---------|
| "IT" | Equal to IT |
| ">50000" | Greater than 50000 |
| "<100" | Less than 100 |
| "<>HR" | Not equal to HR |

---

## Real-World Example

Calculate the average salary of employees working in the **IT Department**.

---

## Best Practices

- Use cell references instead of typing criteria directly.

Example

```excel
=AVERAGEIF(A2:A20,E2,B2:B20)
```

Where **E2** contains the department name.

---

# 3. AVERAGEIFS Function

## What is AVERAGEIFS?

The **AVERAGEIFS** function calculates the average of cells that satisfy **multiple conditions**.

It is one of the most useful functions for business reporting and data analysis.

---

## Purpose

Use AVERAGEIFS to:

- Average salary by department and city.
- Average sales by region and month.
- Average marks by class and subject.
- Analyze business performance using multiple filters.

---

## Syntax

```excel
=AVERAGEIFS(average_range,criteria_range1,criteria1,[criteria_range2,criteria2]...)
```

---

# Arguments

| Argument | Description |
|----------|-------------|
| average_range | Cells to average |
| criteria_range1 | First criteria range |
| criteria1 | First condition |
| criteria_range2 | Second criteria range |
| criteria2 | Second condition |

---

## Example

| Department | City | Salary |
|------------|------|--------|
|IT|Mumbai|50000|
|IT|Pune|60000|
|HR|Mumbai|40000|
|IT|Mumbai|55000|
|Sales|Pune|45000|

Formula

```excel
=AVERAGEIFS(C2:C6,A2:A6,"IT",B2:B6,"Mumbai")
```

Result

```
52500
```

---

## Real-World Example

Find the average salary of employees who:

- Work in the **IT Department**
- Are located in **Mumbai**

This is a common HR reporting requirement.

---

## Best Practices

- Keep all criteria ranges equal in size.
- Use cell references for dynamic reports.

Example

```excel
=AVERAGEIFS(C2:C100,A2:A100,F2,B2:B100,G2)
```

---

## Comparison Table

| Function | Number of Conditions |
|----------|----------------------|
| AVERAGE | No conditions |
| AVERAGEIF | One condition |
| AVERAGEIFS | Multiple conditions |

---

## Common Errors

| Error | Reason |
|--------|--------|
| #DIV/0! | No cells match the criteria or no numeric values found |
| #VALUE! | Invalid argument or mismatched range sizes |
| #NAME? | Incorrect function name |

---

# 📌 Key Takeaways

- **AVERAGE()** calculates the arithmetic mean of a dataset.
- **AVERAGEIF()** calculates an average based on a single condition.
- **AVERAGEIFS()** calculates an average based on multiple conditions.
- Use absolute references (`$`) when copying formulas.
- These functions are widely used in dashboards, reports, HR analytics, finance, and business intelligence.

---

