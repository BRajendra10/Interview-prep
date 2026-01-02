# HTML Interview Preparation Guide

---

## 1. What is HTML?

### Explanation

HTML (HyperText Markup Language) is the standard markup language used to define the **structure and meaning** of web content.
It describes **what content exists**, not how it looks or behaves.

* HTML → Structure
* CSS → Styling
* JavaScript → Behavior

### Interview Question

**Q:** What is HTML?  
**A:** HTML (HyperText Markup Language) is a markup language used to define the structure and meaning of web content. It tells the browser what elements exist on a page, such as headings, paragraphs, forms, and images.

### Code Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is HTML structure</p>
  </body>
</html>
```

---

## 2. Is HTML a Programming Language?

### Explanation

HTML has no logic, variables, loops, or conditions.

### Interview Question

**Q:** Is HTML a programming language?  
**A:** No, HTML is not a programming language because it does not support logic, conditions, loops, or variables. It is a markup language used only for structuring content.

### Code Example

```html
<!-- HTML can structure content -->
<p>This is a paragraph</p>

<!-- Logic like conditions is NOT possible in HTML -->
```

---

## 3. HTML vs HTML5

### Explanation

HTML5 is the modern standard and introduced:

* Semantic elements
* Native audio/video
* Better forms & validation
* Browser APIs (storage, canvas)

### Interview Question

**Q:** What is the difference between HTML and HTML5?  
**A:** HTML5 is the modern version of HTML that introduced semantic elements, native audio and video support, improved form controls, and browser APIs like localStorage and canvas.

### Code Example

```html
<header>
  <nav>Menu</nav>
</header>
<main>
  <article>Content</article>
</main>
<footer>Footer</footer>
```

---

## 4. HTML Document Structure

### Explanation

Browsers expect a standard structure to correctly parse HTML.

### Interview Question

**Q:** What is the basic structure of an HTML document?  
**A:** A basic HTML document consists of <!DOCTYPE html>, the <html> tag, a <head> section for metadata, and a <body> section for visible content.

### Code Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Document</title>
  </head>
  <body>
    Page content
  </body>
</html>
```

---

## 5. `<!DOCTYPE html>`

### Explanation

Informs the browser to render the page in **standards mode**.

### Interview Questions

**Q:** Why do we use `<!DOCTYPE html>`?  
**A:** It tells the browser to render the page in standards mode, ensuring consistent behavior across modern browsers.

**Q:** What happens if DOCTYPE is missing?  
**A:** The browser may switch to quirks mode, which can cause layout and rendering inconsistencies.

### Code Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Standards Mode</title>
  </head>
  <body>
    Content
  </body>
</html>
```

---

## 6. `<head>` vs `<body>`

### Explanation

* `<head>` → metadata, SEO, styles, scripts
* `<body>` → visible UI shown to users

The browser reads `<head>` first to understand **how** to render the page, then renders the actual UI from `<body>`.

### Interview Question

**Q:** What goes inside the `<head>` tag?  
**A:** The `<head>` contains metadata such as the page title, meta tags, linked stylesheets, fonts, and scripts that help browsers understand how to render the page.

### Code Example

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Page</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is visible content</p>
  </body>
</html>
```

---

## 7. Meta Tags

### Explanation

Meta tags provide **information about the page** to browsers and search engines. They do not appear in the UI.

Common uses:

* SEO
* Character encoding
* Responsive design
* Browser behavior

### Interview Questions

**Q:** What are meta tags used for?  
**A:** Meta tags provide metadata about a webpage, such as character encoding, SEO information, responsiveness, and browser instructions.

**Q:** What is the viewport meta tag?  
**A:** The viewport meta tag controls how a webpage scales and displays on different screen sizes, especially on mobile devices.

### Code Example

```html
<head>
  <meta charset="UTF-8" />
  <meta name="description" content="HTML interview preparation guide" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</head>
```

---

## 8. Block vs Inline Elements

### Explanation

* **Block elements** take full width and start on a new line
  Examples: `div`, `p`, `h1`
* **Inline elements** take only content width
  Examples: `span`, `a`, `strong`

### Interview Question

**Q:** What is the difference between `div` and `span`?  
**A:** A `div` is a block-level element that starts on a new line and takes full width, while a `span` is an inline element that flows within text and only takes up content width.

### Code Example

```html
<div>This is a block element</div>
<span>This is inline</span>
<span>Inline continues</span>
```

---

## 9. Inline vs Inline-Block vs Block

### Explanation

* **Inline** → width/height not respected
* **Inline-block** → width/height allowed
* **Block** → full width by default

### Interview Question

**Q:** Why do we use `inline-block`?  
**A:** `inline-block` allows elements to sit inline while still respecting width and height, which is useful for buttons and layout components.

### Code Example

```html
<style>
  .inline { display: inline; width: 100px; }
  .inline-block { display: inline-block; width: 100px; height: 40px; }
  .block { display: block; width: 100px; }
</style>

<span class="inline">Inline</span>
<span class="inline-block">Inline-Block</span>
<div class="block">Block</div>
```

