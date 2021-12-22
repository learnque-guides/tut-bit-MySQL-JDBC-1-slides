# Connection to database by using Driver manager

```java
public static Connection getConnectionFromDriverManager() throws SQLException {
    Connection connection = null;
    Properties connectionProps = new Properties();
    connectionProps.put("user", USERNAME);
    connectionProps.put("password", PASSWORD);

    connection = DriverManager.getConnection(
            String.format("jdbc:mysql://%s:%s/", HOST, PORT),
            connectionProps
    );
    connection.setCatalog(DATABASE);

    return connection;
}
```