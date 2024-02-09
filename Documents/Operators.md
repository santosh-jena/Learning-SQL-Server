## Operators
1. [Arithmetic operators](#arithmetic-operators)
2. [Relational Operators](#relational-operators)
3. [Logical operators](#logical-operators)
4. [Special Operators](#special-operators)

### Arithmetic operators:

|Operator|Name|Description|
|--------|----|-----------|
|+ | Addition|add two numeric value together.|
|- |Substations |Subtracts one numeric value from other.|
|* |Multiplication | Multiplies tow numbers together.|
|/ |Division |Divides one number by another. |
|% |Modulus  | Returns reminder of a division operation.|

### Relational Operators:
|Operator|Name|Description|
|--------|----|-----------|
|>|Greater  then|Check one value is greater then another.|
|>=|Greater then equal to|Check one value is greater or equal to another.|
|<|Less then|Check one value is less then another.|
|<=|Less then equal to|Check one value is less or equal to another value.|
|=|equal|Check tow numbers are equal|
|<>|Not Equal|Check two numbers are not equal|

### Questions
1. [Write a query to display employee details whose empId is 103 ?](#write-a-query-to-display-employee-details-whose-empid-is-103)
2. [Write a query to display employee details who is earning more then 5000?](#write-a-query-to-display-employee-details-who-is-earning-more-then-5000)
3. [Write a query to display EMPLOYEE list who joined after 2020 ?](#write-a-query-to-display-employee-list-who-joined-after-2020)
4. [Write a query to display EMPLOYEE list who joined after 2020 ?](#write-a-query-to-display-employee-list-who-joined-before-2020)
#### Write a query to display employee details whose empId is 103 ?
```SQL
SELECT * FROM EMPLOYEE WHERE empId = 103
```

#### Write a query to display employee details who is earning more then 5000?
```SQL
SELECT * FROM EMPLOYEE WHERE SALARY > 5000
```
#### Write a query to display EMPLOYEE list who joined after 2020 ?
```SQL
SELECT * FROM EMPLOYEE WHERE HIREDATE > '2020-12-31'
```
#### Write a query to display EMPLOYEE list who joined before 2020 ?
```SQL
SELECT * FROM EMPLOYEE WHERE HIREDATE < '2021-01-01'
```
### Logical operators:
|Operator|Name|Description|
|--------|----|-----------|
|AND| And| This is used to combine tow and more conditions, it should return true if all condition true or else return false.|
|OR|Or|This is used to combine tow or more conditions, resulting expression is true at least one of the individual conditions is true. |
|NOT|Not|This is used for negative condition.|' 

__Compound Conditions :__
Multiple conditions are combined with (AND / OR) operators called compound conditions.

### Questions:
1. [Write a query to display employee details who joined in 2020 ?](#write-a-query-to-display-employee-details-who-joined-in-2020)
2. [Write a query to retrieve employee details who is working as clark, manager ?](#write-a-query-to-retrieve-employee-details-who-is-working-as-clark-manager)
3. [Write a query to display employee details who are not in IT department ?](#write-a-query-to-display-employee-details-who-are-not-in-it-department)
#### Write a query to display employee details who joined in 2020 ?
```SQL
--- Based on range
SELECT * FROM EMPLOYEE WHERE HIREDATE > '2019-12-31' AND HIREDATE < '2021-01-01'

--- Based year select
SELECT * FROM EMPLOYEE WHERE YEAR(HIREDATE) = 2020

```
#### Write a query to retrieve employee details who is working as clark, manager ?
```SQL
SELECT * FROM EMPLOYEE WHERE JOB = 'Clark' || JOB = 'Manager'
```

#### Write a query to display employee details who are not in IT department ?
```SQL 
SELECT * FROM EMPLOYEE WHERE NOT JOB = 'IT'
```


### Special Operators:
```
LIKE
BETWEEN
IN
IS
ANY

```