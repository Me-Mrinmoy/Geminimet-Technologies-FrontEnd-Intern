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
