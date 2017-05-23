![GitHub Logo](https://s3.ap-south-1.amazonaws.com/greyatom-social/GreyAtom-logo.png)

# WHERE Clause

The SQL WHERE clause is used to specify a condition while fetching the data from a single table or by joining with multiple tables. If the given condition is satisfied, then only it returns a specific value from the table. You should use the WHERE clause to filter the records and fetching only the necessary records.

The WHERE clause is not only used in the SELECT statement, but it is also used in the UPDATE, DELETE statement, etc., which we would examine in the subsequent chapters.

The WHERE clause is not only used in SELECT statement, but it is also used in UPDATE, DELETE statement, etc., which we would examine in subsequent chapters.

### Syntax

The basic syntax of the SELECT statement with the WHERE clause is as shown below.

        SELECT column1, column2, columnN
        FROM table_name
        WHERE [condition]

You can specify a condition using the comparison or logical operators like >, <, =, LIKE, NOT, etc. The following examples would make this concept clear.

### Example

The following code is an example which would fetch the CustomerID, CustomerName, ContactName fields from the Customers table, where the City is London −

        Select CustomerID, CustomerName, Address from greyatom.Customers WHERE City='London';

This would produce the following result −

 | CustomerID | CustomerName | Address |
 | ---------- | ------------ | ------- |
 | 4 | Around the Horn | 120 Hanover Sq. |
 | 11 | B's Beverages | Fauntleroy Circus |
 | 16 | Consolidated Holdings | Berkeley Gardens 12 Brewery |
 | 19 | Eastern Connection | 35 King George |
 | 53 | North/South | South House 300 Queensbridge |
 | 72 | Seven Seas Imports | 90 Wadhurst Rd. |

**Note:**

Here, it is important to note that all the strings should be given inside single quotes (''). Whereas, numeric values should be given without any quote as in the above example.

