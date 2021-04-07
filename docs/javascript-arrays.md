---
title: Javascript Arrays
---

### ARRAYS

An arrays is basically a special variable which can hold more than one value at at time. Array in simple language means a list of information. This is very useful when working with large datasets.

`Syntax`

```jsx
var arr_name = [item_1, item_2, item_3, ....];
```

`Example`

```jsx
var arr = [17, 21, 1, 13, 19];

var arr1 = ["banana", "oranges", "papaya", "apple"];

var arr2 = [true, false, false, true];
```

### Why Do We need Arrays

Suppose you have to declare five variables. Earlier what you were doing is the following

```jsx
var a = 12;
var b = 23;
var c = 324;
var d = 3424;
var e = 1729;
```

When the number of variables increases, it becomes cumbersome to first name the variable as well as write the same thing again and again.

In order to resolve that we can use arrays, the same thing can be written in a short syntax

```jsx
var arr = [12, 23, 324, 3424, 1729];
```

You need to remember the following things about arrays -

- The array is a contiguous block of memory

  When you declare a variable, a random memory is allocated to variable, and the value associated with that particular variable is stored at the memory location. But in case of arrays, a continuous block of memory is allocated to the array, and the elements are thus stored in the array at continuous positions.

- The Array starts from index 0

  The array stores elements in contiguous form. The starting position of the array is marked as zero. So taking the above example only, suppose we need to access the variables

  ```jsx
  var arr = [12, 23, 324, 3424, 1729];

  console.log(ar[0]); // 12
  console.log(ar[1]); // 23
  console.log(ar[2]); // 324
  console.log(ar[3]); // 3424
  console.log(ar[4]); // 1729
  ```

- The Array can hold multiple data types

  Unlike other programming languages, you don't need to have just one data type in the array. It can contain multiple data-types also

  ```jsx
  var arr = ["Abhishek", 26, true];
  ```

- The Array size is dynamic
  Unlike other programming languages, you don't need to have a fixed size of the array. The array size can be increased and decreased at any point of time.

### METHODS IN ARRAYS

`push()`
The push method takes into input an element, the item then gets added to array at last position

```jsx
var arr = [1, 2342, 43];
arr.push(1729);

console.log(arr);
// [1, 2342, 43, 1729]
```

`pop()`
The pop method removes the last element from the array

```jsx
var arr = [1, 23, 432, 4324];
arr.pop();

console.log(arr);
// [1, 23, 432]
```

### PROPERTY IN ARRAYS

`length`
The length property gives the number of elements present in the array

```jsx
var arr = [2134, 4134, 3241, 213];
console.log(arr.length);
```

### SOME INBUILT FUNCTIONS

We can use some inbuilt functions present in Javascript

`Math.ceil()`
Takes into argument a number and returns the integer which is just bigger than the number.

```jsx
Math.ceil(1.7); // 2
Math.ceil(2.1); // 3
Math.ceil(-2.5); // -2
```

`Math.floor()`
Takes into argument a number and returns the integer which is just smaller than the number.

```jsx
Math.floor(1.7); // 1
Math.floor(2.1); // 2
Math.floor(-2.5); // -3
```

### SPLIT METHOD

The split() method is used to split a string into an array of substrings

```jsx
var input = `21 321 3213 3213 321`;
var data = input.split(" ");

console.log(data);
// [ '21', '321', '3213', '3213', '321' ]
```

### OJ

```jsx
function runProgram(input) {
  var newInput = input.split(/[\r\n]+/);
  var length = Number(newInput[0]);
  var data = newInput[1].split(" ").map(Number);

  /* Write your code here */
}

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
```
