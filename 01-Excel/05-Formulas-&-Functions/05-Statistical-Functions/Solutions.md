# 📘 Solution – Statistical Functions Lab.

# Part A – Average Functions

## Solution 1

**Task:** Calculate the average salary.

**Formula**

```excel
=AVERAGE(H2:H51)
```

**Result**

Returns the average salary of all employees.

---

## Solution 2

**Task:** Calculate the average bonus.

**Formula**

```excel
=AVERAGE(I2:I51)
```

**Result**

Returns the average bonus.

---

## Solution 3

**Task:** Calculate the average sales.

**Formula**

```excel
=AVERAGE(J2:J51)
```

**Result**

Returns the average sales amount.

---

## Solution 4

**Task:** Calculate the average attendance.

**Formula**

```excel
=AVERAGE(L2:L51)
```

**Result**

Returns the average attendance percentage.

---

## Solution 5

**Task:** Average salary of IT employees.

**Formula**

```excel
=AVERAGEIF(C2:C51,"IT",H2:H51)
```

**Result**

Returns the average salary of employees in the IT department.

---

## Solution 6

**Task:** Average salary of Sales employees.

**Formula**

```excel
=AVERAGEIF(C2:C51,"Sales",H2:H51)
```

**Result**

Returns the average salary of employees in the Sales department.

---

## Solution 7

**Task:** Average salary of employees located in Mumbai.

**Formula**

```excel
=AVERAGEIF(D2:D51,"Mumbai",H2:H51)
```

**Result**

Returns the average salary of employees working in Mumbai.

---

## Solution 8

**Task:** Average salary of IT employees in Mumbai.

**Formula**

```excel
=AVERAGEIFS(H2:H51,C2:C51,"IT",D2:D51,"Mumbai")
```

**Result**

Returns the average salary of IT employees located in Mumbai.

---

## Solution 9

**Task:** Average sales of employees from Pune.

**Formula**

```excel
=AVERAGEIF(D2:D51,"Pune",J2:J51)
```

**Result**

Returns the average sales of employees from Pune.

---

## Solution 10

**Task:** Average attendance of HR employees.

**Formula**

```excel
=AVERAGEIF(C2:C51,"HR",L2:L51)
```

**Result**

Returns the average attendance percentage of HR employees.

---

# Part B – MEDIAN

## Solution 11

**Task:** Find the median salary.

**Formula**

```excel
=MEDIAN(H2:H51)
```

**Result**

Returns the middle salary.

---

## Solution 12

**Task:** Find the median age.

**Formula**

```excel
=MEDIAN(F2:F51)
```

**Result**

Returns the median employee age.

---

## Solution 13

**Task:** Find the median bonus.

**Formula**

```excel
=MEDIAN(I2:I51)
```

**Result**

Returns the median bonus amount.

---

## Solution 14

**Task:** Find the median sales amount.

**Formula**

```excel
=MEDIAN(J2:J51)
```

**Result**

Returns the median sales amount.

---

# Part C – MODE.SNGL

## Solution 15

**Task:** Find the most common performance rating.

**Formula**

```excel
=MODE.SNGL(K2:K51)
```

**Result**

Returns the performance rating that occurs most frequently.

---

## Solution 16

**Task:** Find the most common attendance percentage.

**Formula**

```excel
=MODE.SNGL(L2:L51)
```

**Result**

Returns the attendance percentage that appears most often.

---

## Solution 17

**Task:** Find the most common employee age.

**Formula**

```excel
=MODE.SNGL(F2:F51)
```

**Result**

Returns the age that appears most frequently.

---

# Part D – LARGE

## Solution 18

**Task:** Find the highest salary.

**Formula**

```excel
=LARGE(H2:H51,1)
```

**Result**

Returns the highest salary.

---

## Solution 19

**Task:** Find the second highest salary.

**Formula**

```excel
=LARGE(H2:H51,2)
```

