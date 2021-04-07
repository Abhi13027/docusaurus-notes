---
title: Javascript Loops Advanced
---

### THINGS TO REMEMBER

_Suppose you want to keep the count of the numbers which are divisible by 7 between 50 to 100._

In such cases when you wish to do a count, you take a variable, you can name it anything, we will take counter for now and initialise it to 0. So basically `counter=0`. Now when you are doing a count of things, we basically make sure that as soon as are condition is met, we increment the counter variable. So For the above question

```jsx
var counter = 0;

for (var i = 50; i <= 100; i++) {
  if (i % 7 == 0) {
    counter++;
  }
}
console.log(counter);
```

### NESTED LOOPS

A nested loop is a one in which one loop is present inside another loop, one inner and the other one outer. The inner loop runs for every iteration of the outer loop.

```jsx
for (var i = 1; i <= 3; i++) {
  for (var j = 1; j <= 3; j++) {
    console.log(i, j);
  }
}

/* The output will be
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
*/
```

As you can see in the above example,

- When `i=1` for the outer loop, the inner loop runs completely for `j=1` `j=2` and `j=3`
- When `i=2` for the outer loop, the inner loop runs completely for `j=1` `j=2` and `j=3`
- When `i=3` for the outer loop, the inner loop runs completely for `j=1` `j=2` and `j=3`

### PATTERN PRINTING

We can print patterns with the help of nested loops. The limitation or one of the shortcomings of Javascript is that we cannot print a output in a single line with the help of `console.log` . We need to do some sort of manipulation to achieve that goal. So basically we concatenate string and print the resultant string as output.

So Suppose if you have to print the following output for `n=10`

```jsx
*
* *
* * *
* * * *
* * * * *
* * * * * *
* * * * * * *
* * * * * * * *
* * * * * * * * *
* * * * * * * * * *
```

The code will look like this

```jsx
var n = 10;
for (var i = 1; i <= n; i++) {
  var result = "";
  for (j = 1; j <= i; j++) {
    result += "* ";
  }
  console.log(result);
}
```

### PRIME CHECKING

```jsx
var isPrime = true;
for (var i = 2; i * i <= n; i++) {
  if (n % i == 0) {
    isPrime = false;
    break;
  }
}
if (isPrime) {
  console.log("Is Prime");
} else {
  console.log("Not a Prime");
}
```
