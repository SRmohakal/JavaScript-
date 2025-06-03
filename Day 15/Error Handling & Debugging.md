---

## 📘 **Error Handling & Debugging in JavaScript**

---

### 🔹 1. Try...Catch

Handle errors gracefully so your app doesn’t crash.

```javascript
try {
  // Code that might throw an error
  let result = riskyFunction();
  console.log(result);
} catch (error) {
  console.error("Caught an error:", error.message);
}
```

---

### 🔹 2. Finally

Runs after try/catch no matter what.

```javascript
try {
  throw new Error("Oops!");
} catch (e) {
  console.log("Error caught");
} finally {
  console.log("Always runs");
}
```

---

### 🔹 3. Throwing Errors

Create your own errors when something goes wrong.

```javascript
function checkAge(age) {
  if (age < 18) {
    throw new Error("Too young!");
  }
  return true;
}

try {
  checkAge(15);
} catch (e) {
  console.error(e.message); // Too young!
}
```

---

### 🔹 4. Debugging Tips

* Use `console.log()` to check values.
* Use browser dev tools (Sources tab) to set breakpoints and step through code.
* Use `debugger;` statement in code to pause execution.

---

## ✏️ Practice Code

```javascript
function divide(a, b) {
  if (b === 0) {
    throw new Error("Cannot divide by zero");
  }
  return a / b;
}

try {
  console.log(divide(10, 2)); // 5
  console.log(divide(10, 0)); // Throws error
} catch (e) {
  console.error(e.message);
}
```

---

## 🎯 Mini Challenges

1. Write a function that throws an error if input is not a number.
2. Use try/catch to handle invalid input gracefully.
3. Add debugging logs to trace function execution.

---

