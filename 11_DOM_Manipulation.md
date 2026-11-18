# 11 — DOM Manipulation

DOM stands for Document Object Model. The browser represents an HTML document as a tree of objects.

## Select elements

```javascript
const title = document.querySelector("#title");
const cards = document.querySelectorAll(".card");
```

## Change content and styles

```javascript
title.textContent = "Welcome to JavaScript";
title.style.color = "blue";
```

Use `textContent` for plain text. Avoid assigning untrusted user input to `innerHTML`, because it can introduce cross-site scripting (XSS) vulnerabilities.

## Change classes

```javascript
const panel = document.querySelector(".panel");

panel.classList.add("active");
panel.classList.remove("hidden");
panel.classList.toggle("expanded");
```

## Create and append an element

```javascript
const item = document.createElement("li");
item.textContent = "Learn DOM";
document.querySelector("#task-list").append(item);
```

## Example HTML

```html
<h1 id="title">Original title</h1>
<ul id="task-list"></ul>
<button id="change-button">Change title</button>
<script src="script.js" defer></script>
```

## Practice

Create a button that changes a heading's text when clicked. Add a new list item when another button is clicked.
