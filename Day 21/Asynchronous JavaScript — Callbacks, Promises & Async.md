---

## 📘 **Asynchronous JavaScript — Callbacks, Promises & Async/Await**

---

### 🔹 1. Callbacks

Functions passed as arguments to run after async work.

```javascript
function doAsyncTask(callback) {
  setTimeout(() => {
    callback('Task done!');
  }, 1000);
}

doAsyncTask(message => {
  console.log(message);
});
```

---

### 🔹 2. Promises

Objects representing future completion/failure.

```javascript
const promise = new Promise((resolve, reject) => {
  setTimeout(() => {
    const success = true;
    if (success) resolve('Success!');
    else reject('Failure!');
  }, 1000);
});

promise
  .then(result => console.log(result))
  .catch(error => console.error(error));
```

---

### 🔹 3. Async/Await (Syntax sugar over Promises)

```javascript
async function asyncFunc() {
  try {
    const result = await promise;
    console.log(result);
  } catch (error) {
    console.error(error);
  }
}

asyncFunc();
```

---

## ✏️ Practice Code

* Convert a callback-based function to return a Promise.
* Write async functions that use await to fetch data.
* Handle errors in async functions using try/catch.

---

## 🎯 Mini Challenges

1. Create a function that returns a promise which resolves after 2 seconds.
2. Chain multiple promises to run tasks sequentially.
3. Use async/await to fetch data from an API and handle errors.

---
