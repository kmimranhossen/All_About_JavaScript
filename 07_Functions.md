# 07 — Functions

A function is a reusable block of code designed to perform a task.

## Function declaration

```javascript
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet("Imran"));
```

## Function expression

```javascript
const add = function (a, b) {
  return a + b;
};

console.log(add(5, 3));
```

## Arrow function

```javascript
const multiply = (a, b) => a * b;

console.log(multiply(4, 5));
```

## Parameters and arguments

- Parameters are names listed in the function definition.
- Arguments are actual values passed when calling the function.

## Default parameters

```javascript
function welcome(name = "Guest") {
  return `Welcome, ${name}`;
}
```

## Scope

Variables declared with `let` and `const` are block-scoped. A function can access variables from its outer lexical scope.

```javascript
const course = "JavaScript";

function showCourse() {
  const level = "Beginner";
  console.log(course, level);
}
```

## Practice

1. Write a function that returns the square of a number.
2. Write a function that checks whether a number is even.
3. Create an arrow function that converts Celsius to Fahrenheit.
