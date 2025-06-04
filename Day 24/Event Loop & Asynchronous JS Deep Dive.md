---

## 📘 **Event Loop & Asynchronous JS Deep Dive**

---

### 🔹 1. Call Stack & Task Queue

* **Call Stack:** Where JS runs your code line by line.
* **Task Queue (Callback Queue):** Holds callbacks waiting to run after the stack clears.

---

### 🔹 2. Event Loop

Continuously checks if the call stack is empty and moves callbacks from the task queue to the stack.

---

### 🔹 3. Microtasks vs Macrotasks

* **Microtasks:** Promises, `process.nextTick`
* **Macrotasks:** `setTimeout`, `setInterval`, I/O events

Microtasks run before macrotasks after the current stack.

---

### 🔹 4. Example

```javascript
console.log('Start');

setTimeout(() => {
  console.log('Timeout');
}, 0);

Promise.resolve().then(() => {
  console.log('Promise');
});

console.log('End');
```

**Output:**

```
Start
End
Promise
Timeout
```

---

### 🔹 5. Why It Matters?

Helps you understand async behavior, race conditions, UI rendering, and performance.

---

## ✏️ Practice Code

* Experiment with nested `setTimeout` and promises.
* Use async functions to see order of execution.
* Write code with mixed sync and async to predict output.

---

## 🎯 Mini Challenges

1. Predict outputs for different async examples.
2. Create a small scheduler that uses micro and macrotasks.
3. Explain how async/await works under the hood with event loop.

---
