# 📘 Conditional Formatting in Microsoft Excel

## 🎯 Objective

Conditional Formatting is one of Excel's most powerful features that automatically changes the appearance of cells based on specified conditions or rules.

Instead of manually highlighting important information, Conditional Formatting helps visualize data by applying colors, icons, and formatting whenever certain criteria are met.

---

# Why Learn Conditional Formatting?

In real-world business environments, datasets often contain thousands of records. Finding important values manually is time-consuming and prone to errors.

Conditional Formatting helps you:

- Identify high and low values instantly.
- Highlight duplicate records.
- Detect missing or unusual data.
- Compare performance.
- Improve report readability.
- Create interactive dashboards.
- Visualize trends without charts.

---

# What is Conditional Formatting?

Conditional Formatting is an Excel feature that automatically applies formatting to cells when specified conditions are met.

The formatting can include:

- Font Color
- Fill Color
- Borders
- Data Bars
- Color Scales
- Icon Sets

Unlike manual formatting, Conditional Formatting updates automatically whenever the underlying data changes.

---

# Advantages of Conditional Formatting

- Automatically updates when data changes.
- Improves data visualization.
- Saves time.
- Reduces manual work.
- Helps identify trends quickly.
- Makes reports easier to understand.
- Useful for dashboards and KPI reports.

---

# How Conditional Formatting Works

Conditional Formatting follows a simple process:

```
Data
   ↓
Condition
   ↓
Rule Evaluation
   ↓
Formatting Applied
```

Example:

```
Salary > 50000
```

If the condition is TRUE:

- Cell becomes Green

If the condition is FALSE:

- No formatting is applied.

---

# Where to Find Conditional Formatting

In Excel:

```
Home Tab
      ↓
Styles Group
      ↓
Conditional Formatting
```

You will see options such as:

- Highlight Cells Rules
- Top/Bottom Rules
- Data Bars
- Color Scales
- Icon Sets
- New Rule
- Clear Rules
- Manage Rules

---

# Types of Conditional Formatting

Excel provides several categories:

1. Highlight Cells Rules
2. Top/Bottom Rules
3. Data Bars
4. Color Scales
5. Icon Sets
6. Formula-Based Rules

This part focuses on **Highlight Cells Rules**.

---

# 1. Highlight Cells Rules

These rules highlight cells based on specific values or conditions.

Available rules include:

- Greater Than
- Less Than
- Between
- Equal To
- Text That Contains
- A Date Occurring
- Duplicate Values

---

## 1. Greater Than

## Purpose

Highlights cells whose values are greater than a specified number.

---

## Use Cases

- Employees earning more than ₹75,000
- Sales greater than target
- Marks above 90
- Profit above expected value

---

## Steps

1. Select the data range.
2. Go to **Home → Conditional Formatting**.
3. Choose **Highlight Cells Rules**.
4. Select **Greater Than**.
5. Enter the comparison value.
6. Choose a formatting style.
7. Click **OK**.

---

## Business Scenario

A company wants to identify employees earning more than ₹80,000.

Using the **Greater Than** rule, Excel automatically highlights qualifying employees.

---

## 2. Less Than

## Purpose

Highlights cells whose values are smaller than a specified number.

---

## Use Cases

- Attendance below 90%
- Sales below target
- Low stock quantity
- Marks below passing score

---

## Steps

1. Select the range.
2. Open **Conditional Formatting**.
3. Choose **Less Than**.
4. Enter the comparison value.
5. Select formatting.
6. Click **OK**.

---

## Business Scenario

Highlight all products with stock less than 20 units to identify items that need replenishment.

---

## 3. Between

## Purpose

Highlights values that fall within a specified range.

---

## Use Cases

- Salary between ₹40,000 and ₹60,000
- Marks between 70 and 90
- Sales within a target range
- Employee age between 25 and 35 years

---

## Steps

1. Select the cells.
2. Go to **Highlight Cells Rules**.
3. Select **Between**.
4. Enter the lower value.
5. Enter the upper value.
6. Choose formatting.
7. Click **OK**.

---

## Business Scenario

Highlight employees whose salaries fall within the company's standard pay range.

