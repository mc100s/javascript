# All Exercises


<!-- Exercise -->
{% exercise %}
Substration of 2 numbers<br>
- <u>Input</u>: 2 numbers (ex: <code>42</code> and <code>38</code>) <br>
- <u>Output</u>: The difference (ex: <code>4</code>)

{% initial %}
function subs(a, b) {
} 

{% solution %}
function subs(a, b) {
    return a - b;
} 

{% validation %}
assert(subs(42, 38) === 4, "Fail for subs(42, 38)");
assert(subs(38, 42) === -4, "Fail for subs(38, 42)");
assert(subs(100,100) === 0, "Fail for subs(100,100)");

{% endexercise %}



<!-- Exercise -->
{% exercise %}
Even or Odd number?<br>
- <u>Input</u>: A number (ex: <code>42</code>) <br>
- <u>Output</u>: A string that is either "Even" or "Odd" (ex: <code>"Even"</code>)

{% initial %}
function evenOrOdd(n) {
} 

{% solution %}
function evenOrOdd(n) {
    if (n % 2 === 0) {
        return "Even";
    }
    else {
        return "Odd";
    }
} 

{% validation %}
assert(evenOrOdd(42) === "Even", "Fail for evenOrOdd(42)");
assert(evenOrOdd(1) === "Odd", "Fail for evenOrOdd(1)");

{% endexercise %}



<!-- Exercise -->
{% exercise %}
Find the maximum of 2 numbers <br>
- <u>Input</u>: 2 numbers (ex: <code>42</code> and <code>38</code>) <br>
- <u>Output</u>: The biggest number (ex: <code>42</code>)

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
assert(maxOfTwoNumbers(42, 38) === 42, "Fail for maxOfTwoNumbers(42, 38)");
assert(maxOfTwoNumbers(38, 42) === 42, "Fail for maxOfTwoNumbers(38, 42)");
assert(maxOfTwoNumbers(100,100) === 100, "Fail for maxOfTwoNumbers(100,100)");

{% endexercise %}


<!-- Exercise -->
{% exercise %}
Find the maximum of 3 numbers <br>
- <u>Input</u>: 3 numbers (ex: <code>42</code>, <code>38</code> and <code>12</code>) <br>
- <u>Output</u>: The biggest number (ex: <code>42</code>)

{% initial %}
function maxOfThreeNumbers(a, b, c) {
}  

{% solution %}
function maxOfThreeNumbers(a, b, c) {
    if (a > b && a > c) {
        return a;
    }
    else if (b > c) {
        return b;
    }
    else {
        return c;
    }
} 

{% validation %}
assert(maxOfThreeNumbers(42, 38, 12) === 42, "Fail for maxOfThreeNumbers(42, 38, 12)");
assert(maxOfThreeNumbers(38, 42, 12) === 42, "Fail for maxOfThreeNumbers(38, 42, 12)");
assert(maxOfThreeNumbers(12, 38, 42) === 42, "Fail for maxOfThreeNumbers(12, 38, 42)");

{% endexercise %}


<!-- Exercise  -->
{% exercise %}
Calculate the sum of all elements<br>
<u>Input</u>: Array of number (ex: <code>[2, 10, 30]</code>) <br>
<u>Output</u>: The sum (ex: <code>42</code>)

{% initial %}
function sumArray(array) {
}

{% solution %}
function sumArray(array) {
    var curSum = 0;
    for (var i = 0; i < array.length; i++) {
        curSum += array[i];
    }
    return curSum;
}

{% validation %}
assert(sumArray([2, 10, 30]) === 42, "Fail for sumArray([2, 10, 30])");
assert(sumArray([8]) === 8, "Fail for sumArray([8])");

{% endexercise %}



<!-- Exercise -->
{% exercise %}
Find the maximum of a non-empty array <br>
- <u>Input</u>: Array of numbers (ex: <code>[ 3, 5, 42, 12, 38 ]</code> ) <br>
- <u>Output</u>: The biggest number (ex: <code>42</code> )

{% initial %}
function maxOfArray(numbers) {
}

{% solution %}
function maxOfArray(numbers) {
    if (numbers.length === 0) {
        return null;
    }
    var currentMax = numbers[0];
    for (var i = 1; i < numbers.length; i++) {
        if (currentMax < numbers[i]) {
            currentMax = numbers[i];
        }
    }
    return currentMax;
}

{% validation %}
assert(maxOfArray([42, 38, 12]) === 42, "Fail for maxOfArray([42, 38, 12])");
assert(maxOfArray([38, 42, 12]) === 42, "Fail for maxOfArray([38, 42, 12])");
assert(maxOfArray([12, 38, 42]) === 42, "Fail for maxOfArray([12, 38, 42])");

{% endexercise %}




<!-- Exercise -->
{% exercise %}
Find the longest word <br>
- <u>Input</u>: Array of strings (ex: <code>[ "car", "plane", "bike"]</code>) <br>
- <u>Output</u>: The longest string (ex: <code>"plane"</code>)

