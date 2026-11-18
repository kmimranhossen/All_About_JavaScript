# 04 — Operators and Expressions

## Arithmetic operators

```javascript
let a = 10;
let b = 3;

console.log(a + b); // 13
console.log(a - b); // 7
console.log(a * b); // 30
console.log(a / b); // 3.333...
console.log(a % b); // 1
console.log(a ** b); // 1000
```

## Assignment operators

```javascript
let total = 10;
total += 5; // 15
total -= 2; // 13
total *= 2; // 26
```

## Comparison operators

```javascript
console.log(5 > 3);       // true
console.log(5 === "5");   // false
console.log(5 == "5");    // true (type coercion)
console.log(5 !== 4);     // true
```

Prefer strict equality (`===`) and strict inequality (`!==`) unless there is a clear reason not to.

## Logical operators

```javascript
const hasID = true;
const isAdult = true;

console.log(hasID && isAdult); // AND
console.log(hasID || isAdult); // OR
console.log(!hasID);           // NOT
```

## Ternary operator

```javascript
const age = 20;
const message = age >= 18 ? "Adult" : "Minor";
console.log(message);
```

## Practice

Write a program that takes two numbers and prints their sum, difference, product and remainder.
