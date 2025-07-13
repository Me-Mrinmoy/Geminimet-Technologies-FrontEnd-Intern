# 📅 Day 3: Lists, Tables & Forms

## 🎯 Objective

Learn how to structure and display data using lists and tables, and how to create interactive web forms for collecting user input.

---

## 🔹 PART 1: HTML LISTS

### ✅ 1. Ordered List (`<ol>`) – Numbered

Used when the order of items matters.

```html
<ol>
  <li>Wake up</li>
  <li>Brush teeth</li>
  <li>Have breakfast</li>
</ol>
```

📌 This will display:

* Wake up
* Brush teeth
* Have breakfast

---

### ✅ 2. Unordered List (`<ul>`) – Bulleted

Used when order doesn’t matter.

```html
<ul>
  <li>Apples</li>
  <li>Bananas</li>
  <li>Oranges</li>
</ul>
```

📌 This will display:

* Apples
* Bananas
* Oranges

---

### ✅ 3. Description List (`<dl>`) – Definitions

Useful for glossaries or key-value pairs.

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

### 🎯 Hands-On Task:

Create a webpage with:

* An ordered list of your daily tasks
* An unordered list of your favorite foods
* A description list explaining at least 3 web technologies

---

## 🔹 PART 2: HTML TABLES

### ✅ Basic Table Structure

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>24</td>
    <td>New York</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>30</td>
    <td>London</td>
  </tr>
</table>
```

### 🔍 Explanation:

* `<table>`: Wraps the entire table
* `<tr>`: Table row
* `<th>`: Table heading (bold, centered by default)
* `<td>`: Table data cell

### ✅ Table Formatting Tips

* Add borders using CSS or the `border` attribute
* Use `colspan` or `rowspan` to merge cells

```html
<td colspan="2">Combined Cell</td>
```

### 🎯 Hands-On Task:

Build a student report card table:

* Include columns: Name, Subject, Marks, Grade
* Use headings and at least 3 rows of data

---

## 🔹 PART 3: HTML FORMS

### ✅ Basic Form Syntax

```html
<form action="#" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="username">

  <label for="email">Email:</label>
  <input type="email" id="email" name="useremail">

  <input type="submit" value="Submit">
</form>
```

### ✅ Common Input Types

| Input Type | Usage                    |
| ---------- | ------------------------ |
| text       | Single-line text input   |
| email      | Email address            |
| password   | Password field (masked)  |
| number     | Numeric input            |
| radio      | Select one from multiple |
| checkbox   | Select multiple options  |
| submit     | Submit the form          |

### ✅ Form Elements

```html
<select name="country">
  <option value="india">India</option>
  <option value="usa">USA</option>
</select>
```

### ✅ Radio Buttons

```html
<p>Gender:</p>
<input type="radio" id="male" name="gender" value="male">
<label for="male">Male</label>

<input type="radio" id="female" name="gender" value="female">
<label for="female">Female</label>
```

### ✅ Checkboxes

```html
<p>Skills:</p>
<input type="checkbox" id="html" name="skill" value="HTML">
<label for="html">HTML</label>

<input type="checkbox" id="css" name="skill" value="CSS">
<label for="css">CSS</label>
```

### 🎯 Hands-On Task:

Create a form with:

* Text input for name
* Email input
* Password input
* Dropdown to select country
* Radio buttons for gender
* Checkboxes for skills
* A submit button

---

## 🔹 Bonus Styling Practice

Apply CSS to:

* Style list bullets, table borders, and headers
* Add spacing to form fields
* Highlight form labels
* Color alternating table rows using `nth-child`

```css
tr:nth-child(even) {
  background-color: #f2f2f2;
}
```

---

## ✅ Summary

Today you learned how to:

* ✅ Use different types of **lists** to organize content
* ✅ Create **tables** to display structured data
* ✅ Build **forms** to collect user input

These are core building blocks for creating real-world websites like survey pages, product listings, or sign-up pages.

---

## 📝 Homework

Create a webpage with:

* 📋 One **unordered list** of 5 hobbies
* ✅ One **ordered list** of your top 5 goals
* 🗓️ One **table** showing your weekly schedule
* 📬 A **form** titled "Contact Me" with inputs:

  * Name
  * Email
  * Message

### 🎨 Apply Basic CSS:

* Add colors, spacing, and background styling to enhance the appearance of your content.

Happy Coding! 💻
