---

## 📘 **Working with JSON & Fetch API**

---

### 🔹 1. JSON (JavaScript Object Notation)

* Format for exchanging data.
* Use `JSON.stringify()` to convert JS object to JSON string.
* Use `JSON.parse()` to convert JSON string back to JS object.

```javascript
const obj = { name: 'Alice', age: 25 };
const jsonString = JSON.stringify(obj);
console.log(jsonString); // '{"name":"Alice","age":25}'

const parsedObj = JSON.parse(jsonString);
console.log(parsedObj.name); // Alice
```

---

### 🔹 2. Fetch API (To get or send data over network)

```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
  .then(response => response.json())  // Parse JSON from response
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

---

### 🔹 3. Async/Await with Fetch

```javascript
async function getPost() {
  try {
    const response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}
getPost();
```

---

### 🔹 4. Sending Data (POST Request)

```javascript
fetch('https://jsonplaceholder.typicode.com/posts', {
  method: 'POST',
  body: JSON.stringify({ title: 'foo', body: 'bar', userId: 1 }),
  headers: {
    'Content-type': 'application/json; charset=UTF-8',
  },
})
  .then(response => response.json())
  .then(data => console.log(data));
```

---

## ✏️ Practice Code

* Fetch a list of users and display in console.
* Send a POST request to an API with some data.
* Handle errors gracefully.

---

## 🎯 Mini Challenges

1. Write a function to fetch and display data from any public API.
2. Build a small app that fetches and displays user info dynamically.
3. Implement loading and error UI states during fetch.

---

