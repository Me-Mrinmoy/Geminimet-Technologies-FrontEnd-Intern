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

---

## 🔹 HTML Images

```html
<img src="https://via.placeholder.com/150" alt="Placeholder Image">
```

### 📝 Description:

- `src`: The **URL or file path** of the image to display.
- `alt`: The **fallback text** shown if the image fails to load (also helps with screen readers and SEO).

### 🛠 Challenge:

Add an image of your choice and make it **clickable** using the format below:

```html
<a href="https://your-link.com" target="_blank">
  <img src="your-image.jpg" alt="Description">
</a>
```

---

## 🔹 HTML Tables

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>22</td>
  </tr>
  <tr>
    <td>Bob</td>
    <td>25</td>
  </tr>
</table>
```

### 📝 Description:

- `<table>`: Wraps the entire table.
- `<tr>`: Defines a **table row**.
- `<th>`: Table **header cell**, bold and centered by default.
- `<td>`: Table **data cell**, contains actual values.

### 🛠 Try it:

Create your own HTML table showing:

✅ Your **weekly class schedule**  
✅ A **list of favorite books**, including title and author  
✅ Or a table of any **structured data** you like!

### 💡 Example:

```html
<table border="1">
  <tr>
    <th>Day</th>
    <th>Subject</th>
  </tr>
  <tr>
    <td>Monday</td>
    <td>Web Development</td>
  </tr>
  <tr>
    <td>Tuesday</td>
    <td>Data Structures</td>
  </tr>
</table>
```

---

## 🔹 HTML Forms (Introduction)

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <br><br>
  <input type="submit" value="Submit">
</form>
```

### 📝 Description:

- `<form>`: Container for **collecting user input**
- `<label>`: Describes the **input field**
- `<input>`: Allows the user to **enter data**  
  Common types: `text`, `email`, `password`

✳️ More input types like `<textarea>`, **radio buttons**, and **dropdowns** will be introduced later.

### 🛠 Try it:

Build a basic form on your HTML page with the following:

✅ A **Name** input field  
✅ An **Email** input field  
✅ A **Submit** button

### 💡 Example:

```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name"><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>

  <input type="submit" value="Submit">
</form>
```

---

## 🔹 Semantic HTML (Intro)

```html
<header>
  <h1>My Blog</h1>
</header>
<main>
  <section>
    <h2>Latest Posts</h2>
    <p>Welcome to my blog...</p>
  </section>
</main>
```

### 📝 Description:

Semantic HTML elements describe their meaning **clearly** to both developers and browsers:

- `<header>`: Intro or branding section  
- `<main>`: Primary content area  
- `<section>`: Thematic grouping of content

These tags improve:

✅ **SEO**  
✅ **Accessibility**  
✅ **Code readability**

### 🛠 Try it:

Structure your page using semantic tags such as:

- `<header>`
- `<main>`
- `<section>`
- `<footer>`

### 💡 Example:

```html
<header>
  <h1>My Portfolio</h1>
</header>

<main>
  <section>
    <h2>About Me</h2>
    <p>I am learning web development!</p>
  </section>

  <section>
    <h2>Projects</h2>
    <p>Check out some of my work.</p>
  </section>
</main>

<footer>
  <p>&copy; 2025 Mrinmoy</p>
</footer>
```

---

## 🔹 Final Activity

🎯 **Build a Simple Profile Page**

Include the following elements in your HTML page:

- `<h1>` with your **name**
- `<p>` introducing yourself
- `<ul>` listing your **hobbies**
- `<img>` of yourself or a placeholder image
- `<a>` linking to your **favorite website**
- `<table>` showing your **weekly schedule**

💾 **Save the file as** `profile.html` and open it in your browser to see your creation!

---

## 🏁 Wrap-Up & Homework

### ✅ Review

Today, you learned:

- 📄 Basic **HTML structure**
- 📝 How to use **headings**, **paragraphs**, and **lists**
- 🔗 How to add **links**, **images**, **tables**, and **forms**
- 🧱 An **introduction to semantic HTML**

---

### 🏠 Homework

✍️ **Create a second page:**

- File name: `about.html`  
- Content: Info about your **interests**
- ✅ Link it from `profile.html` using an `<a>` tag

🔍 **Explore:**

- Visit **2–3 websites**
- Use **Right Click → View Page Source**
- Observe how they structure their HTML code

---
