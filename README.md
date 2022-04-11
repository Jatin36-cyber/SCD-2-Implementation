# SCD-2-Implementation

![alt text](https://news.blr.com/app/uploads/sites/3/2019/09/relocation-assistance.jpg)

# Introduction: 
A company X wants to keep its employee data up to date in their central database.  
Since, over the time, many employees prefer to change their base location, it is essential to update the employee information in the company's central database. 
 
# Problem Statement: 
The field 'Location' is a Slowly changing Dimension (  a dimension whose attribute or attributes for a record (row) change slowly over time). We will be using SCD-2 type implementation to keep a full history of dimension data in the table. The Type 2 Dimension mapping filters source rows based on user-defined comparisons and inserts both new and changed dimensions into the target. Changes are tracked in the target table by looking up the primary key and creating a version number for each dimension in the table called a surrogate key.  
 
# ETL Process: 
We are sourcing the data from MS SQL Server, transforming it using Informatica and loading it to Oracle server.

# Source Table

![image](https://user-images.githubusercontent.com/100192162/155977866-6f203037-d0f4-4c18-b33e-f5a515714f2b.png)

# Target Table

<img width="661" alt="Oracle_Result" src="https://user-images.githubusercontent.com/100192162/155978551-b887c5ca-56c8-447c-ac67-98b12862bd6c.png">
