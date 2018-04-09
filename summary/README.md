# Summary

## Basics
```javascript
var float = 3.1416;
var integer = 42;
var boolean = true;
var n = null;
```

## Numbers
```javascript
var x = 0;  // =  0
x = x + 10; // = 10
x += 5;     // = 15
x++;        // = 16
```

## Strings
```javascript
var firstname = "John";
var lastname = "Doe";
var fullname = firstname + " " + lastname; // = "John Doe"
var size = fullname.length; // = 8
```

## Conditional Logic
```javascript
if(country === 'England') { 
  // ...
} else if(country === 'France') {
  // ...
} else if(country === 'Germany') {
  // ...
} else {
  // ...
}

// AND
if(x > 10 && x < 20) {
  // ...
}

// OR
if(x < 10 || x > 20) {
  // ...
}
```




## Arrays
```javascript
// Creation
var cars = ["Mazda", "Tesla", "Chevy", "Ford"];

// Access
var myCar = cars[1]; // = "Tesla"

// Length
let nb = cars.length; // = 4

// Add a new element
cars.push("Peugeot"); // = ["Mazda", "Tesla", "Chevy", "Ford", "Peugeot"]

// Sort
cars.sort(); // = ["Chevy", "Ford", "Mazda", "Peugeot", "Tesla"]
```

## Loops
```javascript
// For i from 0 to 10 excluded and incremented by 1
for(var i = 0; i < 10; i++){
  // do this code ten-times
}

while(condition){
  // do it as long as condition is true
}
```

## Functions
```javascript
function myFunctionName(param1, param2, param3) {
  return param1 + param2 + param3;
}
```

## Objects
```javascript
var myEmptyObject = {};

var language = {
  name: 'JavaScript',
  isSupportedByBrowsers: true,
  createdIn: 1995,
  author:{
    firstName: 'Brendan',
    lastName: 'Eich'
  },
  getAuthorFullName: function(){
    return this.author.firstName + " " + this.author.lastName;    
  }
};
language.name; // = "JavaScript"
language["name"]; // = "JavaScript"
language.author.lastName; // = "Eich"
language.getAuthorFullName(); // = "Brendan Eich"
```