# Database

1. Database: mySQL server
     https://dev.mysql.com/downloads/mysql/

2. Database URL for connection:
   ```
	jdbc:mysql://localhost:3306/myPatient
   ```
 myPatient is the name of database

3. Driver class for connectivity:
 ```
	com.mysql.cj.jdbc.Driver
```
4. Connection Object to link the program to the database

```
Class.forName("com.mysql.cj.jdbc.Driver");
            conn = DriverManager.getConnection(
                "jdbc:mysql://localhost:3306/myPatient", "sqluser", "password");
```

Example Code
```
import java.sql.*;
public class mySQLConn {
    public static void main(String[] args) {
        Connection conn = null;
        try{

            Class.forName("com.mysql.cj.jdbc.Driver");
            conn = DriverManager.getConnection(
                "jdbc:mysql://localhost:3306/myPatient", "sqluser", "password");

            Statement sta ;
            sta = conn.createStatement();    
            ResultSet reSet;
            reSet = sta.executeQuery("select * from patientRecord");
            System.out.println("reSEt"+reSet.toString());
            reSet.close();
            sta.close();
            conn.close();
        } catch (Exception e){
            System.out.println(e);

        }
    }
}
```

Reference: Connect to Mysql Server Using VS Code




[1] [How to connect to mySql Server](https://www.geeksforgeeks.org/how-to-connect-to-mysql-server-using-vs-code-and-fix-errors/) Retrieved from https://www.geeksforgeeks.org/how-to-connect-to-mysql-server-using-vs-code-and-fix-errors/

 
