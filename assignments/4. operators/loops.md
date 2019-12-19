1. 🎖 Write a program to calculate the total price of your phone purchase. With these conditions
 * [ ] You will keep purchasing phones (hint: loop!) until you run out of bank balance.
 * [ ] You'll also buy accessories for each phone as long as your purchase amount is below your spending threshold.
 * [ ] After you've calculated your purchase amount, add in the tax, then print out the calculated purchase amount, properly formatted.
 * [ ] Finally, check the amount against your bank account balance to see if you can afford it or not.
 * [ ] Write a function called calculateTax which takes an argument 'amount' and calculates the tax you need to pay.
 * [ ] Write a function named formatAmount which returns you amount in this format '$ 132.45' make the decimal fixed to 2 places.
```js
const SPENDING_THRESHOLD = 200;
const TAX_RATE = 0.08;
const PHONE_PRICE = 99.99;
const ACCESSORY_PRICE = 9.99;

let calculateTax = amount => amount * TAX_RATE;
let formatAmount = amount => `$ ${amount.toFixed(2)}`;

var bank_balance = 303.91;
var amount = 0;
let phoneCount = 0;
// keep adding phones till the bank balance allows us
while (amount + PHONE_PRICE < bank_balance) {
	amount += PHONE_PRICE;
	phoneCount++;
}
// calculate amount of indvidual phone to check it doesn't cross the threshold
let singlePhoneAmount = PHONE_PRICE;
// check that adding one accessory to each phone does not make the amount exceed bank balance
while ((amount + (ACCESSORY_PRICE * phoneCount)) <= bank_balance) {
    //check if single phone amount doesn't cross threshold
	if (singlePhoneAmount + ACCESSORY_PRICE > SPENDING_THRESHOLD) {
		break;
	}
	singlePhoneAmount += ACCESSORY_PRICE;
	amount += ACCESSORY_PRICE * phoneCount;
}
amount += calculateTax(amount);
console.log(formatAmount(amount));
```
 ⛑ Answer of the above will `$334.76`.

2. 🎖 Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen using `alert` (e.g. "2 is even").
```js
for (let i = 0; i <= 20; i++) {
    alert(`${i} is ${i % 2 == 0 ? "even" : "odd"}`)
}
```

3. 🎖Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result in console (e.g. "2 * 9 = 18").
```js
for (let i = 0; i <= 10; i++) {
    alert(`${i} * 9 = ${i * 9}`)
}
```

4. 🎖Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).
(e.g.
"1 * 1 = 1"
"1 * 2 = 2"
"1 * 3 = 3"
"1 * 4 = 4"
.... for all 100 results)
```js
for (let i = 1; i <= 10; i++) {
    for (let j = 1; j <= 10; j++) {
        alert(`${i} * ${j} = ${i * j}`);
    }
}
```

5. 🎖Show the following output using one loop.
```js
// 1, 2, 3, 4, 5
// 6, 7, 8, 9, 10

let message = "";
for (let i = 1; i <= 10; i++) {
    message += i;
    if (i == 5 || i == 10) {
        message += "\n";
    } else {
        message += ", ";
    }
}
console.log(message);
```

6. 🎖Use a while loop to add up the numbers 1 to 20.
```js
let index = 1;
let sum = 0;
while (index <= 20) {
    sum += index++;
}
console.log(sum);
```

7. 🎖Use a while loop to print out the even number from 1 to 20. (You'll need Modulus for this. And an IF Statement.)
```js
let index = 1;
while (index <= 20) {
    if (index % 2 == 0) {
        console.log(index);
    }
    index++;
}
```
