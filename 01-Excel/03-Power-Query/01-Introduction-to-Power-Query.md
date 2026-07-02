# 📘 Introduction to Power Query

## 🎯 Objective

Learn the fundamentals of Power Query in Microsoft Excel, including its purpose, architecture, interface, features, and why it is one of the most powerful tools for Data Analysts.

---

# What is Power Query?

Power Query is an **Extract, Transform, and Load (ETL)** tool built into Microsoft Excel and Microsoft Power BI.

It allows users to:

- Import data from multiple sources
- Clean messy datasets
- Transform data without writing complex formulas
- Combine multiple datasets
- Automate repetitive data preparation tasks

Power Query records every transformation step, allowing data to be refreshed automatically whenever the source data changes.

---

# What is ETL?

ETL stands for:

| Step | Description |
|-------|-------------|
| **Extract** | Import data from one or more sources |
| **Transform** | Clean, modify, and prepare the data |
| **Load** | Load the transformed data into Excel or the Data Model |

Example:

```
CSV File
     │
     ▼
Power Query
     │
Clean + Transform
     │
     ▼
Excel Table / Pivot Table / Dashboard
```

---

# Why Use Power Query?

Before Power Query, analysts often:

- Copied and pasted data manually
- Used multiple Excel formulas
- Repeated the same cleaning steps every day
- Spent hours preparing reports

Power Query automates these repetitive tasks.

Instead of repeating the work, you simply click **Refresh**, and all transformation steps are applied automatically.

---

# Features of Power Query

- Import data from multiple sources
- Remove duplicates
- Replace values
- Filter rows
- Sort data
- Split columns
- Merge columns
- Change data types
- Combine multiple files
- Merge queries
- Append queries
- Create calculated columns
- Refresh data automatically

---

# Data Sources Supported

Power Query can import data from:

- Excel Workbook
- CSV Files
- Text Files
- XML
- JSON
- PDF
- SQL Server
- MySQL
- PostgreSQL
- Oracle Database
- SharePoint
- Microsoft Access
- Folder
- Web
- Power Platform

---

# Power Query Workflow

```
Import Data
      │
      ▼
Power Query Editor
      │
      ▼
Clean Data
      │
      ▼
Transform Data
      │
      ▼
Load Data
      │
      ▼
Analysis & Dashboard
```

---

# Opening Power Query

In Excel:

```
Data
   ↓
Get Data
```

or

```
Data
   ↓
From Text/CSV
```

or

```
Data
   ↓
From Workbook
```

---

# Common Power Query Transformations

- Remove Duplicates
- Remove Blank Rows
- Replace Values
- Split Columns
- Merge Columns
- Pivot Columns
- Unpivot Columns
- Change Data Types
- Fill Down
- Fill Up
- Sort
- Filter
- Group By

---

# Refreshing Data

One of Power Query's biggest advantages is automatic refresh.

Example:

1. Import Sales.csv
2. Clean the data
3. Load to Excel
4. New sales are added to Sales.csv
5. Click **Refresh**

Excel automatically performs every cleaning step again.

No manual work is required.

---

# Difference Between Excel Formulas and Power Query

| Excel Formulas | Power Query |
|----------------|-------------|
| Cell-based | Table-based |
| Manual updates | Refresh updates everything |
| Best for calculations | Best for data cleaning and transformation |
| Slower on large datasets | Optimized for large datasets |
| Changes individual cells | Transforms entire datasets |

---

# Real-World Example

A company receives a daily sales report in CSV format.

Without Power Query:

- Open CSV
- Remove duplicates
- Remove blanks
- Change date format
- Convert text to numbers
- Create reports

Time: **30–45 minutes every day**

With Power Query:

- Create the transformation once.
- Save the query.
- Next day, replace the CSV file.
- Click **Refresh**.

Time: **Less than one minute**

---

# Best Practices

- Keep the original data unchanged.
- Perform all cleaning inside Power Query.
- Name queries clearly.
- Check data types after importing.
- Remove unnecessary columns early.
- Use descriptive step names.
- Refresh instead of repeating manual work.
- Test the query with updated data.

---

# Key Takeaways

- Power Query is Excel's built-in ETL tool.
- It automates data cleaning and transformation.
- Every transformation is recorded as an Applied Step.
- Data can be refreshed with a single click.
- It supports a wide range of file types and databases.
- Power Query is one of the most important skills for Data Analysts.

---
