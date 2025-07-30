# 📅 Day 20: Deploying Your Website

Welcome to the final and one of the most rewarding days of the program! Today, you will deploy your website online, making it live and accessible to the world. You'll also learn the basics of version control with Git & GitHub, and submit your final project.

---

## 🧠 Learning Objectives

By the end of the day, you will be able to:

* Understand the basics of version control and how to use Git and GitHub.
* Deploy a static website using GitHub Pages and/or Netlify.
* Handle basic errors during deployment.
* Share your website with others using a public link.
* Submit your final project and reflect on your learning journey.

---

## 🧱 Part 1: Version Control with Git & GitHub

### 🔄 What is Version Control?

Version control is a system that records changes to files over time. It allows you to:

* Track code changes
* Collaborate with others
* Revert to earlier versions if needed
* Work on multiple features using branches

### 🛠 Git Basics

Git is a version control tool used locally.

#### 🔧 Common Git Commands:

| Command                       | Description                          |
| ----------------------------- | ------------------------------------ |
| `git init`                    | Initializes a new Git repository     |
| `git add .`                   | Adds all files to the staging area   |
| `git commit -m "Message"`     | Saves a snapshot with a message      |
| `git status`                  | Shows the current status             |
| `git log`                     | Views commit history                 |
| `git branch`                  | Shows all branches                   |
| `git checkout -b branch-name` | Creates and switches to a new branch |

### 🌐 GitHub: Remote Repository Hosting

GitHub is used to host your Git repositories in the cloud.

#### Steps to Connect to GitHub:

1. Create a GitHub account
2. Create a new repository
3. Connect your local project:

```bash
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main
```

---

## 🚀 Part 2: Deploying Your Website

### 🟣 Option 1: Deploy Using Gi📅 Day 20: Deploying Your Website


###

This is the final and one of the most rewarding days of the program! Today, you’ll learn how to deploy your website online, making it live and accessible from anywhere in the world. We’ll also introduce you to version control using Git & GitHub, an industry-standard skill. Finally, you’ll submit your final project and receive feedback.

🧠 Learning Objectives

By the end of the day, you will be able to

Understand the basics of version control and how to use Git and GitHub.

Deploy a static website using GitHub Pages and/or Netlify.

Handle basic errors during deployment.

Share your website with others using a public link.

Submit your final project and reflect on your learning journey.

🧱 Part 1: Version Control with Git & GitHub (Foundational Knowledge)

🔄 What is Version Control?

Version control is a system that records changes to files over time so you can recall specific versions later. It helps:

Track changes made to your code

Collaborate with others

Revert to earlier versions if something breaks

Work on multiple features simultaneously (branches)

🛠 Git Basics

Git is a version control tool installed on your computer.

🔧 Common Git Commands:

Command	Description

git init	Initializes a new Git repository

git add .	Adds all files to the staging area

git commit -m "Message"	Saves your snapshot with a message

git status	Shows current status of the repository

git log	View commit history

git branch	Shows all branches

git checkout -b branch-name	Create and switch to a new branch

🌐 GitHub: Remote Repository Hosting

GitHub hosts your Git repositories in the cloud, so others can see and collaborate on them.

Steps:

Create a GitHub account

Create a new repository

Connect your local project to GitHub using:

