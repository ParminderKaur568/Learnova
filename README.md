# 🎓 Learnova – E-Learning Website

> A modern, responsive, performance-optimized, and accessible e-learning website built using HTML5 and CSS3.
> LVE LINK:-https://learnova-website.netlify.app/

## 📌 Project Overview

**Learnova** is a responsive e-learning platform designed to provide students with a clean, engaging, and accessible interface for discovering and exploring online courses.

This project was developed as part of a **Web Development Internship – Week 4 Task: Enhancing Web Page Performance and Accessibility**.

The primary focus of the project is not only visual design but also improving:

* ⚡ Website loading performance
* ♿ Web accessibility
* 📱 Responsive design
* 🧩 Semantic HTML structure
* 🎨 Efficient CSS
* 🔍 Search-engine-friendly structure
* ⌨️ Keyboard navigation
* 🖥️ Cross-device usability

---

## 🎯 Project Objective

The objective of this project is to transform a static webpage into a **fast, accessible, responsive, and user-friendly website**.

The website demonstrates practical implementation of modern frontend development practices, including semantic HTML5 elements, optimized images, lazy loading, accessible navigation, responsive layouts, and performance-conscious CSS.

---

## ✨ Key Features

### 🎓 E-Learning Interface

* Attractive educational landing page
* Featured online courses
* Course categories
* Instructor section
* Student testimonials
* Newsletter subscription section
* Call-to-action sections

### ♿ Accessibility

The website follows accessibility-focused development practices:

* Semantic HTML5 elements such as:

  * `<header>`
  * `<nav>`
  * `<main>`
  * `<section>`
  * `<article>`
  * `<footer>`
* Skip-to-content link
* Descriptive image `alt` attributes
* Accessible navigation
* Proper form labels
* Keyboard-friendly interactive elements
* Visible `:focus-visible` states
* Screen-reader-friendly text
* Appropriate ARIA labels
* Decorative icons hidden from screen readers
* Reduced-motion support using `prefers-reduced-motion`

### ⚡ Performance Optimization

Several techniques were implemented to improve page performance:

* Optimized WebP images
* Lazy loading for below-the-fold images
* High-priority loading for the main hero image
* Asynchronous image decoding
* Explicit image dimensions to reduce layout shifts
* Lightweight HTML and CSS
* No unnecessary JavaScript libraries
* System font stack to avoid external font requests
* Reusable CSS variables
* Minimal CSS redundancy
* Responsive CSS instead of unnecessary JavaScript-based layout logic

### 📱 Responsive Design

The website adapts to different screen sizes:

* 🖥️ Desktop
* 💻 Laptop
* 📱 Tablet
* 📱 Mobile

CSS media queries adjust:

* Navigation
* Hero section
* Course grid
* Benefits section
* Instructor section
* Testimonials
* Newsletter form
* Footer layout

---

## 🛠️ Technologies Used

| Technology            | Purpose                                        |
| --------------------- | ---------------------------------------------- |
| **HTML5**             | Page structure and semantic markup             |
| **CSS3**              | Styling, layout, animations and responsiveness |
| **WebP**              | Optimized image format                         |
| **CSS Media Queries** | Responsive design                              |
| **ARIA**              | Accessibility enhancement                      |
| **Git & GitHub**      | Version control and project hosting            |
| **Lighthouse**        | Performance and accessibility testing          |
| **WAVE / axe**        | Accessibility testing                          |

---


```

### 2. Open the Project

Navigate to the project directory:

```bash
cd Learnova
```

### 3. Run the Website

Open:

```text
index.html
```

in any modern web browser.

You can also use **VS Code Live Server** for local development.

---

## 🖼️ Image Optimization

Images are stored in the `images` folder and use the **WebP format** to reduce file size while maintaining good visual quality.

The main hero image is prioritized:

```html
<img
    src="images/hero-learning.webp"
    alt="Student learning online using a laptop"
    width="800"
    height="650"
    fetchpriority="high"
    decoding="async"
>
```

Images that appear further down the page use lazy loading:

```html
<img
    src="images/web-development.webp"
    alt="Web development course showing code on a laptop"
    width="600"
    height="400"
    loading="lazy"
    decoding="async"
>
```

This helps prevent unnecessary image downloads before the user reaches those sections.

---

## ♿ Accessibility Implementation

Accessibility was considered throughout the development process.

### Skip Navigation

A skip link allows keyboard and screen-reader users to quickly move to the main content:

```html
<a href="#main-content" class="skip-link">
    Skip to main content
