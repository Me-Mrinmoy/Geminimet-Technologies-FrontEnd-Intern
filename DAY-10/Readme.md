# 🌟 Day 10: Mini Project – Styled Product Landing Page

## 🎯 Objective

By the end of this session, you will:

* Apply everything learned so far to build a fully styled Product Landing Page using HTML and CSS.
* Demonstrate understanding of layout, positioning, styling, and responsiveness.
* Showcase the ability to create a clean and functional web page layout with visual appeal.

---

## 🔹 Project Overview

Create a **Product Landing Page** combining all core concepts learned:

* Semantic HTML structure
* CSS Box Model
* Layout and positioning
* Visual styling
* Responsive design

---

## 🔹 Project Requirements

### ✅ Header Section

* Fixed navigation bar at the top.
* Links to page sections: `Home`, `Features`, `Testimonials`, `Contact`.
* Use Flexbox or inline-block for layout.

### ✅ Hero Section

* Full-width section with background image.
* Centralized heading and CTA button.
* Use Flexbox/Grid for alignment.

### ✅ Features Section

* Three feature cards with:

  * Padding
  * Borders
  * Shadows
  * Responsive Flex layout

### ✅ Testimonials Section

* Customer testimonials in styled cards.
* Use relative/absolute positioning for effect.
* Include margin and padding.

### ✅ Footer Section

* Company info, social links, policy links.
* Use Flexbox/Grid for alignment.

### ✅ Responsive Design

* Layout adapts to all screen sizes.
* Use media queries for smaller viewports.

---

## 🔧 HTML Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Product Landing Page</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <!-- Header Section -->
  <header>
    <nav class="navbar">
      <ul>
        <li><a href="#hero">Home</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#testimonials">Testimonials</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="hero">
    <div class="hero-content">
      <h1>Product Name</h1>
      <p>Introducing the most amazing product you'll ever need.</p>
      <a href="#features" class="cta-button">Learn More</a>
    </div>
  </section>

  <!-- Features Section -->
  <section id="features">
    <div class="feature-card">
      <h2>Feature 1</h2>
      <p>Description of feature 1</p>
    </div>
    <div class="feature-card">
      <h2>Feature 2</h2>
      <p>Description of feature 2</p>
    </div>
    <div class="feature-card">
      <h2>Feature 3</h2>
      <p>Description of feature 3</p>
    </div>
  </section>

  <!-- Testimonials Section -->
  <section id="testimonials">
    <div class="testimonial">
      <p>"This product changed my life!" - Customer 1</p>
    </div>
    <div class="testimonial">
      <p>"Highly recommend it!" - Customer 2</p>
    </div>
  </section>

  <!-- Footer Section -->
  <footer>
    <p>© 2025 Your Company</p>
  </footer>

</body>
</html>
```

---

## 🎨 CSS Code

```css
/* General Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

a {
  text-decoration: none;
  color: inherit;
}

/* Header Section */
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background-color: #333;
  padding: 10px 0;
  z-index: 1000;
}

.navbar ul {
  list-style: none;
  display: flex;
  justify-content: center;
  margin: 0;
  padding: 0;
}

.navbar ul li {
  margin: 0 20px;
}

.navbar ul li a {
  color: white;
  font-size: 18px;
}

/* Hero Section */
#hero {
  background-image: url('hero-image.jpg');
  background-size: cover;
  background-position: center;
  height: 400px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  text-align: center;
  padding: 20px;
}

.cta-button {
  background-color: #ff5733;
  padding: 10px 20px;
  color: white;
  font-size: 16px;
  border-radius: 5px;
  margin-top: 15px;
  display: inline-block;
}

/* Features Section */
#features {
  display: flex;
  justify-content: space-around;
  padding: 40px 20px;
  background-color: #f4f4f4;
  flex-wrap: wrap;
}

.feature-card {
  background-color: white;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  width: 30%;
  text-align: center;
  margin: 10px;
}

/* Testimonials Section */
#testimonials {
  background-color: #f9f9f9;
  padding: 40px 20px;
  text-align: center;
}

.testimonial {
  margin: 20px auto;
  padding: 20px;
  background-color: white;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
  max-width: 600px;
}

/* Footer Section */
footer {
  background-color: #333;
  color: white;
  text-align: center;
  padding: 20px 0;
}

/* Responsive Design */
@media (max-width: 768px) {
  #features {
    flex-direction: column;
    align-items: center;
  }

  .feature-card {
    width: 80%;
  }

  .navbar ul {
    flex-direction: column;
    gap: 10px;
  }
}
```

---

## 📈 Explanation of Key CSS Concepts

### Fixed Navigation Bar

* Positioned using `position: fixed` so it remains visible during scrolling.
* `z-index: 1000` ensures it appears above all other content.

### Hero Section

* Uses `background-image` with `background-size: cover` to fully fill the section.
* `display: flex` is used to center the content horizontally and vertically.

### Product Features Section

* Flexbox aligns feature cards horizontally.
* Cards styled with `padding`, `border-radius`, and `box-shadow` for emphasis.

### Responsive Design

* `@media` queries adjust layout for smaller screens.
* Features stack vertically on devices <768px for better usability.

---

## ✅ Summary

In this mini project, you applied:

* Semantic HTML layout structure
* CSS display and box model
* Positioning: fixed, relative, flexbox
* Visual styling with shadows, padding, spacing
* Responsive design with media queries

🚀 You now have a fully styled **Product Landing Page** as a foundation for real-world portfolio projects.

Want to deploy this using GitHub Pages? I can guide you next! ✨
