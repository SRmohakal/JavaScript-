---

## 📘 **Day 3: JavaScript Operators**

---

Operators let you perform actions on variables and values.

---

## 🔹 1. **Arithmetic Operators**

Used to do math.

| Operator | Description         | Example  | Result |
| -------- | ------------------- | -------- | ------ |
| `+`      | Addition            | `5 + 2`  | `7`    |
| `-`      | Subtraction         | `5 - 2`  | `3`    |
| `*`      | Multiplication      | `5 * 2`  | `10`   |
| `/`      | Division            | `10 / 2` | `5`    |
| `%`      | Modulus (remainder) | `7 % 3`  | `1`    |
| `**`     | Exponentiation      | `2 ** 3` | `8`    |
| `++`     | Increment           | `x++`    | `x+1`  |
| `--`     | Decrement           | `x--`    | `x-1`  |

---

## 🔹 2. **Assignment Operators**

Used to assign values.

| Operator | Example  | Same as     |
| -------- | -------- | ----------- |
| `=`      | `x = 10` | `x = 10`    |
| `+=`     | `x += 5` | `x = x + 5` |
| `-=`     | `x -= 5` | `x = x - 5` |
| `*=`     | `x *= 2` | `x = x * 2` |
| `/=`     | `x /= 2` | `x = x / 2` |
| `%=`     | `x %= 3` | `x = x % 3` |

---

## 🔹 3. **Comparison Operators**

Used in conditions to compare values.

| Operator | Description          | Example     | Result  |
| -------- | -------------------- | ----------- | ------- |
| `==`     | Equal (type ignored) | `5 == "5"`  | `true`  |
| `===`    | Equal (type strict)  | `5 === "5"` | `false` |
| `!=`     | Not equal            | `5 != 3`    | `true`  |
| `!==`    | Not equal (strict)   | `5 !== "5"` | `true`  |
| `>`      | Greater than         | `5 > 2`     | `true`  |
| `<`      | Less than            | `3 < 1`     | `false` |
| `>=`     | Greater or equal     | `5 >= 5`    | `true`  |
| `<=`     | Less or equal        | `3 <= 4`    | `true`  |

---

## 🔹 4. **Logical Operators**

| Operator | Description     | Example         | Result                 |        |   |         |        |
| -------- | --------------- | --------------- | ---------------------- | ------ | - | ------- | ------ |
| `&&`     | AND (both true) | `true && false` | `false`                |        |   |         |        |
| \`       |                 | \`              | OR (at least one true) | \`true |   | false\` | `true` |
| `!`      | NOT (negation)  | `!true`         | `false`                |        |   |         |        |

---

## ✏️ Practice Code

In `script.js`, try:

```javascript
let a = 10;
let b = 5;

console.log("Add:", a + b);
console.log("Multiply:", a * b);
console.log("a is greater than b?", a > b);

let isAdult = true;
let hasID = false;

console.log("Can enter club?", isAdult && hasID);
console.log("Can enter with either?", isAdult || hasID);
```

---

## 🎯 Mini Challenges

1. What does `10 % 3` return?
2. What's the difference between `==` and `===`?
3. Try:

```javascript
let x = 5;
x += 3;
console.log(x); // What is the result?
```

---
