---

## 📘 **Working with Dates & Times in JavaScript**

---

### 🔹 1. Create a Date Object

```javascript
const now = new Date();
console.log(now);
```

---

### 🔹 2. Create Specific Date

```javascript
const specificDate = new Date('2025-12-31T23:59:59');
console.log(specificDate);
```

---

### 🔹 3. Get Components of Date

```javascript
console.log(now.getFullYear());    // 2025
console.log(now.getMonth());       // 0–11 (0 = January)
console.log(now.getDate());        // Day of month
console.log(now.getHours());
console.log(now.getMinutes());
console.log(now.getSeconds());
```

---

### 🔹 4. Set Components of Date

```javascript
now.setFullYear(2030);
now.setMonth(11);  // December
now.setDate(25);
console.log(now);
```

---

### 🔹 5. Date Math

```javascript
const tomorrow = new Date();
tomorrow.setDate(tomorrow.getDate() + 1);
console.log(tomorrow);
```

---

### 🔹 6. Format Date String

```javascript
console.log(now.toDateString());  // e.g. "Tue May 24 2030"
console.log(now.toISOString());   // e.g. "2030-12-25T00:00:00.000Z"
```

---

## ✏️ Practice Code

* Create a countdown timer to a specific date.
* Display the current date and time updating every second.
* Calculate the difference (in days) between two dates.

---

## 🎯 Mini Challenges

1. Write a function that tells if a given year is a leap year.
2. Format a date as `DD/MM/YYYY` string.
3. Create a stopwatch that starts, stops, and resets.

---

