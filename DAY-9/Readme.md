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
