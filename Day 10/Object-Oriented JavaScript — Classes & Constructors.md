---

## 📘 **Object-Oriented JavaScript — Classes & Constructors**

Classes let you create **blueprints** for objects with shared properties and methods.

---

### 🔹 1. Class Syntax (ES6+)

```javascript
class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  greet() {
    console.log(`Hi, I am ${this.name} and I am ${this.age} years old.`);
  }
}

const person1 = new Person("Alice", 25);
person1.greet(); // Hi, I am Alice and I am 25 years old.
```

---

### 🔹 2. Constructor Method

* Runs automatically when you create a new object (`new Person(...)`).

---

### 🔹 3. Adding Methods

* Methods go inside the class but outside constructor.

---

### 🔹 4. Inheritance (Extending Classes)

```javascript
class Student extends Person {
  constructor(name, age, grade) {
    super(name, age);
    this.grade = grade;
  }

  study() {
    console.log(`${this.name} is studying.`);
  }
}

const student1 = new Student("Bob", 20, "A");
student1.greet();
student1.study();
```

---

## ✏️ Practice Code

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a sound.`);
  }
}

class Dog extends Animal {
  speak() {
    console.log(`${this.name} barks.`);
  }
}

const dog1 = new Dog("Rex");
dog1.speak(); // Rex barks.
```

---

## 🎯 Mini Challenges

1. Create a `Car` class with properties: `make`, `model`, and method `drive()`.
2. Extend `Car` class with `ElectricCar` that adds `batteryLevel` property and a method `charge()`.
3. Create instances and test all methods.

---
