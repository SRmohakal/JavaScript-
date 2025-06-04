---

## 📘 **DOM Manipulation & Event Handling**

---

### 🔹 1. What is DOM?

* Document Object Model — representation of HTML as a tree of nodes.
* JavaScript can read and modify this structure.

---

### 🔹 2. Selecting Elements

```javascript
const el = document.getElementById('myId');
const els = document.getElementsByClassName('myClass');
const els2 = document.querySelectorAll('.myClass');
const el2 = document.querySelector('#myId');
```

---

### 🔹 3. Changing Content & Attributes

```javascript
el.textContent = 'Hello, world!';
el.innerHTML = '<strong>Bold text</strong>';
el.setAttribute('data-info', '123');
```

---

### 🔹 4. Creating & Adding Elements

```javascript
const newDiv = document.createElement('div');
newDiv.textContent = 'New Element';
document.body.appendChild(newDiv);
```

---

### 🔹 5. Removing Elements

```javascript
const elementToRemove = document.getElementById('removeMe');
elementToRemove.remove();
```

---

### 🔹 6. Event Handling

```javascript
el.addEventListener('click', () => {
  alert('Clicked!');
});
```

---

### 🔹 7. Event Object

```javascript
el.addEventListener('click', (event) => {
  console.log('Clicked element:', event.target);
});
```

---

## ✏️ Practice Code

* Change text content on button click.
* Add new list items dynamically.
* Remove items on click.
* Use event delegation for dynamic elements.

---

## 🎯 Mini Challenges

1. Build a simple to-do list with add and delete functionality.
2. Toggle CSS classes on click to show/hide elements.
3. Use event delegation to handle clicks on list items.

---

