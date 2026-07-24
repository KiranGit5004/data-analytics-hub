# 📘 Solution – Conditional Formatting Lab

## Dataset Used

**Conditional_Formatting_Dataset.xlsx**

Worksheet Name:

```
Employee_Data
```

---

# Part A – Highlight Cells Rules

## Solution 1

**Task:** Highlight Salary greater than ₹80,000

**Rule**

```
Highlight Cells Rules → Greater Than
```

**Value**

```
80000
```

**Result**

Employees earning more than ₹80,000 are highlighted.

---

## Solution 2

**Task:** Highlight Salary less than ₹40,000

**Rule**

```
Highlight Cells Rules → Less Than
```

**Value**

```
40000
```

**Result**

Employees earning less than ₹40,000 are highlighted.

---

## Solution 3

**Task:** Highlight Salary between ₹50,000 and ₹70,000

**Rule**

```
Highlight Cells Rules → Between
```

**Values**

```
50000
70000
```

**Result**

Employees whose salary falls within the specified range are highlighted.

---

## Solution 4

**Task:** Highlight IT Department

**Rule**

```
Highlight Cells Rules → Equal To
```

**Value**

```
IT
```

**Result**

All IT department employees are highlighted.

---

## Solution 5

**Task:** Highlight Mumbai Employees

**Rule**

```
Highlight Cells Rules → Equal To
```

**Value**

```
Mumbai
```

**Result**

Employees working in Mumbai are highlighted.

---

## Solution 6

**Task:** Highlight Pending Status

**Rule**

```
Highlight Cells Rules → Text that Contains
```

**Value**

```
Pending
```

**Result**

Pending records are highlighted.

---

## Solution 7

**Task:** Highlight Employee Name containing Rahul

**Rule**

```
Highlight Cells Rules → Text that Contains
```

**Value**

```
Rahul
```

**Result**

Names containing Rahul are highlighted.

---

## Solution 8

**Task:** Highlight employees joined Today

**Rule**

```
Highlight Cells Rules → A Date Occurring
```

**Option**

```
Today
```

**Result**

Today's joining employees are highlighted.

---

## Solution 9

**Task:** Highlight employees joined in Last 7 Days

**Rule**

```
Highlight Cells Rules → A Date Occurring
```

**Option**

```
Last 7 Days
```

**Result**

Employees who joined during the last seven days are highlighted.

---

## Solution 10

**Task:** Highlight Duplicate Employee IDs

**Rule**

```
Highlight Cells Rules → Duplicate Values
```

**Result**

Duplicate Employee IDs are highlighted.

---

## Solution 11

**Task:** Highlight Duplicate Employee Names

**Rule**

```
Highlight Cells Rules → Duplicate Values
```

**Result**

Duplicate Employee Names are highlighted.

---

## Solution 12

**Task:** Highlight Blank Employee Names

**Formula**

```excel
=ISBLANK(B2)
```

**Result**

Blank Employee Name cells are highlighted.

---

# Part B – Top / Bottom Rules

## Solution 13

**Task:** Highlight Top 10 Salaries

**Rule**

```
Top/Bottom Rules → Top 10 Items
```

**Value**

```
10
```

**Result**

Top 10 salary values are highlighted.

---

## Solution 14

**Task:** Highlight Top 10% Sales

**Rule**

```
Top/Bottom Rules → Top 10%
```

**Result**

Highest 10% sales values are highlighted.

---

## Solution 15

**Task:** Highlight Bottom 5 Salaries

**Rule**

```
Top/Bottom Rules → Bottom Items
```

**Value**

```
5
```

**Result**

Lowest five salaries are highlighted.

---

## Solution 16

**Task:** Highlight Bottom 10% Sales

**Rule**

```
Top/Bottom Rules → Bottom 10%
```

**Result**

Lowest 10% sales values are highlighted.

---

## Solution 17

**Task:** Highlight Above Average Salary

**Rule**

```
Top/Bottom Rules → Above Average
```

**Result**

Employees earning above average salary are highlighted.

---

## Solution 18

**Task:** Highlight Below Average Sales

**Rule**

```
Top/Bottom Rules → Below Average
```

**Result**

Sales below average are highlighted.

---

# Part C – Data Bars

## Solution 19

**Task:** Apply Data Bars on Salary

**Rule**

```
Conditional Formatting → Data Bars
```

**Column**

```
Salary
```

**Result**

Salary values are displayed using data bars.

---

## Solution 20

**Task:** Apply Data Bars on Sales

**Rule**

```
Conditional Formatting → Data Bars
```

**Column**

```
Sales
```

**Result**

Sales values are displayed using data bars.

---

## Solution 21

**Task:** Apply Data Bars on Bonus

**Rule**

```
Conditional Formatting → Data Bars
```

**Column**

```
Bonus
```

**Result**

Bonus values are displayed using data bars.

---

# Part D – Color Scales

## Solution 22

**Task:** Apply 3-Color Scale on Salary

**Rule**

```
Conditional Formatting → Color Scales
```

**Result**

Salary values are displayed using a three-color gradient.

---

## Solution 23

**Task:** Apply 3-Color Scale on Sales

**Rule**

```
Conditional Formatting → Color Scales
```

**Result**

Sales values are displayed using a three-color gradient.

---

## Solution 24

