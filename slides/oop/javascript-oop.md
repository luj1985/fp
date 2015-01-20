Javascript OOP

```
function Point(x, y, z) {
  this.x = x;
  this.y = y;
  this.z = z;
}

Point.prototype.distance = function {
  var x = this.x, y = this.y, z = this.z;
  return Math.sqrt(x*x + y*y + z*z);
};

var p = new Point(3, 4, 12);
p.distance();

```