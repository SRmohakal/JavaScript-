---

## 📘 **Functions in JavaScript**

Functions allow you to **group code** and **reuse it** with different values.

---

### 🔹 1. Function Declaration

```javascript
function greet(name) {
  console.log("Hello, " + name + "!");
}

greet("Alice"); // Output: Hello, Alice!
```

---

### 🔹 2. Function with Return

```javascript
function add(a, b) {
  return a + b;
}

let result = add(5, 3); // 8
console.log(result);
```

---

### 🔹 3. Function Expression

```javascript
const multiply = function (x, y) {
  return x * y;
};

console.log(multiply(4, 3)); // 12
```

---

### 🔹 4. Arrow Functions (ES6+)

```javascript
const square = (num) => {
  return num * num;
};

console.log(square(5)); // 25
```

**One-line version:**

```javascript
const square = num => num * num;
```

---

### 🔹 5. Default Parameters

```javascript
function greetUser(name = "Guest") {
  console.log("Welcome, " + name);
}

greetUser(); // Welcome, Guest
```

---

## ✏️ Practice Code

In `script.js`, try:

```javascript
function isEven(num) {
  return num % 2 === 0;
}

console.log(isEven(4)); // true
console.log(isEven(7)); // false

const greet = (name = "friend") => {
  console.log(`Hello, ${name}!`);
};

greet("Bob");
greet();
```

---

## 🎯 Mini Challenges

1. Write a function `factorial(n)` to return factorial of a number.
2. Write an arrow function `isPositive(num)` to check if a number is positive.
3. Create a function that converts Celsius to Fahrenheit.

```javascript
// Celsius to Fahrenheit formula
// F = (C × 9/5) + 32
```

---
