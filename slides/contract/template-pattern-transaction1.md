Interface as contract

```
public class InsertRecord extends JDBCExecutor {
  @Override
  public void execute(Connection conn) {
    PrepareStatement stat = conn.prepareStatement('INSERT INTO ....');
    ....
    stat.close();
  }
}
```

```
JDBCExecutor task = new InsertRecord();
task.run();
```