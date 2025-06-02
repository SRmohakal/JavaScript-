---

## 📘 **JavaScript Modules & ES6 Imports/Exports**

Organizing code into **modules** helps keep projects clean and manageable.

---

### 🔹 1. What are Modules?

Modules are separate files that **export** code (variables, functions, classes) and **import** them in other files.

---

### 🔹 2. Exporting

```javascript
// mathUtils.js
export function add(a, b) {
  return a + b;
}

export const PI = 3.14159;
```

---

### 🔹 3. Importing

```javascript
// main.js
import { add, PI } from './mathUtils.js';

console.log(add(2, 3));  // 5
console.log(PI);         // 3.14159
```

---

### 🔹 4. Default Export

```javascript
// greeting.js
export default function greet(name) {
  console.log(`Hello, ${name}!`);
}
```

```javascript
// main.js
import greet from './greeting.js';

greet('Alice');  // Hello, Alice!
```

---

### 🔹 5. Import Everything

```javascript
import * as utils from './mathUtils.js';

console.log(utils.add(5, 6)); // 11
console.log(utils.PI);        // 3.14159
```

---

## ✏️ Practice Code

* Create two JS files: one exporting multiple functions and constants.
* Create a main file importing and using them.
* Try both named and default exports/imports.

---

## 🎯 Mini Challenges

1. Write a module that exports a class `Calculator` with basic methods.
2. Import that class in another file and use it.
3. Create a utility module that exports constants and functions, then use them in main.

---
