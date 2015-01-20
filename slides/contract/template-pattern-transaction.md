Interface as contract (Template Pattern)

```
public abstract class JDBCExecutor {
  public abstract void execute(Connection conn);

  public void run() throws SQLException {
    Connection conn;
    try {
      conn = openConnection();
      this.execute(conn);
      conn.commit();
    } catch (Exception e) {
      conn.rollback();
    } finally {
      conn.close();
    }
  }
}

```