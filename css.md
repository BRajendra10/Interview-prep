# **CSS - CASCADING STYLE SHEET**

---

## 1. What is CSS?

### Explanation

CSS (Cascading Style Sheets) is used to **style and layout HTML elements**.
It defines **how content looks**, while HTML defines **what content exists**.

* HTML → Structure
* CSS → Styling
* JavaScript → Behavior

### Interview Question

**Q:** What is CSS?
**A:** CSS is used to control the appearance and layout of HTML elements on a webpage, including colors, fonts, spacing, and positioning.

### Code Example

```css
p {
  color: red;
  font-size: 16px;
}
```

---

## 2. Ways to Write CSS

### Explanation

1. **Inline CSS** → written inside the HTML element
2. **Internal CSS** → written inside `<style>` tag in HTML
3. **External CSS** → written in a separate `.css` file (**best practice**)

### Interview Question

**Q:** Which CSS method is best and why?
**A:** External CSS is best because it improves **maintainability, reusability**, and **separation of concerns**.

### Code Example

**Inline CSS**:

```html
<p style="color: red;">Hello</p>
```

**Internal CSS**:

```html
<style>
  p { color: red; }
</style>
```

**External CSS** (`style.css`):

```css
p { color: red; }
```

---

## 3. CSS Syntax

### Explanation

CSS is made of three parts:

* **Selector** → the HTML element you want to style
* **Property** → what aspect you want to change
* **Value** → the setting of that property

### Interview Question

**Q:** What is the structure of a CSS rule?
**A:** A CSS rule consists of a selector, property, and value.

### Code Example

```css
h1 {
  color: blue;
  font-size: 24px;
  text-align: center;
}
```

---

## 4. CSS Selectors

### Explanation

Selectors define **which elements** the styles apply to.

* Element → `p`
* Class → `.box`
* ID → `#main`
* Universal → `*`
* Attribute → `input[type="text"]`

### Interview Question

**Q:** What is the difference between class and id?
**A:** Class can be reused on multiple elements; ID must be unique on a page.

### Code Example

```css
/* Element selector */
p { color: green; }

/* Class selector */
.box { border: 1px solid black; }

/* ID selector */
#main { background-color: yellow; }
```

---

## 5. Pseudo-Classes

### Explanation

Pseudo-classes target elements based on **state or position**.

* `:hover` → when mouse is over
* `:active` → when element is clicked
* `:focus` → when input is focused
* `:first-child` / `:last-child`
* `:nth-child(n)` → target specific child

### Interview Question

**Q:** What is `:hover`?
**A:** It applies styles when the user places the mouse over an element.

### Code Example

```css
button:hover {
  background-color: blue;
  color: white;
}
```

---

## 6. Pseudo-Elements

### Explanation

Pseudo-elements target **parts of an element**, not the element itself.

* `::before` → inserts content before element
* `::after` → inserts content after element
* `::first-letter` → styles first letter
* `::first-line` → styles first line

### Interview Question

**Q:** Difference between pseudo-class and pseudo-element?
**A:** Pseudo-class targets a **state** (hover, focus), pseudo-element targets a **part** of an element (first letter, content before/after).

### Code Example

```css
p::first-letter {
  font-size: 2em;
  color: red;
}

p::before {
  content: "Note: ";
  font-weight: bold;
}
```

---

## 7. CSS Combinators

### Explanation

Combinators define **relationships between selectors**:

* Descendant → `div p` (any level)
* Child → `div > p` (direct child)
* Adjacent sibling → `h1 + p`
* General sibling → `h1 ~ p`

### Interview Question

**Q:** Difference between descendant and child selector?
**A:** Descendant selects **all nested elements**; child selects **only direct children**.

### Code Example

```css
div p { color: green; }   /* all p inside div */
div > p { color: blue; }  /* only direct children */
h1 + p { font-weight: bold; } /* first p after h1 */
```

---

## 8. CSS Specificity

### Explanation

Specificity determines **which style wins** if multiple rules target the same element.

**Priority order:**

1. `!important`
2. Inline styles
3. ID
4. Class / pseudo-class
5. Element

### Interview Question

**Q:** What happens if two CSS rules conflict?
**A:** The rule with **higher specificity** takes precedence.

### Code Example

```css
#main { color: red; }      /* higher specificity than .box */
.box { color: blue; }
```

---

## 9. Box Model

### Explanation

Every element has **four parts**:

* **Content** → text or image
* **Padding** → space inside border
* **Border** → around padding
* **Margin** → space outside element

### Interview Question

**Q:** Difference between padding and margin?
**A:** Padding is inside the border; margin is outside the border.

### Code Example

```css
div {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  margin: 10px;
}
```

---

## 10. Box-Sizing

### Explanation

`box-sizing` controls whether **padding and border are included in width/height**.

### Interview Question

**Q:** Why use `box-sizing: border-box`?
**A:** Makes layout predictable, because width/height includes padding and border.

### Code Example

```css
* {
  box-sizing: border-box;
}
```

---

## 11. CSS Display Property

### Explanation

`display` determines **how an element is rendered** on the page.

* `block` → takes full width, starts on new line
* `inline` → flows inline with text, width/height ignored
* `inline-block` → inline but allows width/height
* `none` → hides element
* `flex` → enables flex container
* `grid` → enables grid container

