---

## 📘 **JavaScript Forms & Validation**

---

### 🔹 1. Accessing Form Elements

```html
<form id="myForm">
  <input type="text" id="name" />
  <button type="submit">Submit</button>
</form>
```

```javascript
const form = document.getElementById('myForm');
const nameInput = document.getElementById('name');
```

---

### 🔹 2. Handling Form Submission

Prevent default to control submit behavior.

```javascript
form.addEventListener('submit', (e) => {
  e.preventDefault();
  console.log('Form submitted!');
});
```

---

### 🔹 3. Basic Validation

```javascript
form.addEventListener('submit', (e) => {
  e.preventDefault();
  if(nameInput.value.trim() === '') {
    alert('Name is required!');
  } else {
    alert(`Hello, ${nameInput.value}`);
  }
});
```

---

### 🔹 4. Advanced Validation (Regex)

```javascript
const emailInput = document.getElementById('email');
const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

form.addEventListener('submit', (e) => {
  e.preventDefault();
  if(!emailPattern.test(emailInput.value)) {
    alert('Invalid email!');
  } else {
    alert('Valid email!');
  }
});
```

---

### 🔹 5. Real-time Validation (oninput/onchange)

```javascript
nameInput.addEventListener('input', () => {
  if(nameInput.value.trim() === '') {
    nameInput.style.borderColor = 'red';
  } else {
    nameInput.style.borderColor = 'green';
  }
});
```

---

## ✏️ Practice Code

* Create a form with name, email, and password fields.
* Validate fields before submission.
* Show error messages dynamically.
* Reset form on successful submission.

---

## 🎯 Mini Challenges

1. Build a signup form with validation for all fields.
2. Disable submit button until all validations pass.
3. Add password strength indicator.

---

