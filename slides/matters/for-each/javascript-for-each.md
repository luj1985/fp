Javascript for each
```javascript
var arr = [1, 2, 3, 4, 5];
arr.forEach(function(v) {
  console.log(v);
});
```

Even for Browsers which doesn't support forEach
```javascript
Array.prototype.forEach = function(action, that /*opt*/) {
  for (var i = 0, n = this.length; i < n; i++)
    if (i in this)
      action.call(that, this[i], i, this);
};
```