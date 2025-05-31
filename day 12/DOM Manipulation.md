---

## 📘 **DOM Manipulation**

DOM = Document Object Model, which is the structure of the webpage.
JavaScript can **access, change, and create elements** on the page.

---

### 🔹 1. Access Elements

```javascript
// by id
const heading = document.getElementById("myHeading");

// by class name
const items = document.getElementsByClassName("list-item");

// by tag name
const paragraphs = document.getElementsByTagName("p");

// querySelector (CSS selector)
const firstItem = document.querySelector(".list-item");

// querySelectorAll (all matching)
const allItems = document.querySelectorAll(".list-item");
```

---

### 🔹 2. Change Content

```javascript
heading.textContent = "New Heading Text";
```

---

### 🔹 3. Change Styles

```javascript
heading.style.color = "blue";
heading.style.fontSize = "30px";
```

---

### 🔹 4. Add / Remove Elements

```javascript
const ul = document.querySelector("ul");
const li = document.createElement("li");
li.textContent = "New item";
ul.appendChild(li);  // add new list item

// Remove element
ul.removeChild(ul.lastElementChild);
```

---

### 🔹 5. Event Listeners

```javascript
const button = document.querySelector("button");

button.addEventListener("click", () => {
  alert("Button clicked!");
});
```

---

## ✏️ Practice Code

Try creating an HTML file with a button and a div. Use JavaScript to:

* Change the text inside the div when the button is clicked.
* Add a new paragraph inside the div.
* Change the div’s background color.

---

## 🎯 Mini Challenges

1. Create a list dynamically from an array of strings.
2. Build a button that toggles the visibility of an element.
3. Create an input box and a button that, when clicked, adds the input text to a list.

---
