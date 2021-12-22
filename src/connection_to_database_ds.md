# Connection to database by using Data source

```java
public static Connection getConnectionFromDataSource() throws SQLException {
    Connection connection;
    MysqlDataSource dataSource = new MysqlDataSource();
    dataSource.setUrl(String.format("jdbc:mysql://%s:%s/", HOST, PORT));
    dataSource.setUser(USERNAME);
    dataSource.setPassword(PASSWORD);
    connection = dataSource.getConnection();
    connection.setCatalog(DATABASE);

    return connection;
}
```