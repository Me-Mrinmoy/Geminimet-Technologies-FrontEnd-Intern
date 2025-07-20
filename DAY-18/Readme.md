## 📅 Day 18: Website Project – Part 2 (Styling)

### 🎯 Objective

By the end of Day 18, trainees will:

* Learn how to apply consistent CSS styles to the base HTML structure created in Day 17.
* Understand how to style various website components, such as headers, navigation, main content, and footer.
* Learn the importance of responsive design and how to make the website mobile-friendly using media queries and flexible layouts.
* Apply styles to make their portfolio or product website visually appealing and functional across various devices (mobile, tablet, desktop).

---

### 🔹 Introduction

On Day 17, you focused on creating the base HTML structure for your website, including the header, navigation, main content, and footer. Now, it’s time to enhance this structure visually. This day’s focus is on applying CSS styles to your HTML structure to make it visually appealing, readable, and usable across different screen sizes.

You will begin by applying basic CSS styles to elements like the header, body, and sections. You will then proceed to implement responsive design techniques using media queries and CSS layout methods such as Flexbox and Grid to ensure that your website looks good on various devices (e.g., mobile phones, tablets, desktops).

---

### 🔹 Overview of the Styling Process

#### ✅ Setting Up Your CSS

* Link your CSS file to your HTML document:

```html
<link rel="stylesheet" href="styles.css">
```

* Choose a consistent color scheme, typography, and layout rules to maintain visual harmony across the website.

#### 🎨 Basic CSS Styling

* Style key elements like text, buttons, and images.
* Use the CSS Box Model to adjust spacing (padding, margin), borders, and alignment.
* Apply text styles: `font-family`, `font-size`, `color`, `line-height`, etc., to improve readability.

#### 📱 Responsive Design

* Use media queries to adjust layout for different screen sizes.
* Create fluid layouts using relative units (%, em, rem).
* Ensure the site adapts to mobile, tablet, and desktop screens for a seamless experience.

#### 🧱 Enhancing Layout with Flexbox and Grid

* Use **Flexbox** for one-dimensional layouts (like nav menus).
* Use **CSS Grid** for two-dimensional layouts (like portfolio galleries).

---

### 🔹 Step-by-Step Process for Applying CSS to Your Website

#### 1. Set Up the CSS File

Ensure that your HTML file is linked to your CSS file using:

```html
<link rel="stylesheet" href="styles.css">
```

Place this inside the `<head>` section. Ensure the `styles.css` file is in the same directory as your HTML file.

#### 2. Apply Basic Styles to the Body

```css
body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f4;
    color: #333;
    margin: 0;
    padding: 0;
}
```

**Explanation:**

* `font-family`: Sets the default font for the website.
* `background-color`: Light gray background for the page.
* `color`: Dark gray text color.
* `margin`, `padding`: Resets default spacing.

#### 3. Style the Header and Navigation

```css
header {
    background-color: #333;
    padding: 10px;
    color: #fff;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    font-size: 1.1rem;
}

nav ul li a:hover {
    color: #ff6347;
}
```

**Explanation:**

* `header`: Dark background and white text.
* `nav ul`: Flexbox layout, center aligned.
* `nav ul li`: Adds space between links.
* `nav ul li a`: Styled links with hover effect.

#### 4. Style the Main Content Sections

```css
section {
    padding: 50px;
    margin: 20px 0;
    background-color: #fff;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

h1, h2 {
    color: #333;
}

p {
    font-size: 1rem;
    line-height: 1.6;
    color: #555;
}
```

**Explanation:**

* `section`: Spacing and box shadow for depth.
* `h1, h2`: Clear heading color.
* `p`: Readable font size and spacing.

#### 5. Style the Footer

```css
footer {
    background-color: #333;
    color: #fff;
    padding: 20px;
    text-align: center;
}

footer a {
    color: #fff;
    margin: 0 10px;
    text-decoration: none;
}

footer a:hover {
    color: #ff6347;
}
```

**Explanation:**

* `footer`: Dark background, centered content.
* `footer a`: White links, hover effect.

#### 6. Implement Responsive Design with Media Queries

```css
@media screen and (max-width: 768px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    section {
        padding: 30px;
    }
}
```

**Explanation:**

* Applies to screens 768px or smaller.
* Changes nav to vertical stack.
* Reduces section padding for better fit.

---

This guide helps you implement a fully styled and responsive layout for your website using clean and modern CSS.
