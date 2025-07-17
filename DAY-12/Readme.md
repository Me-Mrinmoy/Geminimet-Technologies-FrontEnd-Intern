## 📅 Day 12: Grid Layout

### 🎯 Objective:

By the end of this session, trainees will:

* Understand the basics of CSS Grid Layout, one of the most powerful and complex layout systems in CSS.
* Learn how to create a grid container and manipulate grid items.
* Master the use of `grid-template-areas`, `grid-template-columns`, `grid-template-rows`, and other properties to create highly customizable, flexible grid layouts.

---

### 🔹 Introduction to CSS Grid:

CSS Grid Layout is a two-dimensional layout system that allows you to create complex, flexible grid-based designs. Unlike Flexbox, which is primarily for one-dimensional layouts (either in a row or column), Grid allows you to create both rows and columns simultaneously, giving you greater control over the structure of your layout.

With Grid, you can define the size of the grid, place items into specific areas, and create complex layouts using a simple set of CSS properties. It works seamlessly across both large and small screen sizes, making it ideal for responsive design.

---

### 🔹 Key Concepts in CSS Grid:

#### 🧩 Grid Container:

The parent element that holds the grid items. To create a grid layout, the parent element must be designated as a grid container by applying the `display: grid` property.

```css
.container {
    display: grid;
}
```

#### 🧩 Grid Items:

The child elements of the grid container are the grid items. These items can be placed in any part of the grid, spanning across rows and columns as needed.

---

### 🔹 Grid Layout Properties for the Container:

#### 🔧 `grid-template-columns`:

Defines the number and size of the columns in the grid.

```css
.container {
  grid-template-columns: 200px 1fr 2fr;
}
```

* You can use absolute units (px), relative units (%), or flexible units (fr).

#### 🔧 `grid-template-rows`:

Defines the number and size of the rows in the grid.

```css
.container {
  grid-template-rows: 100px auto 1fr;
}
```

* Use `auto` to allow the row height to adjust based on content.

#### 🔧 `grid-template-areas`:

Lets you name grid areas and assign them to grid items.

```css
.container {
  grid-template-areas:
    "header header"
    "sidebar content";
}
```

* Items are then placed using `grid-area: name;`

#### 🔧 `grid-gap` or `gap`:

Sets spacing between rows and columns.

```css
.container {
  gap: 20px; /* shorthand for row-gap and column-gap */
}
```

---

### 🔹 Key Topics:

#### ✅ Creating a Grid Container

```css
.container {
  display: grid;
}
```

#### ✅ Defining Rows and Columns

```css
.container {
  display: grid;
  grid-template-columns: 200px 200px 200px;
  grid-template-rows: 100px 100px;
}
```

* You can use fractional units (`fr`) to distribute space.

```css
grid-template-columns: 1fr 2fr 1fr;
```

#### ✅ Grid Gap

```css
grid-gap: 20px;
/* or */
gap: 20px;
```

#### ✅ Placing Grid Items

```css
.item1 {
  grid-column: 1 / 3; /* Starts at column 1, ends before column 3 */
  grid-row: 1 / 2;
}
```

#### ✅ Named Areas (Optional)

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content";
}

.header {
  grid-area: header;
}
.sidebar {
  grid-area: sidebar;
}
.content {
  grid-area: content;
}
```

---

### 🔹 Positioning Grid Items:

Now that the grid container is set up, you can position the grid items using the following methods:

#### 1. `grid-column` (Positioning Along Columns):

The `grid-column` property defines where an item starts and ends along the columns of the grid.

```css
grid-column: start / end;
```

* `start`: The column where the item starts.
* `end`: The column where the item ends.

Example:

```css
.item {
    grid-column: 1 / 3; /* Item will span from column 1 to column 3 */
}
```

This example means the grid item will span across columns 1 and 2, covering the first two columns of the grid.

#### 2. `grid-row` (Positioning Along Rows):

The `grid-row` property works similarly to `grid-column`, but for rows. It defines where the item starts and ends along the rows of the grid.

```css
grid-row: start / end;
```

* `start`: The row where the item starts.
* `end`: The row where the item ends.

Example:

```css
.item {
    grid-row: 1 / 2; /* Item will span from row 1 to row 2 */
}
```

This example places the item in the first row, spanning just that row.

---

### 💻 Practice Task:

✅ **Task:** Create a 2x3 grid layout with six boxes:

* First row: spans three columns
* Second row: three equally divided columns

✅ **Bonus:** Add padding and background colors to each grid item.

---

### 🧠 Summary:

* CSS Grid provides powerful 2D layout control.
* Use `grid-template-columns` and `grid-template-rows` to define structure.
* Use `grid-gap`, `grid-area`, and `grid-column/row` for customization.
* Combine Grid and Flexbox for complex responsive designs.

---

### ✅ Additional Resources:

* [CSS Grid Guide by MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
* [Grid Garden Game](https://cssgridgarden.com/)
* [CSS Tricks Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)

---
