# 16 — JavaScript Interview and Practice

## Beginner questions

### 1. What is JavaScript?

JavaScript is a programming language used to create interactive web experiences and applications.

### 2. What is the difference between let, const and var?

`let` and `const` are block-scoped. `var` is function-scoped. `const` prevents reassignment of the binding.

### 3. What are primitive data types?

String, Number, BigInt, Boolean, Undefined, Null and Symbol.

### 4. What is the difference between == and ===?

`==` performs type coercion in many comparisons. `===` compares without that coercion.

### 5. What is an array?

An ordered collection of values.

## Intermediate questions

### 6. What is a function?

A reusable block of code that can accept inputs and return a result.

### 7. What is the DOM?

The Document Object Model is the browser's object representation of an HTML document.

### 8. What is an event listener?

A function registered to run when a specified event occurs.

### 9. What is a Promise?

An object representing the eventual success or failure of an asynchronous operation.

### 10. What is async/await?

Syntax that makes Promise-based asynchronous code easier to read and write.

### 11. What is the difference between map() and forEach()?

`map()` returns a new array containing transformed values. `forEach()` runs a callback for each item and returns `undefined`.

### 12. What is JSON?

JavaScript Object Notation is a text format commonly used to exchange structured data.

## Practice tasks

1. Reverse a string.
2. Find the largest number in an array.
3. Check whether a number is even or odd.
4. Count vowels in a string.
5. Remove duplicate values from an array.
6. Create a simple calculator function.
7. Fetch data from a public API.
8. Add and remove DOM elements with event listeners.

## Mini quiz

**Q1. Which keyword declares a block-scoped variable that can be reassigned?**

A. `const`  
B. `let`  
C. `static`

**Q2. Which method creates a new array by transforming each item?**

A. `map()`  
B. `pop()`  
C. `push()`

**Q3. Which keyword is used to declare an asynchronous function?**

A. `await`  
B. `async`  
C. `promise`

**Answers:** 1-B, 2-A, 3-B.

## Final challenge

Build a responsive To-Do application. Add tasks, mark them complete, delete them and persist them using `localStorage`. Include clear empty and error states.
