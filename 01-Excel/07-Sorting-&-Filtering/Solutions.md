# 📘 Solution – Sorting & Filtering Lab

## Dataset Used

**Employee_Sorting_Filtering_Dataset.xlsx**

Worksheet:

```
Employee_Data
```

---

# Part A – Basic Sorting

## Solution 1

**Task:** Sort Employee Names from A to Z.

**Steps**

```
Data → Sort A to Z
```

**Result**

Employee names are sorted alphabetically in ascending order.

---

## Solution 2

**Task:** Sort Employee Names from Z to A.

**Steps**

```
Data → Sort Z to A
```

**Result**

Employee names are sorted in reverse alphabetical order.

---

## Solution 3

**Task:** Sort Salary from Smallest to Largest.

**Steps**

```
Data → Smallest to Largest
```

**Result**

Salary values are arranged in ascending order.

---

## Solution 4

**Task:** Sort Salary from Largest to Smallest.

**Steps**

```
Data → Largest to Smallest
```

**Result**

Salary values are arranged in descending order.

---

## Solution 5

**Task:** Sort Join Date from Oldest to Newest.

**Steps**

```
Data → Oldest to Newest
```

**Result**

Employees are arranged according to their joining date.

---

## Solution 6

**Task:** Sort Join Date from Newest to Oldest.

**Steps**

```
Data → Newest to Oldest
```

**Result**

Most recently joined employees appear first.

---

# Part B – Custom Sorting

## Solution 7

**Task:** Sort employees by Department.

**Steps**

```
Data → Sort → Custom Sort
Sort By → Department
Order → A to Z
```

**Result**

Employees are grouped department-wise.

---

## Solution 8

**Task:** Sort by Department, then Salary.

**Steps**

```
Sort By → Department
Add Level
Then By → Salary
Order → Largest to Smallest
```

**Result**

Employees are grouped by department, with highest salaries listed first within each department.

---

## Solution 9

**Task:** Sort by City, then Employee Name.

**Steps**

```
Sort By → City
Add Level
Then By → Employee Name
```

**Result**

Employees are grouped by city and sorted alphabetically within each city.

---

## Solution 10

**Task:** Sort by Status, then Join Date.

**Steps**

```
Sort By → Status
Add Level
Then By → Join Date
Order → Oldest to Newest
```

**Result**

Employees are grouped by status and arranged by joining date.

---

## Solution 11

**Task:** Sort by Performance Rating.

**Steps**

```
Sort By → Performance Rating
Order → Largest to Smallest
```

**Result**

Highest-rated employees appear first.

---

## Solution 12

**Task:** Sort by Sales, then Bonus.

**Steps**

```
Sort By → Sales
Add Level
Then By → Bonus
Order → Largest to Smallest
```

**Result**

Employees are sorted by sales, then by bonus.

---

# Part C – Text Filters

## Solution 13

**Task:** Display IT Department employees.

**Filter**

```
Department = IT
```

**Result**

Only IT department employees are displayed.

---

## Solution 14

**Task:** Display Mumbai employees.

**Filter**

```
City = Mumbai
```

**Result**

Only employees from Mumbai are displayed.

---

## Solution 15

**Task:** Display Completed Status.

**Filter**

```
Status = Completed
```

**Result**

Only completed records are shown.

---

## Solution 16

**Task:** Display names containing Rahul.

**Filter**

```
Text Filters → Contains → Rahul
```

**Result**

Employees whose names contain "Rahul" are displayed.

---

## Solution 17

**Task:** Display names beginning with A.

**Filter**

```
Text Filters → Begins With → A
```

**Result**

Employees whose names start with A are displayed.

---

## Solution 18

**Task:** Display departments other than HR.

**Filter**

```
Text Filters → Does Not Equal → HR
```

**Result**

All departments except HR are displayed.

---

# Part D – Number Filters

## Solution 19

**Task:** Salary greater than ₹80,000.

**Filter**

```
Number Filters → Greater Than → 80000
```

**Result**

Employees earning above ₹80,000 are displayed.

---

## Solution 20

**Task:** Salary less than ₹50,000.

**Filter**

```
Number Filters → Less Than → 50000
```

**Result**

Employees earning below ₹50,000 are displayed.

---

## Solution 21

**Task:** Salary between ₹60,000 and ₹90,000.

**Filter**

```
Number Filters → Between
60000
90000
```

**Result**

Employees within the salary range are displayed.

---

## Solution 22

**Task:** Sales above ₹500,000.

**Filter**

```
Number Filters → Greater Than → 500000
```

**Result**

Employees having sales above ₹500,000 are displayed.

---

## Solution 23

**Task:** Attendance below 85%.

**Filter**

```
Number Filters → Less Than → 85
```

**Result**

Employees with attendance below 85% are displayed.

---

## Solution 24

**Task:** Performance Rating = 5.

**Filter**

```
Equals → 5
```

**Result**

Employees with a rating of 5 are displayed.

---

## Solution 25

**Task:** Above Average Salary.

**Filter**

```
Number Filters → Above Average
```

**Result**

Employees earning above average salary are displayed.

---

## Solution 26

**Task:** Below Average Sales.

**Filter**

```
Number Filters → Below Average
```

