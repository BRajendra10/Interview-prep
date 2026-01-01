# HTML Interview Preparation Guide  

---

## 1. What is HTML?

### Explanation
HTML (HyperText Markup Language) is the standard markup language used to define the **structure and meaning** of content on the web.  
It describes **what content exists**, not how it looks or behaves.

- HTML → Structure  
- CSS → Styling  
- JavaScript → Behavior  

### Interview Question
**Q: What is HTML?**  
HTML is a markup language used to structure web content. It defines elements like headings, paragraphs, forms, images, and links that browsers render and JavaScript can manipulate.

---

## 2. Is HTML a Programming Language?

### Explanation
HTML does not have variables, loops, conditions, or logic.

### Interview Question
**Q: Is HTML a programming language? Why or why not?**  
No. HTML is a markup language because it only describes structure, not logic or behavior.

---

## 3. HTML vs HTML5

### Explanation
HTML5 is the latest version of HTML and introduced:
- Semantic elements
- Native audio and video
- Better forms and validation
- Browser APIs (local storage, canvas, etc.)

### Interview Question
**Q: Difference between HTML and HTML5?**  
HTML5 introduced semantic elements, native multimedia support, improved forms, and APIs, reducing reliance on plugins.

---

## 4. HTML Document Structure

### Explanation
Browsers expect a standard structure to correctly parse and render pages.

### Interview Question
**Q: What is the basic structure of an HTML document?**  
It includes `<!DOCTYPE html>`, `<html>`, `<head>` for metadata, and `<body>` for visible content.

---

## 5. `<!DOCTYPE html>`

### Explanation
The DOCTYPE declaration tells the browser to render the page in **standards mode**.

### Interview Questions
**Q: Why do we use DOCTYPE?**  
To ensure consistent rendering across modern browsers.

**Q: What happens if it’s missing?**  
The browser may enter quirks mode, causing layout inconsistencies.

---

## 6. `<head>` vs `<body>`

### Explanation
- `<head>` → Metadata, SEO, styles, scripts
- `<body>` → Visible UI content

### Interview Question
**Q: What goes inside the head tag?**  
Title, meta tags, stylesheets, fonts, and scripts.

---

## 7. Meta Tags

### Explanation
Meta tags provide information **about the page**, not visible content.

### Interview Questions
**Q: What are meta tags used for?**  
SEO, responsiveness, character encoding, and browser behavior.

**Q: What is the viewport meta tag?**  
It controls layout and scaling on mobile devices.

---

## 8. Block vs Inline Elements

### Explanation
- Block elements start on a new line and take full width  
- Inline elements take only required width

### Interview Question
**Q: Difference between div and span?**  
`div` is block-level; `span` is inline.

---

## 9. Inline vs Inline-Block vs Block

### Explanation
- Inline → no width/height  
- Inline-block → width/height allowed  
- Block → full width

### Interview Question
**Q: Why use inline-block?**  
To keep elements inline while controlling size.

---

## 10. Void (Self-Closing) Elements

### Explanation
Void elements do not wrap content and don’t need closing tags.

### Interview Question
**Q: What are void elements?**  
Elements like `img`, `input`, `br`, `hr`, and `meta`.

---

## 11. Semantic HTML (Very Important)

### Explanation
Semantic HTML uses meaningful tags that describe content purpose.

Common semantic elements:
- `header`, `nav`, `main`
- `section`, `article`
- `aside`, `footer`

### Interview Questions
**Q: What is semantic HTML?**  
HTML that uses meaningful tags to improve readability, SEO, and accessibility.

**Q: Section vs Article?**  
Article is standalone content; section groups related content.

---

## 12. Global Attributes

### Explanation
Attributes that work on all HTML elements.

### Interview Question
**Q: What are global attributes?**  
Attributes like `id`, `class`, `style`, `title`, and `tabindex`.

---

## 13. `id` vs `class`

