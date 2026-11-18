# 12 — Events and Event Handling

Events are actions or occurrences that the browser can detect, such as clicks, typing and form submission.

## addEventListener()

```javascript
const button = document.querySelector("#my-button");

button.addEventListener("click", () => {
  console.log("Button clicked!");
});
```

## Event object

```javascript
document.querySelector("#name-input").addEventListener("input", event => {
  console.log(event.target.value);
});
```

## Form submission

```javascript
const form = document.querySelector("#signup-form");

form.addEventListener("submit", event => {
  event.preventDefault();

  const formData = new FormData(form);
  const email = formData.get("email");

  console.log(email);
});
```

`preventDefault()` prevents the browser's default action for that event.

## Event bubbling and delegation

Events usually bubble from the target through ancestor elements. Delegation lets a parent handle events from its children.

```javascript
document.querySelector("#task-list").addEventListener("click", event => {
  if (event.target.matches(".delete-button")) {
    event.target.closest("li")?.remove();
  }
});
```

## Common events

- `click`
- `input`
- `change`
- `submit`
- `keydown`
- `keyup`
- `mouseover`
- `DOMContentLoaded`

## Practice

Build a counter with increment and decrement buttons. Update the displayed value after each click.