**Result**

Returns the second highest salary.

---

## Solution 20

**Task:** Find the third highest salary.

**Formula**

```excel
=LARGE(H2:H51,3)
```

**Result**

Returns the third highest salary.

---

## Solution 21

**Task:** Find the highest sales amount.

**Formula**

```excel
=LARGE(J2:J51,1)
```

**Result**

Returns the highest sales amount.

---

## Solution 22

**Task:** Find the top five salaries.

**Formula**

```excel
=LARGE(H2:H51,{1;2;3;4;5})
```

**Result**

Returns the five highest salaries as a spilled array (Excel 365) or use five separate formulas with k = 1 to 5 in older Excel.

---

## Solution 23

**Task:** Find the lowest salary.

**Formula**

```excel
=SMALL(H2:H51,1)
```

**Result**

Returns the lowest salary.

---

## Solution 24

**Task:** Find the second lowest salary.

**Formula**

```excel
=SMALL(H2:H51,2)
```

**Result**

Returns the second lowest salary.

---

## Solution 25

**Task:** Find the third lowest salary.

**Formula**

```excel
=SMALL(H2:H51,3)
```

**Result**

Returns the third lowest salary.

---

## Solution 26

**Task:** Find the lowest sales amount.

**Formula**

```excel
=SMALL(J2:J51,1)
```

**Result**

Returns the lowest sales amount.

---

## Solution 27

**Task:** Find the five lowest salaries.

**Formula**

```excel
=SMALL(H2:H51,{1;2;3;4;5})
```

**Result**

Returns the five lowest salaries as a spilled array (Excel 365) or use five separate formulas with k = 1 to 5.

---

# Part F – RANK.EQ

## Solution 28

**Task:** Rank employees based on Salary (Highest Salary = Rank 1)

**Formula**

```excel
=RANK.EQ(H2,$H$2:$H$51,0)
```

**Result**

Returns the salary rank of each employee.

---

## Solution 29

**Task:** Rank employees based on Sales.

**Formula**

```excel
=RANK.EQ(J2,$J$2:$J$51,0)
```

**Result**

Returns the sales rank of each employee.

---

## Solution 30

**Task:** Rank employees based on Attendance.

**Formula**

```excel
=RANK.EQ(L2,$L$2:$L$51,0)
```

**Result**

Returns the attendance rank.

---

## Solution 31

**Task:** Rank employees based on Bonus.

**Formula**

```excel
=RANK.EQ(I2,$I$2:$I$51,0)
```

**Result**

Returns the bonus rank.

---

# Part G – PERCENTILE.INC

## Solution 32

**Task:** Find the 25th percentile of Salary.

**Formula**

```excel
=PERCENTILE.INC(H2:H51,0.25)
```

**Result**

Returns the salary at the 25th percentile.

---

## Solution 33

**Task:** Find the 50th percentile of Salary.

**Formula**

```excel
=PERCENTILE.INC(H2:H51,0.50)
```

**Result**

Returns the median salary.

---

## Solution 34

**Task:** Find the 75th percentile of Salary.

**Formula**

```excel
=PERCENTILE.INC(H2:H51,0.75)
```

**Result**

Returns the salary at the 75th percentile.

---

## Solution 35

**Task:** Find the 90th percentile of Sales.

**Formula**

```excel
=PERCENTILE.INC(J2:J51,0.90)
```

**Result**

Returns the sales value at the 90th percentile.

---

# Part H – QUARTILE.INC

## Solution 36

**Task:** Find the First Quartile (Q1).

**Formula**

```excel
=QUARTILE.INC(H2:H51,1)
```

**Result**

Returns the first quartile of salaries.

---

## Solution 37

**Task:** Find the Second Quartile (Median).

**Formula**

```excel
=QUARTILE.INC(H2:H51,2)
```

**Result**

Returns the median salary.

---

## Solution 38

**Task:** Find the Third Quartile (Q3).

