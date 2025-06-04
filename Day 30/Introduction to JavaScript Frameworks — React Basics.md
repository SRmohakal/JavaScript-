---

## 📘 **Introduction to JavaScript Frameworks — React Basics**

---

### 🔹 1. What is React?

* A library for building UI components.
* Uses **JSX** — HTML-like syntax in JavaScript.
* Works with a **virtual DOM** for efficient updates.

---

### 🔹 2. Setting Up

* Use [Create React App](https://reactjs.org/docs/create-a-new-react-app.html#create-react-app) or online playgrounds like [CodeSandbox](https://codesandbox.io/).

---

### 🔹 3. Basic Component

```jsx
function Hello(props) {
  return <h1>Hello, {props.name}!</h1>;
}
```

---

### 🔹 4. Rendering Component

```jsx
import React from 'react';
import ReactDOM from 'react-dom/client';

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<Hello name="World" />);
```

---

### 🔹 5. State & Events

```jsx
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>
    </>
  );
}
```

---

### 🔹 6. Props vs State

* **Props:** Data passed to components, read-only.
* **State:** Internal data managed by the component, mutable.

---

## ✏️ Practice Code

* Build a component that shows a message passed via props.
* Create a counter component with increment/decrement buttons.
* Combine components to create a simple app.

---

## 🎯 Mini Challenges

1. Build a todo list app in React.
2. Add input field to add new todos.
3. Implement delete functionality.

---

React is a big topic, but this will give you a solid start for modern frontend development.

---

