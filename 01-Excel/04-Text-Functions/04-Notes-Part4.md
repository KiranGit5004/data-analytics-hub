# Text Functions in Excel - Part 4

---

# 1. FIND()

## Definition

The **FIND** function returns the position of one text string inside another text string.

Unlike the SEARCH function, **FIND is case-sensitive**, meaning uppercase and lowercase letters are treated as different characters.

This function is useful when you need to locate specific characters, symbols, or words within a text string.

---

## Syntax

```excel
=FIND(find_text, within_text, [start_num])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| find_text | The text you want to find |
| within_text | The text containing the search value |
| start_num | (Optional) Position from where the search should begin |

---

## Return Value

Returns the position number where the specified text first appears.

If the text is not found, Excel returns:

```text
#VALUE!
```

---

## Example 1

```excel
=FIND("A","Analytics")
```

Result

```
1
```

---

## Example 2

Email Address

```
rahul@gmail.com
```

Formula

```excel
=FIND("@",A2)
```

Result

```
6
```

The "@" symbol is located at the 6th position.

---

## Real-World Data Analytics Example

Customer Emails

| Email |
|--------|
| rahul@gmail.com |
| priya@yahoo.com |
| amit@company.in |

Find the position of "@"

```excel
=FIND("@",A2)
```

This is useful for:

- Extracting usernames
- Extracting email domains
- Validating email addresses

---

## Extract Domain Name

Email

```
rahul@gmail.com
```

Formula

```excel
=MID(A2,FIND("@",A2)+1,100)
```

Result

```
gmail.com
```

---

## Tips

- FIND is case-sensitive.
- Returns only the first occurrence.
- Works well with LEFT(), RIGHT(), and MID().

---

# 2. SEARCH()

## Definition

The **SEARCH** function also returns the position of one text string inside another.

Unlike FIND, **SEARCH is not case-sensitive**.

It also supports wildcard characters.

---

## Syntax

```excel
=SEARCH(find_text,within_text,[start_num])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| find_text | Text to locate |
| within_text | Text to search |
| start_num | Optional starting position |

---

## Return Value

Returns the position of the searched text.

If not found

```
#VALUE!
```

---

## Example 1

Customer Name

```
Rahul Sharma
```

Formula

```excel
=SEARCH("Sharma",A2)
```

Result

```
7
```

---

## Example 2

Website URL

```
www.google.com
```

Formula

```excel
=SEARCH(".",A2)
```

Result

```
4
```

---

# Wildcard Support

SEARCH supports wildcards.

### Asterisk (*)

Represents any number of characters.

Example

```excel
=SEARCH("Mic*",A2)
```

Can match

```
Microsoft
```

---

### Question Mark (?)

Represents exactly one character.

Example

```excel
=SEARCH("A?C",A2)
```

Matches

```
ABC
```

or

```
A1C
```

---

# FIND vs SEARCH

| Feature | FIND | SEARCH |
|----------|------|---------|
| Case Sensitive | ✔ Yes | ✘ No |
| Wildcards Supported | ✘ No | ✔ Yes |
| Returns Position | ✔ Yes | ✔ Yes |
| First Match Only | ✔ Yes | ✔ Yes |

---

# Which Function Should You Use?

| Situation | Recommended Function |
|-----------|----------------------|
| Password Validation | FIND |
| Email Parsing | FIND |
| Search Product Keywords | SEARCH |
| Search Customer Names | SEARCH |
| Case-sensitive Matching | FIND |
| Flexible Text Search | SEARCH |

---

# Business Scenario

Customer Database

| Customer | Email |
|-----------|----------------------|
| Rahul | rahul@gmail.com |
| Priya | priya@yahoo.com |
| Amit | amit@company.in |

Tasks

| Task | Function |
|------|----------|
| Find @ position | FIND |
| Extract email domain | FIND + MID |
| Search company emails | SEARCH |
| Search keywords in product names | SEARCH |

---

# Best Practices

- Use FIND when character case matters.
- Use SEARCH for user-entered text.
- Combine FIND with LEFT, MID, and RIGHT for advanced text extraction.
- Always handle errors using IFERROR() when appropriate.

Example

```excel
=IFERROR(FIND("@",A2),"Not Found")
```

---

# 3. REPLACE()

## Definition

The **REPLACE** function replaces a specific number of characters in a text string based on their position.

Unlike SUBSTITUTE, REPLACE works using **character positions**, not the actual text.

This function is useful when the position of the data is fixed.

---

## Syntax

