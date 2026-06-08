# 🌐 Web Technology - HTML & CSS
> IT Student Notes | Topic: Web Tech Fundamentals — Part 1

---

## 📌 Table of Contents
1. [Web Kaise Kaam Karta Hai](#1-web-kaise-kaam-karta-hai)
2. [HTML Kya Hai](#2-html-kya-hai)
3. [HTML Structure](#3-html-structure)
4. [Important HTML Tags](#4-important-html-tags)
5. [CSS Kya Hai](#5-css-kya-hai)
6. [CSS Basics](#6-css-basics)
7. [Quick Revision](#7-quick-revision)

---

## 1. Web Kaise Kaam Karta Hai

```
Tu URL type karta hai
        ↓
Browser → Internet → Server
        ↓
Server HTML/CSS/JS file bhejta hai
        ↓
Browser screen pe render karta hai ✅
```

### Key Players:

| Term | Matlab | Example |
|------|--------|---------|
| **Browser** | Web pages dikhane wala software | Chrome, Firefox |
| **Server** | Files store karne wali machine | Apache, Nginx |
| **URL** | Web address | https://google.com |
| **HTML** | Page ka structure | Skeleton |
| **CSS** | Page ki styling | Kapde/Look |
| **JavaScript** | Page ki functionality | Actions |

---

## 2. HTML Kya Hai

- HTML = **HyperText Markup Language**
- Web page ka **structure** define karta hai
- HTML **tags** use karta hai
- Browser HTML padhta hai aur page dikhata hai

```
HTML = Web page ka skeleton/dhanche
CSS  = Uski dress/style
JS   = Uski movement/actions
```

---

## 3. HTML Structure

```html
<!DOCTYPE html>          ← HTML5 document hai
<html>                   ← Page shuru
  <head>                 ← Browser info (user ko nahi dikhta)
    <title>My Page</title>
  </head>
  <body>                 ← Ye dikhta hai screen pe
    <h1>Hello World!</h1>
    <p>Yeh mera pehla page hai.</p>
  </body>
</html>                  ← Page khatam
```

### Head vs Body:

| | Head | Body |
|--|------|------|
| Visible | Nahi ❌ | Haan ✅ |
| Content | Title, CSS links | Text, Images, Buttons |
| Example | `<title>` | `<h1>`, `<p>` |

---

## 4. Important HTML Tags

### Text Tags:
```html
<h1>Sabse bada heading</h1>
<h2>Thoda chhota</h2>
<h3>Aur chhota</h3>
<p>Normal paragraph text</p>
<b>Bold text</b>
<i>Italic text</i>
<br>   ← Line break (closing tag nahi)
<hr>   ← Horizontal line
```

### Links & Images:
```html
<!-- Link -->
<a href="https://google.com">Google pe jao</a>

<!-- Image -->
<img src="photo.jpg" alt="Meri photo">
```

### Lists:
```html
<!-- Unordered (bullet) List -->
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<!-- Ordered (numbered) List -->
<ol>
  <li>Pehle HTML sikho</li>
  <li>Phir CSS</li>
</ol>
```

### Table:
```html
<table>
  <tr>                  ← Table Row
    <th>Name</th>       ← Table Header
    <th>Age</th>
  </tr>
  <tr>
    <td>Rahul</td>      ← Table Data
    <td>20</td>
  </tr>
</table>
```

### Form:
```html
<form>
  <input type="text" placeholder="Name likho">
  <input type="password" placeholder="Password">
  <input type="email" placeholder="Email">
  <button type="submit">Submit</button>
</form>
```

### Layout Tags (HTML5):
```html
<header>   ← Page ka upar wala hissa
<nav>      ← Navigation menu
<main>     ← Main content
<section>  ← Ek section
<footer>   ← Page ka niche wala hissa
<div>      ← Generic container
<span>     ← Inline container
```

---

## 5. CSS Kya Hai

- CSS = **Cascading Style Sheets**
- HTML elements ko **style** karna
- Color, size, position sab CSS se hota hai

### CSS 3 Tarike se Use Karo:

```html
<!-- 1. Inline (directly tag mein) -->
<p style="color: red;">Red text</p>

<!-- 2. Internal (head mein) -->
<style>
  p { color: blue; }
</style>

<!-- 3. External (alag file) ← Best practice ✅ -->
<link rel="stylesheet" href="style.css">
```

---

## 6. CSS Basics

### CSS Syntax:
```css
selector {
  property: value;
}

/* Example: */
h1 {
  color: red;
  font-size: 24px;
}
```

### Selectors:
```css
/* Element selector */
p { color: black; }

/* Class selector (. se) */
.highlight { background: yellow; }

/* ID selector (# se) */
#main-title { font-size: 32px; }
```

```html
<!-- HTML mein use: -->
<p class="highlight">Yellow background</p>
<h1 id="main-title">Big title</h1>
```

### Common CSS Properties:
```css
/* Text */
color: red;
font-size: 16px;
font-weight: bold;
text-align: center;

/* Background */
background-color: blue;
background-image: url("bg.jpg");

/* Box */
width: 200px;
height: 100px;
padding: 10px;      ← Andar ki jagah
margin: 20px;       ← Bahar ki jagah
border: 1px solid black;
border-radius: 5px; ← Rounded corners

/* Display */
display: block;
display: flex;
display: none;      ← Chhupa do
```

### Box Model:
```
┌─────────────────────────┐
│         MARGIN          │  ← Bahar ki space
│  ┌───────────────────┐  │
│  │      BORDER       │  │  ← Line/border
│  │  ┌─────────────┐  │  │
│  │  │   PADDING   │  │  │  ← Andar ki space
│  │  │  ┌───────┐  │  │  │
│  │  │  │CONTENT│  │  │  │  ← Actual text/image
│  │  │  └───────┘  │  │  │
│  │  └─────────────┘  │  │
│  └───────────────────┘  │
└─────────────────────────┘
```

---

## 7. Quick Revision

```
HTML    = Web page ka structure (skeleton)
CSS     = Web page ki styling (look)
Tag     = HTML ka building block → <p>, <h1>
Element = Opening + Content + Closing tag
Selector= CSS mein kaunsa element style karo
Class   = . se select (.myClass)
ID      = # se select (#myId)
Margin  = Element ke bahar ki space
Padding = Element ke andar ki space
```

### HTML Tags Summary:
```
<h1>-<h6> → Headings
<p>       → Paragraph
<a>       → Link
<img>     → Image
<ul><li>  → Bullet list
<ol><li>  → Numbered list
<table>   → Table
<form>    → Form
<div>     → Container (block)
<span>    → Container (inline)
```

---

*Notes by: IT Student*
*Topic: Web Technology — Part 1: HTML & CSS*
*Phase 7 of IT Learning Path 🌐*
