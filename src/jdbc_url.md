# MySQL Connector/J Database URL

The following is the database connection URL syntax for MySQL Connector/J:
```
jdbc:mysql://[host][:port]/[database][?propertyName1][=propertyValue1][&propertyName2][=propertyValue2]...
```

* *host:port* is the host name and port number of the computer hosting your database. If not specified, the default values of host and port are 127.0.0.1 and 3306, respectively.
* *database* is the name of the database to connect to. If not specified, a connection is made with no default database.
* *propertyName=propertyValue* represents an optional, ampersand-separated list of properties. These attributes enable you to instruct MySQL Connector/J to perform various tasks.
