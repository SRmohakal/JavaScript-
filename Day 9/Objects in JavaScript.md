---

## 📘 **Objects in JavaScript**

Objects store **key-value pairs** — great for grouping related data.

---

### 🔹 1. Creating Objects

```javascript
const person = {
  name: "Alice",
  age: 25,
  city: "New York"
};
```

---

### 🔹 2. Accessing Properties

```javascript
console.log(person.name);  // Alice
console.log(person["age"]); // 25
```

---

### 🔹 3. Adding & Modifying Properties

```javascript
person.job = "Engineer";
person.age = 26;
```

---

### 🔹 4. Methods (Functions inside objects)

```javascript
const person = {
  name: "Alice",
  greet: function() {
    console.log("Hello, " + this.name);
  }
};

person.greet(); // Hello, Alice
```

---

### 🔹 5. Shortcut for Methods (ES6)

```javascript
const person = {
  name: "Bob",
  greet() {
    console.log("Hi, " + this.name);
  }
};
```

---

### 🔹 6. Looping through Object Properties

```javascript
for (let key in person) {
  console.log(key + ": " + person[key]);
}
```

---

## ✏️ Practice Code

```javascript
const car = {
  brand: "Toyota",
  model: "Corolla",
  year: 2020,
  start() {
    console.log("Car started");
  }
};

console.log(car.brand); // Toyota
car.start(); // Car started
car.color = "red";

for (let prop in car) {
  console.log(prop + " -> " + car[prop]);
}
```

---

## 🎯 Mini Challenges

1. Create an object `book` with properties: `title`, `author`, `pages`. Add a method to print a summary.
2. Update the `book` object by adding a new property `year`.
3. Loop through the object and print all keys and values.

---
