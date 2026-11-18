# 06 — Loops

Loops repeat code while a condition is satisfied or for each item in a collection.

## for loop

```javascript
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

## while loop

```javascript
let count = 1;

while (count <= 5) {
  console.log(count);
  count++;
}
```

## do...while loop

```javascript
let number = 1;

do {
  console.log(number);
  number++;
} while (number <= 3);
```

A `do...while` loop runs its body at least once.

## for...of

Use it to iterate over iterable values such as arrays and strings.

```javascript
const fruits = ["Apple", "Mango", "Banana"];

for (const fruit of fruits) {
  console.log(fruit);
}
```

## break and continue

```javascript
for (let i = 1; i <= 5; i++) {
  if (i === 3) continue;
  if (i === 5) break;
  console.log(i);
}
```

## Practice

1. Print numbers from 1 to 100.
2. Print the multiplication table of 5.
3. Calculate the sum of numbers from 1 to 10.
