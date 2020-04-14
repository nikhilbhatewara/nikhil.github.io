---
layout: default
---
# SQL

 - The DUAL table (1x1) is a special table in Oracle which can be leveraged as sequence generator or selecting pseudo fields such as SYSDATE. 
 - MySQL has a 1x1 dual table with dummy as field name
 - SQL Server does not have dual table.
 - We can insert more rows in dual table with admin access.
 - We cannot download all columns from a table #rookiemistake
 - count(1),count(*) provides same results using same resources
 - An IN operator can only take upto 999 values
 - **IN vs EXISTS:** When IN is used, *inner query will be executed first* and then outer query. When EXISTS is used, the *outer query is executed first* and then based on number of records form outer query, the inner query is executed. 
 - EXISTS operator works based on the “at least found” principle. It returns true and stops scanning table once at least one matching row found. Hence it is good to check if query would give any result or not
 - **WHERE vs HAVING:** Where is used to filter data *before aggregation* and Having is used to filter data *after aggregation*
 - DELETE is selective removal, transaction can be rollbacked, triggers will be fired before delete command
 - TRUNCATE removes all rows, no rollback is possible however no index/triggers/table dependencies will be impacted. Hence it is faster as no undo log is maintained.
 - To delete duplicate records, leverage rowid in oracle
 - **JOINS:** [A quick introduction](https://blog.codinghorror.com/a-visual-explanation-of-sql-joins/) 
 - If no join condition is specified. a CARTESIAN join (CROSS JOIN) will be performed
 - We can declare composite data type in SQL (Custom data type)
 - Use Conversion functions (TO_CHAR, TO_NUMBER) to typecast various data types.
 - 
 - 