---
title: Introduction to Javascript Advanced++
---

### Typeof Operator

`Typeof`

The typeof operator returns a string indicating the data type of the variable

```jsx
console.log(typeof 73); // number
console.log(typeof "Masai"); // string
console.log(typeof true); // boolean
console.log(typeof temp); // undefined
```

### Type Conversion

`Type Conversion`

The Javascript variables can be converted into different data types with the help of inbuilt Javascript functions.

- `Number()`

```jsx
var a = "21321";
console.log(Number(a));

var b = "221.3123";
console.log(Number(b));

var c = true;
console.log(Number(c));

var d = false;
console.log(Number(d));
```

- `String()`

```jsx
var a = 1231234;
console.log(String(a));

var b = true;
console.log(String(b));

var c = false;
console.log(String(c));
```

- `Boolean()`

```jsx
var a = 12312;
var b = "";

console.log(Boolean(a));
console.log(Boolean(b));
```

### String Concatenation

```jsx
// There is a difference between the following 4 strings
var myName1 = "Abhishek";
var myName2 = " Abhishek";
var myName3 = "Abhishek ";
var myName4 = "abhishek";

console.log(myName1 === myName2);
console.log(myName1 === myName3);
console.log(myName1 === myName4);

var firstName = "Abhishek";
var lastName = "Jain";

console.log(firstName + lastName);
```

### CODE FOR OJ

**FOR SINGLE INPUT**

```jsx
function runProgram(input) {
  var a = Number(input);
}

process.stdin.resume();
process.stdin.setEncoding("ascii");
let read = "";
process.stdin.on("data", function (input) {
  read += input;
});
process.stdin.on("end", function () {
  read = read.replace(/\n$/, "");
  runProgram(read);
});

process.on("SIGINT", function () {
  read = read.replace(/\n$/, "");
  runProgram(read);
  process.exit(0);
});
```

**FOR MULTIPLE INPUTS**

```jsx
function runProgram(input) {
  var newInput = input.split(" ");
  var a = Number(newInput[0]);
  var b = Number(newInput[1]);
}

process.stdin.resume();
process.stdin.setEncoding("ascii");
let read = "";
process.stdin.on("data", function (input) {
  read += input;
});
process.stdin.on("end", function () {
  read = read.replace(/\n$/, "");
  runProgram(read);
});

process.on("SIGINT", function () {
  read = read.replace(/\n$/, "");
  runProgram(read);
  process.exit(0);
});
```

---
