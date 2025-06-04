---

## 📘 **JavaScript Modules (ES6 import and export)**

---

### 🔹 1. What are Modules?

* Pieces of code split into files.
* Encapsulate logic and variables.
* Help organize and reuse code.

---

### 🔹 2. Exporting

**Named exports:**

```javascript
// math.js
export function add(a, b) {
  return a + b;
}

export const PI = 3.14;
```

**Default export:**

```javascript
// greeting.js
export default function greet(name) {
  console.log(`Hello, ${name}!`);
}
```

---

### 🔹 3. Importing

**Named imports:**

```javascript
import { add, PI } from './math.js';
console.log(add(2, 3)); // 5
console.log(PI);        // 3.14
```

**Default import:**

```javascript
import greet from './greeting.js';
greet('Alice'); // Hello, Alice!
```

**Rename imports:**

```javascript
import { add as sum } from './math.js';
console.log(sum(4, 5)); // 9
```

---

### 🔹 4. Import all as object

```javascript
import * as math from './math.js';
console.log(math.add(1,2)); // 3
```

---

### 🔹 5. Benefits of Modules

* Avoid polluting global scope.
* Reuse and maintain code easily.
* Load code on demand (with bundlers).

---

## ✏️ Practice Code

* Create two modules: one exporting math functions, another exporting string utils.
* Import and use them in a main app file.
* Use default and named exports/imports in your modules.

---

## 🎯 Mini Challenges

1. Write a module exporting a class, import and instantiate it.
2. Refactor a big script into multiple modules.
3. Use dynamic `import()` to load a module on-demand.

---