---

## 4. Equal To

## Purpose

Highlights cells that exactly match a specified value.

---

## Use Cases

- Department equals IT
- Rating equals 5
- Status equals Completed
- Gender equals Female

---

## Steps

1. Select the range.
2. Open **Conditional Formatting**.
3. Choose **Equal To**.
4. Enter the required value.
5. Select formatting.
6. Click **OK**.

---

## Business Scenario

Highlight all employees belonging to the IT department.

---

## 5. Text That Contains

## Purpose

Highlights cells containing specific text.

---

## Use Cases

- Customer names containing "Ltd"
- Product category containing "Laptop"
- Email addresses containing "@gmail.com"
- Status containing "Pending"

---

## Steps

1. Select the data.
2. Open **Conditional Formatting**.
3. Choose **Text That Contains**.
4. Enter the required text.
5. Choose formatting.
6. Click **OK**.

---

## Business Scenario

Highlight all products that contain the word "Laptop" in the product name.

---

## 6. A Date Occurring

## Purpose

Highlights cells containing dates based on predefined time periods.

Available options include:

- Yesterday
- Today
- Tomorrow
- Last 7 Days
- Last Week
- This Week
- Next Week
- Last Month
- This Month
- Next Month

---

## Use Cases

- Track upcoming deadlines.
- Monitor project timelines.
- Highlight today's tasks.
- Identify overdue invoices.

---

## Steps

1. Select the date range.
2. Choose **Conditional Formatting**.
3. Select **A Date Occurring**.
4. Choose the required date option.
5. Select formatting.
6. Click **OK**.

---

## Business Scenario

Highlight invoices due today so the finance team can process them immediately.

---

## 7. Duplicate Values

## Purpose

Highlights duplicate or unique values within a selected range.

---

## Use Cases

- Duplicate Employee IDs
- Duplicate Invoice Numbers
- Duplicate Customer Records
- Duplicate Product Codes
- Duplicate Email Addresses

---

## Steps

1. Select the dataset.
2. Open **Conditional Formatting**.
3. Choose **Duplicate Values**.
4. Select either:
   - Duplicate
   - Unique
5. Choose formatting.
6. Click **OK**.

---

## Business Scenario

An HR team wants to ensure every employee has a unique Employee ID. The Duplicate Values rule immediately highlights repeated IDs.

---

# 2. Top/Bottom Rules

Top/Bottom Rules automatically highlight the highest-performing or lowest-performing values in a dataset.

Unlike Highlight Cells Rules, these rules compare values with other values in the selected range instead of comparing them with a fixed value.

---

## Types of Top/Bottom Rules

Excel provides the following options:

- Top 10 Items
- Top 10%
- Bottom 10 Items
- Bottom 10%
- Above Average
- Below Average

---

## 1. Top 10 Items

## Purpose

Highlights the highest values in a dataset.

Although the default is **10**, Excel allows you to change this number.

---

## Use Cases

- Top 10 Sales Employees
- Top 5 Products
- Highest Revenue
- Best Performing Branches

---

## Steps

1. Select the dataset.
2. Home → Conditional Formatting.
3. Top/Bottom Rules.
4. Select **Top 10 Items**.
5. Enter the required number.
6. Choose a formatting style.
7. Click **OK**.

---

## Business Scenario

Highlight the Top 5 employees based on monthly sales.

---

## 2. Top 10%

## Purpose

Highlights the highest percentage of values in a dataset.

The default is **10%**, but this percentage can be modified.

---

## Use Cases

- Top 20% Employees
- Top 15% Sales
- Highest Performing Products
- Best Customer Ratings

---

## Steps

1. Select the range.
2. Conditional Formatting.
3. Top/Bottom Rules.
4. Top 10%.
5. Enter percentage.
6. Select formatting.
7. Click OK.

---

## Business Scenario

Highlight the Top 20% sales performers for bonus eligibility.

---

## 3. Bottom 10 Items

## Purpose

Highlights the lowest values in a dataset.

---

## Use Cases

- Lowest Sales
- Lowest Profit
- Lowest Attendance
- Lowest Product Stock

---

## Steps