```excel
=REPLACE(old_text,start_num,num_chars,new_text)
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| old_text | Original text |
| start_num | Position where replacement begins |
| num_chars | Number of characters to replace |
| new_text | New text |

---

## Return Value

Returns a modified text string after replacing characters.

---

## Example 1

```excel
=REPLACE("Excel",2,3,"123")
```

Result

```
E123l
```

---

## Example 2

Employee ID

```
EMP-1001
```

Formula

```excel
=REPLACE(A2,1,3,"HR")
```

Result

```
HR-1001
```

---

## Real-World Data Analytics Example

Mask customer phone numbers before sharing reports.

Original

```
9876543210
```

Result

```
98*****10
```

This protects customer privacy.

---

## Tips

REPLACE is useful when:

- Character positions are fixed
- IDs have consistent formats
- Phone numbers need masking
- Product codes require modification

---

# 4. SUBSTITUTE()

## Definition

The **SUBSTITUTE** function replaces specific text with new text.

Unlike REPLACE, SUBSTITUTE searches for actual text rather than character positions.

It is commonly used to clean imported datasets.

---

## Syntax

```excel
=SUBSTITUTE(text,old_text,new_text,[instance_num])
```

---

## Arguments

| Argument | Description |
|----------|-------------|
| text | Original text |
| old_text | Text to replace |
| new_text | Replacement text |
| instance_num | Optional occurrence number |

---

## Return Value

Returns updated text.

---

## Example 1

```excel
=SUBSTITUTE("Excel Training","Training","Course")
```

Result

```
Excel Course
```

---

## Example 2

Address

```
Mumbai, India
```

Formula

```excel
=SUBSTITUTE(A2,"Mumbai","Nashik")
```

Result

```
Nashik, India
```

---

## Example 3

Replace only second occurrence

Original

```
Apple Apple Apple
```

Formula

```excel
=SUBSTITUTE(A2,"Apple","Orange",2)
```

Result

```
Apple Orange Apple
```

---

## Real-World Data Analytics Example

Department Codes

Original

```
IT Dept
HR Dept
Finance Dept
```

Formula

```excel
=SUBSTITUTE(A2,"Dept","Department")
```

Result

```
IT Department
HR Department
Finance Department
```

---

# REPLACE vs SUBSTITUTE

| Feature | REPLACE | SUBSTITUTE |
|----------|----------|------------|
| Works using position | ✔ Yes | ✘ No |
| Works using text | ✘ No | ✔ Yes |
| Replace first occurrence | ✔ Yes | ✔ Yes |
| Replace specific occurrence | ✘ No | ✔ Yes |
| Best for fixed-length data | ✔ Yes | ✘ No |
| Best for cleaning text | ✘ No | ✔ Yes |

---

# Complete Text Function Comparison

| Function | Purpose | Common Use Case |
|----------|----------|----------------|
| LEFT | Extract characters from left | Employee Prefix |
| RIGHT | Extract characters from right | Last 4 digits of phone |
| MID | Extract text from middle | Employee Number |
| LEN | Count characters | Password Validation |
| TRIM | Remove extra spaces | Imported CSV files |
| UPPER | Convert to uppercase | Department Codes |
| LOWER | Convert to lowercase | Email Addresses |
| PROPER | Proper capitalization | Customer Names |
| CONCAT | Combine text | Full Name |
| TEXTJOIN | Combine with delimiter | Address |
| TEXT | Format numbers | Dates, Currency |
| VALUE | Convert text to number | Imported Sales Data |
| FIND | Locate text (case-sensitive) | Email Parsing |
| SEARCH | Locate text (case-insensitive) | Keyword Search |
| REPLACE | Replace by position | Mask Phone Number |
| SUBSTITUTE | Replace by text | Standardize Data |

---

# Real-World Business Scenario

Suppose you receive the following customer data from different systems.

| Customer ID | Name | Email | Phone |
|-------------|----------------|-----------------------|------------|
| CUS-1001 | rahul   sharma | RAHUL@GMAIL.COM | 9876543210 |
| CUS-1002 | PRIYA SINGH | PRIYA@YAHOO.COM | 9988776655 |
| CUS-1003 | amit patel | AMIT@COMPANY.IN | 9123456789 |

### Required Tasks

| Task | Function |
|------|----------|
| Extract Customer Prefix | LEFT |
| Extract Customer Number | MID |
| Count Name Characters | LEN |
| Remove Extra Spaces | TRIM |
| Convert Name to Proper Case | PROPER |
| Convert Email to Lowercase | LOWER |
| Create Full Address | TEXTJOIN |
| Format Joining Date | TEXT |
| Convert Imported Numbers | VALUE |
| Find Email Domain | FIND |
| Search Company Email | SEARCH |
| Mask Phone Number | REPLACE |
| Standardize Department Names | SUBSTITUTE |

These are typical tasks performed by Data Analysts before creating reports or dashboards.

---

# Best Practices

- Clean your data before analysis.
- Use TRIM after importing CSV or web data.
- Standardize names using PROPER.
- Store email addresses in lowercase.
- Convert imported numbers using VALUE.
- Use TEXT only for presentation.
- Prefer TEXTJOIN over CONCAT when separators are required.
- Combine FIND with MID or LEFT for advanced extraction.
- Validate formulas on sample data before applying them to large datasets.
- Use IFERROR to handle formula errors gracefully.

---
