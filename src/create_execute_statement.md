# Creating and executing statements

```java
public static void executeQueryAndPrint(Connection conn, String SQL) throws SQLException {
    try (PreparedStatement ps = conn.prepareStatement(SQL)) {
        // Getting results from resultSet
        ResultSet rs = ps.executeQuery();
        while (rs.next()) {
            System.out.printf("Order id: %s%n", rs.getString("orderid"));
        }
    }
}
```

Statements that begin with *DELETE*, *INSERT*, or *UPDATE* typically use a method called executeUpdate()

It is also possible to pass parameters when *PreparedStatement* is used

```java
// SELECT * FROM Orders WHERE orderid = ?
ps.setInt(index, value) // 1, 11050
```