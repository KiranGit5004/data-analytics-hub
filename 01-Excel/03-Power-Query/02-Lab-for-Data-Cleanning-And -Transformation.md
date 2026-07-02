# Lab 01: Data Cleaning and Transformation using Power Query

## Objective

Import the **2020 Summer Olympics Medal Table** from a website into Excel using **Power Query**, perform data cleaning and transformation, and load the cleaned data back into Excel.

---

## Lab Details

**Tool:** Microsoft Excel - Power Query

**Data Source:**
https://en.wikipedia.org/wiki/2020_Summer_Olympics_medal_table

---

# Task

Import the medal table from the Wikipedia website and perform the following transformations before loading the data into Excel.

---

# Requirements

### Step 1: Import Data

- Open Microsoft Excel.
- Navigate to **Data → Get Data → From Other Sources → From Web**.
- Paste the following URL:

```
https://en.wikipedia.org/wiki/2020_Summer_Olympics_medal_table
```

- Select the **2020 Summer Olympics Medal Table**.
- Click **Transform Data**.

---

### Step 2: Fill Blank Values

Some rows have blank values in the **NOC** (Country) column.

Perform:

- Select the appropriate column.
- Go to

```
Transform → Fill → Up
```

---

### Step 3: Remove Extra Spaces

Clean unnecessary leading and trailing spaces from all text columns.

Perform:

```
Transform → Format → Trim
```

Apply this transformation to every text column.

---

### Step 4: Remove the Total Row

The last row contains overall totals.

Remove the last row by using:

```
Home → Remove Rows → Remove Bottom Rows
```

Number of rows to remove:

```
1
```

---

### Step 5: Create Gold Percentage Column

Create a new custom column named:

```
Gold Percentage
```

Formula:

```powerquery
=[Gold]/[Total]
```

Change the data type to:

```
Percentage
```

Format the values to display two decimal places.

---

### Step 6: Load Data

After completing all transformations,

Select:

```
Home → Close & Load
```

Load the cleaned table into a new worksheet.

---

# Expected Output

The final dataset should contain:

- Clean country names
- No unnecessary spaces
- No total row
- A new **Gold Percentage** column
- Data loaded into an Excel worksheet

---