---

## 10. Void (Self-Closing) Elements

### Explanation

Void elements do not wrap content and do not have closing tags.

### Interview Question

**Q:** What are void elements?  
**A:** Void elements are HTML elements that do not have closing tags and cannot contain content, such as `img`, `input`, `br`, `hr`, and `meta`.

### Code Example

```html
<img src="logo.png" alt="Company Logo" />
<input type="text" placeholder="Enter name" />
<br />
<hr />
<meta charset="UTF-8" />
```

---

## 11. Semantic HTML (CRITICAL)

### Explanation

Semantic HTML uses **meaningful tags** that clearly describe the purpose of the content. It helps browsers, search engines, and assistive technologies understand the structure of the page.

Common semantic tags:

* `header`, `nav`, `main`
* `section`, `article`
* `aside`, `footer`

### Interview Questions

**Q:** What is semantic HTML?  
**A:** Semantic HTML uses meaningful tags that describe the purpose of content, improving readability, accessibility, and SEO.

**Q:** What is the difference between `section` and `article`?  
**A:** An `article` represents standalone, reusable content, while a `section` groups related content within a page.

### Code Example

```html
<header>
  <nav>Navigation</nav>
</header>

<main>
  <article>
    <h2>Blog Title</h2>
    <p>Independent blog content</p>
  </article>

  <section>
    <h3>Comments</h3>
    <p>User comments here</p>
  </section>
</main>

<footer>© 2026</footer>
```

---

## 12. Global Attributes

### Explanation

Global attributes are attributes that can be applied to **any HTML element**.

Common global attributes:

* `id`
* `class`
* `style`
* `title`
* `tabindex`

### Interview Question

**Q:** What are global attributes in HTML?  
**A:** Global attributes are attributes that can be applied to any HTML element, such as `id`, `class`, `style`, `title`, and `tabindex`.

### Code Example

```html
<p id="intro" class="text" title="Introduction">Hello World</p>
```

---

## 13. id vs class

### Explanation

* `id` → unique (one element)
* `class` → reusable (multiple elements)

### Interview Question

**Q:** Why should IDs not be repeated?  
**A:** IDs must be unique because they uniquely identify elements for JavaScript access, CSS specificity, and accessibility tools.

### Code Example

```html
<div id="header">Header</div>
<div class="card">Card 1</div>
<div class="card">Card 2</div>
```

---

## 14. Lists in HTML

### Explanation

Lists group related items in a structured and readable way.

Types of lists:

* Ordered (`ol`)
* Unordered (`ul`)
* Description (`dl`)

### Interview Questions

**Q:** What is the difference between `ol` and `ul`?  
**A:** `ol` displays ordered lists with a sequence, while `ul` displays unordered lists with bullet points.

**Q:** What is a description list?  
**A:** A description list is used to display term–definition pairs using `dl`, `dt`, and `dd`.

### Code Example

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
</ul>

<ol>
  <li>Login</li>
  <li>Dashboard</li>
</ol>

<dl>
  <dt>HTML</dt>
  <dd>Markup language</dd>
</dl>
```

---

## 15. Tables in HTML

### Explanation

Tables display **tabular data**, not layout.

Core elements:
`table`, `thead`, `tbody`, `tfoot`, `tr`, `th`, `td`

### Interview Questions

**Q:** What is the difference between `th` and `td`?  
**A:** `th` defines a header cell and is usually bold and centered, while `td` defines standard data cells.

**Q:** Why should tables not be used for layout?  
**A:** Tables are not responsive and create accessibility issues, making them unsuitable for layout design.

### Code Example

```html
<table border="1">
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Rajendra</td>
      <td>Developer</td>
    </tr>
  </tbody>
</table>
```

---

## 16. Forms (FULL-STACK CORE)

### Explanation

Forms collect user input and send it to the backend server.

Key attributes:

* `action`
* `method`
* `name`
* `value`

### Interview Questions

**Q:** How does form data reach the backend?  
**A:** Form data is sent to the backend as an HTTP request using methods like GET or POST.

**Q:** What is the difference between GET and POST?  
**A:** GET sends data in the URL and is used for fetching data, while POST sends data in the request body and is used for secure submissions.

### Code Example

```html
<form action="/login" method="POST">
  <input type="email" name="email" />
  <input type="password" name="password" />
  <button type="submit">Login</button>
</form>
```

---

## 17. Form Validation

### Explanation

HTML provides built-in **client-side validation**.

### Interview Question

**Q:** What is the difference between client-side and server-side validation?
**A:** Client-side validation improves user experience, while server-side validation ensures data security and cannot be bypassed.

### Code Example

```html
<input type="email" required />
<input type="password" minlength="6" />
```

---

## 18. Label & Accessibility

### Explanation

`label` associates descriptive text with form inputs, improving accessibility.

### Interview Question

**Q:** Why should we use `<label>` instead of placeholders?  
**A:** Labels improve accessibility and usability, especially for screen readers and form focus handling.

### Code Example

```html
<label for="email">Email</label>
<input id="email" type="email" />
```

---

## 19. Input Types

### Explanation

HTML5 input types improve validation and user experience.

### Interview Question

**Q:** Why should we use `type="email"`?  
**A:** It provides built-in validation and shows optimized keyboards on mobile devices.

### Code Example

```html
<input type="email" />
<input type="date" />
<input type="number" />
```

---

## 20. DOM (Document Object Model)

### Explanation

The DOM is a **tree representation** of HTML created by the browser in memory.

### Interview Question

**Q:** What is the DOM?  
**A:** The DOM is a tree-like representation of an HTML document that allows JavaScript to dynamically access and modify content.

### Code Example

```html
<p id="text">Hello</p>
<script>
  document.getElementById("text").textContent = "Updated";
