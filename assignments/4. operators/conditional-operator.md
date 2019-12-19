## If Statement
1.  🎖Make a simple calculator with these functions. Using prompt, type conversion, if else statement. Use prompt to take the input from user i.e two numbers and an operation (Add, Sub, Mul, Div).

  ⛑ Rule
    * [ ] While substracting and dividing keep in mind the number one should be greater then number two. If not show alert saying `Number Two is larger then Number one`.
  ⚡️ Operations
    * [ ] Add
    * [ ] Sub
    * [ ] Mul
    * [ ] Div

```js
let n1 = +prompt("Enter first number");
let n2 = +prompt("Enter second number");
let operation = prompt("Choose operation\n\n1 Add\n2 Sub\n3 Mul\n4 Div");
let message;
switch (operation) {
	case "1":
		message = `Sum is ${n1 + n2}`;
		break;
	case "2":
        message = n1 < n2 ? "Number Two is larger then Number one" : `Difference is ${n1 - n2}`;
		break;
	case "3":
		message = `Product is ${n1 * n2}`;
		break;
	case "4":
		message = n1 < n2 ? "Number Two is larger then Number one" : `Quotient is ${n1 / n2}`;
		break;
	default:
		message = "Invalid operation";
		break;
}
alert(message);

```

2. 🎖Write a if else statement which checks if the status is single `console.log` the message `John is single` or else `John is married`
```js
var firstName = 'John';
var status = 'single';
console.log(`${firstName} is ${status == 'single' ? 'single' : 'married'}`);
```

3. 🎖Write a JavaScript program that takes two `integers` from user (using prompt) and alerts the larger number.
```js
let n1 = +prompt("Enter first number");
let n2 = +prompt("Enter second number");
alert(Math.max(n1, n2));
```

4. 🎖Write a JavaScript conditional statement to find the sign (+, -) of product of three numbers. Take those three numbers from user using `prompt`. Display an alert box with the specified sign.

```js
let n1 = +prompt("Enter first number");
let n2 = +prompt("Enter second number");
let n3 = +prompt("Enter third number");
let product = n1 * n2 * n3;
alert(product < 0 ? "-" : "+");
```

## Switch Statement

1. 🎖Using switch statement do the following

Take a number value from user and alert the message if it matches the conditions.
* [ ] ONE, if `number` is equal to 1.
* [ ] TWO, if `number` is equal to 2.
* [ ] THREE, if `number` is equal to 3.
* [ ] FOUR, if `number` is equal to 4.
* [ ] FIVE, if `number` is equal to 5.
* [ ] SIX, if `number` is equal to 6.
* [ ] SEVEN, if `number` is equal to 7.
* [ ] EIGHT, if `number` is equal to 8.
* [ ] NINE, if `number` is equal to 9.
* [ ] PLEASE TRY AGAIN, if  is none of the above.
```js
let num = +prompt("Enter number");
let message;
switch (num) {
	case 1:
		message = "ONE";
		break;
	case 2:
		message = "TWO";
		break;
	case 3:
		message = "THREE";
		break;
	case 4:
		message = "FOUR";
		break;
	case 5:
		message = "FIVE";
		break;
	case 6:
		message = "SIX";
		break;
	case 7:
		message = "SEVEN";
		break;
	case 8:
		message = "EIGHT";
		break;
	case 9:
		message = "NINE";
		break;
	default:
		message = "PLEASE TRY AGAIN";
		break;
}
alert(message);
```

2. 🎖Using switch statement do the following

Take the value of `marks` (0-100) from user using `prompt` and `alert` the message (Your Grade is AA) as giver below.
* [ ] `AA` if `marks` is greater than 90.
* [ ] `AB` if `marks` is greater than 80 and less than or equal to 90
* [ ] `BB` if `marks` is greater than 70 and less than or equal to 80
* [ ] `BC` if `marks` is greater than 60 and less than or equal to 70
* [ ] `CC` if `marks` is greater than 50 and less than or equal to 60
* [ ] `CD` if `marks` is greater than 40 and less than or equal to 50
* [ ] `DD` if `marks` is greater than 30 and less than or equal to 40
* [ ] `FF` if `marks` is less than or equal to 30
```js
let marks = +prompt("Enter marks");
let grade;
if (marks > 90) {
  grade = "AA";
} else if (marks > 80) {
  grade = "AB";
} else if (marks > 70) {
  grade = "BB";
} else if (marks > 60) {
  grade = "BC";
} else if (marks > 50) {
  grade = "CC";
} else if (marks > 60) {
  grade = "CD";
} else if (marks > 30) {
  grade = "DD";
} else {
  grade = "FF";
}
alert(grade);
```
