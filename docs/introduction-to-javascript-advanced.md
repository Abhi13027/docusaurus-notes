---
title: Introduction to Javascript Advanced
---

### Comments in Javascript

Comments in Javascript are generally used to give some extra information. The comments are not executed at all.

There are 2 types of comments -

- **Single line Comments**

  ```jsx
  var a; // this is a variable named a
  a = 10; // the varibale a has been assigned a value of 10
  ```

- **Multi line Comments**

  ```jsx
  /* Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum. */

  var a = 10;
  console.log(a);
  ```

### Variable Naming Conventions

The variables in Javascript should be named according to some rules

- The variable names should be in `Camel Case`

  ```jsx
  var myAge;
  var numOfStudents;
  ```

- The variable names should not start with a number. If a number is required in the front, then use and `underscore`

  ```jsx
  var 12name; // incorrect
  var _12name;
  ```

- The variable names are case sensitive.

  ```jsx
  var myAge;
  var myage;

  // The above are treated as 2 different variables
  ```

### Comparison Operators

- `==` - Equal to

  ```jsx
  10 == 10;
  ```

- `!=` - not Equal to

  ```jsx
  10 != 11;
  ```

- `>` - Greater than

  ```jsx
  9 > 8;
  ```

- `<` - less than

  ```jsx
  8 < 9;
  ```

- `>=` - Greater than or equal to

  ```jsx
  10 >= 7;
  ```

- `<=` - Less than or equal to

  ```jsx
  6 <= 8;
  ```

- `===` - Strict equal to

  ```jsx
  10 == "10";
  10 === "10";
  ```

- `!==` - Strict not equal to

  ```jsx
  10 != "10";
  10 !== "10";
  ```

### Assignment Operators

- `=` - Simple Assignment

  ```jsx
  var a;
  a = 2;
  ```

- `+=` - Add and assignment

  ```jsx
  var a = 1;
  a += 2;
  console.log(a);
  ```

- `-=` - Subtract and assignment

  ```jsx
  var a = 20;
  a -= 13;
  console.log(a);
  ```

- `*=` - multiply and assignment

  ```jsx
  var a = 2;
  a *= 7;
  console.log(a);
  ```

- `/=` - divide and assignment

  ```jsx
  var a = 6;
  a /= 2;
  console.log(a);
  ```

- `%=` - modulo and assignment

  ```jsx
  var a = 13;
  a %= 6;
  console.log(a);
  ```

### Logical Operators

- Logical `AND`

  ```jsx
  true && true;
  true && false;
  false && true;
  false && false;

  /* some examples of the same */
  var a = 2 < 3 && 5 == 5;
  console.log(a);

  var b = 3 > 1 && 5 > 6;
  console.log(b);

  var c = 1 == 2 && 2 == 2;
  console.log(c);

  var d = 1 == 2 && 1 == 2;
  console.log(d);
  ```

- Logical `OR`

  ```jsx
  true || true;
  true || false;
  false || true;
  false || false;

  /* some example of the same */
  var a = 2 < 3 || 5 == 5;
  console.log(a);

  var b = 3 > 1 || 5 > 6;
  console.log(b);

  var c = 1 == 2 || 2 == 3;
  console.log(c);

  var d = 1 == 2 || 1 == 1;
  console.log(d);
  ```

- Logical `NOT`

  ```jsx
  !true;
  !false;

  /* some examples of the same */
  var a = !(2 < 3);
  console.log(a);

  var b = !(!(2 > 3) || !(2 < 5));
  console.log(b);
  ```

---