### Explanation
- `id` → Unique
- `class` → Reusable

### Interview Question
**Q: Why shouldn’t IDs repeat?**  
IDs uniquely identify elements and are used by JavaScript and accessibility tools.

---

## 14. Forms (Full-Stack Core)

### Explanation
Forms collect user input and send it to the backend.

Key attributes:
- `action`
- `method`
- `name`
- `value`

### Interview Questions
**Q: How does form data reach the backend?**  
Through an HTTP request using the form’s action URL and method.

**Q: GET vs POST?**  
GET sends data via URL; POST sends data in the request body.

---

## 15. Form Validation

### Explanation
HTML provides built-in client-side validation.

### Interview Questions
**Q: Client vs server validation?**  
Client improves UX; server ensures security.

**Q: Can client validation be bypassed?**  
Yes, always validate on the backend.

---

## 16. Label & Accessibility

### Explanation
Labels associate text with form inputs.

### Interview Question
**Q: Why use label instead of placeholder?**  
Labels improve accessibility and usability.

---

## 17. Input Types

### Explanation
HTML5 introduced semantic input types like `email`, `number`, `date`.

### Interview Question
**Q: Why use type="email" instead of text?**  
It enables validation and mobile-friendly keyboards.

---

## 18. DOM (Document Object Model)

### Explanation
The DOM is a tree-like representation of HTML in memory.

### Interview Question
**Q: What is DOM?**  
A programming interface that allows JavaScript to access and manipulate HTML.

---

## 19. Data Attributes

### Explanation
Custom attributes for storing extra information.

### Interview Question
**Q: Why use data-* attributes?**  
To store custom data without affecting structure or semantics.

---

## 20. Script Loading (`async` vs `defer`)

### Explanation
Controls how scripts are loaded and executed.

### Interview Question
**Q: Difference between async and defer?**  
Defer preserves execution order; async does not.

---

## 21. Accessibility (Important)

### Explanation
Accessibility ensures websites are usable by everyone.

### Interview Questions
**Q: What is accessibility?**  
Designing web apps usable by people with disabilities.

**Q: What are ARIA attributes?**  
They help screen readers understand dynamic UI components.

---

## 22. Images & Media

### Explanation
HTML supports native images, audio, and video.

### Interview Questions
**Q: What is lazy loading?**  
Loading images only when they enter the viewport.

**Q: Img vs background image?**  
`img` is semantic; background images are decorative.

---

## 23. SEO (HTML Perspective)

### Explanation
Search engines rely heavily on HTML structure.

### Interview Questions
**Q: Title vs H1?**  
Title is for search engines; H1 is the page’s main heading.

**Q: Why only one H1?**  
To clearly define the main topic of the page.

---

## 24. HTML Security Basics

### Explanation
HTML can introduce security risks if misused.

### Interview Questions
**Q: What is XSS?**  
A vulnerability where attackers inject malicious scripts.

**Q: Why is backend validation mandatory?**  
Client-side checks can be bypassed.

---

## 25. HTML in Modern Frameworks

### Explanation
Frameworks like React generate HTML dynamically.

### Interview Questions
**Q: Is HTML still relevant in React?**  
Yes, HTML is still the final output rendered in the browser.

**Q: CSR vs SSR?**  
CSR builds HTML in the browser; SSR sends HTML from the server.

---

## 26. HTML Best Practices

### Interview Questions
- Why avoid inline styles?
- Why use semantic HTML?
- Why keep HTML clean and minimal?

**Answer Summary:**  
Clean HTML improves maintainability, accessibility, performance, and SEO.

---

## Final Interview Tip

When answering HTML questions:
**Define → Explain → Connect to full-stack usage**

Example:
> HTML structures the UI, forms send data to backend APIs, and JavaScript dynamically updates the DOM.

---

### Author
**Rajendra Behera**  
Full-Stack Web Developer (Fresher)
