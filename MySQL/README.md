# Employee Performance Metrics  ![logo-mysql-mysql-logo-png-images-are-download-crazypng-1](https://github.com/KaroLili1/myBAPortfolio.com/assets/155495785/d61c708f-fcdc-41c4-b2f2-d141790c6455)

- [General Info](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/README.md#general-info)
- [Technologies](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/README.md#technologies)
- [Tasks I have performed for this project](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/README.md#tasks-i-have-performed-for-this-project)
---

### **General Info**

This project aims to deliver a detailed report that identifies key performance indicators, discovers trends and provides data-based recommendations that support the strategic decision making of HR professionals, optimize the allocation of resources in accordance with the organization's standards, and foster a high-performance work culture in employees.
- - -

### **Technologies**
The data sets were provided by Simplilearn in the [Post Graduate Program in Business Analysis](https://www.simplilearn.com/pgp-business-analysis-certification-training-course) that I completed and which you can download for review here 👉 [emp_record_table.csv](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/emp_record_table.csv), [proj_table.csv](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/proj_table.csv) and [data_science_team.csv](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/data_science_team.csv).

For Exploratory Data Analysis I used several aggregate functions, such as COUNT(), AVG(), MIN(), MAX(),ROUND() and CONCAT(); operators such as BETWEEN, AND, LIKE, UNION.  Also I applied IF-THEN-ELSEIF statements to execute some logical conditions; Joins to combine data from different tables, and other codes like Stored Procedures, Stored Functions, Views, Indexes, Query Execution Plan to improve database performance.

For example, to calculate the 5% salary bonus for all employees, depending on their performance ratings and salaries, use the following formula in my query:

*MySQL*
```SQL
SELECT Emp_ID, FIRST_NAME, LAST_NAME, ROLE, DEPT, ROUND((SALARY * 0.05) * EMP_RATING) AS EMP_BONUS
FROM emp_record_table
ORDER BY EMP_BONUS DESC;
```

*Output:*


| Emp_ID | FIRST_NAME | LAST_NAME | ROLE | DEPT | EMP_BONUS |
|-------:|------------|-----------|------|------|-----------|
| E001   | Arthur     | Black     | PRESIDENT                | ALL        |      4125 |
| E083   | Patrick    | Voltz     | MANAGER                  | HEALTHCARE |      2375 |
| E428   | Pete       | Allen     | MANAGER                  | AUTOMOTIVE |      2200 |
| E103   | Emily      | Grove     | MANAGER                  | FINANCE    |      2100 |
| E204   | Karene     | Nowak     | SENIOR DATA SCIENTIST    | AUTOMOTIVE |      1875 |
| E612   | Tracy      | Norris    | MANAGER                  | RETAIL     |      1700 |
| E052   | Dianna     | Wilson    | SENIOR DATA SCIENTIST    | HEALTHCARE |      1375 |
| E005   | Eric       | Hoffman   | LEAD DATA SCIENTIST      | FINANCE    |      1275 |
| E260   | Roy        | Collins   | SENIOR DATA SCIENTIST    | RETAIL     |      1050 |
| E583   | Janet      | Hale      | MANAGER                  | RETAIL     |      1000 |
| E010   | William    | Butler    | LEAD DATA SCIENTIST      | AUTOMOTIVE |       900 |
| E478   | David      | Smith     | ASSOCIATE DATA SCIENTIST | RETAIL     |       800 |
| E403   | Steve      | Hoffman   | ASSOCIATE DATA SCIENTIST | FINANCE    |       750 |
| E245   | Nian       | Zhen      | SENIOR DATA SCIENTIST    | RETAIL     |       650 |
| E640   | Jenifer    | Jhones    | JUNIOR DATA SCIENTIST    | RETAIL     |       560 |
| E505   | Chad       | Wilson    | ASSOCIATE DATA SCIENTIST | HEALTHCARE |       500 |
| E057   | Dorothy    | Wilson    | SENIOR DATA SCIENTIST    | HEALTHCARE |       385 |
| E532   | Claire     | Brennan   | ASSOCIATE DATA SCIENTIST | AUTOMOTIVE |       215 |
| E620   | Katrina    | Allen     | JUNIOR DATA SCIENTIST    | RETAIL     |       150 |



- - -

### **Tasks I have performed for this project**
✔️ Data acquisition.  Download from the Simplilearn’s platform, the datasets containing information about employees’ first and last name, gender, role, department, years of experience, country, continent, salary, performance rating, direct manager, projects in charge.  As well as information about the project, such as field of the project, start and closure date, quarter in which project was scheduled and status, and detailed information about all the employees in the Data Science team.<br />
✔️ Cleaning & Preprocessing.  Prepare the raw dataset through cleaning operations that include dealing with NA/NULLS, duplicates, and outliers in it.<br />
✔️ Prepare the EER diamagra in MySQL of the ‘employee’ schema for modelling the data stored in the database.  <br />
✔️ Carry out the Exploratory Data Analysis (EDA).  Select KPSs that are most relevant to measuring employee performance trends.  <br />
✔️ Tend Analysis. Use subqueries and ranking window functions RANK(), OVER(), for analyzing patterns in specific metrics over different time periods. <br />
✔️ Visualization. Create charts in PBI to better present analysis results and provide deeper insights. <br />
<br />
> [!NOTE]
> You can download the final ScenceQtech Employee Performance Mapping Project here 👉 [pdf](https://github.com/KaroLili1/myBAPortfolio.com/blob/main/MySQL/Project1SQL.pdf)
<br />

**EERD of Employee's database designed by me in MySQL**

![Employee EERD](https://github.com/KaroLili1/myBAPortfolio.com/assets/155495785/8b69f853-c17c-4274-8a2b-c24f07f3183e)


🔙 Back to [Table of Contents](https://github.com/KaroLili1/myBAPortfolio.com)