{% initial %}
function findLongestWord (words) {
}

{% solution %}
function findLongestWord (words) {
    var currentMax = "";
    for (var i = 0; i < words.length; i++) {
        if (currentMax.length < words[i].length) {
            currentMax = words[i];
        }
    }
    return currentMax;
}


{% validation %}
assert(findLongestWord([ "car", "plane", "bike"]) === "plane", 'Fail for findLongestWord([ "car", "plane", "bike"])');
assert(findLongestWord([ "mystery", "brother", "aviator", "crocodile", "pearl", "orchard", "crackpot"]) === "crocodile", 'Fail for findLongestWord([ "mystery", "brother", "aviator", "crocodile", "pearl", "orchard", "crackpot"])');

{% endexercise %}







<!-- Exercise  -->
{% exercise %}
Finding a word inside an array<br>
- <u>Input</u>: Array of strings and a string (ex: <code>["Madrid", "Barcelona", "Miami"]</code> and <code>"Paris"</code>) <br>
- <u>Output</u>: A boolean that is true when the word is in the array (ex: <code>false</code>)

{% initial %}
function doesWordExist(wordsArray, word) {
}

{% solution %}
function doesWordExist(wordsArray, word) {
    for (var i = 0; i < wordsArray.length; i++) {
        if (wordsArray[i] === word) {
            return true;
        }
    }
    return false;
}

{% validation %}
assert(doesWordExist(["Madrid", "Barcelona", "Miami"], "Paris") === false, 'Fail for doesWordExist(["Madrid", "Barcelona", "Miami"], "Paris")');
assert(doesWordExist(["Madrid", "Barcelona", "Miami"], "Madrid") === true, 'Fail for doesWordExist(["Madrid", "Barcelona", "Miami"], "Madrid")');

{% endexercise %}



<!-- Exercise  -->
{% exercise %}
Get the fullname<br>
- <u>Input</u>: An object with at least 2 string properties "firstname" and "lastaname" (ex: <code>{firstname: "John", lastname: "Doe"}</code>) <br>
- <u>Output</u>: A string the represents the fullname (dont' forget the space in the middle) (ex: <code>John Doe</code>)

{% initial %}
function getFullname(person) {
}

{% solution %}
function getFullname(person) {
    return person.firstname + ' ' + person.lastname;
}

{% validation %}
assert(getFullname({firstname: 'John', lastname: 'Doe'}) === 'John Doe', "Fail for getFullname({firstname: 'John', lastname: 'Doe'})");
assert(getFullname({firstname: 'A', lastname: 'B'}) === 'A B', "Fail for getFullname({firstname: 'A', lastname: 'B'})");

{% endexercise %}




<!-- Exercise -->
{% exercise %}
Find the maximum of a two dimensional array <br>
- <u>Input</u>: Array of array of numbers (ex: <code>[ [1,6], [3,8], [5,6] ]</code> ) <br>
- <u>Output</u>: The maximum of everything (ex: <code>8</code> )

{% initial %}
function maxTwoDimArray(matrix) {
}

{% solution %}
function maxTwoDimArray(matrix) {
    var currentMax = 0;
    for (var row = 0; row < matrix.length; row++) {
        for (var col = 0; col < matrix[row].length; col++) {
            if (currentMax < matrix[row][col]) {
                currentMax = matrix[row][col];
            }
        }
    }
    return currentMax;
}

{% validation %}
assert(maxTwoDimArray([[42]]) === 42, "Fail for maxTwoDimArray([[42]])");
assert(maxTwoDimArray([ [1,6], [3,8], [5,6] ]) === 8, "Fail for maxTwoDimArray([ [1,6], [3,8], [5,6] ])");

{% endexercise %}





<!-- Exercise  -->
{% exercise %}
Build a triangle<br>
- <u>Input</u>: A number "n" (ex: <code>2</code>) <br>
- <u>Output</u>: An array of length "n", that contains an array of "*" with a size incrementing by one each time  (ex: <code>[ ["*"],["*","*"] ]</code>)<br>
Example output for 4:<br>
<code style="white-space: pre;">[
    ["*"],
    ["*","*"],
    ["*","*","*"],
    ["*","*","*","*"],
]</code>

{% initial %}
function buildTriangle(n) {
}

{% solution %}
function buildTriangle(n) {
  var res = [];
  for (var row = 0; row < n; row++) {
      res.push([]);
      for (var col = 0; col < row+1; col++) {
          res[row].push("*");
      }
  }
  return res;
}

{% validation %}
assert(buildTriangle(1).length === 1, "Fail for buildTriangle(1)");
assert(buildTriangle(5).length === 5, "Fail for buildTriangle(5)");
assert(buildTriangle(5) && buildTriangle(5)[3].length === 4, "Fail for buildTriangle(5)");
assert(buildTriangle(5) && buildTriangle(5)[3][3] === "*", "Fail for buildTriangle(5)");

{% endexercise %}








