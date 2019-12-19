# Logical Operator

1. 🥇What's the output of the following, write the output next to the code as comment.

* [ ] Logical AND operation

```js
true  && true; //true
true  && false; //false 
false && true; //false
false && false; //false
"foo" && "bar"; //"bar"
"bar" && "foo"; //"foo"
"foo" && "";  //""
""    && "foo"; //"foo"
" "   && "John" && "" && false //""
false && "Hey" && undefined //false
"undefined" && false && 42 //false
```

* [ ] Logical OR operation
```js
true  || true; //true
true  || false; //true
false || true; //true
false || false; //false
"foo" || "bar"; //"foo"
"bar" || "foo"; //"bar"
"foo" || ""; //"foo"
""    || "foo"; //""
" "   || "John" || "" || false //" "
false || "Hey" || undefined //"Hey"
"undefined" || false || 42 "undefined"
```

2. 🥈You have two variables i.e `isGuestOneVeg` and  `isGuestTwoVeg` according to the value using logical && and || opeartor do the following.

* [ ] If both are veg "Only offer up vegan dishes."
* [ ] At least one veg  "Make sure to offer up some vegan options."
* [ ] Else, "Offer up anything on the menu"
```js
let isGuestOneVeg = false;
let isGuestTwoVeg = false;
let message;
if (isGuestOneVeg && isGuestTwoVeg) {
    message = "Only offer up vegan dishes.";
} else if (isGuestOneVeg || isGuestTwoVeg) {
    message = "Make sure to offer up some vegan options.";
} else {
    message = "Offer up anything on the menu";
}
alert(message);
```


3. 🎖Using the variable `temperature` and logical operators do the following
* [ ] If temperature is less then 32 alert "It is freezing outside"
* [ ] If the temperature is greater then 110 alert "It is hot outside"
* [ ] else 'Go for it. It is pretty nice out'
```js
let temperature = 4;
let message;
if (temperature < 32) {
    message = "It is freezing outside";
} else if (temperature > 110) {
    message = "It is hot outside";
} else {
    message = "Go for it. It is pretty nice out";
}
alert(message);
```

4. 🎖 Output of this and the reason behind the output.
```js
alert( alert(1) || 2 || alert(3) );
```
<!-- It will alert 1 and then alert 2. Let's go from left to right. Before the outermost alert can execute, it must calculate its message's value. So, inside it's message block lies the code " alert(1) || 2 || alert(3) ".  When this inner code is executing, the alert(1) will first execute to get its return value. Hence, the user can see an alert with the number 1. When the value of that alert is returned as undefined, we then move on to the next item in the or condition. The next condition is 2, which is a truthy value. Since we search for the first truthy value in an or condition, 2 is returned as the value to the outer alert function. Hence, the user can then see an alert with the number 2.-->