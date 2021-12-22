# Establish a connection

* DriverManager: This fully implemented class connects an application to a data source, which is specified by a database URL. When this class first attempts to establish a connection, it automatically loads any JDBC 4.0 drivers found within the class path.
* DataSource: This interface is preferred over DriverManager because it allows details about the underlying data source to be transparent to your application. (Typically by using JNDI (Java Naming and Directory Interface))
