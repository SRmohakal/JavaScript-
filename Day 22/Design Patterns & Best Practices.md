---

## 📘 **JavaScript Design Patterns & Best Practices**

---

### 🔹 1. Module Pattern

Encapsulate code, avoid polluting global scope.

```javascript
const Counter = (function () {
  let count = 0;
  return {
    increment() {
      count++;
      return count;
    },
    reset() {
      count = 0;
    }
  };
})();
console.log(Counter.increment()); // 1
console.log(Counter.increment()); // 2
Counter.reset();
```

---

### 🔹 2. Singleton Pattern

Ensure only one instance of an object exists.

```javascript
const Singleton = (function () {
  let instance;
  
  function createInstance() {
    return { id: Math.random() };
  }
  
  return {
    getInstance() {
      if (!instance) {
        instance = createInstance();
      }
      return instance;
    }
  };
})();

const obj1 = Singleton.getInstance();
const obj2 = Singleton.getInstance();
console.log(obj1 === obj2); // true
```

---

### 🔹 3. Observer Pattern (Event Listeners)

Objects listen and respond to events.

---

### 🔹 4. Best Practices

* Use `const`/`let` instead of `var`
* Write pure functions where possible
* Keep functions small and focused
* Use meaningful variable and function names
* Avoid deep nesting; use early returns
* Comment your code when logic is complex
* Use ESLint to enforce coding style

---

## ✏️ Practice Code

* Implement a module pattern to manage a shopping cart.
* Create a singleton logger object.
* Use event listeners to implement an observer pattern for UI events.

---

## 🎯 Mini Challenges

1. Refactor a piece of code to use the module pattern.
2. Create a singleton database connection object (mock).
3. Build a simple pub-sub system (observer pattern).

---

