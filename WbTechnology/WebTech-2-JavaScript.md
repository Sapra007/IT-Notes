# ⚡ Web Technology - JavaScript
> IT Student Notes | Topic: Web Tech Fundamentals — Part 2

---

## 📌 Table of Contents
1. [JavaScript Kya Hai](#1-javascript-kya-hai)
2. [JS Kaise Use Karo](#2-js-kaise-use-karo)
3. [Variables & Data Types](#3-variables--data-types)
4. [Conditions & Loops](#4-conditions--loops)
5. [Functions](#5-functions)
6. [DOM Manipulation](#6-dom-manipulation)
7. [Quick Revision](#7-quick-revision)

---

## 1. JavaScript Kya Hai

- Web pages ko **interactive** banane ki language
- Browser mein directly chalta hai
- HTML/CSS ke saath milke kaam karta hai

```
HTML  → Structure   (kya hai)
CSS   → Style       (kaisa dikhta hai)
JS    → Behaviour   (kya karta hai)
```

### JS Kya Karta Hai:
```
✅ Button click pe kuch ho
✅ Form validate karo
✅ Animation chalao
✅ Data server se load karo
✅ Alert/Popup dikhao
```

---

## 2. JS Kaise Use Karo

```html
<!-- 1. HTML ke andar (script tag) -->
<script>
  alert("Hello!");
</script>

<!-- 2. External file (best practice ✅) -->
<script src="script.js"></script>
```

### Console Use Karo (Debugging):
```javascript
console.log("Hello");        // Output print karo
console.log(2 + 2);          // 4
```

---

## 3. Variables & Data Types

### Variables:
```javascript
let   name = "Rahul";    // Change ho sakta hai ✅
const age  = 20;         // Change nahi hoga ✅
var   city = "Surat";    // Purana tarika (avoid karo)
```

### Data Types:
```javascript
let name    = "Rahul";    // String (text)
let age     = 20;         // Number
let isAdmin = true;       // Boolean (true/false)
let score   = null;       // Null (koi value nahi)
let x;                    // Undefined (value assign nahi)
```

### Operations:
```javascript
// Math
let a = 10 + 5;   // 15
let b = 10 - 3;   // 7
let c = 4 * 3;    // 12
let d = 10 / 2;   // 5
let e = 10 % 3;   // 1 (remainder)

// String joining
let firstName = "Rahul";
let lastName  = "Sharma";
let full = firstName + " " + lastName; // "Rahul Sharma"
```

---

## 4. Conditions & Loops

### If-Else:
```javascript
let marks = 75;

if (marks >= 90) {
  console.log("A Grade");
} else if (marks >= 60) {
  console.log("B Grade");   // ← Yeh chalega
} else {
  console.log("Fail");
}
```

### For Loop:
```javascript
// 1 se 5 tak print karo
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
// Output: 1 2 3 4 5
```

### While Loop:
```javascript
let i = 1;
while (i <= 3) {
  console.log(i);
  i++;
}
// Output: 1 2 3
```

---

## 5. Functions

- Ek kaam ka reusable code block
- Baar baar call kar sako

```javascript
// Function banana
function greet(name) {
  console.log("Hello " + name);
}

// Function call karna
greet("Rahul");   // Hello Rahul
greet("Priya");   // Hello Priya
```

### Return value wala function:
```javascript
function add(a, b) {
  return a + b;
}

let result = add(5, 3);
console.log(result);   // 8
```

---

## 6. DOM Manipulation

- DOM = **Document Object Model**
- JS se HTML elements ko change karna

```
HTML page load hota hai
        ↓
Browser DOM tree banata hai
        ↓
JS DOM ko read/change kar sakta hai ✅
```

### Elements Select Karo:
```javascript
// ID se
let title = document.getElementById("myTitle");

// Class se
let items = document.getElementsByClassName("item");

// CSS selector se (most used ✅)
let btn = document.querySelector("#myBtn");
```

### Content Change Karo:
```javascript
// Text change karo
document.getElementById("myTitle").innerText = "New Title!";

// HTML change karo
document.getElementById("box").innerHTML = "<b>Bold text</b>";

// Style change karo
document.getElementById("box").style.color = "red";
```

### Events (Button Click etc.):
```javascript
// Button click pe function chalao
document.getElementById("myBtn").addEventListener("click", function() {
  alert("Button dabaya!");
});
```

```html
<!-- HTML mein directly bhi likh sakte ho -->
<button onclick="alert('Hello!')">Click Me</button>
```

---

## 7. Quick Revision

```
JavaScript = Web pages ko interactive banana
let/const  = Variables declare karna
String     = Text data → "Hello"
Number     = Numeric data → 42
Boolean    = True/False
if-else    = Condition check karna
for loop   = Baar baar kuch karna
Function   = Reusable code block
DOM        = HTML ko JS se control karna
Event      = Click, hover jaise actions
console.log= Output print karna (debugging)
```

### Comparison Operators:
```javascript
==   → Equal (value)        5 == "5"  → true
===  → Strict equal         5 === "5" → false ✅
!=   → Not equal
>    → Greater than
<    → Less than
>=   → Greater or equal
<=   → Less or equal
```

---

*Notes by: IT Student*
*Topic: Web Technology — Part 2: JavaScript*
*Phase 7 of IT Learning Path 🌐*
