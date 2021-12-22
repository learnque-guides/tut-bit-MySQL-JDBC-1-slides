# JDBC functionalicty

JDBC support creating and executing statements. These may be update statements such as SQL's CREATE, INSERT, UPDATE and DELETE, or they may be query statements such as SELECT. Additionally, stored procedures may be invoked through a JDBC connection. JDBC represents statements using one of the following classes:
* Statement - the statement is sent to the database server each and every time.
* PreparedStatement - the statement is cached and then the execution path is pre-determined on the database server allowing it to be executed multiple times in an efficient manner.
* CallableStatement - used for executing stored procedures on the database.
* Update statements such as INSERT, UPDATE and DELETE return an update count that indicates how many rows were affected in the database. These statements do not return any other information.

Query statements return a JDBC row result set. The row result set is used to walk over the result set. Individual columns in a row are retrieved either by name or by column number. There may be any number of rows in the result set. The row result set has metadata that describes the names of the columns and their types.

JDBC connections are often managed via a connection pool rather than obtained directly from the driver.
