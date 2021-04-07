---
title: Conditional Statements
---

Conditional statements basically evaluates whether the condition is `true` or `false` and based on that performs the task given.

### IF STATEMENT

`Syntax`

```jsx
if(condition to be true){
	// perform the task given in the following block
}
```

`Examples`

```jsx
var a = 10;

if (a > 5) {
  a = 4;
}

console.log(a);
```

```jsx
var a = 1729;

if (a === 1729) {
  console.log("The number is a Ramanujan number");
}
```

```jsx
var a = false;
if (!a) {
  console.log("Hello World");
}
```

### ELSE STATEMENT

Optionally with the if statements, you can add something called as the `else` statement. The else statements gets executed when the `if` condition evaluates to false

`Syntax`

```jsx
if(condition to be true){
	// perform the task in if block
}else {
	// perform the task in else block
}
```

`Examples`

```jsx
var a = 10;

if (a > 10) {
  console.log("a is greater than 10");
} else {
  console.log("a is less than or equal to 10");
}
```

```jsx
var myName = "Abhisek";

if(myName == "Abhishek"){
	console.log("My name is correctly typed";
}else{
	console.log("Please type my name correctly")
}
```

`Note` - The else statement cannot be independently executed. But the if statements can be executed independently without the else statements.

### ELSE-IF STATEMENT

Just like you have an additional option of `else` statement with `if` statement, you also have an `else if` statement.

The difference between the two is that, `else` automatically gets evaluated if the condition in `if` statement gets evaluated to false while in case of `else if`, you need to check the condition.

`Syntax`

```jsx
if( condition to be true){
	// perform the task in this block
}
else if (condition to be true){
	// perform the task in this block
}

```

`Examples`

```jsx
var a = 10;

if (a > 15) {
  console.log("a is greater than 15");
} else if (a < 12) {
  console.log("a is less than 12");
} else {
  console.log("a is between 12 and 15");
}
```

### THINGS TO REMEMBER

When you write `if` statements, the Javascript Engine checks all the conditions.

```jsx
var a = 10;

if (a > 5) {
  console.log("a is greater than 5");
}

if (a > 6) {
  console.log("a is greater than 6");
}

if (a > 7) {
  console.log("a is greater than 7");
}
```

```jsx
var a = 10;

if (a > 5) {
  console.log("a is greater than 5");
} else if (a > 6) {
  console.log("a is greater than 6");
} else if (a > 7) {
  console.log("a is greater than 7");
}
```