1. Select data.
2. Conditional Formatting.
3. Top/Bottom Rules.
4. Bottom 10 Items.
5. Enter number.
6. Choose formatting.
7. Click OK.

---

## Business Scenario

Highlight the Bottom 5 performing products that require attention.

---

## 4. Bottom 10%

## Purpose

Highlights the lowest percentage of values.

---

## Use Cases

- Lowest Performing Employees
- Lowest Revenue Products
- Bottom Customer Ratings

---

## Steps

1. Select range.
2. Conditional Formatting.
3. Top/Bottom Rules.
4. Bottom 10%.
5. Enter percentage.
6. Choose formatting.
7. Click OK.

---

## Business Scenario

Highlight the Bottom 15% sales representatives for additional training.

---

## 5. Above Average

## Purpose

Highlights values greater than the average of the selected dataset.

---

## Use Cases

- Above Average Salary
- Above Average Sales
- Above Average Attendance
- Above Average Profit

---

## Steps

1. Select dataset.
2. Conditional Formatting.
3. Top/Bottom Rules.
4. Above Average.
5. Select formatting.
6. Click OK.

---

## Business Scenario

Highlight employees whose sales exceed the team's average sales.

---

## 6. Below Average

## Purpose

Highlights values lower than the average.

---

## Use Cases

- Below Average Sales
- Below Average Salary
- Below Average Marks
- Below Average Profit

---

## Steps

1. Select range.
2. Conditional Formatting.
3. Top/Bottom Rules.
4. Below Average.
5. Select formatting.
6. Click OK.

---

## Business Scenario

Highlight employees whose attendance is below the company average.

---

# 3. Data Bars

## What are Data Bars?

Data Bars display colored bars inside cells based on their values.

The longer the bar, the larger the value.

The shorter the bar, the smaller the value.

No chart is required.

---

## Purpose

Use Data Bars to compare values visually.

---

## Use Cases

- Monthly Sales
- Revenue
- Profit
- Attendance
- Budget Analysis

---

## Steps

1. Select data.
2. Home → Conditional Formatting.
3. Data Bars.
4. Choose Gradient Fill or Solid Fill.
5. Select the desired color.

---

## Business Scenario

Display monthly sales using Data Bars to quickly identify the highest-performing months.

---

## Advantages

- Easy comparison
- Improves visualization
- Requires no charts
- Updates automatically

---

# 4. Color Scales

## What are Color Scales?

Color Scales apply different colors based on the relative value of each cell.

Typically:

- Green = High
- Yellow = Medium
- Red = Low

Excel also supports two-color scales.

---

## Purpose

Visualize data distribution using colors.

---

## Use Cases

- Student Marks
- Sales Reports
- Financial Performance
- KPI Dashboards

---

## Steps

1. Select dataset.
2. Conditional Formatting.
3. Color Scales.
4. Choose a color scheme.

---

## Business Scenario

Highlight the highest sales values in green and the lowest values in red.

---

## Advantages

- Easy to identify trends.
- Excellent for dashboards.
- Improves report readability.

---

# 5. Icon Sets

## What are Icon Sets?

Icon Sets display icons based on value ranges.

Common icons include:

- Green Arrows
- Yellow Arrows
- Red Arrows
- Traffic Lights
- Flags
- Stars
- Ratings
- Shapes

---

## Purpose

Represent performance using symbols instead of numbers.

---

## Use Cases

- KPI Dashboards
- Employee Performance
- Sales Reports
- Budget Monitoring

---

## Steps

1. Select data.
2. Conditional Formatting.
3. Icon Sets.
4. Choose an icon style.

---

## Business Scenario

Display:

- 🟢 High Sales
- 🟡 Average Sales
- 🔴 Low Sales

without creating charts.

---

## Advantages

- Easy to understand.
- Professional appearance.
- Excellent for dashboards.
- Quick performance comparison.

---

# Comparison of Visualization Rules

| Feature | Best For |
|----------|----------|
| Top/Bottom Rules | Highest and Lowest Values |
| Data Bars | Compare Magnitude |
| Color Scales | Compare Distribution |
| Icon Sets | Performance Indicators |

---

