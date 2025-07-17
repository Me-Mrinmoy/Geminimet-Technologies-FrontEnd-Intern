# 💡 Day 11: Flexbox

## 🎯 Objective

By the end of this session, trainees will:

* Understand the basics of Flexbox, one of the most powerful and flexible layout systems in CSS.
* Learn how to create a flex container and manipulate its flex items.
* Master the key Flexbox properties: `flex-direction`, `flex-wrap`, `justify-content`, and `align-items`, enabling them to create complex, flexible layouts that adapt to various screen sizes.

---

## 🔹 Introduction to Flexbox

Flexbox, short for **Flexible Box**, is a CSS layout model designed to create responsive and dynamic layouts. It allows elements to grow, shrink, and align themselves within a container, making it an essential tool for modern web design.

The primary idea behind Flexbox is that it gives you control over the **alignment and spacing of elements** within a container, even when the size of the elements is unknown or dynamic.

---

## 🔹 Key Concepts in Flexbox

### ✅ Flex Container

The **parent element** that holds the flex items. By applying `display: flex` to a container, all its direct child elements automatically become flex items.

```css
.container {
  display: flex;
}
```

### ✅ Flex Items

The **direct child elements** of the flex container. These items can be arranged and aligned according to various properties provided by Flexbox.

---

## 🔹 Flexbox Properties for the Container

### 1. `flex-direction` (Direction of Items)

Defines the direction in which the flex items are laid out inside the flex container.

**Values:**

* `row` *(default)* – Left to right
* `row-reverse` – Right to left
* `column` – Top to bottom
* `column-reverse` – Bottom to top

```css
.container {
  display: flex;
  flex-direction: row;
}
```

### 2. `flex-wrap` (Wrapping Items)

Controls whether the items should wrap onto multiple lines.

**Values:**

* `nowrap` *(default)* – No wrapping
* `wrap` – Wrap to next line
* `wrap-reverse` – Wrap in reverse order

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

### 3. `justify-content` (Horizontal Alignment)

Aligns flex items along the main axis.

**Values:**

* `flex-start` *(default)*
* `flex-end`
* `center`
* `space-between`
* `space-around`
* `space-evenly`

```css
.container {
  display: flex;
  justify-content: center;
}
```

### 4. `align-items` (Vertical Alignment)

Aligns flex items along the cross axis.

**Values:**

* `flex-start`
* `flex-end`
* `center`
* `baseline`
* `stretch` *(default)*

```css
.container {
  display: flex;
  align-items: center;
}
```

---

## 🔹 Flexbox Properties for the Items

### 1. `flex-grow` (Item Growth)

Defines how much an item grows relative to others.

```css
.item {
  flex-grow: 1;
}
```

### 2. `flex-shrink` (Item Shrinking)

Defines how much an item shrinks relative to others.

```css
.item {
  flex-shrink: 1;
}
```

### 3. `flex-basis` (Initial Size)

Defines the initial size before space distribution.

```css
.item {
  flex-basis: 200px;
}
```

---

## 🔹 Combining Flexbox Properties

Create a centered, responsive layout:

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

.item {
  flex-grow: 1;
  flex-basis: 200px;
}
```

---

## 🔹 Practical Exercise

1. Create a flex container and several flex items.
2. Use `flex-direction` to arrange them horizontally or vertically.
3. Experiment with `justify-content` and `align-items`.
4. Use `flex-wrap` for responsive behavior.

---

## ✅ Summary

Trainees now understand:

* What Flexbox is and how it works.
* How to control direction, wrapping, and alignment.
* How to use grow/shrink/basis on items.

Flexbox is now part of their modern CSS toolbox for creating flexible, responsive layouts.

---

## 📁 Project Repository Structure

```
Day11-Flexbox/
├── index.html
├── styles.css
└── README.md
```

---
