---

## 📘 **Closures & Scope in JavaScript**

---

### 🔹 1. What is Scope?

* **Scope** is where variables are accessible.
* **Global scope:** accessible anywhere.
* **Local scope:** inside functions or blocks.

---

### 🔹 2. Closure Definition

A **closure** is a function that **remembers** its lexical scope even when executed outside that scope.

---

### 🔹 3. Example of Closure

```javascript
function outer() {
  let count = 0;
  return function inner() {
    count++;
    console.log(count);
  }
}

const counter = outer();

counter(); // 1
counter(); // 2
counter(); // 3
```

---

### 🔹 4. Why Closures?

* Encapsulation (private variables)
* Data persistence between function calls
* Function factories and callbacks

---

### 🔹 5. Practical Closure Example

```javascript
function makeAdder(x) {
  return function(y) {
    return x + y;
  }
}

const add5 = makeAdder(5);
console.log(add5(3));  // 8
console.log(add5(10)); // 15
```

---

## ✏️ Practice Code

* Write a function that returns another function which keeps track of how many times it was called.
* Create a function factory that creates multiplier functions.

---

## 🎯 Mini Challenges

1. Implement a counter function that can increase, decrease, and reset its value using closures.
2. Create a private variable inside a function and provide getter/setter functions to access it.
3. Use closure to create a memoized version of a Fibonacci function.

---

