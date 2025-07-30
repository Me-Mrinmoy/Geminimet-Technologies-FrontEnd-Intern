# 💻 Day 19: Website Project – Part 3 (Final Touches)

## 🎯 Objective:
By the end of **Day 19**, trainees will:

- ✅ Add **interactive elements** such as **forms**, **icons**, and **hover effects**.
- ✅ Enhance **User Experience (UX)** by making the website more engaging and visually appealing.
- ✅ Implement **active styles** and use **icon libraries** like FontAwesome or Material Icons.
- ✅ Finalize the website with a polished, **responsive**, and **interactive** design.

---

## 🔹 Introduction:
In the previous days, trainees built the HTML structure and applied CSS styling. On Day 19, we focus on adding the final touches that bring the website to life through **interactivity** and **UX enhancements**.

This includes:

- Adding **interactive forms** (contact, subscription).
- Using **icons** for better visual communication.
- Implementing **hover, active, and focus states**.
- Enhancing **accessibility and usability**.

---

## 🧩 Overview of Final Touches:

### 1. 📬 Adding Forms

Forms let users interact with the website by submitting data.

#### Types of Forms:
- Contact Form
- Subscription Form
- Feedback Form

#### 📄 Sample HTML Form:
```html
<form action="submit_form.php" method="post">
  <label for="name">Your Name:</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Your Email:</label>
  <input type="email" id="email" name="email" required>

  <label for="message">Your Message:</label>
  <textarea id="message" name="message" rows="4" required></textarea>

  <button type="submit">Submit</button>
</form>
```
