---

## 📘 **Fetch API & Working with APIs**

JavaScript can fetch data from servers to make your apps dynamic and interactive.

---

### 🔹 1. Fetch Basic Syntax

```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

---

### 🔹 2. Async/Await with Fetch

```javascript
async function getPost() {
  try {
    let response = await fetch('https://jsonplaceholder.typicode.com/posts/1');
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}

getPost();
```

---

### 🔹 3. Posting Data

```javascript
async function createPost() {
  try {
    let response = await fetch('https://jsonplaceholder.typicode.com/posts', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json'
      },
      body: JSON.stringify({ title: 'foo', body: 'bar', userId: 1 })
    });
    let data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error:', error);
  }
}

createPost();
```

---

## ✏️ Practice Code

* Fetch and display a list of posts from an API.
* Post new data to the API and log the response.
* Handle errors gracefully with try/catch.

---

## 🎯 Mini Challenges

1. Fetch user data from an API and show it on the page.
2. Build a small app that lets users add posts and see them listed.
3. Implement loading and error messages while fetching data.

---

