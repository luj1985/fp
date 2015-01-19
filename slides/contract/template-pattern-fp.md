Function as contract
```
function executeSQL(command) {
  var conn;
  try {
    conn = getConnection();
    command(conn);
    conn.commit();
  } catch(e) {
    conn.rallback();
    throw e;
  } finally {
    conn.close();
  }
}

```
```
executeSQL(function(conn) {
  conn.execute('INSERT INTO ...');
});
```