**Task:** Apply 2-Color Scale on Attendance

**Rule**

```
Conditional Formatting → Color Scales
```

**Result**

Attendance values are displayed using a two-color gradient.

---

# Part E – Icon Sets

## Solution 25

**Task:** Apply Traffic Lights on Performance Rating

**Rule**

```
Conditional Formatting → Icon Sets
```

**Result**

Performance Ratings are displayed using Traffic Light icons.

---

## Solution 26

**Task:** Apply Arrow Icons on Sales

**Rule**

```
Conditional Formatting → Icon Sets
```

**Result**

Sales values display directional arrows.

---

## Solution 27

**Task:** Apply Rating Icons on Attendance

**Rule**

```
Conditional Formatting → Icon Sets
```

**Result**

Attendance percentages display rating icons.

---

# Part F – Formula-Based Conditional Formatting

## Solution 28

**Task:** Highlight Actual Sales greater than Target Sales

**Formula**

```excel
=N2>M2
```

**Result**

Employees exceeding sales targets are highlighted.

---

## Solution 29

**Task:** Highlight Actual Sales less than Target Sales

**Formula**

```excel
=N2<M2
```

**Result**

Employees below target sales are highlighted.

---

## Solution 30

**Task:** Highlight Stock less than 10

**Formula**

```excel
=L2<10
```

**Result**

Low-stock items are highlighted.

---

## Solution 31

**Task:** Highlight Attendance below 85%

**Formula**

```excel
=I2<85
```

**Result**

Employees with low attendance are highlighted.

---

## Solution 32

**Task:** Highlight Salary greater than Average Salary

**Formula**

```excel
=F2>AVERAGE($F$2:$F$61)
```

**Result**

Employees earning above average salary are highlighted.

---

## Solution 33

**Task:** Highlight Performance Rating = 5

**Formula**

```excel
=J2=5
```

**Result**

Top-rated employees are highlighted.

---

## Solution 34

**Task:** Highlight IT employees earning more than ₹80,000

**Formula**

```excel
=AND(C2="IT",F2>80000)
```

**Result**

Only IT employees with salary above ₹80,000 are highlighted.

---

# Part G – Managing Rules

## Solution 35

**Task:** View all Conditional Formatting Rules

**Steps**

```
Home → Conditional Formatting → Manage Rules
```

**Result**

Displays all existing formatting rules.

---

## Solution 36

**Task:** Edit an Existing Rule

**Steps**

```
Manage Rules → Select Rule → Edit Rule
```

**Result**

Selected rule is modified successfully.

---

## Solution 37

**Task:** Change Rule Priority

**Steps**

```
Manage Rules → Move Up / Move Down
```

**Result**

Rule execution order is updated.

---

## Solution 38

**Task:** Delete One Rule

**Steps**

```
Manage Rules → Delete Rule
```

**Result**

Selected formatting rule is removed.

---

## Solution 39

**Task:** Clear Rules from Selected Cells

**Steps**

```
Conditional Formatting → Clear Rules → Clear Rules from Selected Cells
```

**Result**

Formatting is removed only from the selected cells.

---

## Solution 40

**Task:** Clear Rules from Entire Worksheet

**Steps**

```
Conditional Formatting → Clear Rules → Clear Rules from Entire Sheet
```

**Result**

All Conditional Formatting rules are removed.

---

# ⭐ Challenge Questions

## Solution 41

**Task:** Highlight Top 5 Sales Performers

**Rule**

```
Top/Bottom Rules → Top Items
```

**Value**

```
5
```

**Result**

Top five sales performers are highlighted.

---

## Solution 42

**Task:** Highlight Attendance below 80%

**Formula**

```excel
=I2<80
```

**Result**

Attendance below 80% is highlighted in red.

---

## Solution 43

**Task:** Highlight Salary greater than ₹90,000

**Formula**

```excel
=F2>90000
```

**Formatting**

- Green Fill
- Bold Font

**Result**

High-salary employees are highlighted.

---

## Solution 44

**Task:** Highlight Completed Status

**Formula**

```excel
=K2="Completed"
```

**Result**

Completed records are highlighted.

---

## Solution 45

**Task:** Highlight Duplicate Employee IDs

**Rule**

```
Duplicate Values
```

**Result**

Duplicate Employee IDs receive one formatting style.

---

## Solution 46

**Task:** Highlight Duplicate Employee Names

**Rule**

```
Duplicate Values
```

**Result**

Duplicate Employee Names receive a different formatting style.

---

## Solution 47

**Task:** Apply Color Scale on Salary

**Rule**

```
3-Color Scale
```

**Result**

Salary distribution is visualized using colors.

---

## Solution 48

**Task:** Apply Color Scale on Sales

**Rule**

```
3-Color Scale
```

**Result**

Sales distribution is visualized using colors.

---

## Solution 49

**Task:** Highlight employees exceeding Target Sales by more than ₹50,000

**Formula**

```excel
=(N2-M2)>50000
```

**Result**

Employees exceeding their target by more than ₹50,000 are highlighted.

---

## Solution 50

**Task:** Create Dashboard Formatting

**Apply**

- Data Bars
- Color Scales
- Icon Sets
- Highlight Cells Rules

**Result**

A visually appealing dashboard with automatic highlighting and performance indicators is created.

---