</script>
```

---

### 21. Data Attributes

**Explanation**
Data attributes allow you to store custom data on HTML elements without affecting semantics.

**Interview Question**

**Q:** Why use `data-*` attributes?  
**A:** They allow developers to store custom data on elements for JavaScript logic without affecting HTML semantics.

```html
<button data-user-id="42" data-role="admin">Click</button>

<script>
  const btn = document.querySelector("button");
  console.log(btn.dataset.userId); // 42
</script>
```

---

### 22. Script Loading (`async` vs `defer`)

**Explanation**
Controls when JavaScript is executed during page load.

**Interview Question**

**Q:** What is the difference between `async` and `defer`? 
**A:** `defer` loads scripts in order after HTML parsing, while `async` loads scripts independently and may execute out of order.

```html
<script src="app.js" defer></script>
<script src="analytics.js" async></script>
```

---

### 23. Accessibility (IMPORTANT)

**Explanation**
Accessibility ensures websites are usable by people with disabilities.

**Interview Questions**
**Q:** What is accessibility?
Designing apps usable by everyone.

**Q:** What is web accessibility?  
**A:** Web accessibility ensures that websites can be used by people with disabilities using assistive technologies.

**Q:** What are ARIA attributes?  
**A:** ARIA attributes provide additional context to screen readers for dynamic or complex UI components.

```html
<button aria-label="Close Modal">✖</button>

<nav role="navigation" aria-label="Main Navigation"></nav>
```

---

### 24. Images & Media

**Explanation**
HTML provides native elements for images and media.

**Interview Questions**

**Q:** What is lazy loading?  
**A:** Lazy loading delays loading images until they are needed, improving performance.

**Q:** `img` vs background image?  
**A:** `img` is semantic and accessible, while background images are decorative.

```html
<img src="photo.jpg" alt="Profile photo" loading="lazy" />

<video controls>
  <source src="movie.mp4" type="video/mp4" />
</video>
```

---

### 25. SEO (HTML Perspective)

**Explanation**
HTML structure directly affects SEO.

**Interview Question**

**Q:** What is the difference between `<title>` and `<h1>`?  
**A:** `<title>` is used for SEO and browser tabs, while `<h1>` is the main visible heading on the page.

```html
<head>
  <title>Best Frontend Interview Prep</title>
</head>
<body>
  <h1>Frontend Interview Guide</h1>
</body>
```

---

### 26. HTML Entities

**Explanation**
Entities represent reserved or special characters.

**Interview Question**

**Q:** Why do we use HTML entities?
**A:** They allow reserved or special characters to be displayed correctly in HTML.

```html
<p>5 &lt; 10 &amp;&amp; 10 &gt; 5</p>
```

---

### 27. iframe & Embedding Content

**Explanation**
`iframe` embeds external documents.

**Interview Question**

**Q:** When should iframes be avoided?  
**A:** Iframes should be avoided when possible due to security, performance, and SEO concerns.

```html
<iframe src="https://example.com" title="External Content"></iframe>
```

---

### 28. HTML Parsing & Rendering Flow

**Explanation**
Browser rendering flow:
HTML → DOM → CSSOM → Render Tree → Paint

**Interview Question**

**Q:** How does a browser render HTML?  
**A:** The browser parses HTML into the DOM, combines it with CSSOM, builds a render tree, and then paints pixels on the screen.

```html
<!-- HTML parsed into DOM nodes internally -->
<div>Hello World</div>
```

---

### 29. HTML Performance Best Practices

**Explanation**
Clean HTML improves performance.

**Interview Question**

**Q:** How can HTML improve performance?  
**A:** By using semantic markup, optimized images, proper script loading, and minimal DOM complexity.

```html
<img src="image.webp" alt="Optimized" />
<script src="main.js" defer></script>
```

---

### 30. HTML Security Basics

**Explanation**
HTML can expose security vulnerabilities if misused.

**Interview Questions**

**Q:** What is XSS?  
**A:** Cross-Site Scripting is a security vulnerability where attackers inject malicious scripts into webpages.

**Q:** Why is backend validation mandatory?  
**A:** Because client-side validation can be bypassed, backend validation is required to ensure security.

```html
<!-- Bad -->
<div>{{ userInput }}</div>

<!-- Good (escaped on backend) -->
<div>&lt;script&gt;alert('xss')&lt;/script&gt;</div>
```

---
