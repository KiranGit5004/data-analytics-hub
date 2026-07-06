# Excel Text Functions - Interview Questions & Answers

------------------------------------------------------------------------

# Table of Contents

1.  Basic Questions
2.  Function-Based Questions
3.  Difference-Based Questions
4.  Scenario-Based Questions
5.  Rapid Fire
6.  Interview Tips

------------------------------------------------------------------------

# Basic Interview Questions

## Q1. What are Text Functions in Excel?

**Answer:** Text Functions manipulate, clean, extract, combine, search,
and format text values.

## Q2. Why are Text Functions important for Data Analysts?

**Answer:** They help clean imported datasets, standardize values,
extract useful information, and prepare data for analysis.

## Q3. Name four commonly used Text Functions.

**Answer:** LEFT, RIGHT, MID, TRIM.

## Q4. Which function counts characters?

**Answer:** `LEN()`.

## Q5. Which function removes extra spaces?

**Answer:** `TRIM()`.

------------------------------------------------------------------------

# Function-Based Questions

## Q6. What does LEFT() do?

**Answer:** Returns characters from the beginning of a text string.

## Q7. What does RIGHT() do?

**Answer:** Returns characters from the end of a text string.

## Q8. What is MID() used for?

**Answer:** Extracts characters from any position in a text string.

## Q9. What does LEN() return?

**Answer:** Total number of characters including spaces.

## Q10. Why use TRIM()?

**Answer:** Removes leading, trailing and extra spaces between words.

## Q11. What does UPPER() do?

**Answer:** Converts all letters to uppercase.

## Q12. What does LOWER() do?

**Answer:** Converts all letters to lowercase.

## Q13. What does PROPER() do?

**Answer:** Capitalizes the first letter of each word.

## Q14. What does CONCAT() do?

**Answer:** Combines multiple text strings.

## Q15. Why use TEXTJOIN() instead of CONCAT()?

**Answer:** TEXTJOIN supports delimiters and can ignore blank cells.

## Q16. What does TEXT() do?

**Answer:** Converts numbers into formatted text.

## Q17. What does VALUE() do?

**Answer:** Converts numeric text into an actual number.

## Q18. What does FIND() return?

**Answer:** Position of text. It is case-sensitive.

## Q19. What does SEARCH() return?

**Answer:** Position of text. It is case-insensitive and supports
wildcards.

## Q20. What does REPLACE() do?

**Answer:** Replaces characters based on position.

## Q21. What does SUBSTITUTE() do?

**Answer:** Replaces matching text with new text.

------------------------------------------------------------------------

# Difference-Based Questions

## Q22. LEFT vs RIGHT

**Answer:** LEFT extracts from the beginning; RIGHT extracts from the
end.

## Q23. LEFT vs MID

**Answer:** LEFT starts at the first character; MID starts at any
specified position.

## Q24. FIND vs SEARCH

**Answer:** FIND is case-sensitive; SEARCH is not and supports
wildcards.

## Q25. REPLACE vs SUBSTITUTE

**Answer:** REPLACE uses character position; SUBSTITUTE replaces
matching text.

## Q26. CONCAT vs TEXTJOIN

**Answer:** CONCAT joins values; TEXTJOIN joins values with a delimiter
and can ignore blanks.

## Q27. TEXT vs VALUE

**Answer:** TEXT converts numbers to formatted text; VALUE converts text
to numbers.

## Q28. UPPER vs PROPER

**Answer:** UPPER capitalizes every letter; PROPER capitalizes the first
letter of each word.

## Q29. TRIM vs CLEAN

**Answer:** TRIM removes extra spaces; CLEAN removes non-printable
characters.

------------------------------------------------------------------------

# Scenario-Based Questions

## Q30. How would you extract the employee prefix from `EMP-1001`?

**Answer:** `=LEFT(A2,3)`

## Q31. How would you extract `1001` from `EMP-1001`?

