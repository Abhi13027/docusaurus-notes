---
title: Introduction to Javascript
---

## Fundamentals to Unix

### What is command Line ?

There are 2 ways in which you can interact with a computer. One is the graphical User interface (GUI) and the other is the Command Line Interface (CLI). Once you get comfortable with the commands, you will realise it is a very powerful and faster way of interacting with the computer. The name “bash” is an acronym for `Bourne Again Shell`

### What is a shell ?

The shell is a sort of a program which takes into input the keyboard commands and passes them onto the operating system to carry out the required operations. Almost all Linux distributions supply a shell program from the GNU Project called bash.

> In command line terms, folders are called directories

We will learn few commands to begin our journey -

`ls` - lists all the files in the current directory

```jsx
ls;
ls - a;
ls - S;
ls - l;
```

`cd` - change directory

```jsx
cd
cd ..
cd ../..
cd ~/Desktop/
```

`pwd` - to print working directory path

```jsx
pwd;
```

`rm` - to remove a file or a directory

```jsx
rm <file_name>
rm -r <folder_name>
```

`mkdir` - to make/create a directory

```jsx
mkdir masai
```

`touch` - to create a file

```jsx
touch app.js
```

`echo` - display a line of text/string on standard output or a file

```jsx
echo "My name is Abhishek Jain" > app.js
echo "I am from Kota Rajasthan" >> app.js
```

`cat` - to see the contents of the file

```jsx
cat app.js
```

`cp` - Copy the file/folder from one place to another

```jsx
cp <src_file> <destination file_name or destination folder>
cp a.txt b.txt
```

`mv` - Cut the file/folder from one place to another

```jsx
mv <src file/folder> <destination file or folder>
```

## Introduction to Javascript

### What is Programming ?

Programming is the way to give instructions to a machine to get the required work done. The computer doesn't understand the vocal languages like we do. Machines understand the language which consists of 0's and 1's. This language which consists of only 0's and 1's is called as the machine level language. The programming languages are divided into 2 types

1. High Level Language
2. Low Level Language

### Why Javascript ?

There are so many languages that a person can learn. Like Hindi, English, Gujarati, Marathi, Marwari etc. So you chose a language which basically fulfills your requirements. Similarly there are so many languages that are available in the market to learn, but you will try to learn only that one which is as per your requirement. So why Javascript ? Earlier Javascript was only used in the for DOM manipulation because it was

### Different Data Types in Javascript

There are various data types in JS, but for now we will learn about the following 3 ones

- **Numbers**

  The numbers data type is used to hold any type of number.

  ```jsx
  3.143142; // Floating point numbers
  5; // Integers
  ```

- **Strings**

  The strings data type is used to hold any type of textual data

  ```jsx
  "Abhishek Jain";
  "masai school";
  "1231";

  ```

- **Boolean**

  The boolean data type is used to hold 2 type of value, `true` or `false`

  ```jsx
  true;
  false;
  ```

- **Undefined**

  The undefined data type is used to represent when something is not defined.

  ```jsx
  undefined;
  ```

### Variables in Javascript

Just like you have encountered a variable in algebra, almost similar is the concept of variables in Javascript. A variable thus means anything that can vary. You can imagine it like a box that contains a certain value. The process generally comprises of 2 parts.

1. Variable Declaration
2. Variable Assignment

### Different Operators in Javascript

There are various operators in Javascript

- **Addition**

```jsx
var a = 10;
var b = 20;

console.log(a + b);
```

- **Subtraction**

```jsx
var a = 10;
var b = 20;

console.log(a - b);
```

- **Multiplication**

```jsx
var a = 10;
var b = 20;

console.log(a * b);
```

- **Division**

```jsx
var a = 10;
var b = 20;

console.log(a / b);

// when b = 0;
```

- **Modulus (Remainder)**

```jsx
var a = 10;
var b = 8;

console.log(a % b);
```

- **Increment**

```jsx
var a = 10;
a++;

console.log(a);
```

- **Decrement**

```jsx
var a = 10;
a--;

console.log(a);
```

- **Exponential**

```jsx
var a;
a = 3 ** 2;
console.log(a);
```

---
