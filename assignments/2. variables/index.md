1. In code below "Mark" is a string.  What is name?
```js
var name = "Mark";
```
name is a variable

2. Find the error if any
```js
  var product cost = 3.45;
```
Variable name cannot have space in between

3. Write `Right or Wrong` next to the code below.

```js
  "Hello World" // Right
  'Hello World" // Wrong
  "Hello World' // Wrong
  'Hello World' // Right
```

## Write `VALID` and `INVALID` infront of the variable name defined below
```js
var man; // VALID
var 1girl; //INVALID
var woman3; // VALID
var -girl; // INVALID
var blackDog; // VALID
var 42; // INVALID
var $42; // VALID
var userName; // VALID
var x, y, z; // VALID
var x = 5, y = 6, z = 7; // VALID
var x = 5 + 10 + 2; // VALID
```

## Basic Operations

Mathematical Operations:

Solve this using mathematical operations. (+, -, *, / , etc)

```js
var amount = 2080;
// Define a new variable and store the value that is 80 less then the value of amount.
var n1 = amount - 80;

// Define a new variable and store the value that is 200 more then the value of amount.
var n2 = amount + 200;

// Define a new variable and store the value that is 4 times the value of amount.
var n3 = amount * 4;

// Define a new variable and store the reminder when the value of amount is  divided by 21.
var n4 = amount % 21;
```

Logical Operation:

Solve this using logical operations. (<, >, &&, ||)

```js
var johnAge = 45;
var markAge = 35;

// Check who is older eithe John or Mark
var older = Math.max(johnAge, markAge);
// Check who is younger
var younger = Math.min(johnAge, markAge);
// Check if their age is equal
var isEqual = johnAge == markAge;
// Create a new variable and assign the age of john to new variable.
var newJohn = johnAge;
// Check if john is equal to or greater then mark.
var equalOrGreaterThan = johnAge >= markAge;
// Check if john is less then or equal to mark.
var equalOrGreaterThan = johnAge <>= markAge;

// Calculate the average age of john and mark and assign to a new variable.
var averageAge = (johnAge + markAge) / 2;
```