# 02 — JavaScript Setup and Console

## What do you need?

- A code editor such as Visual Studio Code.
- A modern web browser.
- Node.js (optional, for running JavaScript outside the browser).

## Browser console

1. Open a web page.
2. Press `F12` or `Ctrl + Shift + J` in Chrome.
3. Open the Console tab.
4. Type:

```javascript
console.log("Hello!");
```

## Useful console methods

```javascript
console.log("Normal message");
console.warn("Warning message");
console.error("Error message");
console.table([{ name: "Imran", role: "Student" }]);
```

## Run a JavaScript file with Node.js

Save this as `app.js`:

```javascript
console.log("JavaScript running with Node.js");
```

Run it from the terminal:

```bash
node app.js
```

## Comments

```javascript
// Single-line comment

/*
  Multi-line
  comment
*/
```

## Practice

Create `app.js`, print three messages and display one warning using `console.warn()`.
