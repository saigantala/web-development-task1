Personal Portfolio Website — Yethendra Sai Gantala
A clean, responsive, semantic HTML5 personal portfolio website built for Week 1: HTML - Your First Website.
Author: Yethendra Sai Gantala
Repository: saigantala/web-development-task1
GitHub: github.com/saigantala
LinkedIn: Yethendra Sai Gantala
Project Overview
This project demonstrates core HTML5 web development fundamentals by building a personal portfolio page from scratch. It uses semantic markup, internal navigation links, an edited portrait image with descriptive `alt` text, categorized skill lists, a milestone gallery, and an HTML5-validated contact form.
HTML Concepts Learned
Document Structure: `<!DOCTYPE html>`, `<html lang="en">`, `<head>`, `<meta charset="UTF-8">`, `<meta name="viewport">`, `<title>`, and `<body>`.
Semantic Landmarks: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<figcaption>`, and `<footer>`.
Core Elements & Attributes: Headings (`<h1>`–`<h3>`), paragraphs (`<p>`), lists (`<ul>`, `<li>`), anchor links (`<a href="...">`), images (`<img src="..." alt="...">`), and `id` / `class` attributes.
Forms & Validation: `<form>`, `<label for="...">`, `<input type="text">`, `<input type="email">`, `<textarea>`, `<button type="submit">`, and built-in attributes (`required`, `minlength`).
Code Structure
```text
web-development-task1/
├── index.html          # Main semantic HTML5 portfolio page (with embedded CSS & JS)
├── README.md           # Project documentation, setup guide, and testing evidence
├── requirements.txt    # Dependency note (no external packages required)
└── images/
    └── profile.jpg     # Portrait photo of Yethendra Sai Gantala (ID card removed)
```
Setup Instructions
Install Visual Studio Code and the Live Server extension.
Clone or download this repository to your computer:
```bash
   git clone https://github.com/saigantala/web-development-task1.git
   ```
Open the `web-development-task1` folder in VS Code.
Right-click `index.html` and select Open with Live Server (or double-click `index.html` to open it in any web browser).
Technical Details
Layout & Styling: Uses CSS custom properties (`:root`), a sticky translucent `<header>`, CSS Grid (`.about-grid`, `.skills-grid`, `.gallery-grid`, `.contact-layout`), and a `@media (max-width: 768px)` responsive breakpoint for mobile screens.
Form Validation Logic: Combines native HTML5 constraint validation (`required`, `type="email"`, `minlength`) with a JavaScript `submit` event listener that calls `checkValidity()`, displays an accessible confirmation message in `#form-status` (`aria-live="polite"`), and resets the form without reloading the page.
Testing Evidence
Test ID	Feature Tested	Input / Action	Expected Result	Status
TC-01	Internal Navigation	Click About, Skills, Gallery, Contact links	Smooth scroll to the matching section	Passed
TC-02	External Profile Links	Click GitHub and LinkedIn links	Opens profile in a new browser tab	Passed
TC-03	Image & Alt Text	Load `images/profile.jpg`	Portrait displays cleanly with descriptive `alt` text	Passed
TC-04	Form Validation (Invalid)	Submit empty fields or invalid email	Browser blocks submission and highlights invalid input	Passed
TC-05	Form Submission (Valid)	Submit valid name, email, and 10+ char message	Displays confirmation banner and resets form	Passed
Quality Standards Checklist
Requirement	Status
Project Overview	Complete
Setup Instructions	Complete
Code Structure	Complete
Technical Details	Complete
Testing Evidence	Complete
Visual Documentation (add browser screenshots in repo)	Ready for screenshots