**Formula**

```excel
=QUARTILE.INC(H2:H51,3)
```

**Result**

Returns the third quartile of salaries.

---

## Solution 39

**Task:** Find the Maximum Salary using QUARTILE.INC.

**Formula**

```excel
=QUARTILE.INC(H2:H51,4)
```

**Result**

Returns the maximum salary.

---

# Part I – STDEV.S

## Solution 40

**Task:** Calculate the standard deviation of Salary.

**Formula**

```excel
=STDEV.S(H2:H51)
```

**Result**

Returns the sample standard deviation of employee salaries.

---

## Solution 41

**Task:** Calculate the standard deviation of Bonus.

**Formula**

```excel
=STDEV.S(I2:I51)
```

**Result**

Returns the sample standard deviation of bonuses.

---

## Solution 42

**Task:** Calculate the standard deviation of Sales.

**Formula**

```excel
=STDEV.S(J2:J51)
```

**Result**

Returns the sample standard deviation of sales.

---

## Solution 43

**Task:** Calculate the standard deviation of Attendance.

**Formula**

```excel
=STDEV.S(L2:L51)
```

**Result**

Returns the sample standard deviation of attendance percentage.

---

# ⭐ Challenge Questions

## Solution 44

**Task:** Find the Top 5 highest-paid employees.

**Formula**

```excel
=SORT(H2:L51,1,-1)
```

**Result**

Displays employees sorted by highest salary.

---

## Solution 45

**Task:** Find the Bottom 5 employees based on Salary.

**Formula**

```excel
=SORT(H2:L51,1,1)
```

**Result**

Displays employees with the lowest salaries.

---

## Solution 46

**Task:** Rank employees based on Sales Performance.

**Formula**

```excel
=RANK.EQ(J2,$J$2:$J$51,0)
```

**Result**

Returns the sales rank of each employee.

---

## Solution 47

**Task:** Calculate the average salary of Female employees.

**Formula**

```excel
=AVERAGEIF(E2:E51,"Female",H2:H51)
```

**Result**

Returns the average salary of female employees.

---

## Solution 48

**Task:** Calculate the average salary of Male employees.

**Formula**

```excel
=AVERAGEIF(E2:E51,"Male",H2:H51)
```

**Result**

Returns the average salary of male employees.

---

## Solution 49

**Task:** Calculate the average sales of employees having Performance Rating = 5.

**Formula**

```excel
=AVERAGEIF(K2:K51,5,J2:J51)
```

**Result**

Returns the average sales of employees with a rating of 5.

---

## Solution 50

**Task:** Find the department with the highest average salary.

**Formula**

```excel
=AVERAGEIF(C2:C51,"IT",H2:H51)
```

Repeat the formula for each department and compare the results.

**Result**

Identifies the department with the highest average salary.

---

## Solution 51

**Task:** Determine whether employee salaries have high or low variation.

**Formula**

```excel
=STDEV.S(H2:H51)
```

**Result**

Returns the standard deviation, which indicates salary variation.

---

## Solution 52

**Task:** Identify employees whose salary is greater than the 75th percentile.

**Formula**

```excel
=H2>PERCENTILE.INC($H$2:$H$51,0.75)
```

**Result**

Returns **TRUE** for employees earning above the 75th percentile and **FALSE** otherwise.

---

## Solution 53

**Task:** Create a Statistical Summary Report.

**Formulas**

Average Salary

```excel
=AVERAGE(H2:H51)
```

Median Salary

```excel
=MEDIAN(H2:H51)
```

Highest Salary

```excel
=MAX(H2:H51)
```

Lowest Salary

```excel
=MIN(H2:H51)
```

Most Common Rating

```excel
=MODE.SNGL(K2:K51)
```

Salary Standard Deviation

```excel
=STDEV.S(H2:H51)
```

**Result**

Displays a complete statistical summary of the employee dataset.

---

