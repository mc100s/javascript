# Reference (Advanced)

The difference between objects and primitive values is that **we can change objects**, whereas primitive values are immutable. 

Objects are **never copied**. They are passed around by reference.

```js
var myPrimitive1 = "first value";
var myPrimitive2 = myPrimitive1;
myPrimitive2 = "second value";

var myObject1 = { key: "first value"};
var myObject2 = myObject1;
myObject2.key = "second value";

// myPrimitive1 = "first value"
// myPrimitive2 = "second value"

// myObject1 = { key: "second value"}
// myObject2 = { key: "second value"}
```
