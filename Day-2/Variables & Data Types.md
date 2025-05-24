---

## 📘 **Day 2: Variables & Data Types**

---

### 🔹 What is a Variable?

A **variable** is a container for storing data values.

In JavaScript, you can declare variables using:

* `let` – block-scoped, can be updated
* `const` – block-scoped, **cannot be reassigned**
* `var` – function-scoped (older, mostly avoided)

---

### ✅ Syntax Examples:

```javascript
let age = 25;       // can be reassigned
const name = "Alice"; // constant, cannot change
var city = "Dhaka";   // older syntax
```

---

### ❗ Difference Summary:

| Keyword | Can Reassign | Scope        | Hoisted |
| ------- | ------------ | ------------ | ------- |
| `let`   | ✅            | Block (`{}`) | ❌       |
| `const` | ❌            | Block        | ❌       |
| `var`   | ✅            | Function     | ✅       |

---

## 🔹 Data Types in JavaScript

There are **two categories**: **Primitive** and **Reference** types.

---

### ✅ Primitive Types:

| Type        | Example                      |
| ----------- | ---------------------------- |
| `Number`    | `42`, `3.14`                 |
| `String`    | `"hello"`, `'world'`         |
| `Boolean`   | `true`, `false`              |
| `Undefined` | declared but not assigned    |
| `Null`      | no value (manually set)      |
| `Symbol`    | unique identifier (advanced) |
| `BigInt`    | very large integers          |

```javascript
let score = 95; // Number
let username = "Alice"; // String
let isLoggedIn = true; // Boolean
let email; // Undefined
let data = null; // Null
```

---

### ✅ Reference Types (just a preview)

* Objects: `{ name: "John", age: 30 }`
* Arrays: `[1, 2, 3]`
* Functions: `function greet() {}`

---

## ✏️ Practice Tasks

Open your `script.js` file and try the following:

```javascript
let myName = "Bob";
const age = 20;
let isStudent = true;

console.log("Name:", myName);
console.log("Age:", age);
console.log("Is a student?", isStudent);

// Undefined and null
let job;
let salary = null;

console.log("Job:", job);      // undefined
console.log("Salary:", salary); // null
```

---

### 🎯 Bonus Challenge:

Try changing the value of a `const` variable. What happens?

```javascript
const country = "Bangladesh";
country = "India"; // ❌ This will cause an error
```

---

### 🧠 Mini Quiz

1. What is the difference between `let` and `const`?
2. What will this print?

   ```javascript
   let x;
   console.log(x);
   ```
3. Is `null` the same as `undefined`?

---

