---

## 📘 **Loops (for, while, do...while, for...of)**

Loops let you **repeat code** without writing it multiple times.

---

### 🔹 1. `for` Loop

**Used when you know how many times to loop.**

```javascript
for (let i = 1; i <= 5; i++) {
  console.log("Number:", i);
}
```

---

### 🔹 2. `while` Loop

**Used when you want to loop until a condition is false.**

```javascript
let i = 1;
while (i <= 5) {
  console.log("While loop:", i);
  i++;
}
```

---

### 🔹 3. `do...while` Loop

**Runs at least once, then checks the condition.**

```javascript
let i = 1;
do {
  console.log("Do-While:", i);
  i++;
} while (i <= 5);
```

---

### 🔹 4. `for...of` Loop

**Used to loop through elements of an array or string.**

```javascript
let fruits = ["apple", "banana", "mango"];

for (let fruit of fruits) {
  console.log("Fruit:", fruit);
}
```

---

## 🛑 Loop Control Statements

* `break` → exit the loop early
* `continue` → skip current iteration

```javascript
for (let i = 1; i <= 5; i++) {
  if (i === 3) continue;
  console.log(i); // Skips 3
}
```

---

## ✏️ Practice Tasks

In `script.js`, try the following:

```javascript
// 1. Print numbers 1 to 10 using for loop
for (let i = 1; i <= 10; i++) {
  console.log(i);
}

// 2. Print even numbers from 1 to 20
for (let i = 1; i <= 20; i++) {
  if (i % 2 === 0) console.log(i);
}

// 3. Use while loop to print numbers from 5 to 1
let j = 5;
while (j >= 1) {
  console.log("Countdown:", j);
  j--;
}

// 4. for...of with string
let message = "JavaScript";
for (let char of message) {
  console.log(char);
}
```

---

## 🎯 Mini Challenges

1. Sum all numbers from 1 to 100 using a `for` loop.
2. Count how many vowels are in a word using `for...of`.

---
