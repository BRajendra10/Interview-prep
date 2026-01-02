# HTML Interview Preparation Guide  
### Full-Stack Web Developer (Fresher Level)

This document is a **complete HTML interview reference**, covering **everything that can realistically be asked** in frontend or full-stack interviews.

---

## 1. What is HTML?

### Explanation
HTML (HyperText Markup Language) is the standard markup language used to define the **structure and meaning** of web content.  
It describes **what content exists**, not how it looks or behaves.

- HTML → Structure  
- CSS → Styling  
- JavaScript → Behavior  

### Interview Question
**Q: What is HTML?**  
HTML is a markup language used to structure web content such as headings, paragraphs, forms, images, and links.

---

## 2. Is HTML a Programming Language?

### Explanation
HTML has no logic, variables, loops, or conditions.

### Interview Question
**Q: Is HTML a programming language?**  
No. HTML is a markup language because it only describes structure, not logic or behavior.

---

## 3. HTML vs HTML5

### Explanation
HTML5 is the modern standard and introduced:
- Semantic elements
- Native audio/video
- Better forms & validation
- Browser APIs (storage, canvas)

### Interview Question
**Q: Difference between HTML and HTML5?**  
HTML5 adds semantic tags, multimedia support, APIs, and improved form handling.

---

## 4. HTML Document Structure

### Explanation
Browsers expect a standard structure to correctly parse HTML.

### Interview Question
**Q: What is the basic structure of an HTML document?**  
It includes `<!DOCTYPE html>`, `<html>`, `<head>`, and `<body>`.

---

## 5. `<!DOCTYPE html>`

### Explanation
Informs the browser to render the page in **standards mode**.

### Interview Questions
**Q: Why do we use DOCTYPE?**  
To ensure consistent rendering across browsers.

**Q: What if it’s missing?**  
The browser may enter quirks mode.

---

## 6. `<head>` vs `<body>`

### Explanation
- `<head>` → metadata, SEO, styles, scripts  
- `<body>` → visible UI  

### Interview Question
**Q: What goes inside the head tag?**  
Title, meta tags, stylesheets, fonts, and scripts.

---

## 7. Meta Tags

### Explanation
Meta tags provide information about the page.

### Interview Questions
**Q: What are meta tags used for?**  
SEO, responsiveness, encoding, browser behavior.

**Q: What is viewport meta tag?**  
Controls layout on mobile devices.

---

## 8. Block vs Inline Elements

### Explanation
- Block → full width, new line  
- Inline → content width only  

### Interview Question
**Q: Difference between div and span?**  
Div is block-level; span is inline.

---

## 9. Inline vs Inline-Block vs Block

### Explanation
- Inline → no width/height  
- Inline-block → width/height allowed  
- Block → full width  

### Interview Question
**Q: Why use inline-block?**  
To style inline elements with size control.

---

## 10. Void (Self-Closing) Elements

### Explanation
Void elements don’t wrap content.

### Interview Question
**Q: What are void elements?**  
img, input, br, hr, meta.

---

## 11. Semantic HTML (CRITICAL)

### Explanation
Semantic HTML uses meaningful tags that describe content purpose.

Common tags:
- header, nav, main  
- section, article  
- aside, footer  

### Interview Questions
**Q: What is semantic HTML?**  
HTML that improves readability, accessibility, and SEO.

**Q: Section vs Article?**  
Article is standalone; section groups related content.

---

## 12. Global Attributes

### Explanation
Attributes that work on all elements.

### Interview Question
**Q: What are global attributes?**  
id, class, style, title, tabindex.

---

## 13. id vs class

### Explanation
- id → unique  
- class → reusable  

### Interview Question
**Q: Why should IDs not repeat?**  
They uniquely identify elements for JS and accessibility.

---

## 14. Lists in HTML

### Explanation
Lists group related items in a structured way.

Types:
- Ordered (`ol`)
- Unordered (`ul`)
- Description (`dl`)

### Interview Questions
**Q: Difference between ol and ul?**  
ol is ordered; ul is unordered.

**Q: What is a description list?**  
Used for term–definition pairs.

---

## 15. Tables in HTML

