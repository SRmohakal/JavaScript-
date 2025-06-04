---

## 📘 **Web Storage (LocalStorage & SessionStorage)**

---

### 🔹 1. LocalStorage

* Stores data with no expiration (persists even after closing browser).

```javascript
localStorage.setItem('username', 'john_doe');
const user = localStorage.getItem('username');
console.log(user); // john_doe
localStorage.removeItem('username');
localStorage.clear(); // clears all
```

---

### 🔹 2. SessionStorage

* Stores data for one session (cleared when tab/browser closes).

```javascript
sessionStorage.setItem('sessionId', 'abc123');
const session = sessionStorage.getItem('sessionId');
console.log(session);
sessionStorage.removeItem('sessionId');
sessionStorage.clear();
```

---

### 🔹 3. Storing Objects

You must stringify objects before storing and parse when retrieving.

```javascript
const user = { name: 'Alice', age: 25 };
localStorage.setItem('user', JSON.stringify(user));

const storedUser = JSON.parse(localStorage.getItem('user'));
console.log(storedUser.name); // Alice
```

---

### 🔹 4. Practical Use Cases

* Remembering user preferences
* Saving shopping cart contents
* Storing form data temporarily

---

## ✏️ Practice Code

* Save and load a theme preference (dark/light) using localStorage.
* Store and retrieve a todo list (array of objects).
* Clear storage on user logout.

---

## 🎯 Mini Challenges

1. Build a small app that saves user notes in localStorage.
2. Implement a session timer using sessionStorage.
3. Sync data between tabs using storage events.

---

