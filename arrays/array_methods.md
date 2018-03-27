# Push

You can insert elements inside an array with their method `push`. In fact, there is many other properties:
- `push(n)`: Add the element `n` at the end
- `pop()`: Remove the last element
- `sort()`: Sort the array by lexicographical order

```javascript
var array = [1, 2, 4];
array.push(8);
// Now array = [1, 2, 4, 8]
```

{% exercise %}
Add the city "Paris" to cities and sort it
{% initial %}
var cities = ["Madrid", "Barcelona", "Miami"];


var a =
{% solution %}
var cities = ["Madrid", "Barcelona", "Miami"];
cities.push("Paris");
cities.sort();

{% validation %}
assert (cities.length === 4);
assert (cities[0] === "Barcelona");
assert (cities[1] === "Madrid");
assert (cities[2] === "Miami");
assert (cities[3] === "Paris");
{% endexercise %}