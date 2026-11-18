# 09 — Objects

Objects store data as key-value pairs.

## Create an object

```javascript
const student = {
  name: "Imran",
  department: "CSE",
  semester: 3,
  isActive: true
};

console.log(student.name);
console.log(student["department"]);
```

## Add, update and delete properties

```javascript
student.university = "IUBAT";
student.semester = 4;
delete student.isActive;
```

## Methods

A method is a function stored as an object property.

```javascript
const user = {
  name: "Imran",
  greet() {
    return `Hello, I am ${this.name}`;
  }
};

console.log(user.greet());
```

## Destructuring

```javascript
const { name, department } = student;
console.log(name, department);
```

## Object iteration

```javascript
for (const [key, value] of Object.entries(student)) {
  console.log(key, value);
}
```

## Practice

Create a product object with `name`, `price`, `category` and a method that returns a short product description.
