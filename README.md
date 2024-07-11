# SQL1_Uebungen
## Airways ERM + Create Tables

Create an ERM including a relational model. After finishing the ERM create the tables in your database.

### Overview
The All Airways Association (AAA) is an association that brings together all airlines. This association plans to install a comprehensive information system for flight handling. An initial survey produces the following situation report:

- When a passenger (passenger number, name, Mr/Mrs, title, etc.) wants to book a flight (or several), he or she first specifies the desired departure and destination airports, the desired flight date and possibly also a time frame when he or she wants to fly away or arrive.
- There are various airlines (name, headquarters, etc.) that operate flights. Airlines are identified by a code of maximum three digits (e.g., PA for PanAm, FUA for Futura Air).
- Each airline operates aircraft (aircraft number, international registration number, name, date of entry into service, etc.) of different aircraft types (type identification, manufacturer, range, etc.).
- The airports (name, city, country, capacity in aircraft, etc.) are also encrypted with a three-digit code (e.g., VIE for Vienna-Schwechat, JFK for New York - John F. Kennedy, IBZ for Ibiza).
- The distances between airports must be recorded in order to be able to take the range of the aircraft type into account when drawing up the flight plan.
- Each flight has a departure airport and an arrival airport, the flights are numbered consecutively with a three-digit number within a company. (e.g., PA039 between VIE and JFK, FUA916 between IBZ and VIE)
- Each flight has a fixed scheduled departure and arrival time, and the days on which the flight takes place are also specified. (e.g., 'daily', 'only weekends', 'specific day of week').
- Each flight booked by a passenger is summarized on one ticket (ticket number, date of issue, price, currency, sales office, etc.)
- Before starting the flight, the passenger will be given a boarding card at the airport, on which in addition to the flight number, date, departure airport, destination airport and name of the passenger, the allocated seat (row as number, seat as letter, e.g., 18D) appears.
- Each aircraft type has a specific number of available rows and seats (numbers/letters).
- For each flight, it must also be possible to record the actual take-off and landing time in order to be able to make evaluations of the punctuality of individual flights.

## Airways ERM insert and delete data

After you created your tables start by inserting some sample data into your database and delete some of the data. Practice the insert and update statement.

## Create the flight plan

Now you can start to print a full flight plan for your day. Practice the select statement and try to select your sample data.

## Change structure of tables

Change the structure of a table (your choice) and try out the alter table statement.

## SQL Exercise 02

1. **Create table** - Create the tables DEPT and EMP from the file dept_emp.sql. ( [EmpDept.sql](https://github.com/DaStanzel/SQLUebung02/blob/main/dept_emp.sql) )
2. **Simple output 1** - Output of all departments (for DNAME column heading DEPARTMENT NAME).
3. **Date output** - Output of EMPNO, ENAME and HIREDATE (format DD. Month YYYY) for each employee.
4. **Date output 2** - Output of ENAME and the number of days since joining the company (column heading DAYS) for each employee.
5. **Simple output 2** - Output of jobs (only 1 output per job).
6. **Minmax output** - Output of the minimum, maximum and average salary.
7. **Count 1** - Statement to determine "How many employees are there?".
8. **Count 2** - Statement to determine "How many different jobs are there?".

## Competence Check

Create the tables and insert data from the following files: [Create Tables](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung01/CreateTables.sql), [Insert Data](https://github.com/DaStanzel/Unterlagen-Datenbanken-CB/blob/main/%C3%9Cbungen/SQLUebung01/InsertScript.sql). If you are working on the Oracle database adjust the insert script dates and number formats.

1. The HR department wants a query to display the last name, job identifier (JOB_ID), hire date and employee number for each employee, with the employee number as the first value. Specify the alias STARTDATE for the HIRE_DATE column.
2. HR requires a query to display all unique job identifiers (JOB_ID) from the EMPLOYEES table. Duplicates are to be avoided.
3. The HR department wants more meaningful column headings for the reports related to employees. Use the statement from output 3.1 and give the columns the headings Emp #, Employee, Job and Hire Date. Run the query again.
4. For budget purposes, HR needs a report that shows the last name and salary for employees earning more than $12,000. Run the query.
5. Create a report to show the last name and department number for the employee with employee number 176.
6. Create a report to show the last name, job identifier (JOB_ID) and hire date for all employees. Sort the query in ascending order by hire date.
7. View last names and department numbers of all employees in Department 20, sorted alphabetically by last name in ascending order.
8. Create a query that displays last names, salaries and commissions of all employees whose commission is 20%. Give the columns the headings Employee, Monthly Salary and Commission.
