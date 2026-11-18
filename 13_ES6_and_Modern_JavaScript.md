# 13 — ES6 and Modern JavaScript

Modern JavaScript includes syntax and APIs that make code more expressive.

## let and const

```javascript
let score = 10;
score = 20;

const course = "JavaScript";
```

## Template literals

```javascript
const name = "Imran";
console.log(`Welcome, ${name}!`);
```

## Destructuring

```javascript
const user = { name: "Imran", age: 21 };
const { name, age } = user;

const colors = ["red", "green"];
const [firstColor, secondColor] = colors;
```

## Spread and rest

```javascript
const first = [1, 2];
const combined = [...first, 3, 4];

function sum(...numbers) {
  return numbers.reduce((total, number) => total + number, 0);
}
```

## Optional chaining and nullish coalescing

```javascript
const city = user.address?.city ?? "Unknown";
```

`?.` safely accesses a property when an earlier value may be nullish. `??` uses the fallback only for `null` or `undefined`.

## Modules

`math.js`:

```javascript
export const add = (a, b) => a + b;
```

`app.js`:

```javascript
import { add } from "./math.js";
console.log(add(2, 3));
```

In a browser, load the entry file with `<script type="module" src="app.js"></script>`. Node.js module configuration depends on the project setup.

## Practice

Create an array of objects, use destructuring to read a user's name, and use `map()` to create a list of names.
