# Pewlett-Hackard Analysis

PostgreSQL Queries
---
## Overview of Analysis

Our client, Pewlett-Hackard, has recently become aware that an abnormally large number of their employees may become eligible for retirement at the same time, many (or even most) of them in leadership roles.  Given 6 spreadsheets of company/employee data, we used SQL queries to identify the employees who will likely retire, the roles they currently fill, and a list of eligible candidates for mentorship to fill those roles.
---
### Resources:
**Software:** PostreSQL 14, pgAdmin 4 v6.1, Visual Studio Code 1.62.3

**Resource Files:** [departments.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/departments.csv), [dept_emp.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/dept_emp.csv), [dept_manager.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/dept_manager.csv), [employees.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/employees.csv), [salaries.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/salaries.csv), [titles.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/titles.csv)

## Results

- [retirement_titles.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/retirement_titles.csv): A spreadsheet containing names, employment dates and ALL titles held by potentially retiring current employees.

![retirement_titles.png](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Resources/retirement_titles.png)
    - We can see that this table has certain employees appearing multiple times, reflecting the many titles they've held during their employment with Pewlett-Hackard.
- [unique_titles.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/unique_titles.csv): A refined spreadsheet containing only the current title held by employees in the above pool.

![unique_titles.png](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Resources/unique_titles.png)
    - The same list of employees as shown in the first table, except drilled down using the the employment dates from the first table to isolate only the currently held positions.

### Potential Job Vacancies
- [retiring_titles.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/retiring_titles.csv): A Count of potentially retiring employees, by job title.

![retiring_titles.png](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Resources/retiring_titles.png)
    - There are a total of 72,458 employees who could be seeking to retire soon.

![retiring_titles_barchart.png](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Resources/retiring_titles_barchart.png)
    - Of those 72,458 employees, the VAST majority of them hold "Senior" titles.  These are employees with a wealth of professional experience that could be devastating to lose all at once.  Immediate implimentation of an internal mentorship is recommended to mitigate impact to company productivity.

### Candidates for Mentorship
- [mentorship_eligibility.csv](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Data/mentorship_eligibility.csv): A spreadsheet containing the employees who are eligible for mentorship by one of the upcoming retirees.

![mentorship_eligibility.png](https://github.com/ZeroDarkHardy/Pewlett-Hackard_analysis/blob/main/Resources/mentorship_eligibility.png)


## Summary