git remote add origin [https://github.com/your-username/your-repo.git](https://github.com/your-username/your-repo.git)

git push -u origin main

🚀 Part 2: Deploying Your Website

There are two beginner-friendly options we will use:

🟣 Option 1: Deploy Using GitHub Pages (Free & Easy)

💡 Ideal for:

Personal portfolios

Simple static websites (HTML/CSS/JS)

✅ Pre-requisites:

Your website is committed and pushed to GitHub

🚀 Steps to Deploy:

Go to your GitHub repository

Click on Settings > Pages

Under “Source”, select main branch and /root folder

Click Save

GitHub will provide a live link like:

[https://your-username.github.io/project-name/](https://your-username.github.io/project-name/)

🛠 Tips:

Ensure your homepage file is named index.html

Use relative links (./images/logo.png) for images and CSS

Changes require re-commit and push to GitHub

🟢 Option 2: Deploy Using Netlify (Drag & Drop or Git-Linked)

💡 Ideal for:

Static websites with advanced features (contact forms, custom domains)

🚀 Steps to Deploy with Drag & Drop:

Go to netlify.com and create an account

Click on “Add new site” > Deploy manually

Drag your project folder (with index.html, CSS, images) into the upload area

Done! Netlify will give you a free live link instantly

🔁 Git-Connected Deployment:

You can also connect Netlify directly to your GitHub repository

Auto-deploys every time you push new code to GitHub

✨ Netlify Perks:

Free HTTPS certificate

Clean URLs

Custom domain setup

Form handling without backend code

🧪 Part 3: Final Project Submission

📤 How to Submit:

Share the GitHub repository link

Share the Live website link (GitHub Pages or Netlify)

Provide a short write-up:

What the project is about

What you learned

Any challenges you overcame

✅ Evaluation Criteria:

Proper use of HTML structure

Clean, responsive design using CSS

Consistent and accessible navigation

Use of forms, icons, hover effects (from previous day)

Well-commented code

Deployed properly and loads without errors

💬 Part 4: Feedback & Reflection

🧠 Reflection Prompts:

What did you enjoy the most during this program?

What was the biggest challenge you faced?

What concepts do you feel most confident about?

What would you like to explore next? (JavaScript, React, etc.)

🎓 Feedback:

You’ll receive feedback on:

Code quality

Design choices

Best practices

Suggestions for improvement or next steps in your learning journey

🏁 Wrap-Up

You’ve now gone from zero to launching a live website – that’s a huge milestone! You’ve built the foundation for a career in web development, and this final day celebrates all your efforts.

You can submit your final project that is Github linkHub Pages

#### 💡 Ideal For:

* Personal portfolios
* Simple static websites (HTML/CSS/JS)

#### ✅ Pre-requisites:

* Your website is committed and pushed to GitHub

#### 🚀 Steps to Deploy:

1. Go to your GitHub repository
2. Click on `Settings` > `Pages`
3. Under "Source", select `main` branch and `/root` folder
4. Click `Save`

GitHub will provide a live link like:

```
https://your-username.github.io/project-name/
```

#### 🛠 Tips:

* Ensure your homepage file is named `index.html`
* Use relative links like `./images/logo.png`
* Re-deploy by committing and pushing changes again

### 🟢 Option 2: Deploy Using Netlify

#### 💡 Ideal For:

* Static sites with forms, custom domains

#### 🚀 Steps (Drag & Drop):

1. Go to [netlify.com](https://netlify.com)
2. Create an account and login
3. Click "Add new site" > "Deploy manually"
4. Drag your project folder into the upload area
5. Done! You'll get a free live link

#### 🔁 Git-Connected Deployment:

* Connect Netlify to your GitHub repo
* Auto-deploys every time you push code

#### ✨ Netlify Perks:

* Free HTTPS certificate
* Clean URLs
* Custom domain support
* Built-in form handling

---

## 🧪 Part 3: Final Project Submission

### 📤 How to Submit:

* Share your **GitHub repository link**
* Share your **live website link** (GitHub Pages or Netlify)
* Include a short write-up:

  * What your project is about
  * What you learned
  * Any challenges you overcame

### ✅ Evaluation Criteria:

* Proper use of HTML structure
* Clean, responsive CSS
* Consistent, accessible navigation
* Forms, icons, hover effects included
* Well-commented code
* Site loads without errors

---

## 💬 Part 4: Feedback & Reflection

### 🧠 Reflection Prompts:

* What did you enjoy the most during this program?
* What was your biggest challenge?
* What concepts do you feel most confident about?
* What would you like to explore next? (JavaScript, React, etc.)

### 🎓 Feedback Includes:

* Code quality
* Design decisions
* Best practices
* Suggestions for next steps

---

## 🏁 Wrap-Up

Congratulations! 🎉

You've gone from zero to deploying a live website — an incredible achievement. This final day celebrates all your efforts and sets you on the path toward a career in web development.

Happy coding, and see you on your next journey! 🚀
