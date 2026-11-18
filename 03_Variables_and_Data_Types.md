# 03 — Variables and Data Types

## Variables

Variables store values for later use.

```javascript
let age = 21;
const country = "Bangladesh";
var oldStyle = "Avoid var in most modern code";
```

- `let`: use when the variable needs reassignment.
- `const`: use when the binding should not be reassigned.
- `var`: older function-scoped declaration; understand it, but prefer `let` and `const`.

`const` prevents reassignment, but objects and arrays declared with `const` can still be modified.

## Data types

JavaScript has primitive types and objects.

```javascript
const name = "Imran";       // string
const age = 21;             // number
const isStudent = true;     // boolean
const score = null;         // null
let result;                 // undefined
const big = 123456789n;     // bigint
const id = Symbol("id");    // symbol
const user = { name: "Imran" }; // object
```

## Check a type

```javascript
console.log(typeof "Hello"); // string
console.log(typeof 100);     // number
console.log(typeof true);    // boolean
```

Note: `typeof null` returns `"object"` for historical reasons.

## Naming rules

- Use meaningful names: `studentName`, not `x1`.
- Names are case-sensitive.
- A name cannot start with a number.
- Use camelCase by convention.

## Practice

1. Declare your name, age and student status.
2. Print each value and its type.
3. Try changing a `const` variable and observe the error.
