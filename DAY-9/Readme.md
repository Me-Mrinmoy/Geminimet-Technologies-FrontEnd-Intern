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

```html
<img src="https://via.placeholder.com/120" class="float-left">
<p>This text wraps around the image floated to the left.</p>
```
