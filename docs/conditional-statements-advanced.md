---
title: Conditional Statements Advanced
---

### SWITCH STATEMENT

The switch statement evaluates an expression and executes code as a result of a matching case.

`Syntax`

```jsx
switch (expression) {
  case a:
    // perform the task in this particular case
    break;
  case b:
    // perform the task in this particular case
    break;
  case c:
    // perform the task in this particular case
    break;
  default:
  // perform te task
}
```

```jsx
var day = "Monday";

switch (day) {
  case "Monday":
    console.log("Today is the first day of the Week");
    break;
  case "Tuesday":
    console.log("Today is the second day of the Week");
    break;
  case "Wednesday":
    console.log("Today is the third day of the Week");
    break;
  case "Thursday":
    console.log("Today is the fourth day of the Week");
    break;
  case "Friday":
    console.log("Today is the fifth day of the Week");
    break;
  case "Saturday":
    console.log("Today is the sixth day of the Week");
    break;
  case "Sunday":
    console.log("Today is the seventh day of the Week");
    break;
  default:
    console.log("Please check your input");
}
```

### NESTED CONDITIONAL STATEMENTS

You can write a complex nested conditional statements as per your requirements.

```jsx
var a = 10;
var b = 12;

if (a != b) {
  if (a > b) {
    console.log("variable a is greater than variable b");
  } else {
    console.log("variable b is greater than variable a");
  }
} else {
  console.log("variable a is equal to variable b");
}
```

```jsx
var a = 30;

if (a % 2 == 0) {
  if (a % 3 == 0) {
    console.log("Number is divisible by 6");
  } else {
    console.log("Number is not divisible by 6");
  }
} else {
  console.log("Number is not divisible by 6");
}
```

```jsx
var age = 27;

if (age < 18) {
  console.log("You are not eligible for admission in Masai School");
} else {
  if (age <= 28) {
    console.log("You are eligible for admission in Masai School");
  } else {
    console.log("You are not eligible for admission in Masai School");
  }
}
```

### CODE FOR OJ & LOCAL

```jsx
function runProgram(input) {

}

if (process.env.USER === <Enter the User>) {
  runProgram(`Tuesday`);
} else {
  process.stdin.resume();
  process.stdin.setEncoding("ascii");
  let read = "";
  process.stdin.on("data", function (input) {
    read += input;
  });
  process.stdin.on("end", function () {
    read = read.replace(/\n$/, "");
    read = read.replace(/\n$/, "");
    runProgram(read);
  });
  process.on("SIGINT", function () {
    read = read.replace(/\n$/, "");
    runProgram(read);
    process.exit(0);
  });
}
```
