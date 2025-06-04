---

## 📘 **JavaScript Error Handling & Debugging**

---

### 🔹 1. Try...Catch

```javascript
try {
  // code that may throw error
  let result = riskyFunction();
  console.log(result);
} catch (error) {
  console.error('Caught an error:', error.message);
}
```

---

### 🔹 2. Finally

Runs code regardless of error

```javascript
try {
  console.log('Trying...');
  throw new Error('Oops!');
} catch (e) {
  console.log('Caught:', e.message);
} finally {
  console.log('Always runs');
}
```

---

### 🔹 3. Throw Custom Errors

```javascript
function checkNumber(num) {
  if (typeof num !== 'number') {
    throw new TypeError('Not a number!');
  }
  return num;
}

try {
  checkNumber('abc');
} catch (e) {
  console.error(e.message);
}
```

---

### 🔹 4. Debugging with `console`

* `console.log()`, `console.error()`, `console.warn()`
* `console.table()` to show arrays/objects in table
* `console.time()` and `console.timeEnd()` to measure performance

---

### 🔹 5. Using Browser DevTools

* Set breakpoints
* Step through code line by line
* Inspect variables & call stack

---

## ✏️ Practice Code

* Write code that purposely throws and catches errors.
* Log various data types using different console methods.
* Debug a piece of code using breakpoints.

---

## 🎯 Mini Challenges

1. Write a function that validates input and throws errors for invalid data.
2. Use `console.time()` to measure execution time of a loop.
3. Debug a buggy function using browser DevTools.

---

