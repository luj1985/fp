##  Java JDBC Transaction

```
Connection conn = null;
PreparedStatement stat = null;

String sql = "INSERT INTO FRUIT (NAME, COST) VALUES (?,?)";

try {
  conn = getconn();
  conn.setAutoCommit(false);
  stat = conn.prepareStatement(sql);
  stat.setString(1, "Fig");
  stat.setInt(2, 12);
  stat.executeUpdate();

  conn.commit();
} catch (SQLException e) {
  conn.rollback();
  throw e;
} finally {
  if (stat != null) {
    stat.close();
  }
  if (conn != null) {
    conn.close();
  }
}
```
