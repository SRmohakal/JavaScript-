---

## 📘 **Array Higher-Order Methods (`map`, `filter`, `reduce`)**

These methods let you work with arrays more **efficiently** and **functionally**.

---

### 🔹 1. `map()`

* Transforms every element and returns a **new array**.

```javascript
let numbers = [1, 2, 3];
let doubled = numbers.map(num => num * 2);
console.log(doubled); // [2, 4, 6]
```

---

### 🔹 2. `filter()`

* Filters elements based on a condition, returns a **new array**.

```javascript
let numbers = [5, 10, 15, 20];
let bigNumbers = numbers.filter(num => num > 10);
console.log(bigNumbers); // [15, 20]
```

---

### 🔹 3. `reduce()`

* Reduces the array to a **single value** by accumulating results.

```javascript
let numbers = [1, 2, 3, 4];
let sum = numbers.reduce((accumulator, current) => accumulator + current, 0);
console.log(sum); // 10
```

---

### 🔹 4. Bonus: `forEach()`

* Runs a function on every element (no return).

```javascript
let fruits = ["apple", "banana", "cherry"];
fruits.forEach(fruit => console.log(fruit));
```

---

## ✏️ Practice Code

```javascript
const nums = [1, 2, 3, 4, 5];

const squares = nums.map(n => n * n);
console.log("Squares:", squares);

const evens = nums.filter(n => n % 2 === 0);
console.log("Evens:", evens);

const total = nums.reduce((acc, n) => acc + n, 0);
console.log("Sum:", total);

nums.forEach(n => console.log("Number:", n));
```

---

## 🎯 Mini Challenges

1. Use `map` to convert array of strings to uppercase.
2. Use `filter` to keep only numbers divisible by 3.
3. Use `reduce` to find the product of all numbers.

---
