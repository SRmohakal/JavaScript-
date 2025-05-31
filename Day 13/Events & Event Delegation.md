---

## 📘 **Events & Event Delegation**

---

### 🔹 1. Basic Events

Events are user or browser actions — like clicks, key presses, mouse movements.

```javascript
const btn = document.querySelector("button");

btn.addEventListener("click", () => {
  console.log("Button clicked!");
});
```

---

### 🔹 2. Event Object

Inside event handlers, you get an event object giving info:

```javascript
btn.addEventListener("click", (event) => {
  console.log("Clicked at:", event.clientX, event.clientY);
});
```

---

### 🔹 3. Event Delegation

Instead of adding listeners to every item, add one listener to a **parent** to handle events for children.

```html
<ul id="list">
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

```javascript
const list = document.getElementById("list");

list.addEventListener("click", (event) => {
  if (event.target.tagName === "LI") {
    console.log("Clicked on:", event.target.textContent);
  }
});
```

---

### 🔹 4. Prevent Default Behavior

Useful for links, form submits.

```javascript
const link = document.querySelector("a");

link.addEventListener("click", (event) => {
  event.preventDefault();
  console.log("Link clicked, but default action prevented.");
});
```

---

## ✏️ Practice Code

* Create a list with many items, add one event listener on the parent, and detect which item was clicked.
* Make a form that alerts input value on submit but prevents page reload.

---

## 🎯 Mini Challenges

1. Add event delegation for a dynamic list where items can be added or removed.
2. Build a simple to-do list where clicking an item marks it done (strike-through).
3. Use `preventDefault` to stop a form submission and validate input first.

---