### Interview Question

**Q:** Difference between `display: none` and `visibility: hidden`?
**A:**

* `display: none` → element is removed from the layout, no space occupied
* `visibility: hidden` → element is hidden but **space is still taken**

### Code Example

```css
/* Block element */
div { display: block; }

/* Inline element */
span { display: inline; }

/* Hidden element */
p.hidden { display: none; }

/* Flex container */
.container { display: flex; }
```

---

## 12. CSS Positioning

### Explanation

`position` controls **how an element is positioned**.

* `static` → default, normal flow
* `relative` → relative to its normal position
* `absolute` → relative to nearest **positioned ancestor**
* `fixed` → relative to viewport, stays on scroll
* `sticky` → behaves like relative until scroll threshold

### Interview Question

**Q:** Absolute element is positioned relative to what?
**A:** Its nearest **positioned ancestor** (not static).

### Code Example

```css
.relative-box { position: relative; top: 10px; left: 20px; }
.absolute-box { position: absolute; top: 0; right: 0; }
.fixed-header { position: fixed; top: 0; width: 100%; }
```

---

## 13. Flexbox

### Explanation

Flexbox is used for **1-dimensional layout** (row or column).

**Container properties:**

* `display: flex` → enables flex
* `flex-direction` → row / column
* `justify-content` → main axis alignment
* `align-items` → cross axis alignment
* `gap` → spacing between items

**Item properties:**

* `flex-grow` → how much space item takes
* `flex-shrink` → how much item shrinks
* `flex-basis` → initial size

### Interview Question

**Q:** Difference between `justify-content` and `align-items`?
**A:**

* `justify-content` → aligns along **main axis** (row/column)
* `align-items` → aligns along **cross axis**

### Code Example

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
}

.item {
  flex-grow: 1;
}
```

---

## 14. CSS Grid

### Explanation

Grid is used for **2-dimensional layout** (rows + columns).

**Container properties:**

* `display: grid`
* `grid-template-columns` → define column sizes
* `grid-template-rows` → define row sizes
* `gap` → spacing between cells

### Interview Question

**Q:** Grid vs Flexbox?
**A:** Grid → 2D layout (rows + columns)
Flexbox → 1D layout (row **or** column)

### Code Example

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: 100px 200px;
  gap: 10px;
}

.item {
  background-color: lightblue;
}
```

---

## 15. Responsive Design

### Explanation

Responsive design makes websites **adapt to different screen sizes**.

* Media queries → apply CSS conditionally
* `%`, `rem`, `vw`, `vh` → relative units
* Mobile-first approach → write for small screens first

### Interview Question

**Q:** What is a media query?
**A:** A CSS technique to **apply styles based on screen size** or device type.

### Code Example

```css
/* Mobile first */
body { font-size: 14px; }

/* Tablet */
@media (min-width: 768px) {
  body { font-size: 16px; }
}

/* Desktop */
@media (min-width: 1024px) {
  body { font-size: 18px; }
}
```

---

## 16. CSS Units

### Explanation

Units define **measurements in CSS**:

* `px` → fixed pixels
* `%` → percentage of parent
* `em` → relative to parent font-size
* `rem` → relative to root font-size
* `vw` / `vh` → % of viewport width/height

### Interview Question

**Q:** Difference between `em` and `rem`?
**A:**

* `em` → relative to **parent** font-size
* `rem` → relative to **root** font-size

### Code Example

```css
p { font-size: 1.2em; }
h1 { font-size: 2rem; }
div { width: 50vw; height: 30vh; }
```

---

## 17. Colors & Backgrounds

### Explanation

CSS controls **colors and backgrounds**:

* `color` → text color
* `background-color` → background color
* `background-image` → images as background
* `background-size: cover` → fill container

### Interview Question

**Q:** Name different ways to define colors in CSS.
**A:** Hex (`#ff0000`), RGB (`rgb(255,0,0)`), HSL (`hsl(0, 100%, 50%)`)

### Code Example

```css
body { color: white; background-color: black; }
div { background-image: url('bg.jpg'); background-size: cover; }
```

---

## 18. Transitions & Animations

### Explanation

CSS allows **smooth transitions and animations**.

* `transition` → smooth change on state change
* `@keyframes` → define animation frames
* `animation` → run animation automatically

### Interview Question

**Q:** Difference between transition and animation?
**A:** Transition → triggered by **state change** (hover, focus)
Animation → runs **automatically** using keyframes

### Code Example

```css
/* Transition */
button {
  background-color: blue;
  transition: background-color 0.3s;
}

button:hover {
  background-color: red;
}

/* Animation */
@keyframes slide {
  from { transform: translateX(0); }
  to { transform: translateX(100px); }
}

.box {
  animation: slide 2s infinite alternate;
}
```

---

## 19. Common CSS Mistakes

### Explanation

Common mistakes freshers make:

* ❌ Overusing `!important`
* ❌ Styling with IDs
* ❌ Not using Flexbox/Grid for layout
* ❌ Fixed pixel layouts instead of responsive units

### Interview Question

**Q:** Name some common CSS mistakes by beginners.
**A:** Overusing `!important`, using IDs, ignoring responsive design, using fixed pixels instead of relative units.

---
