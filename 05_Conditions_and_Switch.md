# 05 — Conditions and Switch

Conditions allow a program to make decisions.

## if, else if and else

```javascript
const marks = 82;

if (marks >= 80) {
  console.log("Grade A+");
} else if (marks >= 70) {
  console.log("Grade A");
} else if (marks >= 60) {
  console.log("Grade A-");
} else {
  console.log("Keep practicing");
}
```

## switch

```javascript
const day = "Monday";

switch (day) {
  case "Friday":
    console.log("Weekend");
    break;
  case "Monday":
    console.log("Start of the week");
    break;
  default:
    console.log("Regular day");
}
```

Use `break` to prevent execution from falling through to the next case when that is not intended.

## Truthy and falsy values

Falsy values include `false`, `0`, `-0`, `0n`, `""`, `null`, `undefined` and `NaN`. Most other values are truthy, including empty arrays and empty objects.

```javascript
const username = "";

if (username) {
  console.log("Username provided");
} else {
  console.log("Please enter a username");
}
```

## Practice

1. Check whether a number is positive, negative or zero.
2. Check whether a person is eligible to vote based on an age value.
3. Use `switch` to print a message for a selected weekday.
