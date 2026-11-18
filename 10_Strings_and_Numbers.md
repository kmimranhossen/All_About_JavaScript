# 10 — Strings and Numbers

## Strings

Strings represent text.

```javascript
const firstName = "K M Imran";
const greeting = `Hello, ${firstName}!`;

console.log(greeting);
```

Template literals use backticks and support `${expression}` interpolation.

## Useful string methods

```javascript
const text = "  Learn JavaScript  ";

console.log(text.length);
console.log(text.trim());
console.log(text.toUpperCase());
console.log(text.toLowerCase());
console.log(text.includes("JavaScript"));
console.log(text.replace("Learn", "Practice"));
console.log(text.slice(0, 5));
```

Strings are immutable: string methods return new strings rather than changing the original.

## Numbers

```javascript
const price = 125.567;

console.log(price.toFixed(2)); // "125.57"
console.log(Number("42"));     // 42
console.log(Number("hello"));  // NaN
console.log(Number.isNaN(Number("hello"))); // true
console.log(Number.isInteger(10)); // true
```

`toFixed()` returns a string. Be aware that floating-point arithmetic can produce precision surprises.

## Convert values

```javascript
const value = "100";
const numberValue = Number(value);
const textValue = String(numberValue);

console.log(numberValue, textValue);
```

## Practice

1. Convert a name to uppercase.
2. Remove spaces from the beginning and end of a string.
3. Convert `"250"` into a number and add 50.
