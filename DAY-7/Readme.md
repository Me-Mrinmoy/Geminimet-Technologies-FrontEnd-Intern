# 🌈 Day 7: Colors, Fonts, Text Styling, Backgrounds

## 🎯 Objective
By the end of this session, you will:
- Understand how to apply **colors**, **fonts**, and **text styles** in CSS.
- Learn how to manage **background properties** to enhance design.
- Gain hands-on experience applying these styles to a webpage.

---

## 🔹 Part 1: Colors in CSS

### 🎨 CSS Color Notations

| Type        | Example                        |
|-------------|--------------------------------|
| Named       | `color: red;`                  |
| Hex         | `color: #FF5733;`              |
| RGB         | `color: rgb(255, 87, 51);`     |
| RGBA        | `color: rgba(255, 87, 51, 0.5);`|
| HSL         | `color: hsl(9, 100%, 60%);`     |

### 💡 Example
```css
body {
  background-color: #f0f0f0;
  color: #333;
}

h1 {
  color: rgb(255, 87, 51);
}

p {
  color: rgba(0, 128, 128, 0.8);
}
```

---

## 🔹 Part 2: Fonts in CSS

### 🔠 Font Family
```css
body {
  font-family: Arial, sans-serif;
}
```

Using Google Fonts:
```html
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```
```css
body {
  font-family: 'Roboto', sans-serif;
}
```

### 📏 Font Size, Weight & Style
```css
h1 {
  font-size: 2em;
  font-weight: bold;
}

p {
  font-size: 16px;
  font-style: italic;
}
```

---

## 🔹 Part 3: Text Styling

### ✍️ Text Alignment
```css
h1 {
  text-align: center;
}
```

### ✨ Text Decoration
```css
a {
  text-decoration: none;
}
```

### 🔤 Text Transform
```css
h2 {
  text-transform: uppercase;
}
```

### 🔡 Letter Spacing & Line Height
```css
h1 {
  letter-spacing: 2px;
  line-height: 1.5;
}
```

### 🖍️ Text Shadow
```css
h1 {
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}
```

---

## 🔹 Part 4: Backgrounds in CSS

### 🎨 Background Color
```css
body {
  background-color: #f4f4f4;
}
```

### 🖼️ Background Image
```css
body {
  background-image: url('background.jpg');
  background-size: cover;
}
```

### 🔧 Background Properties
```css
body {
  background-image: url('background.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
```

---

## ✅ Mini Project: Product Landing Page

### 📋 Requirements
- Use **Google Fonts**
- Style **headings** and **paragraphs**
- Add **backgrounds** (color or image)
- Layout includes:
  - A **header** with product title
  - A **description section** with image and CTA button
  - Proper **spacing, alignment, and visual hierarchy**

---

## 🧠 Summary

By completing Day 7, you learned:

✅ How to apply **colors** using various formats  
✅ How to style **text** with fonts, spacing, and alignment  
✅ How to use **background properties** for better design  
✅ How to create a visually engaging and readable webpage using CSS  

---
