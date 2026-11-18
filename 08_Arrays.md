# 08 — Arrays

An array stores an ordered collection of values.

## Create an array

```javascript
const fruits = ["Apple", "Mango", "Banana"];

console.log(fruits[0]); // Apple
console.log(fruits.length); // 3
```

Array indexes start at zero.

## Common methods

```javascript
const numbers = [1, 2, 3];

numbers.push(4);    // add at end
numbers.pop();      // remove from end
numbers.unshift(0); // add at start
numbers.shift();    // remove from start
```

## Useful iteration methods

```javascript
const values = [1, 2, 3, 4];

const doubled = values.map(value => value * 2);
const even = values.filter(value => value % 2 === 0);
const total = values.reduce((sum, value) => sum + value, 0);

console.log(doubled, even, total);
```

## Find an item

```javascript
const users = ["Asha", "Imran", "Rafi"];

console.log(users.includes("Imran"));
console.log(users.find(user => user.startsWith("R")));
```

## Important

Methods such as `map()`, `filter()` and `slice()` return new arrays. Methods such as `push()`, `pop()`, `sort()` and `splice()` mutate the original array.

## Practice

1. Create an array of five favorite foods.
2. Find the largest number in an array.
3. Use `filter()` to keep only numbers greater than 10.
