### Javascript high order function examples

```javascript
fn.map( function ( value ) { 
  return value * 2; 
}, [ 0, 1, 2, 3, 4, 5, 6 ] );
// [ 0, 2, 4, 6, 8, 10, 12 ]

fn.reduce( function ( accumulator, value, index ) {
  return accumulator + value + index;
}, 0, [ 1, 2, 3 ] );
// 9

var f = fn.compse( Math.sqrt, Math.abs);
f(-100);
// 10
```
fn.js http://eliperelman.com/fn.js