---

## 📘 **Arrays in JavaScript**

An **array** is a list of items (like numbers, strings, or objects).

```javascript
let fruits = ["apple", "banana", "cherry"];
```

---

## 🔹 1. Access & Modify Elements

```javascript
console.log(fruits[0]); // apple
fruits[1] = "mango";    // changes banana to mango
console.log(fruits);    // ["apple", "mango", "cherry"]
```

---

## 🔹 2. Array Properties & Basic Methods

| Method         | Description                         |
|----------------|-------------------------------------|
| `length`       | Number of items                     |
| `push()`       | Add item to end                     |
| `pop()`        | Remove item from end                |
| `unshift()`    | Add item to beginning               |
| `shift()`      | Remove item from beginning          |

```javascript
let colors = ["red", "blue"];
colors.push("green");  // ["red", "blue", "green"]
colors.pop();          // ["red", "blue"]
colors.unshift("yellow"); // ["yellow", "red", "blue"]
colors.shift();        // ["red", "blue"]
```

---

## 🔹 3. Useful Array Methods

### ✅ `indexOf()`

```javascript
let nums = [1, 2, 3, 4];
console.log(nums.indexOf(3)); // 2
```

### ✅ `includes()`

```javascript
console.log(nums.includes(2)); // true
```

### ✅ `slice(start, end)`

```javascript
let part = nums.slice(1, 3); // [2, 3]
```

### ✅ `splice(start, deleteCount, ...items)`

```javascript
nums.splice(2, 1, 99); // replace item at index 2 with 99
```

---

## 🔹 4. Looping Through Arrays

```javascript
let items = ["pen", "pencil", "eraser"];

for (let i = 0; i < items.length; i++) {
  console.log(items[i]);
}

// for...of
for (let item of items) {
  console.log(item);
}
```

---

## ✏️ Practice Code

Try in your `script.js`:

```javascript
let animals = ["cat", "dog", "rabbit"];
animals.push("tiger");
animals.shift();
console.log(animals); // ["dog", "rabbit", "tiger"]

let prices = [100, 200, 300];
let newPrices = prices.slice(0, 2); // [100, 200]

for (let price of newPrices) {
  console.log("Price:", price);
}
```

---

## 🎯 Mini Challenges

1. Create an array of 5 numbers. Find the sum using a loop.
2. Write a function `getLastElement(arr)` that returns the last element.
3. Use `splice` to remove 2 elements from the middle of an array.

---
