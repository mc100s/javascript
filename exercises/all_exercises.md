# All Exercises

<!-- Exercise 1 -->
{% exercise %}
Substration of 2 numbers

{% initial %}
// Exercise 1: Substration of 2 numbers
function subs(a, b) {
} 

{% solution %}
function subs(a, b) {
    return a - b;
} 

{% validation %}
assert(subs(42, 38) === 4, "Testing subs(42, 38)");
assert(subs(38, 42) === -4, "Testing subs(38, 42)");
assert(subs(100,100) === 0, "Testing subs(100,100)");

{% endexercise %}

<!-- Exercise 2 -->
{% exercise %}
Substration of 2 numbers

{% initial %}
function subs(a, b) {




    
} 

{% solution %}
function subs(a, b) {
    return a - b;
} 

{% validation %}
assert(subs(42, 38) === 4, "Testing subs(42, 38)");
assert(subs(38, 42) === -4, "Testing subs(38, 42)");
assert(subs(100,100) === 0, "Testing subs(100,100)");

{% endexercise %}



<!-- Exercise 2 -->
{% exercise %}
Find the maximum

{% initial %}
function maxOfTwoNumbers(a, b) {




  
}  

{% solution %}
function maxOfTwoNumbers(a, b) {
    if (a > b) {
        return a;
    }
    else {
        return b;
    }
} 

{% validation %}
assert(maxOfTwoNumbers(42, 38) === 42, "Testing maxOfTwoNumbers(42, 38)");
assert(maxOfTwoNumbers(38, 42) === 42, "Testing maxOfTwoNumbers(38, 42)");
assert(maxOfTwoNumbers(100,100) === 100, "Testing maxOfTwoNumbers(100,100)");

{% endexercise %}


```javascript
// Try to solve has many exercises as possible
// You can go to https://repl.it/languages/javascript to test your code
// Send your code the person that sent you the challenge, for example by saving the code in Repl.it and sharing the link

// To help solving it, you can find  

// Good luck ;)

// Exercise 0 (Example): Function that returns the sum of 2 numbers
function sum(a, b) {
  var result = a + b;
  return result;
} 
console.log("> Exercice 0 --- Should display 42");
console.log(sum(20, 22));


// Exercise 1: Substration of 2 numbers
function subs(a, b) {
} 
console.log("\n> Exercice 1 --- Should display 4");
console.log(subs(42, 38));


// Exercise 2: Find the maximum
function maxOfTwoNumbers(a, b) {
} 
console.log("\n> Exercice 2 --- Should display 6");
console.log(maxOfTwoNumbers(2, 6));


// Exercise 3: Find the longest word
// Hint: you can use a variable "currentMax". In the example, its value would be: 0, 3, 5, 42, 42, 42
function maxOfArray(numbers) {
}
console.log("\n> Exercice 3 --- Should display 42");
console.log(maxOfArray([ 3, 5, 42, 12, 38 ]));


// Exercise 4: Find the longest word
function findLongestWord (words) {
}
var words = [
  "mystery",
  "brother",
  "aviator",
  "crocodile",
  "pearl",
  "orchard",
  "crackpot"
];
console.log("\n> Exercice 4 --- Should display 'crocodile'");
console.log(findLongestWord(words));


// Exercise 5: Calculate the sum of all elements
function sumArray (array) {
}
console.log("\n> Exercice 5 --- Should display 20");
console.log(sumArray([6, 3, 1, 10]));

// Exercise 6: Calculate the average of all elements
function averageNumbers (array) {
}
console.log("\n> Exercice 6 --- Should display 5");
console.log(averageNumbers([6, 3, 1, 10]));


// Exercise 7: Calculate the average length of all elements
function averageWordLength (array) {
}
var words = [
  "seat",
  "correspond",
  "linen",
  "motif",
  "hole",
  "smell",
  "smart",
  "chaos",
  "fuel",
  "palace"
];
console.log("\n> Exercice 7 --- Should display 5.3");
console.log(averageWordLength(words));


// Exercise 8: Finding a string inside an array
function doesWordExist (wordsArray, word) {
}
var words = [
  "machine",
  "subset",
  "trouble",
  "starting",
  "matter",
  "eating",
  "truth",
  "disobedience"
];
console.log("\n> Exercice 8 --- Should display true, false");
console.log(doesWordExist(words, "matter"));
console.log(doesWordExist(words, "dog"));


// Exercise 9: Counting Repetion
function howManyTimes (words, word) {
}
var words = [
  "machine",
  "matter",
  "subset",
  "trouble",
  "starting",
  "matter",
  "eating",
  "matter",
  "truth",
  "disobedience",
  "matter"
];
console.log("\n> Exercice 9 --- Should display 4, 0");
console.log(howManyTimes(words, "matter"));
console.log(howManyTimes(words, "dog"));


// Exercise 10 (bonus): find the greatest product, on a row or a on column
// In the following example, the greatest product is on the second column (3 and 4) and its value is 12 (3*4). 
//   [  [1,3]
//      [2,4]  ]
function greatestProduct (matrix) {
}
var matrix = [
  [08,02,22,97,38,15,0,40,0,75,04,05,07,78,52,12,50,77,91,08],
  [49,49,99,40,17,81,18,57,60,87,17,40,98,43,69,48,04,56,62,0],
  [81,49,31,73,55,79,14,29,93,71,40,67,53,88,30,03,49,13,36,65],
  [52,70,95,23,04,60,11,42,69,24,68,56,01,32,56,71,37,02,36,91],
  [22,31,16,71,51,67,63,89,41,92,36,54,22,40,40,28,66,33,13,80],
  [24,47,32,60,99,03,45,02,44,75,33,53,78,36,84,20,35,17,12,50],
  [32,98,81,28,64,23,67,10,26,38,40,67,59,54,70,66,18,38,64,70],
  [67,26,20,68,02,62,12,20,95,63,94,39,63,08,40,91,66,49,94,21],
  [24,55,58,05,66,73,99,26,97,17,78,78,96,83,14,88,34,89,63,72],
  [21,36,23,09,75,0,76,44,20,45,35,14,0,61,33,97,34,31,33,95],
  [78,17,53,28,22,75,31,67,15,94,03,80,04,62,16,14,09,53,56,92],
  [16,39,05,42,96,35,31,47,55,58,88,24,0,17,54,24,36,29,85,57],
  [86,56,0,48,35,71,89,07,05,44,44,37,44,60,21,58,51,54,17,58],
  [19,80,81,68,05,94,47,69,28,73,92,13,86,52,17,77,04,89,55,40],
  [04,52,08,83,97,35,99,16,07,97,57,32,16,26,26,79,33,27,98,66],
  [88,36,68,87,57,62,20,72,03,46,33,67,46,55,12,32,63,93,53,69],
  [04,42,16,73,38,25,39,11,24,94,72,18,08,46,29,32,40,62,76,36],
  [20,69,36,41,72,30,23,88,34,62,99,69,82,67,59,85,74,04,36,16],
  [20,73,35,29,78,31,90,01,74,31,49,71,48,86,81,16,23,57,05,54],
  [01,70,54,71,83,51,54,69,16,92,33,48,61,43,52,01,89,19,67,48],
];
console.log("\n> Exercice 10 (bonus)");
console.log(greatestProduct(matrix));
```
