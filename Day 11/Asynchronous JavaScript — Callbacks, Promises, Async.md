---

## 📘 **Asynchronous JavaScript — Callbacks, Promises, Async/Await**

JavaScript runs code **asynchronously** so it can handle things like fetching data without blocking.

---

### 🔹 1. Callbacks

A function passed into another function to run later.

```javascript
function fetchData(callback) {
  setTimeout(() => {
    callback("Data received");
  }, 1000);
}

fetchData(data => {
  console.log(data); // Data received (after 1 second)
});
```

---

### 🔹 2. Promises

Represents a value that may be available **now, later, or never**.

```javascript
let promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve("Success!");
  }, 1000);
});

promise.then(result => {
  console.log(result); // Success! (after 1 second)
}).catch(error => {
  console.error(error);
});
```

---

### 🔹 3. Async/Await (ES8+)

Syntactic sugar for promises, makes async code look synchronous.

```javascript
function wait(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function asyncFunc() {
  console.log("Start");
  await wait(1000);
  console.log("After 1 second");
}

asyncFunc();
```

---

## ✏️ Practice Code

```javascript
function delayedMessage(msg, delay) {
  return new Promise(resolve => {
    setTimeout(() => {
      resolve(msg);
    }, delay);
  });
}

async function showMessages() {
  const message1 = await delayedMessage("Hello", 1000);
  console.log(message1);
  
  const message2 = await delayedMessage("World", 1000);
  console.log(message2);
}

showMessages();
```

---

## 🎯 Mini Challenges

1. Write a function that returns a promise resolving with "Done" after 2 seconds.
2. Use async/await to call the above function and print the result.
3. Convert a callback-based function into one that returns a promise.

---