**Answer:** `=MID(A2,5,4)`

## Q32. How would you get the last four digits of a phone number?

**Answer:** `=RIGHT(A2,4)`

## Q33. How would you count password length?

**Answer:** `=LEN(A2)`

## Q34. Customer names contain extra spaces. Which function?

**Answer:** `TRIM()`

## Q35. Emails are in uppercase. Which function?

**Answer:** `LOWER()`

## Q36. Employee names are inconsistent (`rAhUl ShArMa`). Which function?

**Answer:** `PROPER()`

## Q37. Numbers imported from CSV are stored as text. Which function?

**Answer:** `VALUE()`

## Q38. You need to find the @ symbol in emails.

**Answer:** `FIND("@",A2)`

## Q39. You need to replace "Dept" with "Department".

**Answer:** `SUBSTITUTE(A2,"Dept","Department")`

## Q40. You need to mask the middle digits of a phone number.

**Answer:** `REPLACE()`

------------------------------------------------------------------------

# Formula-Based Questions

## Q41. Formula to create Full Name?

**Answer:** `=CONCAT(A2," ",B2)`

## Q42. Formula to combine address fields?

**Answer:** `=TEXTJOIN(", ",TRUE,A2:C2)`

## Q43. Format a date as `01-Jul-2025`?

**Answer:** `=TEXT(A2,"dd-mmm-yyyy")`

## Q44. Convert `"500"` into a number?

**Answer:** `=VALUE(A2)`

## Q45. Extract first name from "Rahul Sharma".

**Answer:** `=LEFT(A2,FIND(" ",A2)-1)`

## Q46. Extract email domain.

**Answer:** `=MID(A2,FIND("@",A2)+1,100)`

## Q47. Count characters excluding extra spaces.

**Answer:** `=LEN(TRIM(A2))`

## Q48. Convert department code to uppercase.

**Answer:** `=UPPER(A2)`

## Q49. Standardize customer names.

**Answer:** `=PROPER(A2)`

## Q50. Search for the word "Laptop".

**Answer:** `=SEARCH("Laptop",A2)`

------------------------------------------------------------------------

# Rapid Fire Questions

**Q51. Which function counts spaces?**\
**Answer:** LEN

**Q52. Which function ignores blank cells while joining?**\
**Answer:** TEXTJOIN

**Q53. Which function supports wildcards?**\
**Answer:** SEARCH

**Q54. Which function is case-sensitive?**\
**Answer:** FIND

**Q55. Which function removes extra spaces?**\
**Answer:** TRIM

**Q56. Which function converts text to numbers?**\
**Answer:** VALUE

**Q57. Which function converts numbers to formatted text?**\
**Answer:** TEXT

**Q58. Which function joins text?**\
**Answer:** CONCAT

**Q59. Which function replaces by position?**\
**Answer:** REPLACE

**Q60. Which function replaces matching text?**\
**Answer:** SUBSTITUTE

------------------------------------------------------------------------

# Interview Tips

-   Understand **when** to use each function instead of memorizing
    syntax.
-   Practice combining multiple text functions in a single formula.
-   Be prepared to explain real-world use cases.
-   Know common function differences (FIND vs SEARCH, REPLACE vs
    SUBSTITUTE, CONCAT vs TEXTJOIN).
-   Most Excel interview questions focus on solving business problems
    rather than recalling definitions.

------------------------------------------------------------------------

# Final Revision Checklist

-   ✅ LEFT
-   ✅ RIGHT
-   ✅ MID
-   ✅ LEN
-   ✅ TRIM
-   ✅ UPPER
-   ✅ LOWER
-   ✅ PROPER
-   ✅ CONCAT
-   ✅ TEXTJOIN
-   ✅ TEXT
-   ✅ VALUE
-   ✅ FIND
-   ✅ SEARCH
-   ✅ REPLACE
-   ✅ SUBSTITUTE