</a>
```

### Semantic Structure

Instead of relying only on generic `<div>` elements, meaningful HTML5 elements are used:

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

This makes the page structure easier for assistive technologies to understand.

### Alternative Text

Images contain descriptive alternative text:

```html
<img
    src="images/python.webp"
    alt="Python programming course displayed on a laptop"
>
```

### Keyboard Focus

Interactive elements receive a visible focus state:

```css
:focus-visible {
    outline: 3px solid #4f46e5;
    outline-offset: 3px;
}
```

### Reduced Motion

The website respects users who prefer reduced motion:

```css
@media (prefers-reduced-motion: reduce) {
    * {
        scroll-behavior: auto;
        animation-duration: 0.01ms;
        transition-duration: 0.01ms;
    }
}
```

---

## ⚡ Performance Techniques

The following techniques were used to improve performance:

### 1. WebP Images

Large image files were converted to WebP to reduce page weight.

### 2. Lazy Loading

Below-the-fold images use:

```html
loading="lazy"
```

### 3. Image Dimensions

Explicit `width` and `height` attributes help browsers reserve space for images before they load.

### 4. High-Priority Hero Image

The most important visual element uses:

```html
fetchpriority="high"
```

### 5. Lightweight CSS

The stylesheet avoids unnecessary dependencies and uses reusable CSS variables.

### 6. No External JavaScript Libraries

The website is implemented using HTML and CSS without unnecessary frameworks or libraries, reducing additional network requests.

### 7. System Fonts

A system font stack is used instead of loading large external font files.

---

## 📊 Testing and Evaluation

The website can be evaluated using tools such as:

### Google Lighthouse

Lighthouse can be used to evaluate:

* Performance
* Accessibility
* Best Practices
* SEO

### WAVE

WAVE can help identify:

* Missing alternative text
* Accessibility errors
* ARIA issues
* Structural problems
* Contrast-related issues

### axe DevTools

axe can be used to detect common accessibility violations and validate the page against accessibility best practices.

---

## 📱 Responsive Breakpoints

The CSS uses multiple responsive breakpoints.

| Screen Size      | Layout                         |
| ---------------- | ------------------------------ |
| Large Desktop    | Multi-column layout            |
| 1050px and below | Adjusted desktop/tablet layout |
| 750px and below  | Tablet/mobile layout           |
| 430px and below  | Small mobile layout            |

The course cards, benefits, testimonials, navigation, forms, and other sections automatically adapt according to available screen width.

---

## 🎨 Main Website Sections

### 1. Navigation Bar

Provides access to major sections of the website.

### 2. Hero Section

Introduces Learnova with:

* Main heading
* Supporting description
* Search functionality
* Call-to-action buttons
* Learning image
* Trust indicators

### 3. Course Categories

Displays popular learning categories.

### 4. Featured Courses

Includes courses such as:

* Web Development
* Data Science
* UI/UX Design
* Python Programming

### 5. Why Learnova?

Highlights the benefits of learning through the platform.

### 6. Instructor Section

Introduces professional instructors.

### 7. Testimonials

Displays feedback from students.

### 8. Call-to-Action

Encourages visitors to begin their learning journey.

### 9. Newsletter

Allows users to subscribe for educational updates.

### 10. Footer

Contains navigation links and social media options.

---

## 🌐 Browser Compatibility

The website is designed to work with modern browsers, including:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari
* Opera

---

## 🔮 Future Improvements

Possible future enhancements include:

* User authentication
* Student dashboard
* Course enrollment system
* Video course player
* Course progress tracking
* Search and filtering functionality using JavaScript
* Dark mode
* Backend integration
* Database connectivity
* Payment integration
* Real-time course recommendations

---

## 📚 Learning Outcomes

Through this project, the following concepts were practiced:

* Semantic HTML5
* Accessible web development
* Responsive CSS
* CSS Grid and Flexbox
* Media queries
* Image optimization
* WebP image conversion
* Lazy loading
* Keyboard accessibility
* ARIA attributes
* Performance optimization
* Lighthouse testing
* Accessibility testing
* Clean and maintainable code

---

## 👩‍💻 Author

**Parminder Kaur**

Computer Science Engineering Student
Guru Tegh Bahadur Institute of Technology, GGSIPU Delhi

---

## 📄 Project Purpose

This project was created for educational and internship purposes to demonstrate practical knowledge of **frontend development, responsive web design, performance optimization, and web accessibility**.

---

## ⭐ Acknowledgements

* HTML5 and CSS3 documentation
* Web accessibility best practices
* Lighthouse
* WAVE Accessibility Evaluation Tool
* Unsplash for educational and workspace imagery

---

## 📜 License

This project is intended for educational and portfolio purposes.

If you reuse or modify the project, please ensure that any third-party assets, including images, comply with their respective licenses.
