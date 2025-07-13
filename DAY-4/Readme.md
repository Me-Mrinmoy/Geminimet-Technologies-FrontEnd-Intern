## 🗓️ Day 4: Semantic HTML & Accessibility

---

### 🎯 Objective
- Understand **Semantic HTML** and why it improves code structure.
- Learn how to make your webpages more accessible to everyone, including users with disabilities.

---

### 🧱 PART 1: What is Semantic HTML?

Semantic HTML uses meaningful tags that describe the content.

| Semantic Tag     | Description                                |
|------------------|--------------------------------------------|
| `<header>`       | Top section of a page or section           |
| `<nav>`          | Navigation links                           |
| `<main>`         | Main content of the document               |
| `<section>`      | A standalone thematic grouping             |
| `<article>`      | Independent content like a blog post       |
| `<aside>`        | Sidebar or supplementary content           |
| `<footer>`       | Bottom section of a page                   |
| `<figure>` / `<figcaption>` | Images with captions          |
| `<time>`         | Represents time or date                    |

---

### 📝 Why Use Semantic HTML?
- ✅ Better SEO
- ✅ Better accessibility
- ✅ Cleaner, more maintainable code

---

### 🔁 Example Comparison

**🔴 Non-Semantic**
```html
<div id="top">Welcome</div>
<div class="nav">Home | About | Contact</div>
<div class="main-content">
  <div class="post">This is a blog post</div>
</div>
```

**🟢 Semantic HTML**
```html
<header>Welcome</header>
<nav>
  <a href="#">Home</a> | <a href="#">About</a> | <a href="#">Contact</a>
</nav>
<main>
  <article>This is a blog post</article>
</main>
```

---

### 🛠️ Hands-On Task
Create a layout with:
- `<header>` for a logo or page title
- `<nav>` with 3–4 links
- `<main>` containing 2 `<section>` blocks
- `<footer>` with your copyright

---

### ♿ PART 2: Accessibility (A11Y)

Accessibility = Making your website usable by people with:
- Visual or hearing impairments
- Motor challenges
- Cognitive limitations

---

### ✅ Accessibility Basics

#### 🖼️ Alt Text
```html
<img src="dog.jpg" alt="Golden Retriever playing with a ball">
```

#### 🏷️ Labels for Forms
```html
<label for="email">Email:</label>
<input type="email" id="email" name="email">
```

#### ⌨️ Keyboard Navigation
- Use semantic tags for buttons/links
- Avoid only relying on mouse interaction

#### 🎭 ARIA Roles (when necessary)
```html
<div role="alert">Form submission failed.</div>
```

#### 🎨 Color Contrast
Ensure good readability:
```css
color: #000;
background-color: #fff;
```

Use [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)

---

### 🔢 Heading Structure
```html
<h1>Title</h1>
<h2>Section</h2>
<h3>Subsection</h3>
```
✅ Maintain logical order without skipping levels

---

### 🛠️ Hands-On Accessibility Task
- Add alt text to all images
- Use `<label>` for every form field
- Ensure keyboard accessibility
- Structure using: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- Use a contrast checker tool

---

### 🧠 Accessibility Tips

| Best Practice            | Why It Matters                          |
|--------------------------|------------------------------------------|
| Use semantic HTML        | Screen readers can parse content easily |
| Alt text for images      | Supports visually impaired users        |
| Label form fields        | Forms are accessible and readable       |
| Maintain tab order       | Improves keyboard navigation            |
| Don’t rely on color only | Helps colorblind users                  |

---

### ✅ Summary

You now know:
- The purpose of **Semantic HTML**
- How to structure content with meaning
- How to improve accessibility for all users
- How to make your site keyboard and screen-reader friendly

---

### 📝 Homework

✅ Update your Day 3 webpage to:
- Use semantic tags
- Add `alt` text to all images
- Ensure every form field has a `<label>`
- Use proper heading order (`<h1>` → `<h3>`)

💡 Bonus:
- Explore [ARIA roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)
- Try using:
```html
<div role="navigation">Links here</div>
```

