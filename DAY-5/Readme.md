## 🗓️ Day 5: Hands-on Lab – Build a Simple Resume Page

---

### 🎯 Objective

Build a responsive, well-structured resume webpage using:
- ✅ Semantic HTML
- ✅ CSS styling
- ✅ Layout techniques (Flexbox/Grid)

---

### 🔹 Key Learning Outcomes

#### ✅ Applying HTML Basics
- Use headings, paragraphs, lists, links
- Semantic elements: `<section>`, `<article>`, `<footer>`

#### ✅ Styling with CSS
- Fonts, background, borders, margins, spacing
- Responsive design for mobile and desktop

#### ✅ Creating Layouts
- Flexbox or CSS Grid for clean structure
- Organize sections: profile, experience, education, skills

---

### 🔧 Step 1: Setting Up the HTML Structure

#### 🧱 HTML Boilerplate
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>John Doe - Resume</title>
</head>
<body>
  <header>
    <h1>John Doe</h1>
    <p>Web Developer | johndoe@example.com</p>
  </header>

  <section id="profile">
    <h2>Profile</h2>
    <p>A passionate web developer with experience in HTML, CSS, and JavaScript.</p>
  </section>

  <section id="experience">
    <h2>Work Experience</h2>
    <ul>
      <li>Junior Web Developer at XYZ Corp (2021-Present)</li>
      <li>Intern at ABC Inc. (2020–2021)</li>
    </ul>
  </section>

  <section id="education">
    <h2>Education</h2>
    <ul>
      <li>BSc in Computer Science, University of ABC (2020)</li>
    </ul>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <ul>
      <li>HTML, CSS, JavaScript</li>
      <li>React, Node.js</li>
      <li>Responsive Design</li>
    </ul>
  </section>

  <footer>
    <p>Contact: johndoe@example.com</p>
  </footer>
</body>
</html>
```

---

### 🎨 Step 2: Styling the Resume with CSS

#### 🖼️ Example CSS
```css
/* General Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 20px;
  background-color: #f4f4f9;
}

/* Header */
header {
  text-align: center;
  margin-bottom: 20px;
}
header h1 {
  font-size: 2.5em;
  margin-bottom: 0;
}
header p {
  font-size: 1.2em;
  color: #555;
}

/* Sections */
section {
  background-color: #fff;
  margin: 20px 0;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}
section h2 {
  font-size: 1.8em;
  margin-bottom: 10px;
  color: #333;
}
ul {
  list-style-type: none;
  padding-left: 20px;
}
ul li {
  margin-bottom: 10px;
  font-size: 1.1em;
}

/* Footer */
footer {
  text-align: center;
  margin-top: 30px;
  font-size: 1em;
}
```

---

### 📱 Step 3: Making the Resume Responsive

#### 🔁 Media Queries Example
```css
@media (max-width: 768px) {
  header h1 {
    font-size: 2em;
  }
  section h2 {
    font-size: 1.5em;
  }
  ul {
    padding-left: 15px;
  }
}
```

---

### 💼 Hands-on Project Deliverables

✅ By the end of Day 5, you will:
- Have a working **HTML + CSS resume page**
- Apply **semantic HTML** and **accessible design**
- Upload your project to **GitHub**
- Add this project to your **portfolio**

---

### 📝 Final Notes

- Solidify HTML and CSS knowledge through practice
- Gain confidence in real-world layout building
- Showcase your resume page when applying for jobs

> 💡 **Bonus Tip:** Experiment with additional CSS features like hover effects, transitions, and Google Fonts to personalize your resume even more!

