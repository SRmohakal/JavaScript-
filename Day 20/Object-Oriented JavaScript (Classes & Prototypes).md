---

## 📘 **Object-Oriented JavaScript (Classes & Prototypes)**

---

### 🔹 1. Classes (ES6 Syntax)

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hello, I'm ${this.name} and I'm ${this.age} years old.`);
  }
}

const alice = new Person('Alice', 30);
alice.greet(); // Hello, I'm Alice and I'm 30 years old.
```

---

### 🔹 2. Inheritance

```javascript
class Student extends Person {
  constructor(name, age, studentId) {
    super(name, age);
    this.studentId = studentId;
  }

  study() {
    console.log(`${this.name} is studying.`);
  }
}

const bob = new Student('Bob', 20, 'S1234');
bob.greet();
bob.study();
```

---

### 🔹 3. Prototypes (Old Style)

```javascript
function Animal(name) {
  this.name = name;
}

Animal.prototype.speak = function() {
  console.log(`${this.name} makes a noise.`);
}

const dog = new Animal('Dog');
dog.speak();
```

---

### 🔹 4. Why Use Classes?

* Better syntax for objects & inheritance
* Easier to read & maintain
* Supports encapsulation with private fields (modern JS)

---

## ✏️ Practice Code

* Create a class `Car` with properties and methods.
* Extend `Car` to create `ElectricCar` with extra methods.
* Use prototype to add a new method to an existing class.

---

## 🎯 Mini Challenges

1. Build a `BankAccount` class with deposit, withdraw, and balance methods.
2. Extend it to create `SavingsAccount` with interest calculation.
3. Override a method in subclass and call the parent method.

---

