# 💻 Day 9: Display Types, Float & Clear, Positioning (Static, Relative, Absolute, Fixed)

---

## 🎯 Objective

By the end of this session, you will:

- Understand different **display properties** and their impact on layout.
- Use **float** and **clear** to control wrapping and layout.
- Master **positioning** with `static`, `relative`, `absolute`, `fixed`, and `sticky`.

---

## 🔹 Part 1: Display Types

The `display` property in CSS controls how elements are rendered in the document flow.

### 1️⃣ Block Element

```html
<div>This is a block element</div>
div {
  display: block;
}
```

## 2️⃣ Inline Element

Displays the element inline — it takes only as much width as needed and does **not** start on a new line.

### 🧪 HTML
```html
<p>This is an <span>inline span</span> inside a paragraph.</p>
```

### ✅ CSS
```css
span {
  display: inline;
  background-color: lightblue;
  padding: 5px;
}
```

## 3️⃣ Inline-Block Element

Behaves like an inline element but allows setting `width` and `height`.

Useful for buttons and styled inline components.


#### ✅ HTML
```html
<button>Click Me</button>
```

### ✅ CSS
```css
button {
  display: inline-block;
  width: 120px;
  height: 40px;
  background-color: lightgreen;
  border: none;
  margin-top: 10px;
}
```

## 4️⃣ Display: None

Hides the element completely.  
It will not appear in the layout and won't occupy any space.

#### ✅ HTML
```html
<p>This paragraph is visible.</p>
<p class="hidden">This paragraph is hidden using display: none.</p>
```

### ✅ CSS
```css
.hidden {
  display: none;
}
```

## 🔹 Part 2: Float & Clear

The `float` property is used to align elements to the **left** or **right** within their container.  
The `clear` property prevents floated elements from affecting the layout of other elements.

### ✅ Float Left

The element floats to the **left**, and other content wraps around it.

### ✅ HTML
```html
<img src="https://via.placeholder.com/120" class="float-left">
<p>This text wraps around the image floated to the left.</p>
```

### ✅ CSS
```css
.float-left {
  float: left;
  margin: 10px;
}
```

### ✅ Float Right

The element floats to the **right**, and other content wraps to the **left**.

#### ✅ HTML
```html
<img src="https://via.placeholder.com/120" class="float-right">
<p>This text wraps around the image floated to the right.</p>
```

### ✅ CSS
```css
.float-right {
  float: right;
  margin: 10px;
}
```

### ✅ Float None (Default)

The element does **not float** and behaves like a normal block or inline element.

#### ✅ HTML
```html
<p class="float-none">This element has no float applied.</p>
```

### ✅ CSS
```css
.float-none {
  float: none;
}
```

### ✅ Clear Property

The `clear` property ensures that an element appears **below floated elements** and doesn't wrap beside them.

#### ✅ HTML
```html
<div class="clear"></div>
<footer>This is a footer. It appears below floated content.</footer>
```

### ✅ CSS
```css
.clear {
  clear: both;
}
```

---

## 🧪 Hands-On Activity: Float Left + Clear Footer

Create a layout where:

- An image is floated to the left
- Text wraps around it
- Footer appears below using `clear: both`

---

### ✅ Solution

### ✅ HTML
```html
<div>
  <img src="https://via.placeholder.com/150" class="float-left" alt="Floating Image" />
  <p>
    This paragraph wraps around the floated image. Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
    Suspendisse dignissim nunc in orci faucibus, in malesuada nisl sodales. Curabitur imperdiet libero ut enim.
  </p>
</div>

<div class="clear"></div>

<footer>
  <p>This is the footer section. It appears below the floated image.</p>
</footer>
```

### ✅ CSS
```css
.float-left {
  float: left;
  margin-right: 15px;
  margin-bottom: 10px;
}

.clear {
  clear: both;
}

footer {
  background-color: #f2f2f2;
  padding: 10px;
  margin-top: 20px;
  font-weight: bold;
}
```

---

## 🔹 Part 3: Positioning in CSS

The `position` property determines how an element is positioned in the document or relative to its parent container.

### 1️⃣ Static Positioning (Default)

- Elements follow the normal document flow.
- Cannot be offset using `top`, `right`, `bottom`, or `left`.

#### 🎨 CSS
```css
div {
  position: static; /* Default */
}
```

### 2️⃣ Relative Positioning

- Stays in the normal document flow.
- You can move it using `top`, `left`, `right`, or `bottom`.
- Other elements are **not affected** by its new position.

#### ✅ HTML
```html
<div class="relative">I'm relatively positioned</div>
```

#### 🎨 CSS
```css
.relative {
  position: relative;
  top: 10px;
  left: 20px;
  background-color: lightyellow;
  padding: 10px;
}
```

### 3️⃣ Absolute Positioning

- Removed from the normal document flow.
- Positioned relative to the **nearest ancestor** with `position: relative`, `absolute`, or `fixed`.
- If no such ancestor exists, it’s positioned relative to the **viewport** or `<body>`.

#### ✅ HTML
```html
<div class="parent">
  <div class="absolute">Absolutely Positioned Box</div>
</div>
```

#### 🎨 CSS
```css
.parent {
  position: relative;
  height: 200px;
  background-color: #eee;
}

.absolute {
  position: absolute;
  top: 30px;
  right: 50px;
  background-color: lightcoral;
  padding: 10px;
}
```

### 4️⃣ Fixed Positioning

- Removed from the document flow.
- Stays **fixed relative to the viewport**, even when the page is scrolled.

