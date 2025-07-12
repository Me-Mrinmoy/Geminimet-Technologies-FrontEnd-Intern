# 📘 Day 2: HTML Elements & Structure

## 🎯 Objective
Learn the building blocks of HTML and create a fully structured web page using various elements.

---

## 🔹 What is HTML?

HTML (**HyperText Markup Language**) is the standard language used to structure content on the web.

- It is a **markup language**, not a programming language.
- Uses **tags** like `<p>`, `<h1>`, `<img>`, etc., to define elements.
- Tags are typically enclosed in **opening** and **closing** pairs.

📌 **Example:**
```html
<p>This is a paragraph.</p>
```

---

## 🔹 Basic HTML Document Structure

All HTML documents follow a common structure:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Web Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
    <p>This is my first web page using HTML.</p>
  </body>
</html>
```

### 📝 Description of Each Element:

- `<!DOCTYPE html>`: Declares the document type and version of HTML (HTML5 in this case).
- `<html>`: The root element that wraps the entire HTML content.
- `<head>`: Contains meta-information such as the title, character set, styles, and links to resources (not displayed on the webpage).
- `<title>`: Sets the title of the page, which appears in the browser tab.
- `<body>`: Contains all the visible content on the web page such as headings, paragraphs, images, links, and more.

---

## 🔹 Headings

Headings define the structure and hierarchy of your content.

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Smaller Subheading</h3>
```

### 📝 Description:

- `<h1>` is the **most important heading** (usually the main title).
- `<h6>` is the **least important** and smallest in size.

**For best practices in SEO and accessibility:**
- ✅ Use **only one `<h1>`** per page.
- 🧠 Use `<h2>` to `<h6>` to organize content into sections and subsections.

### 🛠 Try it:

Add multiple headings to your HTML page (from `<h1>` to `<h6>`) and open it in your browser.  
Observe how their **size decreases** and how they help **organize content** visually.

---

## 🔹 Paragraphs

Use the `<p>` tag to define blocks of text content.

```html
<p>This is a paragraph of text.</p>
```

### 📝 Description:

- Paragraphs improve **readability** by grouping related sentences together.
- They automatically create **space between content blocks**, making your webpage cleaner and more structured.

---

## 🔹 Line Breaks & Horizontal Lines

HTML provides simple tags to control text layout and content separation.

### 🧩 Examples:

```html
<p>This is the first line.<br>This is the second line.</p>
<hr>
```

### 📝 Description:

- `<br>`: Inserts a **line break** inside a paragraph without starting a new one.  
  Useful when you want text to continue on a new line within the same block.
- `<hr>`: Inserts a **horizontal rule** (a thin line) to visually divide content or sections on the page.


### 🛠 Try it:

1. Add a `<br>` tag between two sentences inside a `<p>` element and view the result.
2. Insert a `<hr>` tag between two sections on your webpage to see a horizontal line.

---

## 🔹 HTML Lists

### 📌 Unordered List:

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

### 📌 Ordered List:

```html
<ol>
  <li>Login to the site</li>
  <li>Navigate to dashboard</li>
  <li>Start learning</li>
</ol>
```

### 📝 Description:

- `<ul>` creates a **bulleted list**
- `<ol>` creates a **numbered list**
- `<li>` represents each **item** in the list

### 🛠 Practice:

Create a **to-do list** on your HTML page using both `<ol>` and `<ul>` elements.

### 💡 Example:

```html
<h2>Today's To-Do List</h2>

<ol>
  <li>Wake up</li>
  <li>Check emails</li>
  <li>Complete HTML assignment</li>
</ol>

<h3>Technologies to Learn</h3>

<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

---

## 🔹 HTML Links

```html
<a href="https://www.google.com">Visit Google</a>
<a href="https://example.com" target="_blank">Open in New Tab</a>
```

### 📝 Description:

- `href`: Specifies the **URL** to navigate to when the link is clicked.
- `target="_blank"`: Opens the link in a **new browser tab**, allowing users to stay on your page.

### 🛠 Try it:

Create links to your favorite websites using the `<a>` tag.

### 💡 Example:

```html
<a href="https://www.github.com" target="_blank">Visit GitHub</a>
<a href="https://www.youtube.com" target="_blank">Watch YouTube</a>
```
