---
title: Javascript Loops
---

Loops in Javascript are used to repeatedly run a set of instructions. A loop will continue running until the defined condition returns false or true depending on our requirement.

There are 2 types of loops

1. Counter Loops (For Loops)
2. Conditional Loops (While Loops)

### While Loop

Lets say we wanted to run a piece of code multiple times. We could write out duplicate code multiple times but loops save us a lot of time and make our code efficient!

For example, let’s say we wanted to print "Hello World!" 100 times. It would be impractical to write `console.log("Hello World!")` 100 times.

This is where loops are useful.

Example:

```jsx
var i = 0;

while (i < 100) {
  console.log("Hello World!");
  i++;
}
```

The above code prints `Hello World!` 100 times, try it out for yourself!

_How does it work?_

The loop in the code is called a while loop. It can execute a block of code as long as a specified condition is `true`.

In the above example the while loop prints `Hello World!` until `i == 100`.

Notice the line `i++`. This is another simpler way of doing `i = i + 1`. You can also do `i--` which is a simpler way of doing `i = i - 1`.

Once i is equal to 100 the loop **breaks** and stops executing the code within.

### For loop

The next kind of loop in JavaScript is a for loop.

Example:

```jsx
for (var i = 0; i < 100; i++) {
  console.log("Hello World!");
}
```

This again prints `Hello World!` 100 times. For loops work in much the same way as while loops.

`i < 100` represents the limit condition, after which the loop stops executing.

### BREAK

Break statements are used to come out of the loop.

```jsx
var i = 1;

while (true) {
  console.log("Hello World");
  i++;
}
```

The above loop will run infinitely, because in the while loop we have written the condition that run it always, so in order to come out of the loop, we can check for a condition and then break it. For eg.

```jsx
var i = 1;

while (true) {
  if (i == 10) {
    break;
  }
  console.log("Hello World");
  i++;
}
```

### CONTINUE

Continue statement is used to skip one iteration of the loop

```jsx
for (var i = 1; i <= 5; i++) {
  console.log(i);
}
```

The output will be

`1`

`2`

`3`

`4`

`5`

But if we use continue, such as in the following example

```jsx
for (var i = 1; i <= 5; i++) {
  if (i == 3) {
    continue;
  }
  console.log(i);
}
```

The output will be

`1`

`2`

`4`

`5`
