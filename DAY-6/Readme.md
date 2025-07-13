## 📘 Day 6: Introduction to CSS – Inline, Internal, External CSS & Selectors

---

### 🎯 Objective

Understand how to apply CSS (Cascading Style Sheets) to web pages using:
- ✅ Inline
- ✅ Internal
- ✅ External styles
Learn how to use **selectors** to style HTML elements effectively.

---

### 🔹 Key Learning Outcomes

- What CSS is and how it works
- Difference between **inline**, **internal**, and **external CSS**
- Understanding **CSS syntax**
- Use of **selectors** to apply styling

---

### 🧠 1. What is CSS?

CSS is a **styling language** used to control the visual presentation of HTML elements on a webpage.

#### ✅ Basic Syntax
```css
selector {
  property: value;
}
```

#### 💡 Example:
```css
h1 {
  color: blue;
  font-size: 36px;
}
```

- **Selector**: `h1`
- **Properties**: `color`, `font-size`
- **Values**: `blue`, `36px`

---

### 🎨 2. Types of CSS Application

#### 🟢 Inline CSS
- Written inside the HTML element using the `style` attribute
```html
<h1 style="color: blue; font-size: 36px;">Welcome</h1>
```

#### 🟡 Internal CSS
- Written inside a `<style>` tag in the `<head>` section
```html
<head>
  <style>
    h1 {
      color: blue;
      font-size: 36px;
    }
  </style>
</head>
```

#### 🔵 External CSS
- Written in a separate `.css` file and linked with `<link>`
```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```
**styles.css**
```css
h1 {
  color: blue;
  font-size: 36px;
}
```

---

### 📊 3. CSS Selectors

Selectors target HTML elements to apply styles.

#### ✅ Element Selector
```css
p {
  color: black;
}
```

#### ✅ Class Selector
```html
<p class="highlight">This is important</p>
```
```css
.highlight {
  color: red;
}
```

#### ✅ ID Selector
```html
<h1 id="main-title">Hello</h1>
```
```css
#main-title {
  font-size: 40px;
}
```

#### ✅ Universal Selector
```css
* {
  font-family: Arial;
}
```

#### ✅ Descendant Selector
```css
div p {
  color: green;
}
```

#### ✅ Pseudo-class Selector
```css
a:hover {
  color: red;
}
```

#### ✅ Pseudo-element Selector
```css
p::first-letter {
  font-size: 2em;
}
```

---

### 🔧 Hands-on Exercise

Create a webpage that includes:
- A header with an **ID selector**
- A navigation bar using **class selectors** for each link
- A footer using **inline CSS**
- An external `.css` file for overall styling (backgrounds, padding, fonts)

---

### 💻 Sample HTML File
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Day 6 - CSS Practice</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header id="main-header">
    <h1>Welcome to My Page</h1>
  </header>

  <nav>
    <a class="nav-link" href="#">Home</a>
    <a class="nav-link" href="#">About</a>
    <a class="nav-link" href="#">Contact</a>
  </nav>

  <footer style="text-align:center; background-color:#eee; padding:10px;">
    <p>© 2025 MyWebsite</p>
  </footer>
</body>
</html>
```

---

### 🎨 Sample `style.css`
```css
/* External CSS */

body {
  font-family: Arial, sans-serif;
  background-color: #f0f8ff;
  padding: 20px;
}

#main-header {
  color: navy;
  text-align: center;
}

.nav-link {
  margin-right: 15px;
  text-decoration: none;
  color: darkslategray;
}

.nav-link:hover {
  color: crimson;
}
```

---

### ✅ Key Takeaways

- CSS adds visual style to your web pages
- Use **inline** for quick fixes, **internal** for small pages, and **external** for scalability
- Learn and practice **selectors** to style HTML elements
- Combine different CSS methods smartly for better maintainability

---

### 📝 Homework

Create your own webpage using:
- A header styled using **ID**
- Navigation links styled using **classes**
- An external CSS file to control layout and fonts
- Inline CSS in the footer
- Experiment with **pseudo-classes** and **pseudo-elements**

> 💡 Bonus: Try using `:hover`, `:focus`, `::first-letter`, and `::after`

---

