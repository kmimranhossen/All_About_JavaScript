# 14 — Asynchronous JavaScript and APIs

Asynchronous JavaScript allows work to continue without blocking the main flow while waiting for operations such as network requests.

## setTimeout

```javascript
console.log("Start");

setTimeout(() => {
  console.log("Runs later");
}, 1000);

console.log("End");
```

## Promise

A Promise represents the eventual completion or failure of an asynchronous operation.

```javascript
const task = new Promise((resolve, reject) => {
  const success = true;

  if (success) {
    resolve("Task completed");
  } else {
    reject(new Error("Task failed"));
  }
});

task
  .then(result => console.log(result))
  .catch(error => console.error(error));
```

## async and await

```javascript
async function getData() {
  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/users");

    if (!response.ok) {
      throw new Error(`HTTP error: ${response.status}`);
    }

    const users = await response.json();
    console.log(users);
  } catch (error) {
    console.error("Could not load users:", error);
  }
}

getData();
```

## What is an API?

An API (Application Programming Interface) defines how software systems communicate. A web API commonly sends data over HTTP, often as JSON.

## Important HTTP methods

- `GET` — retrieve data
- `POST` — create or submit data
- `PUT` — replace a resource
- `PATCH` — partially update a resource
- `DELETE` — remove a resource

## Practice

Use `fetch()` to request sample users from JSONPlaceholder. Display each user's name on a web page and handle errors.