### Explanation
Tables display **tabular data**, not layout.

Core elements:
table, thead, tbody, tfoot, tr, th, td

### Interview Questions
**Q: th vs td?**  
th is header cell; td is data cell.

**Q: Why not use tables for layout?**  
Bad for responsiveness and accessibility.

---

## 16. Forms (FULL-STACK CORE)

### Explanation
Forms collect user input and send it to the backend.

Key attributes:
- action
- method
- name
- value

### Interview Questions
**Q: How does form data reach backend?**  
Via HTTP request.

**Q: GET vs POST?**  
GET → URL, POST → request body.

---

## 17. Form Validation

### Explanation
HTML provides client-side validation.

### Interview Questions
**Q: Client vs server validation?**  
Client improves UX; server ensures security.

---

## 18. Label & Accessibility

### Explanation
Labels associate text with inputs.

### Interview Question
**Q: Why use label instead of placeholder?**  
Better accessibility and usability.

---

## 19. Input Types

### Explanation
HTML5 input types improve validation & UX.

### Interview Question
**Q: Why use type=email?**  
Built-in validation and mobile keyboards.

---

## 20. DOM (Document Object Model)

### Explanation
DOM is a tree representation of HTML in memory.

### Interview Question
**Q: What is DOM?**  
A programming interface for HTML manipulation.

---

## 21. Data Attributes

### Explanation
Custom attributes for storing extra data.

### Interview Question
**Q: Why use data-* attributes?**  
To store JS-related data without affecting semantics.

---

## 22. Script Loading (`async` vs `defer`)

### Explanation
Controls when scripts execute.

### Interview Question
**Q: async vs defer?**  
Defer preserves order; async doesn’t.

---

## 23. Accessibility (IMPORTANT)

### Explanation
Accessibility ensures usability for all users.

### Interview Questions
**Q: What is accessibility?**  
Designing apps usable by people with disabilities.

**Q: What are ARIA attributes?**  
They help screen readers understand dynamic UI.

---

## 24. Images & Media

### Explanation
HTML supports native media elements.

### Interview Questions
**Q: What is lazy loading?**  
Loading images only when needed.

**Q: img vs background image?**  
img is semantic; background is decorative.

---

## 25. SEO (HTML Perspective)

### Explanation
HTML structure impacts search ranking.

### Interview Questions
**Q: Title vs H1?**  
Title → SEO; H1 → visible heading.

---

## 26. HTML Entities

### Explanation
Entities represent reserved characters.

### Interview Question
**Q: Why use HTML entities?**  
To display reserved symbols correctly.

---

## 27. iframe & Embedding Content

### Explanation
iframe embeds external content.

### Interview Question
**Q: When should iframe be avoided?**  
Due to security and performance concerns.

---

## 28. HTML Parsing & Rendering Flow

### Explanation
Browser:
HTML → DOM → CSSOM → Render Tree → Paint

### Interview Question
**Q: How does browser render HTML?**  
By parsing HTML into DOM and painting it.

---

## 29. HTML Performance Best Practices

### Explanation
Good HTML improves load time.

### Interview Questions
**Q: How can HTML improve performance?**  
Clean structure, optimized images, proper script loading.

---

## 30. HTML Security Basics

### Explanation
HTML can introduce security risks.

### Interview Questions
**Q: What is XSS?**  
Injection of malicious scripts.

**Q: Why backend validation is mandatory?**  
Client checks can be bypassed.

---

## 31. HTML in Modern Frameworks

### Explanation
Frameworks generate HTML dynamically.

### Interview Questions
**Q: Is HTML relevant in React?**  
Yes, HTML is the final output.

**Q: CSR vs SSR?**  
CSR builds in browser; SSR sends from server.

---

## 32. HTML Best Practices (Interview Gold)

### Interview Questions
- Why avoid inline styles?
- Why use semantic HTML?
- Why keep HTML minimal?

**Answer Summary:**  
Clean HTML improves maintainability, accessibility, performance, and SEO.

---

## Final Interview Tip

Always answer like this:
**Define → Explain → Connect to real usage**

> HTML structures the UI, forms send data to backend APIs, and JavaScript updates the DOM dynamically.
