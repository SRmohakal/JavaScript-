---

## 📘 **Conditional Statements**

Conditional statements let you **make decisions** in your code.

---

## 🔹 1. `if`, `else if`, `else`

### ✅ Syntax:

```javascript
if (condition) {
  // runs if true
} else if (anotherCondition) {
  // runs if first is false and this is true
} else {
  // runs if all above are false
}
```

### ✅ Example:

```javascript
let age = 18;

if (age < 13) {
  console.log("You're a child.");
} else if (age < 20) {
  console.log("You're a teenager.");
} else {
  console.log("You're an adult.");
}
```

---

## 🔹 2. `switch` Statement

Useful when comparing one variable with **many values**.

### ✅ Syntax:

```javascript
let day = "Monday";

switch(day) {
  case "Monday":
    console.log("Start of the week!");
    break;
  case "Friday":
    console.log("Almost weekend!");
    break;
  default:
    console.log("Just another day.");
}
```

> 🔸 Don’t forget `break;` – it prevents the code from falling through.

---

## 🔹 3. Ternary Operator (short `if-else`)

```javascript
let age = 16;
let result = (age >= 18) ? "Adult" : "Minor";
console.log(result); // "Minor"
```

---

## ✏️ Practice Code

In `script.js`, try:

```javascript
let score = 85;

if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 80) {
  console.log("Grade: B");
} else if (score >= 70) {
  console.log("Grade: C");
} else {
  console.log("Grade: F");
}

// Switch example
let fruit = "banana";

switch (fruit) {
  case "apple":
    console.log("Apples are red.");
    break;
  case "banana":
    console.log("Bananas are yellow.");
    break;
  default:
    console.log("Unknown fruit.");
}
```

---

## 🎯 Mini Challenges

1. Write a script that checks if a number is even or odd using `%`.
2. Use a `switch` statement to print messages for days of the week.

---