#### ✅ HTML
```html
<div class="fixed-header">Fixed Header</div>
```

#### 🎨 CSS
```css
.fixed-header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #333;
  color: white;
  padding: 15px;
  text-align: center;
  z-index: 1000;
}
```

### 5️⃣ Sticky Positioning

- Acts like `relative` until the element reaches a defined **scroll position**.
- Then it becomes **stuck** like `fixed`, remaining visible at that position.

#### ✅ HTML
```html
<nav class="sticky-nav">Sticky Navigation</nav>
```

#### 🎨 CSS
```css
.sticky-nav {
  position: sticky;
  top: 0;
  background-color: lightblue;
  padding: 10px;
  border-bottom: 1px solid #ccc;
}
```

## 🧪 Hands-On Activity: Float, Clear, Positioning

### ✅ Layout Overview

- Sidebar floated to the left.
- Content wrapped beside it with `clear` used to prevent overlap.
- Positioned box inside a container (`relative` + `absolute`).
- Fixed header at the top of the page.

### ✅ Solution
### ✅ HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Positioning Activity</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <div class="fixed-header">🔝 Fixed Header</div>

  <div class="sidebar">📚 Sidebar</div>

  <div class="content">
    <h2>Main Content Area</h2>
    <p>This section sits beside the floated sidebar. Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
    
    <div class="relative-box">
      This box is <strong>relative</strong>
      <div class="absolute-box">I'm absolutely positioned</div>
    </div>
  </div>

  <div class="clear"></div>

  <footer>
    <p>Footer - below all floated and positioned elements.</p>
  </footer>

</body>
</html>
```

#### 🎨 CSS
```css
body {
  font-family: sans-serif;
  margin: 0;
  padding-top: 60px;
}

.fixed-header {
  position: fixed;
  top: 0;
  left: 0;
  background-color: #333;
  color: #fff;
  width: 100%;
  text-align: center;
  padding: 15px;
  z-index: 1000;
}

.sidebar {
  float: left;
  width: 200px;
  background-color: #f0f0f0;
  padding: 15px;
  height: 300px;
}

.content {
  margin-left: 220px;
  padding: 20px;
  background-color: #fff;
}

.clear {
  clear: both;
}

footer {
  background-color: #ddd;
  padding: 15px;
  text-align: center;
  margin-top: 20px;
}

.relative-box {
  position: relative;
  background-color: lightyellow;
  padding: 30px;
  margin-top: 20px;
}

.absolute-box {
  position: absolute;
  top: 10px;
  right: 10px;
  background-color: lightcoral;
  padding: 10px;
  font-size: 0.9em;
}
```

---

## 🎯 Mini Project: Styled Product Landing Page (Positioning Focus)

This mini project demonstrates how to use different CSS `position` properties and `display` techniques in a real-world layout like a product landing page.

### 🛠️ Task Breakdown

✅ Use **relative positioning** for elements that should shift slightly.  
✅ Use **absolute positioning** for a floating action button inside a container.  
✅ Use **fixed positioning** for a navigation bar that stays at the top during scroll.

#### ✅ Solution
#### ✅ HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Product Landing Page</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <header class="navbar">🚀 My Product</header>

  <section class="hero-section">
    <h1 class="tagline">Innovate with Confidence</h1>
    <p>Empower your productivity with our latest tech.</p>

    <div class="cta-container">
      <button class="cta-button">Buy Now</button>
    </div>
  </section>

  <footer>
    <p>© 2025 Mrinmoy Samanta. All rights reserved.</p>
  </footer>

</body>
</html>
```

#### 🎨 CSS
```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding-top: 70px;
  background-color: #f9f9f9;
}

.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #333;
  color: white;
  padding: 20px;
  text-align: center;
  font-weight: bold;
  z-index: 1000;
}

.hero-section {
  background-color: white;
  padding: 100px 20px;
  text-align: center;
  position: relative;
}

.tagline {
  position: relative;
  top: 5px; /* Slight movement using relative */
  font-size: 2rem;
  color: #444;
}

.cta-container {
  position: relative;
  height: 200px;
  margin-top: 40px;
  background-color: #f1f1f1;
}

.cta-button {
  position: absolute;
  bottom: 20px;
  right: 20px;
  padding: 15px 30px;
  background-color: #28a745;
  color: white;
  border: none;
  font-size: 1rem;
  border-radius: 5px;
  cursor: pointer;
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #ddd;
  margin-top: 60px;
}
```

---

## 🎯 Summary (Day 9)

By the end of **Day 9**, you've gained practical knowledge of:

### 🧱 Display Types

- `block`: Starts on a new line, takes full width  
- `inline`: Flows within text, no width/height control  
- `inline-block`: Like inline, but supports width & height  
- `none`: Hides the element completely from layout

### 📐 Float & Clear

- `float: left | right`: Aligns elements beside text or other elements  
- `clear: both`: Ensures next elements start below floated content

### 📍 CSS Positioning

- `static`: Default positioning in the normal document flow  
- `relative`: Moves element slightly from its original position  
- `absolute`: Removed from flow, positioned inside nearest `relative`/`absolute`/`fixed` ancestor  
- `fixed`: Always stays in the same place relative to the viewport  
- `sticky`: Acts like `relative` until a scroll point, then sticks like `fixed`

✅ You now have the **foundation** to build **advanced, responsive layouts** using CSS layout systems like Flexbox and Grid.

🚀 Keep building, keep experimenting!
