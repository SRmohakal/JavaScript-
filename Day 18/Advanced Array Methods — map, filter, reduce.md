---

## 📘 **Advanced Array Methods — map, filter, reduce**

---

### 🔹 1. map()

Transforms each item in an array and returns a new array.

```javascript
const numbers = [1, 2, 3];
const squares = numbers.map(num => num * num);
console.log(squares); // [1, 4, 9]
```

---

### 🔹 2. filter()

Filters items based on a condition and returns a new array.

```javascript
const numbers = [1, 2, 3, 4, 5];
const evens = numbers.filter(num => num % 2 === 0);
console.log(evens); // [2, 4]
```

---

### 🔹 3. reduce()

Reduces an array to a single value by applying a function.

```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((acc, curr) => acc + curr, 0);
console.log(sum); // 10
```

---

### 🔹 4. Combining Methods

```javascript
const numbers = [1, 2, 3, 4, 5];
const result = numbers
  .filter(num => num % 2 !== 0)
  .map(num => num * 10);
console.log(result); // [10, 30, 50]
```

---

## ✏️ Practice Code

* Use `map` to convert an array of strings to uppercase.
* Use `filter` to get only users over 18 from an array of user objects.
* Use `reduce` to count the total price of items in a shopping cart array.

---

## 🎯 Mini Challenges

1. Given an array of words, return the length of the longest word using `reduce`.
2. Chain `filter` and `map` to get the names of students who passed a test (score >= 60).
3. Use `reduce` to group objects by a property (e.g., group people by age).

---