**Result**

Employees having below-average sales are displayed.

---

# Part E – Date Filters

## Solution 27

**Task:** Employees joined This Year.

**Filter**

```
Date Filters → This Year
```

**Result**

Employees who joined during the current year are displayed.

---

## Solution 28

**Task:** Employees joined Last Year.

**Filter**

```
Date Filters → Last Year
```

**Result**

Employees who joined during the previous year are displayed.

---

## Solution 29

**Task:** Employees joined This Month.

**Filter**

```
Date Filters → This Month
```

**Result**

Employees who joined during the current month are displayed.

---

## Solution 30

**Task:** Employees joined between two dates.

**Filter**

```
Date Filters → Between
```

**Result**

Employees within the selected date range are displayed.

---

# Part F – Advanced Filter

## Solution 31

**Task:** Display Unique Employee IDs.

**Steps**

```
Data → Advanced
Unique Records Only
```

**Result**

Only unique Employee IDs are displayed.

---

## Solution 32

**Task:** Copy IT employees to another location.

**Steps**

```
Advanced Filter
Criteria:
Department = IT

Copy to another location
```

**Result**

Only IT employees are copied.

---

## Solution 33

**Task:** Sales Department with Salary > ₹70,000.

**Criteria**

```
Department = Sales
Salary > 70000
```

**Result**

Matching employees are displayed.

---

## Solution 34

**Task:** Pune employees with Completed status.

**Criteria**

```
City = Pune
Status = Completed
```

**Result**

Matching employees are displayed.

---

## Solution 35

**Task:** Performance Rating = 5.

**Criteria**

```
Performance Rating = 5
```

**Result**

Employees with rating 5 are extracted.

---

# Part G – Business Scenarios

## Solution 36

**Task:** Highest salary.

**Method**

```
Sort Salary
Largest to Smallest
```

**Result**

Highest-paid employee appears first.

---

## Solution 37

**Task:** Lowest sales.

**Method**

```
Sort Sales
Smallest to Largest
```

**Result**

Lowest sales record appears first.

---

## Solution 38

**Task:** Actual Sales exceeded Target Sales.

**Filter**

```
Actual Sales > Target Sales
```

**Result**

Employees exceeding targets are displayed.

---

## Solution 39

**Task:** Stock less than 20.

**Filter**

```
Stock < 20
```

**Result**

Low-stock records are displayed.

---

## Solution 40

**Task:** Sales employees from Mumbai.

**Criteria**

```
Department = Sales
City = Mumbai
```

**Result**

Matching employees are displayed.

---

## Solution 41

**Task:** Attendance greater than 95%.

**Filter**

```
Attendance > 95
```

**Result**

Employees with excellent attendance are displayed.

---

## Solution 42

**Task:** Salary > ₹90,000 and Rating = 5.

**Criteria**

```
Salary > 90000
Performance Rating = 5
```

**Result**

Only high-performing, high-paid employees are displayed.

---

## Solution 43

**Task:** Pending status and Stock < 15.

**Criteria**

```
Status = Pending
Stock < 15
```

**Result**

Pending records with low stock are displayed.

---

## Solution 44

**Task:** Sort by Department → City → Salary.

**Steps**

```
Sort By → Department
Then By → City
Then By → Salary
Order → Largest to Smallest
```

**Result**

Employees are grouped by department and city, with salaries sorted in descending order.

---

## Solution 45

**Task:** Sort by Rating → Sales → Employee Name.

**Steps**

```
Sort By → Performance Rating
Then By → Sales
Then By → Employee Name
```

**Result**

Employees are sorted by performance rating, then sales, then name.

---

# ⭐ Challenge Questions

## Solution 46

**Task:** Top 10 highest-paid employees.

**Filter**

```
Number Filters → Top 10
```

**Result**

Top 10 salary records are displayed.

---

## Solution 47

**Task:** Top 10 Sales Performers.

**Method**

```
Sort Sales
Largest to Smallest
```

**Result**

Top sales performers appear first.

---

## Solution 48

**Task:** Employees earning above average salary.

**Filter**

```
Number Filters → Above Average
```

**Result**

Employees earning above the average salary are displayed.

---

## Solution 49

**Task:** Actual Sales below Target Sales.

**Criteria**

```
Actual Sales < Target Sales
```

**Result**

Employees who missed their sales targets are displayed.

---

## Solution 50

**Task:** Display IT and Finance departments.

**Filter**

```
Department = IT
OR
Department = Finance
```

**Result**

Only IT and Finance department employees are displayed.

---

## Solution 51

**Task:** Employees who joined after 1 January 2024.

**Filter**

```
Join Date > 01-Jan-2024
```

**Result**

Employees who joined after the specified date are displayed.

---

## Solution 52

**Task:** Find duplicate Employee IDs.

**Method**

```
Sort Employee ID
```

or

```
Conditional Formatting → Duplicate Values
```

**Result**

Duplicate Employee IDs are identified.

---

## Solution 53

**Task:** Prepare a filtered business report.

**Criteria**

```
Department = Sales
Status = Completed
Salary > 70000
Attendance > 90
```

**Result**

A report containing only employees meeting all specified conditions is displayed.

---

