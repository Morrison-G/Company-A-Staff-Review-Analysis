# Company-A-Staff-Review-Analysis
> This Excel work on Company A review case study aims to analyze resumption year, months, days of their staffs and how long each staff has worked. Key features are: Clean Dashboard to support business decision making.
Case Study by Morrison (Analyst).

## Project Overview
> This case study analyses Company A work force, number of months, days each staff has been with the company. 

## Data Content
### Rows: were 320 in Total.
 ### Columns: were 16 in Total.
> Product details: name, department, resumption date, exist date, employment type and salary.

## Tool Used
> Microsoft Excel (Excel functions).

## Data Cleaning Actions
> Some data cleaning steps were applied to make the dataset proper for analysis without errors.

## Steps
### Name Column: cleaned using Proper & Upper function (nesting), removing extra spacing in names.
### Helper columns: calculated columns and category columns were used in generating the Dashboard.


## Key Business Questions Answered

1.	Resumption year for each staff?
Add a calculated column:
= year (resumption date)

2.	Resumption month for each staff?

Add a calculated column:

= month (resumption date)

3.	Name of resumption month for each staff?
Add a calculated column:

= text (resumption date,”mmmm”)


4.	Resumption day for each staff?

Add a calculated column:

= day (resumption date)

5.	Name of resumption day for each staff?
Add a calculated column:

= text (resumption date,”dddd”)

6.	Numbers of days in employment for each staff, considering the exit date of some staff?
Add a calculated column:

= if (ISBLANK exit date, TODAY-resumption date, exit date-resumption date)

7.	Numbers of months in employment for each staff, without considering the exit date of some staff?
Add a calculated column:

= Datedif (resumption date,TODAY,”m”)
8.	Numbers of months in employment for each staff, considering the exit date of some staff?
Add a calculated column:
= numbers of days in employment for each staff / 30 (no of days in a month)

## Section Details
> ### Column Names: Emp ID, Name, Department, Resumption date, Exit date, Resumption year, Resumption month, Name of Resumption month, Resumption day, Resumption day in the week, Days in employment, Months in employment considering the exit date, Months in employment without considering the exit date, Location, Employment type, Salary.
> ### Excel formulas used: PROPER() UPPER() TRIM() YEAR() MONTH() DAY() TEXT() DATEDIF() TODAY() IF() ISBLANK() 

## Analytics Dashboard
 

## Findings
> 1.	Total no of year, months and days each staff has stayed in employment with the company.
> 2.	Resumption day for each staff.
> 3.	No of Months existed staff stayed in employment.

## Conclusion
> Using Excel to generate business ready insight from identifying, understanding and knowing months, days each staff existed or not have stayed with the company.




