---

## 📘 **Day 1: Introduction to JavaScript & Setup**

---

> JavaScript is a **high-level**, **interpreted** programming language used to **make web pages interactive**.

It allows you to:

* Add dynamic behavior (like pop-ups, animations, games)
* Modify HTML & CSS from code
* Handle user inputs
* Fetch data from APIs

#### ✅ Example:

```html
<p id="demo">Click the button to change me!</p>
<button onclick="changeText()">Click Me</button>

<script>
  function changeText() {
    document.getElementById("demo").innerText = "Hello, JavaScript!";
  }
</script>
```

---

### 🛠️ How to Run JavaScript

#### Option 1: **Browser Console**

1. Open Chrome → Right Click → Inspect → Go to Console tab
2. Type:

```javascript
console.log("Hello, JavaScript!");
```

#### Option 2: **Using HTML + JS file in VS Code**

1. Create a folder and add:

   * `index.html`
   * `script.js`
2. `index.html`

```html
<!DOCTYPE html>
<html>
<head>
  <title>JS Setup</title>
</head>
<body>
  <h1>JS Setup Test</h1>
  <script src="script.js"></script>
</body>
</html>
```

3. `script.js`

```javascript
console.log("JavaScript is working!");
```

#### Option 3: **Online Editors**

* [JSFiddle](https://jsfiddle.net/)
* [CodePen](https://codepen.io/)
* [Replit](https://replit.com/)

---

### ✏️ Practice Task

1. Create `index.html` and `script.js`.
2. Display a message:

```javascript
alert("Welcome to JavaScript!");
```

3. In the console:

```javascript
let name = "Alice";
console.log("Hi " + name + ", welcome!");
```

---
