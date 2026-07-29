# CSS Interview Answers

---

# 1. What is CSS?

### Answer

CSS stands for **Cascading Style Sheets**.

It is a stylesheet language used to describe the presentation and layout of HTML elements.

CSS controls:

- Colors
- Fonts
- Spacing
- Layout
- Animations
- Responsive design

### Example

HTML:

```html
<h1>Hello World</h1>
```

CSS:

```css
h1 {
  color: blue;
  font-size: 40px;
}
```

### Output

The heading appears blue with a larger font size.

### Interview Tip

HTML creates the structure, CSS controls the appearance.

---

# 2. Why do we use CSS?

### Answer

CSS is used to make web pages attractive, responsive, and easier to maintain.

### Without CSS

```html
<h1>Hello</h1>
<p>Welcome</p>
```

The page uses default browser styles.

### With CSS

```css
body {
  background: white;
  font-family: Arial;
}

h1 {
  color: green;
}
```

### Benefits

- Improves visual design
- Separates content from presentation
- Reduces code duplication
- Makes responsive layouts possible
- Improves user experience

### Interview Tip

CSS follows the principle:

> HTML = Structure  
> CSS = Style  
> JavaScript = Behavior

---

# 3. What are the advantages of CSS?

### Answer

CSS provides many advantages in web development.

### Advantages

## 1. Separation of Concerns

HTML handles structure and CSS handles styling.

Example:

```html
<button>Submit</button>
```

CSS:

```css
button {
  background: blue;
}
```

---

## 2. Code Reusability

One CSS rule can style multiple elements.

```css
.card {
  padding: 20px;
}
```

Applied to:

```html
<div class="card"></div>
<div class="card"></div>
```

---

## 3. Faster Development

External CSS files can style multiple pages.

---

## 4. Better Performance

Browsers can cache CSS files.

---

## 5. Responsive Design

CSS helps create layouts for:

- Mobile
- Tablet
- Desktop

### Interview Tip

The biggest advantage of CSS is maintaining a clean separation between structure and presentation.

---

# 4. What are the different ways to add CSS?

### Answer

There are three ways to apply CSS:

1. Inline CSS
2. Internal CSS
3. External CSS

---

## 1. Inline CSS

CSS is written directly inside the HTML element.

Example:

```html
<h1 style="color:red;">Hello</h1>
```

### Use:

- Quick changes
- Testing

### Disadvantage:

- Hard to maintain
- Not reusable

---

## 2. Internal CSS

CSS is written inside the `<style>` tag.

Example:

```html
<head>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>
```

### Use:

- Single-page styling

---

## 3. External CSS

CSS is written in a separate file.

HTML:

```html
<link rel="stylesheet" href="style.css" />
```

CSS file:

```css
h1 {
  color: red;
}
```

### Use:

- Production applications
- Multiple pages

### Interview Tip

External CSS is the preferred approach for large projects.

---

# 5. Difference between inline, internal, and external CSS?

### Answer

| Inline                | Internal             | External             |
| --------------------- | -------------------- | -------------------- |
| Inside HTML element   | Inside `<style>` tag | Separate `.css` file |
| Highest priority      | Medium priority      | Reusable             |
| Difficult maintenance | Page-specific        | Best for projects    |

### Example

### Inline

```html
<p style="color:red">Text</p>
```

### Internal

```html
<style>
  p {
    color: red;
  }
</style>
```

### External

```css
p {
  color: red;
}
```

### Interview Tip

In professional applications, external CSS or CSS modules are commonly used.

---

# 6. What is CSS syntax?

### Answer

CSS syntax consists of:

- Selector
- Property
- Value

### Syntax

```css
selector {
  property: value;
}
```

### Example

```css
h1 {
  color: blue;
  font-size: 30px;
}
```

Explanation:

```
h1          → Selector

color       → Property

blue        → Value
```

### Interview Tip

Each declaration ends with a semicolon.

---

# 7. What are selectors in CSS?

### Answer

CSS selectors are used to target HTML elements that we want to style.

### Example

HTML:

```html
<p>Hello</p>
```

CSS:

```css
p {
  color: red;
}
```

Here:

```css
p
```

is the selector.

### Types of Selectors

- Element selector
- Class selector
- ID selector
- Universal selector
- Attribute selector
- Pseudo-class selector
- Pseudo-element selector

### Interview Tip

Selectors decide **which elements receive styles**.

---

# 8. What are CSS properties and values?

### Answer

CSS properties define what aspect of an element we want to change.

Values define the setting applied to that property.

### Example

```css
.box {
  width: 200px;

  background-color: blue;
}
```

Here:

```
width
background-color
```

are properties.

```
200px
blue
```

are values.

### Common Properties

- color
- width
- height
- margin
- padding
- display
- position
- font-size

### Interview Tip

A CSS declaration is a combination of property and value.

---

# 9. What are comments in CSS?

### Answer

Comments are notes written inside CSS code that browsers ignore.

They are used for documentation and explanation.

### Syntax

```css
/* This is a CSS comment */

body {
  background: white;
}
```

### Uses

- Explain complex code
- Temporarily disable styles
- Help team members understand code

Example:

```css
/* Header styling */

.header {
  display: flex;
}
```

### Interview Tip

CSS comments do not affect the final output.

---

# 10. What is the difference between CSS2 and CSS3?

### Answer

CSS3 is the advanced version of CSS2 with new features and better browser support.

### Comparison

| CSS2                        | CSS3                     |
| --------------------------- | ------------------------ |
| Single specification        | Divided into modules     |
| Limited animations          | Supports animations      |
| No flexbox                  | Supports Flexbox         |
| No grid                     | Supports CSS Grid        |
| Limited responsive features | Better responsive design |

### CSS3 Features

- Flexbox
- Grid
- Media Queries
- Animations
- Transitions
- Transforms
- Border-radius
- Box-shadow
- Gradients

### Example

CSS3 animation:

```css
.box {
  animation: move 2s;
}

@keyframes move {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(100px);
  }
}
```

### Interview Tip

Modern frontend development heavily depends on CSS3 features.

---

---

# 11. What are different types of CSS selectors?

### Answer

CSS selectors are patterns used to select HTML elements and apply styles.

### Main Types of CSS Selectors

1. Universal Selector
2. Element Selector
3. Class Selector
4. ID Selector
5. Attribute Selector
6. Descendant Selector
7. Child Selector
8. Sibling Selector
9. Pseudo-class Selector
10. Pseudo-element Selector

### Example

```css
/* Element selector */
p {
  color: blue;
}

/* Class selector */
.card {
  padding: 20px;
}

/* ID selector */
#header {
  background: black;
}
```

### Interview Tip

Selectors are the foundation of CSS. Understanding specificity with selectors is important for interviews.

---

# 12. What is an element selector?

### Answer

An element selector targets HTML elements by their tag name.

### Syntax

```css
element {
  property: value;
}
```

### Example

HTML:

```html
<h1>Welcome</h1>

<p>Hello World</p>
```

CSS:

```css
h1 {
  color: blue;
}

p {
  font-size: 18px;
}
```

### Output

All `<h1>` elements become blue, and all `<p>` elements get 18px font size.

### Interview Tip

Element selectors apply styles to all matching elements on the page.

---

# 13. What is a class selector?

### Answer

A class selector selects elements with a specific `class` attribute.

It starts with a dot (`.`).

### Syntax

```css
.className {
  property: value;
}
```

### Example

HTML:

```html
<div class="card">Product</div>

<div class="card">Another Product</div>
```

CSS:

```css
.card {
  padding: 20px;
  border: 1px solid black;
}
```

Both elements receive the same style.

### Interview Tip

Classes are reusable and are the most commonly used selectors in projects.

---

# 14. What is an ID selector?

### Answer

An ID selector selects an element with a specific `id` attribute.

It starts with a hash (`#`).

### Syntax

```css
#idName {
  property: value;
}
```

### Example

HTML:

```html
<h1 id="title">Welcome</h1>
```

CSS:

```css
#title {
  color: red;
}
```

### Important Rule

An ID should be unique within a page.

### Interview Tip

ID selectors have higher specificity than class selectors.

---

# 15. Difference between class and ID selector?

### Answer

| Class Selector             | ID Selector          |
| -------------------------- | -------------------- |
| Starts with `.`            | Starts with `#`      |
| Can be reused              | Should be unique     |
| Lower specificity          | Higher specificity   |
| Used for multiple elements | Used for one element |

### Example

Class:

```css
.card {
  padding: 20px;
}
```

Used:

```html
<div class="card"></div>
<div class="card"></div>
```

ID:

```css
#navbar {
  height: 60px;
}
```

Used:

```html
<nav id="navbar"></nav>
```

### Interview Tip

Prefer classes for styling. IDs are usually used for unique elements and JavaScript targeting.

---

# 16. What is the universal selector?

### Answer

The universal selector (`*`) selects all HTML elements.

### Example

```css
* {
  margin: 0;
  padding: 0;
}
```

### Common Use

CSS reset:

```css
* {
  box-sizing: border-box;
}
```

### Advantages

- Applies common styles globally
- Helps create consistent layouts

### Disadvantages

- Can affect performance on very large pages
- May override default browser styles

### Interview Tip

Universal selectors have the lowest specificity.

---

# 17. What are attribute selectors?

### Answer

Attribute selectors select elements based on their attributes or attribute values.

### Syntax

```css
[attribute] {
  property: value;
}
```

### Example

Select all inputs with type email:

```css
input[type="email"] {
  border: 2px solid blue;
}
```

### Other Examples

Contains attribute:

```css
a[href] {
  color: red;
}
```

Starts with value:

```css
img[src^="profile"] {
  width: 100px;
}
```

Ends with value:

```css
img[src$=".png"] {
  border-radius: 50%;
}
```

### Interview Tip

Attribute selectors are useful when you cannot add extra classes.

---

# 18. What are descendant selectors?

### Answer

A descendant selector selects elements that are inside another element, at any level.

### Syntax

```css
parent child {
  property: value;
}
```

### Example

HTML:

```html
<div>
  <p>Hello</p>
</div>
```

CSS:

```css
div p {
  color: red;
}
```

This selects all `<p>` elements inside `<div>`.

### Interview Tip

The space between selectors represents "inside".

---

# 19. What are child selectors?

### Answer

A child selector selects only direct children of an element.

It uses the `>` symbol.

### Syntax

```css
parent > child {
  property: value;
}
```

### Example

HTML:

```html
<div>
  <p>Direct child</p>

  <section>
    <p>Nested child</p>
  </section>
</div>
```

CSS:

```css
div > p {
  color: blue;
}
```

Only the first `<p>` is selected.

### Interview Tip

Difference:

```
div p
```

Selects all descendants.

```
div > p
```

Selects only direct children.

---

# 20. Difference between `>` and space selector?

### Answer

Both select child elements, but they behave differently.

### Descendant Selector (space)

```css
div p {
  color: red;
}
```

Selects:

```html
<div>
  <p></p>

  <section>
    <p></p>
  </section>
</div>
```

Both paragraphs are selected.

---

### Child Selector (>)

```css
div > p {
  color: blue;
}
```

Selects only:

```html
<div>
  <p></p>
</div>
```

Not:

```html
<div>
  <section>
    <p></p>
  </section>
</div>
```

### Interview Tip

Use `>` when you need strict structure control.

---

# 21. What are sibling selectors?

### Answer

Sibling selectors select elements that share the same parent.

There are two types:

1. Adjacent sibling selector (`+`)
2. General sibling selector (`~`)

### Example HTML

```html
<h2>Heading</h2>

<p>Paragraph</p>

<p>Another Paragraph</p>
```

---

# 22. Difference between adjacent and general sibling selectors?

### Answer

## Adjacent Sibling (`+`)

Selects only the immediately following sibling.

Example:

```css
h2 + p {
  color: red;
}
```

Only the first paragraph after `<h2>` is selected.

---

## General Sibling (`~`)

Selects all following siblings.

Example:

```css
h2 ~ p {
  color: blue;
}
```

Both paragraphs are selected.

### Comparison

| Adjacent (+)      | General (~)            |
| ----------------- | ---------------------- |
| Only next sibling | All following siblings |
| More specific     | Less restrictive       |

### Interview Tip

Both elements must share the same parent.

---

# 23. What are pseudo-classes?

### Answer

Pseudo-classes define a special state of an element.

They start with a single colon (`:`).

### Common Pseudo-classes

- `:hover`
- `:focus`
- `:active`
- `:visited`
- `:first-child`
- `:last-child`
- `:nth-child()`

### Example

```css
button:hover {
  background: blue;
}
```

When the user moves the mouse over the button, the style applies.

### Other Example

```css
input:focus {
  border-color: green;
}
```

### Interview Tip

Pseudo-classes style elements based on state or position.

---

# 24. What are pseudo-elements?

### Answer

Pseudo-elements style a specific part of an element.

They use double colon syntax (`::`).

### Common Pseudo-elements

- `::before`
- `::after`
- `::first-letter`
- `::first-line`
- `::selection`

### Example

```css
h1::before {
  content: "⭐ ";
}
```

Output:

```
⭐ Heading
```

### Example

```css
p::first-letter {
  font-size: 40px;
}
```

### Interview Tip

Pseudo-elements create or style virtual elements.

---

# 25. Difference between pseudo-class and pseudo-element?

### Answer

| Pseudo-class                | Pseudo-element             |
| --------------------------- | -------------------------- |
| Styles element state        | Styles part of an element  |
| Uses single colon           | Uses double colon          |
| Does not create new content | Can create virtual content |
| Example: `:hover`           | Example: `::before`        |

### Examples

Pseudo-class:

```css
button:hover {
  color: red;
}
```

Pseudo-element:

```css
p::first-letter {
  font-size: 30px;
}
```

### Interview Tip

Remember:

- `:` → State
- `::` → Part of element

---

---

# 26. What is CSS specificity?

### Answer

CSS specificity is the rule used by browsers to decide which CSS style should be applied when multiple rules target the same element.

When two or more CSS rules conflict, the selector with higher specificity gets priority.

### Example

HTML:

```html
<p class="text">Hello</p>
```

CSS:

```css
p {
  color: blue;
}

.text {
  color: red;
}
```

Output:

```
Hello
```

Color will be red because the class selector has higher specificity than the element selector.

### Interview Tip

Specificity decides the winner when CSS rules conflict.

---

# 27. How does CSS specificity work?

### Answer

CSS specificity follows a priority order.

The browser calculates the specificity score of selectors.

### Priority Order (Highest to Lowest)

1. Inline styles
2. ID selectors
3. Class selectors, attributes, pseudo-classes
4. Element selectors and pseudo-elements
5. Universal selector

### Example

```css
p {
  color: blue;
}

.text {
  color: green;
}

#title {
  color: red;
}
```

HTML:

```html
<p id="title" class="text">Hello</p>
```

Applied color:

```
red
```

Because:

```
ID > Class > Element
```

### Interview Tip

Specificity is calculated before the cascade rule is applied.

---

# 28. What is the specificity order in CSS?

### Answer

The specificity order is:

```
Inline Style
      ↓
ID Selector
      ↓
Class / Attribute / Pseudo-class
      ↓
Element / Pseudo-element
      ↓
Universal Selector
```

### Example

```css
* {
  color: black;
}

p {
  color: blue;
}

.text {
  color: green;
}

#heading {
  color: red;
}
```

The final color will be:

```css
red
```

because ID has the highest priority.

### Interview Tip

Specificity is not based on how many selectors you write, but on their weight.

---

# 29. Which has higher priority: class or ID?

### Answer

ID selectors have higher priority than class selectors.

### Example

HTML:

```html
<h1 id="title" class="heading">Hello</h1>
```

CSS:

```css
.heading {
  color: blue;
}

#title {
  color: red;
}
```

Output:

```
Hello
```

Color:

```css
red
```

### Reason

Specificity:

```
ID = higher priority
Class = lower priority
```

### Interview Tip

Avoid using many IDs for styling because they make CSS harder to override.

---

# 30. What is the universal selector specificity?

### Answer

The universal selector (`*`) has the lowest specificity.

### Example

```css
* {
  margin: 0;
}
```

Specificity value:

```
0
```

### Example

```css
* {
  color: black;
}

p {
  color: blue;
}
```

The paragraph will be blue.

### Interview Tip

Universal selectors are useful for resets but should be used carefully.

---

# 31. What is inline style specificity?

### Answer

Inline styles have the highest specificity except when `!important` is used.

### Example

HTML:

```html
<p style="color:red;">Hello</p>
```

CSS:

```css
p {
  color: blue;
}
```

Output:

```
red
```

### Reason

Inline style has higher priority.

### Specificity Weight

```
Inline style > ID > Class > Element
```

### Interview Tip

Avoid excessive inline styles because they reduce maintainability.

---

# 32. What is `!important` in CSS?

### Answer

`!important` is used to give a CSS rule the highest priority.

### Example

```css
p {
  color: blue !important;
}
```

Even if another rule has higher specificity, this rule may override it.

### Example

```css
#title {
  color: red;
}

p {
  color: blue !important;
}
```

The paragraph becomes blue.

### Interview Tip

`!important` should be used rarely.

---

# 33. Why should we avoid using `!important`?

### Answer

Although `!important` can force styles, excessive usage creates problems.

### Problems

- Makes CSS difficult to maintain
- Hard to override later
- Creates specificity conflicts
- Makes debugging harder

### Bad Example

```css
.button {
  background: red !important;
}

.primary-button {
  background: blue !important;
}
```

Now managing styles becomes difficult.

### Better Approach

Use proper:

- Class names
- CSS structure
- Component-based styling

### Interview Tip

Use `!important` only for special cases, not as a regular solution.

---

# 34. How does specificity affect inheritance?

### Answer

Inheritance allows some CSS properties to pass from parent elements to child elements.

However, inherited styles have lower priority than directly applied styles.

### Example

HTML:

```html
<div>
  <p>Hello</p>
</div>
```

CSS:

```css
div {
  color: blue;
}

p {
  color: red;
}
```

Output:

```
Hello
```

The paragraph is red because direct styles have higher priority than inherited styles.

### Common Inherited Properties

- color
- font-family
- font-size
- line-height

### Non-inherited Properties

- width
- height
- margin
- padding
- border

### Interview Tip

Specificity applies to direct styles, not inherited styles.

---

# 35. How do you calculate CSS specificity?

### Answer

Specificity is calculated using four values:

```
(a, b, c, d)
```

Where:

### a = Inline styles

Example:

```html
style="color:red"
```

Value:

```
1
```

---

### b = IDs

Example:

```css
#header
```

Value:

```
1
```

---

### c = Classes, attributes, pseudo-classes

Examples:

```css
.card

[type="text"]

:hover
```

Value:

```
1
```

---

### d = Elements and pseudo-elements

Examples:

```css
p

::before
```

Value:

```
1
```

---

### Example

```css
#header .title p {
  color: red;
}
```

Calculation:

```
ID        = 1
Class     = 1
Element   = 1
```

Specificity:

```
(0,1,1,1)
```

---

### Another Example

```css
div.card#box {
  color: red;
}
```

Calculation:

```
ID       = 1
Class    = 1
Element = 1
```

Specificity:

```
(0,1,1,1)
```

### Interview Tip

Compare specificity from left to right:

```
Inline → ID → Class → Element
```

The larger value wins.

---

---

# 36. What is the CSS box model?

### Answer

The CSS box model describes how every HTML element is represented as a rectangular box.

Every element consists of four parts:

1. Content
2. Padding
3. Border
4. Margin

### Structure

```
+-----------------------+
|       Margin          |
|  +-----------------+  |
|  |     Border      |  |
|  | +-------------+ |  |
|  | |  Padding    | |  |
|  | | +---------+ | |  |
|  | | | Content | | |  |
|  | | +---------+ | |  |
|  | +-------------+ |  |
|  +-----------------+  |
+-----------------------+
```

### Example

```css
.box {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
  margin: 10px;
}
```

### Interview Tip

Every HTML element is treated as a box by the browser.

---

# 37. Explain content, padding, border, and margin.

### Answer

The box model has four main areas.

---

## 1. Content

The actual content of the element.

Example:

```html
<p>Hello World</p>
```

"Hello World" is the content.

---

## 2. Padding

Space between content and border.

Example:

```css
.box {
  padding: 20px;
}
```

---

## 3. Border

A line surrounding the padding and content.

Example:

```css
.box {
  border: 1px solid black;
}
```

---

## 4. Margin

Space outside the border.

Example:

```css
.box {
  margin: 20px;
}
```

### Visual Order

```
Margin
 ↓
Border
 ↓
Padding
 ↓
Content
```

### Interview Tip

Padding increases the inside space; margin increases the outside space.

---

# 38. Difference between padding and margin?

### Answer

Both create space around elements, but they work differently.

### Padding

Space inside the element between content and border.

```css
.box {
  padding: 20px;
}
```

### Margin

Space outside the element.

```css
.box {
  margin: 20px;
}
```

### Comparison

| Padding                    | Margin                            |
| -------------------------- | --------------------------------- |
| Inside the border          | Outside the border                |
| Affects element background | Background does not cover margin  |
| Increases element size     | Creates distance between elements |
| Cannot be negative         | Can be negative                   |

### Example

```css
.card {
  padding: 20px;
  margin: 30px;
}
```

### Interview Tip

Remember:

```
Padding = Inside space
Margin = Outside space
```

---

# 39. What is `box-sizing`?

### Answer

`box-sizing` defines how the browser calculates the total width and height of an element.

### Syntax

```css
box-sizing: value;
```

Two main values:

- content-box
- border-box

---

# 40. Difference between `content-box` and `border-box`?

### Answer

## content-box (Default)

Width and height apply only to the content area.

Example:

```css
.box {
  width: 200px;
  padding: 20px;
  border: 5px solid black;
}
```

Total width:

```
200 + 20 + 20 + 5 + 5

= 250px
```

---

## border-box

Width and height include:

- Content
- Padding
- Border

Example:

```css
.box {
  box-sizing: border-box;
  width: 200px;
}
```

Total width remains:

```
200px
```

### Comparison

| content-box                       | border-box                        |
| --------------------------------- | --------------------------------- |
| Default value                     | Commonly used                     |
| Width excludes padding and border | Width includes padding and border |
| Layout calculations are harder    | Easier responsive layouts         |

### Interview Tip

Most modern projects use:

```css
* {
  box-sizing: border-box;
}
```

---

# 41. Why do developers use `box-sizing: border-box`?

### Answer

Developers use `border-box` because it makes layout calculations predictable.

### Example

Without border-box:

```css
.card {
  width: 300px;
  padding: 20px;
}
```

Actual size:

```
340px
```

Because padding is added.

---

With border-box:

```css
.card {
  box-sizing: border-box;
  width: 300px;
  padding: 20px;
}
```

Actual size:

```
300px
```

### Benefits

- Easier responsive design
- Prevents unexpected overflow
- Simplifies width calculations

### Interview Tip

A common CSS reset is:

```css
* {
  box-sizing: border-box;
}
```

---

# 42. What happens when width and height are applied?

### Answer

The behavior depends on the value of `box-sizing`.

---

## With content-box

Example:

```css
.box {
  width: 200px;
  height: 100px;
  padding: 20px;
}
```

Actual size:

Width:

```
200 + 40 = 240px
```

Height:

```
100 + 40 = 140px
```

---

## With border-box

```css
.box {
  box-sizing: border-box;
  width: 200px;
  height: 100px;
  padding: 20px;
}
```

Actual size:

```
200px × 100px
```

Padding is included inside.

### Interview Tip

Always consider padding and border when calculating dimensions.

---

# 43. What is margin collapsing?

### Answer

Margin collapsing is a behavior where vertical margins of adjacent block elements combine into a single margin instead of adding together.

### Example

```css
.box1 {
  margin-bottom: 30px;
}

.box2 {
  margin-top: 20px;
}
```

Expected:

```
30 + 20 = 50px
```

Actual:

```
30px
```

The larger margin wins.

### Happens Between:

- Adjacent block elements
- Parent and first/last child elements

### Interview Tip

Margin collapsing mainly happens with vertical margins.

---

# 44. How do you prevent margin collapse?

### Answer

Several methods can prevent margin collapsing.

### Method 1: Add Border

```css
.parent {
  border: 1px solid transparent;
}
```

---

### Method 2: Add Padding

```css
.parent {
  padding-top: 1px;
}
```

---

### Method 3: Use Flexbox

```css
.parent {
  display: flex;
}
```

---

### Method 4: Create New Formatting Context

```css
.parent {
  overflow: hidden;
}
```

### Interview Tip

Flexbox and Grid layouts do not have traditional margin collapsing behavior.

---

# 45. Difference between outline and border?

### Answer

Both create visible lines around elements, but they behave differently.

### Border

- Takes space
- Affects element size
- Can have different sides
- Part of box model

Example:

```css
.box {
  border: 2px solid black;
}
```

---

### Outline

- Does not take space
- Does not affect element size
- Appears outside the border
- Cannot have different sides

Example:

```css
.box {
  outline: 2px solid red;
}
```

### Comparison

| Border                 | Outline                |
| ---------------------- | ---------------------- |
| Part of box model      | Not part of box model  |
| Takes space            | Does not take space    |
| Can affect layout      | Does not affect layout |
| Supports border-radius | Limited support        |

### Interview Tip

Browsers often use outlines to show keyboard focus.

Example:

```css
button:focus {
  outline: 2px solid blue;
}
```

---

---

# 46. What is the display property?

### Answer

The CSS `display` property defines how an element is displayed on the webpage.

It controls the layout behavior of an element.

### Syntax

```css
element {
  display: value;
}
```

### Common Values

- `block`
- `inline`
- `inline-block`
- `none`
- `flex`
- `grid`

### Example

```css
div {
  display: block;
}
```

### Interview Tip

The display property is one of the most important CSS properties for controlling layouts.

---

# 47. Explain `block` display.

### Answer

A block element takes the full available width of its parent element.

It always starts on a new line.

### Examples of Block Elements

```html
<div>
  <p></p>
  <h1>
    <section>
      <header>
        <footer></footer>
      </header>
    </section>
  </h1>
</div>
```

### Example

```css
.box {
  display: block;
}
```

### Behavior

```text
Element 1

Element 2

Element 3
```

Each block element appears on a new line.

### Characteristics

- Takes full width by default
- Starts on a new line
- Width and height can be applied
- Margin and padding work on all sides

### Interview Tip

`div` is the most commonly used block element.

---

# 48. Explain `inline` display.

### Answer

An inline element takes only the space required by its content.

It does not start on a new line.

### Examples of Inline Elements

```html
<span>
  <a>
    <strong> <em></em></strong></a
></span>
```

### Example

```css
span {
  display: inline;
}
```

### Behavior

```text
Hello World Welcome
```

Elements appear in the same line.

### Characteristics

- Takes only required width
- Width and height cannot be applied properly
- Vertical margin does not work properly
- Padding works horizontally

### Interview Tip

Inline elements are mainly used for styling parts of text.

---

# 49. Explain `inline-block`.

### Answer

`inline-block` combines features of both inline and block elements.

The element stays inline but allows width and height.

### Example

```css
.box {
  display: inline-block;
  width: 200px;
  height: 100px;
}
```

### Behavior

```text
Box 1   Box 2   Box 3
```

Elements remain on the same line.

### Characteristics

- Appears inline
- Supports width and height
- Supports margin and padding
- Useful for creating horizontal layouts

### Interview Tip

Before Flexbox, inline-block was commonly used for layouts.

---

# 50. Difference between block and inline elements?

### Answer

| Block                     | Inline                              |
| ------------------------- | ----------------------------------- |
| Starts on a new line      | Stays in the same line              |
| Takes full width          | Takes only content width            |
| Width and height work     | Width and height usually don't work |
| Margin works on all sides | Vertical margin has limitations     |

### Example

Block:

```html
<div>Box</div>
```

Inline:

```html
<span> Text </span>
```

### CSS Example

```css
div {
  display: block;
}

span {
  display: inline;
}
```

### Interview Tip

Block elements create structure; inline elements style content.

---

# 51. Difference between inline and inline-block?

### Answer

Both appear in the same line, but they behave differently.

| Inline                               | Inline-block           |
| ------------------------------------ | ---------------------- |
| Cannot set width and height properly | Width and height work  |
| Limited margin support               | Full margin support    |
| Used for text content                | Used for small layouts |

### Example

Inline:

```css
span {
  display: inline;
  width: 200px;
}
```

Width will not apply correctly.

---

Inline-block:

```css
span {
  display: inline-block;
  width: 200px;
}
```

Width applies.

### Interview Tip

Use `inline-block` when you need inline positioning with block-like sizing.

---

# 52. What is `display:none`?

### Answer

`display:none` completely removes an element from the document layout.

The element:

- Is not visible
- Does not take space
- Cannot be interacted with

### Example

```css
.menu {
  display: none;
}
```

### Before

```
Header

Menu

Content
```

### After

```
Header

Content
```

### Common Uses

- Hide menus
- Show/hide modals
- Responsive designs

### Interview Tip

`display:none` removes the element from layout flow.

---

# 53. Difference between `display:none` and `visibility:hidden`?

### Answer

Both hide elements, but their behavior is different.

| display:none                | visibility:hidden    |
| --------------------------- | -------------------- |
| Removes element from layout | Keeps element space  |
| Element is not visible      | Element is invisible |
| No space occupied           | Space remains        |
| Cannot interact             | Cannot interact      |

### Example

display:none:

```css
.box {
  display: none;
}
```

Result:

```
Box disappears completely
```

visibility:hidden:

```css
.box {
  visibility: hidden;
}
```

Result:

```
Empty space remains
```

### Interview Tip

Use `display:none` when you want to remove the layout space.

---

# 54. What is `display:flex`?

### Answer

`display:flex` creates a flex container that allows easy alignment and distribution of child elements.

Flexbox is a one-dimensional layout system.

It works with:

- Row
- Column

### Example

```css
.container {
  display: flex;
}
```

HTML:

```html
<div class="container">
  <div>1</div>

  <div>2</div>

  <div>3</div>
</div>
```

### Benefits

- Easy alignment
- Responsive layouts
- Equal spacing
- Centering elements

### Common Properties

Container:

- flex-direction
- justify-content
- align-items
- flex-wrap

Items:

- flex-grow
- flex-shrink
- order

### Interview Tip

Flexbox is best for one-dimensional layouts.

---

# 55. What is `display:grid`?

### Answer

`display:grid` creates a CSS Grid container.

CSS Grid is a two-dimensional layout system.

It works with:

- Rows
- Columns

### Example

```css
.container {
  display: grid;

  grid-template-columns: repeat(3, 1fr);
}
```

HTML:

```html
<div class="container">
  <div>1</div>

  <div>2</div>

  <div>3</div>
</div>
```

### Benefits

- Complex layouts
- Row and column control
- Responsive designs
- Precise positioning

### Common Properties

- grid-template-columns
- grid-template-rows
- gap
- grid-area
- place-items

### Interview Tip

Use:

```
Flexbox → One dimension

Grid → Two dimensions
```

---

---

# 56. What is CSS position property?

### Answer

The CSS `position` property defines how an element is positioned on a webpage.

It controls the placement of elements using properties like:

- `top`
- `right`
- `bottom`
- `left`

### Syntax

```css
.element {
  position: value;
}
```

### Position Values

1. `static`
2. `relative`
3. `absolute`
4. `fixed`
5. `sticky`

### Example

```css
.box {
  position: relative;
  top: 20px;
}
```

### Interview Tip

The `position` property is commonly used for layouts, overlays, and floating elements.

---

# 57. Explain static positioning.

### Answer

`position: static` is the default position value of all HTML elements.

The element follows the normal document flow.

### Example

```css
.box {
  position: static;
}
```

### Characteristics

- Default behavior
- `top`, `right`, `bottom`, `left` do not work
- Element stays in normal flow

Example:

```css
.box {
  position: static;
  top: 50px;
}
```

The `top` property will have no effect.

### Interview Tip

Every element starts with `position: static` by default.

---

# 58. Explain relative positioning.

### Answer

`position: relative` positions an element relative to its original position.

The element remains in the normal document flow.

### Example

```css
.box {
  position: relative;
  top: 20px;
  left: 30px;
}
```

The element moves:

- 20px downward
- 30px right

### Important Point

The original space of the element is still reserved.

### Use Cases

- Creating reference points for absolute elements
- Small position adjustments
- Icons inside buttons

### Interview Tip

A relative parent is commonly used with absolute children.

---

# 59. Explain absolute positioning.

### Answer

`position:absolute` removes an element from the normal document flow and positions it relative to the nearest positioned ancestor.

A positioned ancestor means an element with:

```css
position: relative;
position: absolute;
position: fixed;
position: sticky;
```

### Example

HTML:

```html
<div class="parent">
  <div class="child"></div>
</div>
```

CSS:

```css
.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 0;
  right: 0;
}
```

### Characteristics

- Removed from normal flow
- Positioned using top/right/bottom/left
- Needs a reference parent

### Interview Tip

Most absolute positioning problems happen because the parent does not have `position: relative`.

---

# 60. Explain fixed positioning.

### Answer

`position:fixed` positions an element relative to the browser viewport.

The element stays in the same position even when the page is scrolled.

### Example

```css
.chat-button {
  position: fixed;

  bottom: 20px;

  right: 20px;
}
```

### Common Uses

- Floating buttons
- Chat widgets
- Fixed headers
- Back-to-top buttons

### Characteristics

- Removed from document flow
- Fixed relative to viewport
- Does not move during scrolling

### Interview Tip

Fixed elements are attached to the screen, not the document.

---

# 61. Explain sticky positioning.

### Answer

`position:sticky` is a combination of relative and fixed positioning.

The element behaves like:

- Relative until a scroll point is reached
- Fixed after reaching that point

### Example

```css
.header {
  position: sticky;

  top: 0;
}
```

### Common Uses

- Sticky navigation bars
- Table headers
- Sidebars

### Requirements

A sticky element needs a position value:

```css
top: 0;
```

### Interview Tip

Sticky elements remain inside their parent container unlike fixed elements.

---

# 62. Difference between relative and absolute position?

### Answer

| Relative                      | Absolute                                         |
| ----------------------------- | ------------------------------------------------ |
| Stays in normal flow          | Removed from normal flow                         |
| Positioned relative to itself | Positioned relative to nearest positioned parent |
| Original space remains        | Original space is removed                        |
| Used as a reference container | Used for precise placement                       |

### Example

Relative:

```css
.parent {
  position: relative;
}
```

Absolute:

```css
.child {
  position: absolute;
  top: 0;
}
```

### Interview Tip

A common pattern:

```css
.parent {
  position: relative;
}

.child {
  position: absolute;
}
```

---

# 63. Difference between fixed and sticky position?

### Answer

| Fixed                      | Sticky                          |
| -------------------------- | ------------------------------- |
| Relative to viewport       | Relative to scrolling container |
| Always stays fixed         | Becomes fixed after threshold   |
| Removed from document flow | Acts relative initially         |
| Ignores parent boundaries  | Stays within parent             |

### Fixed Example

```css
button {
  position: fixed;

  bottom: 10px;
}
```

### Sticky Example

```css
nav {
  position: sticky;

  top: 0;
}
```

### Interview Tip

Use fixed for floating UI and sticky for scroll-based layouts.

---

# 64. How does absolute positioning work?

### Answer

Absolute positioning works by removing an element from the normal layout and positioning it using coordinates.

The browser searches for the nearest ancestor with a position value other than `static`.

### Example

```css
.container {
  position: relative;
}

.box {
  position: absolute;

  top: 20px;

  left: 20px;
}
```

The `.box` position is calculated from `.container`.

### If No Positioned Parent Exists

The element is positioned relative to the initial containing block (usually the viewport).

### Interview Tip

Always define a positioned parent when using absolute positioning.

---

# 65. What is containing block in CSS?

### Answer

A containing block is the reference box used to calculate the position and size of an element.

For absolutely positioned elements, the containing block is usually the nearest positioned ancestor.

### Example

```css
.parent {
  position: relative;

  width: 400px;
}

.child {
  position: absolute;

  right: 0;
}
```

The child positions itself relative to `.parent`.

### Common Containing Blocks

- Positioned ancestors
- Flex containers
- Grid containers
- Transformed elements

### Interview Tip

Understanding containing blocks helps debug absolute positioning issues.

---

# 66. What happens when position absolute has no positioned parent?

### Answer

If an absolutely positioned element has no positioned ancestor, it is positioned relative to the initial containing block.

Usually this means the viewport.

### Example

HTML:

```html
<div class="box">Hello</div>
```

CSS:

```css
.box {
  position: absolute;

  top: 0;

  right: 0;
}
```

If no parent has:

```css
position: relative;
```

The element moves relative to the page.

### Solution

Add a positioned parent:

```css
.container {
  position: relative;
}
```

### Interview Tip

Always check the parent element when absolute positioning behaves unexpectedly.

---

---

# 67. What is z-index?

### Answer

`z-index` is a CSS property that controls the stacking order of positioned elements.

It determines which element appears in front of or behind another element when elements overlap.

### Syntax

```css
.element {
  z-index: value;
}
```

### Example

```css
.box1 {
  position: absolute;
  z-index: 1;
}

.box2 {
  position: absolute;
  z-index: 2;
}
```

Output:

```
box2 appears above box1
```

### Interview Tip

A higher `z-index` value appears closer to the user.

---

# 68. How does z-index work?

### Answer

`z-index` works by assigning a stacking level to elements.

An element with a higher z-index appears above an element with a lower z-index.

### Example

```css
.card {
  position: relative;
  z-index: 10;
}

.overlay {
  position: absolute;
  z-index: 5;
}
```

Result:

```
Card
 ↑
Overlay
```

The card appears above the overlay.

### Important Points

- Works on positioned elements
- Default value is `auto`
- Higher value appears on top

### Interview Tip

`z-index` does not work on normal static elements.

---

# 69. Why is z-index not working sometimes?

### Answer

Common reasons why `z-index` does not work:

---

## 1. Element has no position

Wrong:

```css
.box {
  z-index: 10;
}
```

Correct:

```css
.box {
  position: relative;
  z-index: 10;
}
```

---

## 2. Stacking context issue

A parent element may create a separate stacking context.

Example:

```css
.parent {
  transform: translateX(0);
}
```

This creates a new stacking context.

---

## 3. Parent z-index is lower

Example:

```css
.parent1 {
  z-index: 1;
}

.parent2 {
  z-index: 2;
}
```

Children cannot escape their parent's stacking order.

---

## 4. Element is behind another stacking context

The browser compares stacking contexts before individual z-index values.

### Interview Tip

When z-index fails, inspect parent elements first.

---

# 70. What is stacking context?

### Answer

A stacking context is a separate layer where elements are stacked independently.

Elements inside one stacking context cannot overlap elements from another stacking context based only on their child z-index.

### Example

```css
.parent {
  position: relative;
  z-index: 1;
}
```

This creates a stacking context.

### Properties That Create Stacking Context

- Position + z-index
- opacity less than 1
- transform
- filter
- isolation
- fixed positioning

### Example

```css
.box {
  opacity: 0.9;
}
```

Creates a new stacking context.

### Interview Tip

Stacking context is the main reason complex z-index problems happen.

---

# 71. How is stacking order determined?

### Answer

The browser determines stacking order using multiple rules.

General order:

```
1. Background and borders
2. Negative z-index elements
3. Normal document elements
4. Positioned elements
5. Positive z-index elements
```

### Example

```css
.box1 {
  position: absolute;
  z-index: 1;
}

.box2 {
  position: absolute;
  z-index: 2;
}
```

`box2` appears above `box1`.

### Interview Tip

Higher positive z-index values usually appear on top.

---

# 72. Can z-index work without position?

### Answer

Generally, `z-index` does not work on normal positioned static elements.

Example:

```css
.box {
  z-index: 10;
}
```

The element has:

```css
position: static;
```

So z-index has no effect.

### Correct:

```css
.box {
  position: relative;

  z-index: 10;
}
```

### Exception

`z-index` also works with some layout elements like:

- Flex items
- Grid items

Example:

```css
.item {
  z-index: 2;
}
```

inside a flex container.

### Interview Tip

For normal elements, add a position value before using z-index.

---

# 73. Difference between z-index and position?

### Answer

`position` controls where an element is placed.

`z-index` controls the stacking order of overlapping elements.

### Comparison

| Position                                  | z-index                  |
| ----------------------------------------- | ------------------------ |
| Controls element placement                | Controls layer order     |
| Uses top/right/bottom/left                | Uses stacking value      |
| Values: relative, absolute, fixed, sticky | Numeric values           |
| Changes layout behavior                   | Changes visibility order |

### Example

```css
.image {
  position: absolute;

  top: 0;
}

.text {
  position: absolute;

  z-index: 2;
}
```

The text appears above the image.

### Interview Tip

Position decides location; z-index decides depth.

---

# 74. How do you debug z-index issues?

### Answer

Follow these steps:

---

## 1. Check position property

Make sure the element has:

```css
position: relative;
```

or

```css
position: absolute;
```

---

## 2. Inspect stacking contexts

Check parent elements for:

```css
transform
opacity
filter
z-index
```

---

## 3. Compare parent z-index values

Example:

```css
.parent1 {
  z-index: 1;
}

.parent2 {
  z-index: 2;
}
```

A child of `.parent1` cannot appear above `.parent2` even with a large z-index.

---

## 4. Use browser DevTools

Inspect:

- Computed styles
- Position
- Stacking layers

### Example Debug

```css
.modal {
  position: fixed;

  z-index: 9999;
}
```

### Interview Tip

A large z-index number does not always solve the problem. Stacking context matters more.

---

---

# 75. What is Flexbox?

### Answer

Flexbox (Flexible Box Layout) is a CSS layout system used to arrange elements in a single dimension.

It can arrange elements:

- Horizontally (row)
- Vertically (column)

Flexbox makes alignment and spacing easier compared to traditional CSS layouts.

### Example

```css
.container {
  display: flex;
}
```

HTML:

```html
<div class="container">
  <div>Item 1</div>

  <div>Item 2</div>
</div>
```

### Benefits

- Easy alignment
- Responsive layouts
- Equal spacing
- Dynamic sizing

### Interview Tip

Flexbox is a **one-dimensional layout system**.

---

# 76. Why was Flexbox introduced?

### Answer

Flexbox was introduced to solve common layout problems that were difficult with traditional CSS.

Before Flexbox, developers used:

- Floats
- Tables
- Positioning hacks

### Problems Before Flexbox

- Difficult vertical centering
- Complex responsive layouts
- Unequal spacing issues
- Hard alignment

### Example

Centering with Flexbox:

```css
.container {
  display: flex;

  justify-content: center;

  align-items: center;
}
```

### Benefits

- Cleaner code
- Better responsive design
- Easier alignment

### Interview Tip

Flexbox simplified modern UI layout development.

---

# 77. Difference between Flexbox and normal layout?

### Answer

Traditional CSS layout uses normal document flow, while Flexbox provides a flexible alignment system.

### Comparison

| Normal Layout              | Flexbox                   |
| -------------------------- | ------------------------- |
| Uses block and inline flow | Uses flexible containers  |
| Harder alignment           | Easy alignment            |
| Manual spacing             | Built-in spacing controls |
| Less responsive            | Better responsive layouts |

### Example

Normal CSS:

```css
div {
  margin: auto;
}
```

Flexbox:

```css
.container {
  display: flex;

  justify-content: center;
}
```

### Interview Tip

Flexbox is designed specifically for component-based layouts.

---

# 78. How do you create a flex container?

### Answer

A flex container is created by applying:

```css
display: flex;
```

to a parent element.

### Example

```css
.container {
  display: flex;
}
```

HTML:

```html
<div class="container">
  <div>A</div>

  <div>B</div>

  <div>C</div>
</div>
```

The child elements become flex items.

### Flex Container Properties

- flex-direction
- justify-content
- align-items
- flex-wrap
- align-content

### Interview Tip

Only direct children become flex items.

---

# 79. Explain flex-direction.

### Answer

`flex-direction` defines the direction in which flex items are arranged.

### Values

## row (default)

Items are placed horizontally.

```css
.container {
  flex-direction: row;
}
```

Output:

```
A B C
```

---

## column

Items are placed vertically.

```css
.container {
  flex-direction: column;
}
```

Output:

```
A

B

C
```

---

## row-reverse

```css
flex-direction: row-reverse;
```

Output:

```
C B A
```

---

## column-reverse

```css
flex-direction: column-reverse;
```

Output:

```
C

B

A
```

### Interview Tip

Default flex direction is:

```css
row
```

---

# 80. Explain justify-content.

### Answer

`justify-content` controls alignment along the main axis.

The main axis depends on `flex-direction`.

### Example

```css
.container {
  display: flex;

  justify-content: center;
}
```

### Common Values

## flex-start

Items start from beginning.

```
A B C
```

---

## center

Items move to center.

```
  A B C
```

---

## flex-end

Items move to end.

```
      A B C
```

---

## space-between

Equal space between items.

```
A     B     C
```

---

## space-around

Space around each item.

```
 A    B    C
```

---

## space-evenly

Equal space everywhere.

```
  A   B   C
```

### Interview Tip

`justify-content` works on the main axis.

---

# 81. Explain align-items.

### Answer

`align-items` controls alignment along the cross axis.

For default row direction:

- Main axis → horizontal
- Cross axis → vertical

### Example

```css
.container {
  display: flex;

  align-items: center;
}
```

### Values

- flex-start
- center
- flex-end
- stretch
- baseline

### Example

Center vertically:

```css
.container {
  height: 300px;

  display: flex;

  align-items: center;
}
```

### Interview Tip

Remember:

```
justify-content → Main axis

align-items → Cross axis
```

---

# 82. Explain align-content.

### Answer

`align-content` controls spacing between multiple flex rows.

It works only when:

```css
flex-wrap: wrap;
```

is enabled.

### Example

```css
.container {
  display: flex;

  flex-wrap: wrap;

  align-content: center;
}
```

### Values

- flex-start
- center
- flex-end
- space-between
- space-around
- stretch

### Difference

`align-items`

→ Aligns items inside a single row.

`align-content`

→ Aligns multiple rows.

### Interview Tip

`align-content` has no effect on a single-line flex container.

---

# 83. Explain flex-wrap.

### Answer

`flex-wrap` controls whether flex items should move to the next line when there is not enough space.

### Default

```css
flex-wrap: nowrap;
```

Items stay in one line.

---

## wrap

```css
flex-wrap: wrap;
```

Items move to the next line.

Example:

```
A B C

D E F
```

---

## wrap-reverse

```css
flex-wrap: wrap-reverse;
```

Rows wrap in reverse direction.

### Interview Tip

Use `flex-wrap:wrap` for responsive layouts.

---

# 84. Difference between justify-content and align-items?

### Answer

| justify-content             | align-items               |
| --------------------------- | ------------------------- |
| Controls main axis          | Controls cross axis       |
| Horizontal in row direction | Vertical in row direction |
| Controls spacing            | Controls alignment        |

### Example

```css
.container {
  display: flex;

  justify-content: center;

  align-items: center;
}
```

This centers items both horizontally and vertically.

### Interview Tip

For perfect centering:

```css
display: flex;

justify-content: center;

align-items: center;
```

---

# 85. Explain flex-grow.

### Answer

`flex-grow` defines how much a flex item can grow compared to other items.

### Example

```css
.item1 {
  flex-grow: 1;
}

.item2 {
  flex-grow: 2;
}
```

The second item receives twice the available space compared to the first.

### Default

```css
flex-grow: 0;
```

Items do not grow.

### Interview Tip

`flex-grow` distributes extra available space.

---

# 86. Explain flex-shrink.

### Answer

`flex-shrink` defines how much a flex item can shrink when there is not enough space.

### Example

```css
.item {
  flex-shrink: 1;
}
```

Default:

```css
flex-shrink: 1;
```

### Prevent shrinking:

```css
.item {
  flex-shrink: 0;
}
```

### Use Case

Prevent important elements from becoming smaller.

### Interview Tip

Grow handles extra space; shrink handles insufficient space.

---

# 87. Explain flex-basis.

### Answer

`flex-basis` defines the initial size of a flex item before remaining space is distributed.

### Example

```css
.item {
  flex-basis: 200px;
}
```

The item starts with a width of 200px.

### Difference

```css
width: 200px;
```

sets width.

```css
flex-basis: 200px;
```

sets the starting size in a flex layout.

### Interview Tip

Flexbox uses `flex-basis` before applying grow or shrink.

---

# 88. What is the flex shorthand property?

### Answer

The `flex` property is a shorthand for:

- flex-grow
- flex-shrink
- flex-basis

### Syntax

```css
flex: grow shrink basis;
```

### Example

```css
.item {
  flex: 1 1 200px;
}
```

Means:

```
grow = 1

shrink = 1

basis = 200px
```

### Common Example

```css
.item {
  flex: 1;
}
```

Equivalent to:

```css
flex: 1 1 0;
```

### Interview Tip

`flex:1` is commonly used to create equal-width items.

---

# 89. How do you center an element using Flexbox?

### Answer

Use both:

```css
justify-content: center;

align-items: center;
```

### Example

```css
.container {
  display: flex;

  justify-content: center;

  align-items: center;

  height: 100vh;
}
```

### Result

The child element is centered:

- Horizontally
- Vertically

### Interview Tip

This is one of the most common Flexbox interview questions.

---

# 90. Difference between row and column direction?

### Answer

`flex-direction` controls the direction of flex items.

### Row

Default direction.

```css
flex-direction: row;
```

Items appear horizontally.

```
A B C
```

---

### Column

```css
flex-direction: column;
```

Items appear vertically.

```
A

B

C
```

### Comparison

| Row                       | Column                     |
| ------------------------- | -------------------------- |
| Main axis is horizontal   | Main axis is vertical      |
| Default value             | Common for mobile layouts  |
| Items appear side-by-side | Items appear top-to-bottom |

### Interview Tip

Changing flex-direction also changes the meaning of justify-content and align-items.

---

---

# 91. What is CSS Grid?

### Answer

CSS Grid is a two-dimensional CSS layout system used to create complex layouts using rows and columns.

It allows developers to control both:

- Rows
- Columns

at the same time.

### Example

```css
.container {
  display: grid;
}
```

### Basic Layout

```
+-------+-------+
| Box 1 | Box 2 |
+-------+-------+
| Box 3 | Box 4 |
+-------+-------+
```

### Common Uses

- Page layouts
- Dashboards
- Card layouts
- Gallery designs

### Interview Tip

Grid is a **two-dimensional layout system**.

---

# 92. Difference between Grid and Flexbox?

### Answer

Both are CSS layout systems, but they solve different problems.

### Comparison

| Flexbox                  | Grid                        |
| ------------------------ | --------------------------- |
| One-dimensional          | Two-dimensional             |
| Works with row OR column | Works with rows AND columns |
| Best for components      | Best for page layouts       |
| Content-based layout     | Structure-based layout      |

### Flexbox Example

```css
.container {
  display: flex;
}
```

Useful for:

- Navbar
- Buttons
- Small components

---

### Grid Example

```css
.container {
  display: grid;
}
```

Useful for:

- Dashboard
- Website structure
- Complex layouts

### Interview Tip

Use:

```
Flexbox → Component alignment

Grid → Complete layout structure
```

---

# 93. How do you create a grid container?

### Answer

A grid container is created using:

```css
display: grid;
```

### Example

```css
.container {
  display: grid;
}
```

HTML:

```html
<div class="container">
  <div>1</div>

  <div>2</div>

  <div>3</div>
</div>
```

The child elements become grid items.

### Interview Tip

Only direct children become grid items.

---

# 94. Explain `grid-template-columns`.

### Answer

`grid-template-columns` defines the number and size of columns in a grid.

### Example

```css
.container {
  display: grid;

  grid-template-columns: 200px 200px;
}
```

Creates:

```
+---------+---------+
| Column1 | Column2 |
+---------+---------+
```

---

### Using fr unit

```css
.container {
  grid-template-columns: 1fr 1fr;
}
```

Creates two equal columns.

### Multiple Columns

```css
grid-template-columns: 100px 200px 300px;
```

Creates three columns.

### Interview Tip

`fr` represents a fraction of available space.

---

# 95. Explain `grid-template-rows`.

### Answer

`grid-template-rows` defines the height of grid rows.

### Example

```css
.container {
  display: grid;

  grid-template-rows: 100px 200px;
}
```

Creates:

```
Row 1 → 100px

Row 2 → 200px
```

### Using fr

```css
grid-template-rows: 1fr 1fr;
```

Creates equal-height rows.

### Interview Tip

Columns control width; rows control height.

---

# 96. What is grid-gap?

### Answer

`grid-gap` creates spacing between grid items.

It controls the distance between:

- Rows
- Columns

### Example

```css
.container {
  display: grid;

  gap: 20px;
}
```

Output:

```
Box  Box  Box

Box  Box  Box
```

with 20px spacing.

### Modern Syntax

Instead of:

```css
grid-gap
```

use:

```css
gap
```

### Interview Tip

`gap` works in both Grid and Flexbox.

---

# 97. Difference between gap, row-gap, and column-gap?

### Answer

These properties control spacing in different directions.

---

## gap

Controls both row and column spacing.

```css
.container {
  gap: 20px;
}
```

---

## row-gap

Controls vertical spacing.

```css
.container {
  row-gap: 20px;
}
```

---

## column-gap

Controls horizontal spacing.

```css
.container {
  column-gap: 20px;
}
```

### Example

```css
.container {
  row-gap: 10px;

  column-gap: 30px;
}
```

### Interview Tip

Use `gap` for equal spacing and separate properties for custom spacing.

---

# 98. What are grid lines?

### Answer

Grid lines are the dividing lines created by rows and columns in a grid container.

They are used to position grid items.

### Example

```css
.container {
  display: grid;

  grid-template-columns: 100px 100px;
}
```

Grid lines:

```
| 1 | 2 | 3 |
```

Columns exist between these lines.

### Example

```css
.item {
  grid-column-start: 1;

  grid-column-end: 3;
}
```

The item spans across columns.

### Interview Tip

Grid lines are numbered automatically.

---

# 99. What are grid areas?

### Answer

Grid areas allow you to name sections of a grid layout.

They make layouts easier to understand.

### Example

```css
.container {
  display: grid;

  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
}
```

Layout:

```
+-------------+
|   Header    |
+------+------+
|Side  |Content|
+------+------+
| Footer      |
+-------------+
```

### Assign Areas

```css
.header {
  grid-area: header;
}
```

### Interview Tip

Grid areas improve readability in complex layouts.

---

# 100. Explain `grid-template-areas`.

### Answer

`grid-template-areas` defines the layout structure using named areas.

### Example

```css
.container {
  display: grid;

  grid-template-areas:
    "nav nav"
    "main aside"
    "footer footer";
}
```

Assign elements:

```css
.nav {
  grid-area: nav;
}

.main {
  grid-area: main;
}
```

### Benefits

- Easy to visualize layout
- Cleaner code
- Better maintainability

### Interview Tip

Grid areas are useful for website layouts.

---

# 101. What is repeat() function in Grid?

### Answer

The `repeat()` function avoids writing the same grid values multiple times.

### Without repeat()

```css
grid-template-columns: 1fr 1fr 1fr 1fr;
```

### With repeat()

```css
grid-template-columns: repeat(4, 1fr);
```

Both create four equal columns.

### Example

```css
.container {
  display: grid;

  grid-template-columns: repeat(3, 200px);
}
```

Creates:

```
200px 200px 200px
```

### Interview Tip

`repeat()` makes grid code shorter and cleaner.

---

# 102. What is minmax() function?

### Answer

`minmax()` defines a minimum and maximum size for a grid track.

### Syntax

```css
minmax(minimum, maximum)
```

### Example

```css
.container {
  grid-template-columns: minmax(200px, 1fr);
}
```

Meaning:

- Minimum width = 200px
- Maximum width = available space

### Responsive Example

```css
.container {
  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
}
```

Creates responsive cards.

### Interview Tip

`minmax()` is commonly used for responsive Grid layouts.

---

# 103. How do you create responsive grids?

### Answer

Responsive grids automatically adjust columns based on available space.

Common approach:

```css
.container {
  display: grid;

  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));

  gap: 20px;
}
```

### Explanation

`auto-fit`

- Creates as many columns as possible

`minmax()`

- Prevents columns from becoming too small

`1fr`

- Shares available space equally

### Example Result

Desktop:

```
Card Card Card Card
```

Tablet:

```
Card Card
Card Card
```

Mobile:

```
Card
Card
Card
```

### Interview Tip

This pattern is widely used for responsive card layouts.

---

---

# 104. What is overflow in CSS?

### Answer

The CSS `overflow` property controls what happens when content is larger than its container.

It manages content that exceeds the width or height of an element.

### Syntax

```css
.element {
  overflow: value;
}
```

### Values

- `visible`
- `hidden`
- `scroll`
- `auto`

### Example

```css
.box {
  width: 200px;

  height: 100px;

  overflow: hidden;
}
```

### Interview Tip

Overflow is mainly used when content does not fit inside a fixed-size container.

---

# 105. Explain `overflow:hidden`.

### Answer

`overflow:hidden` hides any content that goes outside the boundaries of the element.

Extra content is clipped and not visible.

### Example

```css
.box {
  width: 200px;

  height: 100px;

  overflow: hidden;
}
```

### Before

```
+-------------+
| Text Text   |
| Text Text   |
| Text Text   |
+-------------+

Extra content
```

### After

```
+-------------+
| Text Text   |
| Text Text   |
+-------------+
```

### Common Uses

- Hiding overflowing images
- Creating clean card layouts
- Clearing floats (older technique)

### Interview Tip

`overflow:hidden` removes visibility of extra content but does not delete it.

---

# 106. Explain `overflow:scroll`.

### Answer

`overflow:scroll` always adds scrollbars, even if the content fits.

### Example

```css
.box {
  width: 200px;

  height: 100px;

  overflow: scroll;
}
```

Output:

```
+-------------+
| Content     |
|             |
|        ↕    |
+-------------+
```

### Characteristics

- Always shows scrollbar
- User can scroll through hidden content
- Takes extra space

### Interview Tip

Use `scroll` when scrolling should always be available.

---

# 107. Explain `overflow:auto`.

### Answer

`overflow:auto` adds scrollbars only when the content exceeds the container size.

### Example

```css
.box {
  width: 200px;

  height: 100px;

  overflow: auto;
}
```

### Behavior

Small content:

```
No scrollbar
```

Large content:

```
Scrollbar appears
```

### Common Uses

- Text containers
- Tables
- Modal content
- Chat windows

### Interview Tip

`overflow:auto` is usually preferred over `scroll`.

---

# 108. Difference between overflow-x and overflow-y?

### Answer

`overflow-x` controls horizontal overflow.

`overflow-y` controls vertical overflow.

---

## overflow-x

Controls left-right scrolling.

Example:

```css
.box {
  overflow-x: auto;
}
```

Used for:

- Wide tables
- Horizontal lists

---

## overflow-y

Controls top-bottom scrolling.

Example:

```css
.box {
  overflow-y: auto;
}
```

Used for:

- Long text
- Chat messages

### Comparison

| overflow-x               | overflow-y            |
| ------------------------ | --------------------- |
| Horizontal direction     | Vertical direction    |
| Left and right scrolling | Up and down scrolling |

### Interview Tip

Use separate overflow properties when controlling one direction.

---

# 109. What happens when content exceeds container size?

### Answer

When content becomes larger than its container, the browser handles it based on the overflow property.

### Default Behavior

```css
overflow: visible;
```

Content extends outside the container.

Example:

```css
.box {
  width: 100px;

  height: 50px;
}
```

Large text may overflow outside.

---

### Other Behaviors

Hidden:

```css
overflow: hidden;
```

Content is clipped.

Scroll:

```css
overflow: scroll;
```

Scrollbar always appears.

Auto:

```css
overflow: auto;
```

Scrollbar appears when needed.

### Interview Tip

Always define overflow behavior for fixed-size containers.

---

# 110. What is text-overflow?

### Answer

`text-overflow` controls how overflowing text is displayed when it does not fit inside its container.

The most common value is:

```css
text-overflow: ellipsis;
```

which shows:

```
...
```

### Example

```css
.text {
  width: 200px;

  white-space: nowrap;

  overflow: hidden;

  text-overflow: ellipsis;
}
```

### Output

Before:

```
This is a very long text message
```

After:

```
This is a very long...
```

### Interview Tip

`text-overflow:ellipsis` requires:

```css
overflow: hidden;

white-space: nowrap;
```

---

# 111. How does ellipsis work?

### Answer

Ellipsis (`...`) truncates overflowing text and displays three dots instead of the hidden part.

### Required CSS

```css
.title {
  width: 200px;

  white-space: nowrap;

  overflow: hidden;

  text-overflow: ellipsis;
}
```

### Explanation

## width

Defines available space.

## white-space

Prevents text wrapping.

## overflow

Hides extra text.

## text-overflow

Shows ellipsis.

### Example

HTML:

```html
<p class="title">Frontend Developer Interview Preparation</p>
```

CSS:

```css
.title {
  width: 150px;

  white-space: nowrap;

  overflow: hidden;

  text-overflow: ellipsis;
}
```

Output:

```
Frontend Devel...
```

### Interview Tip

Ellipsis works only when the browser knows where the text should stop.

---

---

# 112. What is responsive web design?

### Answer

Responsive web design is an approach where websites automatically adjust their layout and content based on different screen sizes.

A responsive website works properly on:

- Mobile phones
- Tablets
- Laptops
- Desktop screens

### Example

A desktop layout:

```
Card  Card  Card  Card
```

Mobile layout:

```
Card

Card

Card
```

### Techniques Used

- Flexible layouts
- CSS Grid
- Flexbox
- Media queries
- Responsive units

### Interview Tip

Responsive design ensures a good user experience across all devices.

---

# 113. Why is responsive design important?

### Answer

Responsive design is important because users access websites from different devices and screen sizes.

### Benefits

## 1. Better User Experience

Users can easily navigate websites on mobile devices.

---

## 2. Mobile-Friendly

Most internet users browse using smartphones.

---

## 3. Better SEO

Search engines prefer mobile-friendly websites.

---

## 4. Less Development Work

One responsive website works across multiple devices.

---

## 5. Improved Performance

Optimized layouts improve loading and usability.

### Interview Tip

Modern frontend applications are expected to be responsive by default.

---

# 114. What are different approaches for responsive design?

### Answer

There are several approaches used to create responsive websites.

---

## 1. Fluid Layout

Uses flexible units like:

- %
- rem
- vw
- vh

Example:

```css
.container {
  width: 80%;
}
```

---

## 2. Media Queries

Apply different styles for different screen sizes.

Example:

```css
@media (max-width: 600px) {
  .container {
    width: 100%;
  }
}
```

---

## 3. Flexible Images

Images adjust according to container size.

Example:

```css
img {
  max-width: 100%;

  height: auto;
}
```

---

## 4. Mobile-First Design

Design starts from small screens and expands.

---

## 5. Desktop-First Design

Design starts from large screens and adapts downward.

### Interview Tip

Modern development commonly follows the mobile-first approach.

---

# 115. What is mobile-first design?

### Answer

Mobile-first design means creating the website layout for mobile devices first, then adding styles for larger screens.

The base CSS targets small screens.

### Example

Default mobile style:

```css
.container {
  width: 100%;
}
```

Desktop enhancement:

```css
@media (min-width: 768px) {
  .container {
    width: 80%;
  }
}
```

### Advantages

- Better mobile experience
- Faster loading
- Cleaner CSS
- Focuses on essential content

### Interview Tip

Mobile-first uses `min-width` media queries.

---

# 116. What is desktop-first design?

### Answer

Desktop-first design means creating the website for large screens first and then adjusting it for smaller devices.

### Example

Desktop CSS:

```css
.container {
  width: 1200px;
}
```

Mobile adjustment:

```css
@media (max-width: 600px) {
  .container {
    width: 100%;
  }
}
```

### Advantages

- Useful for desktop-heavy applications
- Easier when desktop layout is primary

### Disadvantages

- May require many overrides
- Mobile performance may suffer

### Interview Tip

Desktop-first usually uses `max-width` media queries.

---

# 117. Difference between mobile-first and desktop-first?

### Answer

| Mobile-first                             | Desktop-first                              |
| ---------------------------------------- | ------------------------------------------ |
| Starts with small screens                | Starts with large screens                  |
| Uses min-width queries                   | Uses max-width queries                     |
| Adds styles for larger screens           | Removes/reduces styles for smaller screens |
| Better for modern responsive development | Useful for desktop-focused apps            |

### Example

Mobile-first:

```css
@media (min-width: 768px) {
}
```

Desktop-first:

```css
@media (max-width: 768px) {
}
```

### Interview Tip

Mobile-first is recommended for most modern frontend projects.

---

# 118. What are responsive units?

### Answer

Responsive units are CSS units that adjust based on screen size or parent size.

Common responsive units:

- %
- em
- rem
- vw
- vh
- vmin
- vmax

### Examples

Percentage:

```css
width: 50%;
```

Viewport width:

```css
width: 50vw;
```

Viewport height:

```css
height: 50vh;
```

### Interview Tip

Responsive units help create flexible layouts instead of fixed layouts.

---

# 119. Difference between px, %, em, rem, vh, and vw?

### Answer

## px (Pixels)

Fixed size unit.

Example:

```css
font-size: 16px;
```

---

## %

Relative to parent element.

Example:

```css
width: 50%;
```

---

## em

Relative to the parent element's font size.

Example:

```css
font-size: 2em;
```

If parent font size is 16px:

```
2em = 32px
```

---

## rem

Relative to root (`html`) font size.

Example:

```css
font-size: 2rem;
```

If root size is 16px:

```
2rem = 32px
```

---

## vw

Viewport width.

```
1vw = 1% of viewport width
```

Example:

```css
width: 50vw;
```

---

## vh

Viewport height.

```
1vh = 1% of viewport height
```

Example:

```css
height: 100vh;
```

### Comparison

| Unit | Relative To      |
| ---- | ---------------- |
| px   | Fixed pixels     |
| %    | Parent element   |
| em   | Parent font size |
| rem  | Root font size   |
| vw   | Viewport width   |
| vh   | Viewport height  |

### Interview Tip

Use `rem` for scalable typography and `vw/vh` for viewport-based layouts.

---

# 120. How do you make images responsive?

### Answer

Images can be made responsive by allowing them to scale within their container.

### Common CSS

```css
img {
  max-width: 100%;

  height: auto;
}
```

### Explanation

`max-width:100%`

- Prevents image overflow
- Allows image to shrink

`height:auto`

- Maintains aspect ratio

### Example

```html
<img src="photo.jpg" />
```

```css
img {
  width: 100%;

  max-width: 600px;

  height: auto;
}
```

### Other Techniques

## Object-fit

```css
img {
  width: 300px;

  height: 200px;

  object-fit: cover;
}
```

## Responsive Containers

Using:

- Flexbox
- Grid
- Aspect-ratio

### Interview Tip

Never use fixed image widths without considering smaller screens.

---

---

# 121. What are media queries?

### Answer

Media queries are CSS features used to apply different styles based on device characteristics like:

- Screen width
- Screen height
- Device orientation
- Resolution

They are mainly used for creating responsive websites.

### Syntax

```css
@media (condition) {
  /* CSS styles */
}
```

### Example

```css
@media (max-width: 600px) {
  .container {
    width: 100%;
  }
}
```

When screen width is 600px or less, the styles are applied.

### Interview Tip

Media queries allow websites to adapt to different screen sizes.

---

# 122. Why are media queries used?

### Answer

Media queries are used to create responsive layouts for different devices.

### Uses

## 1. Mobile Responsive Design

Example:

```css
@media (max-width: 768px) {
  .navbar {
    display: none;
  }
}
```

---

## 2. Changing Layouts

Desktop:

```
Card Card Card
```

Mobile:

```
Card

Card

Card
```

---

## 3. Adjusting Typography

Example:

```css
@media (max-width: 600px) {
  h1 {
    font-size: 24px;
  }
}
```

---

## 4. Changing Navigation

Example:

Desktop:

```
Home About Contact
```

Mobile:

```
Menu Button
```

### Interview Tip

Media queries are the foundation of responsive CSS.

---

# 123. What is the syntax of media queries?

### Answer

The basic syntax is:

```css
@media media-type and (condition) {
  selector {
    property: value;
  }
}
```

### Example

```css
@media screen and (max-width: 768px) {
  body {
    background: white;
  }
}
```

### Parts

## @media

Defines a media query.

## screen

Specifies the device type.

## condition

Defines when styles should apply.

## CSS block

Contains responsive styles.

### Interview Tip

Media queries are written after normal CSS styles.

---

# 124. Difference between min-width and max-width?

### Answer

Both are used to define responsive breakpoints.

---

## max-width

Applies styles when screen width is less than or equal to the given value.

Example:

```css
@media (max-width: 600px) {
  .container {
    width: 100%;
  }
}
```

Used for:

- Desktop-first approach
- Reducing styles for smaller screens

---

## min-width

Applies styles when screen width is greater than or equal to the given value.

Example:

```css
@media (min-width: 768px) {
  .container {
    width: 80%;
  }
}
```

Used for:

- Mobile-first approach
- Adding styles for larger screens

### Comparison

| max-width                      | min-width                     |
| ------------------------------ | ----------------------------- |
| Targets smaller screens        | Targets larger screens        |
| Uses downward changes          | Uses upward enhancements      |
| Desktop-first commonly uses it | Mobile-first commonly uses it |

### Interview Tip

Mobile-first design usually uses `min-width`.

---

# 125. How do you create breakpoints?

### Answer

Breakpoints are screen sizes where the website layout changes.

They are created using media queries.

### Example

```css
/* Mobile */

.container {
  width: 100%;
}

/* Tablet */

@media (min-width: 768px) {
  .container {
    width: 750px;
  }
}

/* Desktop */

@media (min-width: 1200px) {
  .container {
    width: 1100px;
  }
}
```

### Common Breakpoints

```text
Mobile:
320px - 480px

Tablet:
481px - 768px

Laptop:
769px - 1024px

Desktop:
1025px+
```

### Best Practice

Do not choose breakpoints based only on devices.

Choose them based on when your layout breaks.

### Interview Tip

A breakpoint is a design decision, not a device rule.

---

# 126. Common responsive breakpoints?

### Answer

There are no fixed official breakpoints, but commonly used values are:

| Device        | Breakpoint |
| ------------- | ---------- |
| Small mobile  | 320px      |
| Mobile        | 480px      |
| Tablet        | 768px      |
| Laptop        | 1024px     |
| Desktop       | 1200px     |
| Large desktop | 1440px     |

### Example

```css
@media (min-width: 768px) {
  .card {
    width: 50%;
  }
}
```

### Framework Examples

Bootstrap commonly uses:

```text
sm   → 576px

md   → 768px

lg   → 992px

xl   → 1200px

xxl  → 1400px
```

### Interview Tip

Good developers choose breakpoints based on content, not only device names.

---

# 127. What is orientation media query?

### Answer

Orientation media queries apply styles based on device orientation.

There are two values:

- portrait
- landscape

---

## Portrait

Height is greater than width.

Example:

```css
@media (orientation: portrait) {
  .container {
    width: 100%;
  }
}
```

---

## Landscape

Width is greater than height.

Example:

```css
@media (orientation: landscape) {
  .container {
    width: 80%;
  }
}
```

### Common Uses

- Mobile layouts
- Tablets
- Games
- Video interfaces

### Interview Tip

Orientation queries help optimize layouts when users rotate devices.

---

# 128. How do you test responsive designs?

### Answer

Responsive designs can be tested using different methods.

---

## 1. Browser Developer Tools

Chrome DevTools:

```
Right Click
→ Inspect
→ Toggle Device Toolbar
```

Test:

- Mobile
- Tablet
- Desktop

---

## 2. Resize Browser Window

Manually change the browser width.

---

## 3. Test Real Devices

Check:

- Touch behavior
- Performance
- Layout issues

---

## 4. Use Online Tools

Examples:

- BrowserStack
- Responsive Design Mode

---

## 5. Check Different Features

Test:

- Navigation
- Images
- Forms
- Buttons
- Text size
- Overflow

### Interview Tip

Always test responsive layouts before deployment.

---

---

# 129. What are CSS variables?

### Answer

CSS variables (also called custom properties) are reusable values stored in CSS.

They help avoid repeating the same values multiple times.

### Syntax

```css
:root {
  --primary-color: blue;
}
```

Using the variable:

```css
button {
  color: var(--primary-color);
}
```

### Example

```css
:root {
  --main-color: #3498db;
}

.card {
  background: var(--main-color);
}
```

### Benefits

- Reusable values
- Easier maintenance
- Supports dynamic changes
- Reduces duplicate code

### Interview Tip

CSS variables are commonly used in design systems and themes.

---

# 130. How do you create CSS variables?

### Answer

CSS variables are created using two hyphens (`--`) before the variable name.

### Example

```css
:root {
  --primary-color: green;

  --spacing: 20px;
}
```

Using variables:

```css
.container {
  color: var(--primary-color);

  padding: var(--spacing);
}
```

### Where to Define Variables?

Usually inside:

```css
:root {
}
```

because it makes them globally available.

### Interview Tip

`var()` function is used to access CSS variables.

---

# 131. What is inheritance in CSS?

### Answer

CSS inheritance is the process where child elements automatically receive some styles from their parent elements.

### Example

HTML:

```html
<div>
  <p>Hello</p>
</div>
```

CSS:

```css
div {
  color: blue;
}
```

The paragraph inherits:

```css
color: blue;
```

### Common Inherited Properties

- color
- font-family
- font-size
- line-height
- text-align

### Interview Tip

Not all CSS properties are inherited.

---

# 132. Which properties are inherited?

### Answer

Some CSS properties naturally pass from parent elements to child elements.

### Common Inherited Properties

## Text Properties

```css
color

font-family

font-size

font-weight

line-height

text-align
```

---

## List Properties

```css
list-style
```

---

## Visibility

```css
visibility
```

### Example

```css
body {
  font-family: Arial;

  color: black;
}
```

All child elements inherit these styles.

### Interview Tip

Typography-related properties are usually inherited.

---

# 133. Which properties are not inherited?

### Answer

Most layout-related properties are not inherited.

### Non-Inherited Properties

## Box Model

```css
width

height

margin

padding

border
```

---

## Layout

```css
display

position

top

left
```

---

## Background

```css
background

background-color
```

### Example

```css
.parent {
  width: 500px;
}
```

The child does not automatically become 500px wide.

### Interview Tip

Layout properties usually need to be explicitly applied.

---

# 134. What is CSS cascade?

### Answer

The CSS cascade is the process browsers use to decide which styles should be applied when multiple rules target the same element.

The cascade considers:

1. Importance
2. Specificity
3. Source order

### Example

```css
p {
  color: blue;
}

p {
  color: red;
}
```

Output:

```text
red
```

Because the second rule comes later.

### Cascade Order

```
!important
↓
Specificity
↓
Source order
```

### Interview Tip

"Cascade" means CSS rules compete and the browser chooses the winning rule.

---

# 135. What is CSS reset?

### Answer

CSS reset is a technique used to remove default browser styles and create a consistent starting point.

Different browsers apply different default styles.

### Example

```css
* {
  margin: 0;

  padding: 0;

  box-sizing: border-box;
}
```

### Removes

- Default margins
- Default padding
- Browser inconsistencies

### Benefits

- Consistent styling
- Easier layout control
- Predictable design

### Interview Tip

Many projects start with a CSS reset.

---

# 136. What is normalize.css?

### Answer

Normalize.css is a CSS file that makes browser styles consistent while preserving useful default behaviors.

Unlike CSS reset, it does not remove everything.

### CSS Reset

Removes browser styles:

```css
h1 {
  margin: 0;
}
```

### Normalize.css

Keeps useful defaults but fixes inconsistencies.

### Benefits

- Better cross-browser consistency
- Preserves accessibility-friendly styles
- Reduces browser differences

### Interview Tip

Normalize.css is a more gentle alternative to CSS reset.

---

# 137. Difference between reset and normalize CSS?

### Answer

| CSS Reset                    | Normalize CSS                     |
| ---------------------------- | --------------------------------- |
| Removes default styles       | Keeps useful defaults             |
| More aggressive              | More controlled                   |
| Requires more custom styling | Requires fewer overrides          |
| Creates blank starting point | Creates consistent starting point |

### Example

Reset:

```css
* {
  margin: 0;

  padding: 0;
}
```

Normalize:

- Fixes browser differences
- Keeps semantic defaults

### Interview Tip

Both solve browser inconsistency problems but use different approaches.

---

# 138. What are transitions?

### Answer

CSS transitions create smooth changes between two states of an element.

They define how long a property change should take.

### Syntax

```css
.element {
  transition: property duration;
}
```

### Example

```css
button {
  background: red;

  transition: 0.3s;
}

button:hover {
  background: blue;
}
```

The color changes smoothly.

### Common Transition Properties

- transition-property
- transition-duration
- transition-delay
- transition-timing-function

### Interview Tip

Transitions are usually used for hover effects.

---

# 139. What are transforms?

### Answer

CSS transforms allow you to visually modify an element without affecting the document layout.

### Common Transform Functions

- translate()
- rotate()
- scale()
- skew()

### Example

```css
.box {
  transform: translateX(50px);
}
```

Moves the element 50px horizontally.

### Scale Example

```css
.card:hover {
  transform: scale(1.1);
}
```

### Interview Tip

Transforms change appearance but do not affect surrounding elements.

---

# 140. What are animations in CSS?

### Answer

CSS animations allow elements to change styles automatically over time.

They use:

- `@keyframes`
- animation properties

### Example

```css
.box {
  animation: move 2s;
}

@keyframes move {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(100px);
  }
}
```

### Uses

- Loading animations
- Effects
- Interactive UI

### Interview Tip

Animations can run without user interaction.

---

---

# 141. Difference between transition and animation?

### Answer

Both transitions and animations create visual changes in CSS, but they work differently.

### Comparison

| Transition                           | Animation                |
| ------------------------------------ | ------------------------ |
| Needs a trigger (hover, focus, etc.) | Can run automatically    |
| Changes between two states           | Can have multiple states |
| Uses `transition` property           | Uses `@keyframes`        |
| Simple effects                       | Complex effects          |

### Transition Example

```css
button {
  background: red;

  transition: 0.3s;
}

button:hover {
  background: blue;
}
```

Works when user hovers.

---

### Animation Example

```css
.box {
  animation: move 2s;
}

@keyframes move {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(100px);
  }
}
```

Runs automatically.

### Interview Tip

Remember:

```
Transition → Change between states

Animation → Complete movement sequence
```

---

# 142. Explain @keyframes.

### Answer

`@keyframes` defines the steps of a CSS animation.

It specifies how an element should change during animation.

### Syntax

```css
@keyframes animationName {
  from {
    property: value;
  }

  to {
    property: value;
  }
}
```

### Example

```css
@keyframes slide {
  from {
    transform: translateX(0);
  }

  to {
    transform: translateX(200px);
  }
}
```

Apply animation:

```css
.box {
  animation: slide 2s;
}
```

### Multiple Steps

```css
@keyframes colorChange {
  0% {
    background: red;
  }

  50% {
    background: yellow;
  }

  100% {
    background: green;
  }
}
```

### Interview Tip

`@keyframes` controls animation stages.

---

# 143. What are CSS functions?

### Answer

CSS functions are built-in functions that perform calculations or provide dynamic values.

They are written using parentheses.

### Common CSS Functions

- `calc()`
- `min()`
- `max()`
- `clamp()`
- `var()`
- `url()`
- `rgb()`

### Example

```css
.box {
  width: calc(100% - 50px);
}
```

### Benefits

- Dynamic values
- Responsive layouts
- Reusable styles

### Interview Tip

CSS functions make layouts more flexible.

---

# 144. Explain calc().

### Answer

`calc()` allows mathematical calculations inside CSS values.

It supports:

- Addition (+)
- Subtraction (-)
- Multiplication (\*)
- Division (/)

### Syntax

```css
property: calc(expression);
```

### Example

```css
.container {
  width: calc(100% - 100px);
}
```

Meaning:

```
Container width = screen width - 100px
```

### Another Example

```css
.box {
  height: calc(100vh - 80px);
}
```

Useful for layouts with fixed headers.

### Interview Tip

Spaces are required around operators:

Correct:

```css
calc(100% - 20px)
```

Wrong:

```css
calc(100%-20px)
```

---

# 145. Explain clamp().

### Answer

`clamp()` sets a value that stays between a minimum and maximum limit.

### Syntax

```css
clamp(minimum, preferred, maximum)
```

### Example

```css
h1 {
  font-size: clamp(24px, 5vw, 60px);
}
```

Meaning:

- Minimum size: 24px
- Preferred size: 5vw
- Maximum size: 60px

### Benefits

- Responsive typography
- Prevents extremely large or small sizes

### Interview Tip

`clamp()` is commonly used for responsive font sizes.

---

# 146. Explain min() and max().

### Answer

`min()` and `max()` choose values based on multiple options.

---

## min()

Uses the smallest value.

Example:

```css
.box {
  width: min(500px, 80%);
}
```

The browser chooses whichever is smaller.

---

## max()

Uses the largest value.

Example:

```css
.box {
  width: max(300px, 50%);
}
```

The browser chooses whichever is larger.

### Benefits

- Responsive sizing
- Flexible layouts
- Reduces media queries

### Interview Tip

`min()` limits maximum size; `max()` ensures minimum size.

---

# 147. What are gradients?

### Answer

Gradients create smooth transitions between two or more colors.

They are created using CSS functions.

Types:

1. Linear gradient
2. Radial gradient

### Example

```css
.box {
  background: linear-gradient(red, blue);
}
```

Output:

A smooth transition from red to blue.

### Benefits

- No image required
- Lightweight
- Modern UI effects

### Interview Tip

Gradients are background effects created using CSS.

---

# 148. Difference between linear and radial gradients?

### Answer

### Linear Gradient

Colors transition in a straight direction.

Example:

```css
.box {
  background: linear-gradient(to right, red, blue);
}
```

Direction:

```
Red → Blue
```

---

### Radial Gradient

Colors spread from a center point.

Example:

```css
.box {
  background: radial-gradient(red, blue);
}
```

Pattern:

```
Center → Outside
```

### Comparison

| Linear Gradient        | Radial Gradient    |
| ---------------------- | ------------------ |
| Straight direction     | Circular direction |
| Uses angle/direction   | Uses center point  |
| Common for backgrounds | Common for effects |

### Interview Tip

Linear = line, Radial = radius.

---

# 149. What are filters in CSS?

### Answer

CSS filters apply visual effects to elements like images and backgrounds.

### Syntax

```css
.element {
  filter: value;
}
```

### Common Filters

## Blur

```css
filter: blur(5px);
```

## Brightness

```css
filter: brightness(150%);
```

## Grayscale

```css
filter: grayscale(100%);
```

## Contrast

```css
filter: contrast(200%);
```

### Example

```css
img:hover {
  filter: grayscale(100%);
}
```

### Uses

- Image effects
- Hover animations
- Visual adjustments

### Interview Tip

Filters change appearance without modifying the original image.

---

# 150. Difference between opacity and visibility?

### Answer

Both control visibility, but they behave differently.

### Opacity

Controls transparency.

Example:

```css
.box {
  opacity: 0;
}
```

Characteristics:

- Element still occupies space
- Can still receive clicks unless disabled
- Supports animation

---

### Visibility

Controls whether an element is visible.

Example:

```css
.box {
  visibility: hidden;
}
```

Characteristics:

- Element occupies space
- Not visible
- Cannot interact

---

### Comparison

| Opacity                       | Visibility                   |
| ----------------------------- | ---------------------------- |
| Controls transparency         | Controls visibility          |
| Value from 0 to 1             | Values: visible/hidden       |
| Can show partial transparency | Completely hidden            |
| Can still receive events      | Does not receive interaction |

### Interview Tip

For completely removing layout space use:

```css
display: none;
```

For transparent effects use:

```css
opacity
```

---

````md id="c8v4lm"
---
# 151. How do you center a div horizontally?

### Answer

There are multiple ways to center a div horizontally.
---

## Method 1: Using margin auto

```css
.box {
  width: 300px;

  margin: auto;
}
```

The browser automatically calculates equal left and right margins.

---

## Method 2: Using Flexbox

```css
.container {
  display: flex;

  justify-content: center;
}
```

---

## Method 3: Using Grid

```css
.container {
  display: grid;

  justify-content: center;
}
```

### Interview Tip

For modern applications, Flexbox is commonly used.

---

# 152. How do you center a div vertically?

### Answer

The modern approach is using Flexbox.

### Example

```css
.container {
  height: 100vh;

  display: flex;

  align-items: center;
}
```

This centers the child vertically.

### Center Both Horizontally and Vertically

```css
.container {
  height: 100vh;

  display: flex;

  justify-content: center;

  align-items: center;
}
```

### Using Grid

```css
.container {
  display: grid;

  place-items: center;
}
```

### Interview Tip

`place-items:center` is the shortest Grid solution.

---

# 153. How do you create equal height cards?

### Answer

Equal height cards can be created using Flexbox or Grid.

---

## Using Flexbox

```css
.container {
  display: flex;
}

.card {
  flex: 1;
}
```

All cards receive equal available space.

---

## Using Grid

```css
.container {
  display: grid;

  grid-template-columns: repeat(3, 1fr);
}
```

Grid automatically creates equal rows.

---

## Using Stretch

```css
.container {
  align-items: stretch;
}
```

### Interview Tip

Flexbox and Grid are preferred over fixed heights.

---

# 154. How do you create a sticky header?

### Answer

A sticky header stays visible while scrolling.

Use:

```css
header {
  position: sticky;

  top: 0;
}
```

### Example

```css
.header {
  position: sticky;

  top: 0;

  background: white;
}
```

### Requirements

- Must define a position value
- Must define offset (`top`)

### Interview Tip

Sticky headers are commonly used in modern websites.

---

# 155. How do you create an overlay?

### Answer

An overlay is created using absolute positioning.

### Example

HTML:

```html
<div class="card">
  <img src="image.jpg" />

  <div class="overlay">Text</div>
</div>
```

CSS:

```css
.card {
  position: relative;
}

.overlay {
  position: absolute;

  top: 0;

  left: 0;

  width: 100%;

  height: 100%;
}
```

### Common Uses

- Image captions
- Modals
- Loading screens

### Interview Tip

Overlay pattern usually requires:

```
Parent → relative

Child → absolute
```

---

# 156. How do you create a responsive navbar?

### Answer

A responsive navbar changes layout based on screen size.

### Desktop

```css
.nav {
  display: flex;
}
```

### Mobile

```css
@media (max-width: 768px) {
  .nav {
    flex-direction: column;
  }
}
```

### Common Features

- Hamburger menu
- Hidden links
- Mobile dropdown

### Example

```css
.menu {
  display: none;
}

@media (max-width: 768px) {
  .menu {
    display: block;
  }
}
```

### Interview Tip

Responsive navigation is usually handled using Flexbox and media queries.

---

# 157. How do you create a CSS triangle?

### Answer

A triangle can be created using borders.

### Example

```css
.triangle {
  width: 0;

  height: 0;

  border-left: 50px solid transparent;

  border-right: 50px solid transparent;

  border-bottom: 100px solid black;
}
```

Output:

```
   ▲
```

### Explanation

The element has:

- No width
- No height
- Borders create the shape

### Common Uses

- Tooltips
- Dropdown arrows
- Icons

### Interview Tip

CSS shapes are often created using borders.

---

# 158. How do you create a tooltip using CSS?

### Answer

A tooltip displays extra information when hovering over an element.

### HTML

```html
<button class="btn">
  Hover me

  <span class="tooltip"> Hello </span>
</button>
```

### CSS

```css
.tooltip {
  display: none;
}

.btn:hover .tooltip {
  display: block;
}
```

### Modern Approach

Use:

```css
::after;
```

pseudo-element.

Example:

```css
.btn:hover::after {
  content: "Tooltip";
}
```

### Interview Tip

Tooltips can be created without JavaScript.

---

# 159. How do you create a modal popup using CSS?

### Answer

A modal can be created using fixed positioning.

### Example

```css
.modal {
  position: fixed;

  top: 0;

  left: 0;

  width: 100%;

  height: 100%;
}
```

### Common Properties

```css
background: rgba();

z-index: 1000;
```

### Structure

```
Modal Overlay

    ↓

Modal Content
```

### Example

```css
.modal-content {
  background: white;

  padding: 20px;
}
```

### Interview Tip

Modals usually require:

- fixed position
- overlay background
- high z-index

---

# 160. How do you create a dark mode using CSS?

### Answer

Dark mode can be created using CSS variables.

### Example

```css
:root {
  --bg: white;

  --text: black;
}

.dark {
  --bg: black;

  --text: white;
}

body {
  background: var(--bg);

  color: var(--text);
}
```

When the `.dark` class is added:

```
Light Theme → Dark Theme
```

### Benefits

- Easy theme switching
- Less duplicate CSS
- Better maintainability

### JavaScript Example

```javascript
document.body.classList.toggle("dark");
```

### Interview Tip

CSS variables are the preferred way to implement themes.

---

# 161. How do you improve CSS performance?

### Answer

CSS performance can be improved by writing efficient styles.

### Techniques

## 1. Avoid unnecessary selectors

Avoid:

```css
div ul li a span {
}
```

Prefer:

```css
.nav-link {
}
```

---

## 2. Reduce unused CSS

Remove styles that are not used.

---

## 3. Use efficient animations

Prefer:

```css
transform

opacity
```

instead of:

```css
width

height

top

left
```

---

## 4. Minimize CSS files

Use:

- Minification
- Bundling

---

## 5. Avoid excessive nesting

Deep selectors increase browser work.

### Interview Tip

Good CSS should be simple, reusable, and maintainable.

---

# 162. Difference between pseudo-class and pseudo-element?

### Answer

Both are used to style elements without adding extra HTML.

---

## Pseudo-class

Targets a special state of an element.

Examples:

```css
:hover

:focus

:first-child
```

Example:

```css
button:hover {
  background: red;
}
```

---

## Pseudo-element

Targets a specific part of an element.

Examples:

```css
::before

::after

::first-letter
```

Example:

```css
p::first-letter {
  font-size: 30px;
}
```

### Comparison

| Pseudo-class      | Pseudo-element    |
| ----------------- | ----------------- |
| Element state     | Element part      |
| Uses single colon | Uses double colon |
| `:hover`          | `::before`        |

### Interview Tip

Remember:

```
Class → State

Element → Part
```

---
````

## Next section: **CSS Interview Final Revision Questions (163–180)**.

# 163. What is the difference between pseudo-elements `::before` and `::after`?

### Answer

`::before` and `::after` are CSS pseudo-elements used to insert virtual content before or after an element's actual content.

They do not require extra HTML elements.

---

## ::before

Adds content before the element content.

Example:

```css
h1::before {
  content: "⭐";
}
```

Output:

```
⭐ Heading
```

---

## ::after

Adds content after the element content.

Example:

```css
h1::after {
  content: " →";
}
```

Output:

```
Heading →
```

---

### Important Rule

The `content` property is required.

```css
.box::before {
  content: "";
}
```

### Common Uses

- Icons
- Decorative elements
- Tooltips
- Shapes

### Interview Tip

Pseudo-elements create virtual elements using CSS.

---

# 164. What is box-sizing in CSS?

### Answer

`box-sizing` controls how the width and height of an element are calculated.

### Values

- `content-box`
- `border-box`

---

## content-box (default)

Width includes only content.

Example:

```css
.box {
  width: 200px;

  padding: 20px;

  border: 5px solid;
}
```

Actual size:

```
200 + 40 + 10 = 250px
```

---

## border-box

Width includes:

- Content
- Padding
- Border

Example:

```css
.box {
  box-sizing: border-box;

  width: 200px;
}
```

Total size remains:

```
200px
```

### Interview Tip

Most modern projects use:

```css
* {
  box-sizing: border-box;
}
```

---

# 165. Why do we use box-sizing:border-box?

### Answer

`border-box` makes layouts easier because declared width includes padding and borders.

### Without border-box

```css
width: 300px;

padding: 20px;

border: 5px;
```

Actual size becomes:

```
350px
```

---

### With border-box

```css
box-sizing: border-box;

width: 300px;
```

Actual size:

```
300px
```

### Benefits

- Predictable sizing
- Easier responsive layouts
- Prevents overflow issues

### Interview Tip

Always include border-box in CSS resets.

---

# 166. What is the difference between width and max-width?

### Answer

Both control element width, but they behave differently.

---

## width

Sets a fixed width.

Example:

```css
.container {
  width: 500px;
}
```

Element always tries to be 500px.

---

## max-width

Sets the maximum allowed width.

Example:

```css
.container {
  max-width: 500px;
}
```

Element can shrink but cannot exceed 500px.

### Comparison

| width              | max-width          |
| ------------------ | ------------------ |
| Fixed size         | Maximum limit      |
| Can cause overflow | More responsive    |
| Less flexible      | Better for layouts |

### Interview Tip

Use `max-width` for responsive containers.

---

# 167. What is the difference between height and min-height?

### Answer

### height

Sets an exact height.

Example:

```css
.box {
  height: 300px;
}
```

The element remains 300px.

---

### min-height

Sets the minimum required height.

Example:

```css
.box {
  min-height: 300px;
}
```

The element can grow if content needs more space.

### Comparison

| height               | min-height         |
| -------------------- | ------------------ |
| Fixed height         | Minimum height     |
| Content may overflow | Content can expand |
| Less flexible        | More responsive    |

### Interview Tip

Use `min-height` for dynamic content sections.

---

# 168. What is the difference between margin and padding?

### Answer

Both create space, but they work in different areas.

---

## Padding

Space inside the element.

```
+-------------+
|   padding   |
|   Content   |
|             |
+-------------+
```

Example:

```css
.box {
  padding: 20px;
}
```

---

## Margin

Space outside the element.

```
   margin

+-------------+
|  Content    |
+-------------+

   margin
```

Example:

```css
.box {
  margin: 20px;
}
```

### Comparison

| Padding                   | Margin                             |
| ------------------------- | ---------------------------------- |
| Inside space              | Outside space                      |
| Affects background        | Background does not include margin |
| Used for internal spacing | Used between elements              |

### Interview Tip

Padding increases element size; margin separates elements.

---

# 169. What is margin collapsing?

### Answer

Margin collapsing occurs when vertical margins of block elements combine into a single margin.

### Example

```css
.box1 {
  margin-bottom: 30px;
}

.box2 {
  margin-top: 20px;
}
```

Instead of:

```
30px + 20px = 50px
```

The browser uses:

```
30px
```

(the larger margin)

### Happens Between

- Adjacent block elements
- Parent and first/last child elements

### Does Not Happen With

- Flex containers
- Grid containers
- Positioned elements

### Interview Tip

Margin collapsing mainly affects vertical margins.

---

# 170. What is the difference between display:none and opacity:0?

### Answer

Both hide elements visually but behave differently.

| display:none                            | opacity:0                |
| --------------------------------------- | ------------------------ |
| Removes from layout                     | Keeps layout space       |
| Not clickable                           | Can still receive clicks |
| Element removed visually and physically | Only transparent         |

### Example

```css
.box {
  display: none;
}
```

Element disappears completely.

---

```css
.box {
  opacity: 0;
}
```

Element becomes invisible but remains.

### Interview Tip

Use opacity for animations and display:none for removing elements.

---

# 171. What is object-fit in CSS?

### Answer

`object-fit` controls how images and videos fit inside their containers.

### Values

- fill
- contain
- cover
- none
- scale-down

---

## cover

Fills container while maintaining aspect ratio.

```css
img {
  object-fit: cover;
}
```

---

## contain

Shows complete image inside container.

```css
img {
  object-fit: contain;
}
```

### Example

```css
.image {
  width: 300px;

  height: 200px;

  object-fit: cover;
}
```

### Common Uses

- Profile images
- Product cards
- Galleries

### Interview Tip

`object-fit:cover` is commonly used for card images.

---

# 172. What is object-position?

### Answer

`object-position` controls the position of replaced elements like images inside their container.

### Example

```css
img {
  object-fit: cover;

  object-position: center;
}
```

### Values

```css
center

top

bottom

left

right
```

Example:

```css
img {
  object-position: top;
}
```

The top part of the image remains visible.

### Interview Tip

Use object-position with object-fit for better image control.

---

# 173. What is CSS specificity?

### Answer

Specificity determines which CSS rule is applied when multiple rules target the same element.

Higher specificity wins.

### Priority Order

```
!important

Inline styles

ID selector

Class selector

Element selector
```

### Example

```css
#title {
  color: red;
}

.title {
  color: blue;
}
```

ID wins.

### Interview Tip

Specificity decides the winner in CSS conflicts.

---

# 174. How is specificity calculated?

### Answer

Specificity is calculated using four levels:

```
Inline → IDs → Classes → Elements
```

Example:

```css
#header .title p {
}
```

Specificity:

```
ID: 1

Class: 1

Element: 1
```

Higher specificity beats lower specificity.

### Example

```css
p {
  color: red;
}

.text {
  color: blue;
}
```

Class wins.

### Interview Tip

Avoid unnecessarily high specificity.

---

# 175. What is !important in CSS?

### Answer

`!important` gives a CSS rule the highest priority.

### Example

```css
p {
  color: red !important;
}
```

It overrides normal rules.

### Problems

- Makes debugging difficult
- Creates specificity issues
- Hard to maintain

### Best Practice

Avoid using `!important` unless necessary.

### Interview Tip

Use proper selectors instead of relying on `!important`.

---

---

# 176. What is CSS specificity conflict?

### Answer

A specificity conflict occurs when multiple CSS rules target the same element but have different specificity levels.

The browser applies the rule with higher specificity.

### Example

```css
p {
  color: red;
}

.text {
  color: blue;
}
```

HTML:

```html
<p class="text">Hello</p>
```

Output:

```
Blue
```

Because:

```
class selector > element selector
```

### Solution

- Use proper selectors
- Avoid unnecessary nesting
- Avoid excessive `!important`

### Interview Tip

Specificity conflicts are common in large CSS projects.

---

# 177. What is the difference between class selector and ID selector?

### Answer

Both are used to select HTML elements, but they have different purposes.

---

## Class Selector

Used for reusable styles.

Syntax:

```css
.box {
  color: red;
}
```

HTML:

```html
<div class="box"></div>
```

A class can be used multiple times.

---

## ID Selector

Used for unique elements.

Syntax:

```css
#header {
  color: red;
}
```

HTML:

```html
<div id="header"></div>
```

An ID should be unique.

### Comparison

| Class             | ID                 |
| ----------------- | ------------------ |
| Reusable          | Unique             |
| Lower specificity | Higher specificity |
| Uses `.`          | Uses `#`           |

### Interview Tip

Prefer classes for styling and IDs mainly for JavaScript or unique elements.

---

# 178. What are CSS combinators?

### Answer

CSS combinators define relationships between selectors.

They allow selecting elements based on their relationship.

### Types

1. Descendant selector
2. Child selector
3. Adjacent sibling selector
4. General sibling selector

---

## Descendant

Selects all children inside an element.

```css
div p {
  color: red;
}
```

Selects all `p` inside `div`.

---

## Child

Selects direct children only.

```css
div > p {
  color: blue;
}
```

---

## Adjacent sibling

Selects the next sibling.

```css
h1 + p {
  color: green;
}
```

---

## General sibling

Selects all following siblings.

```css
h1 ~ p {
  color: black;
}
```

### Interview Tip

Combinators help write precise CSS selectors.

---

# 179. What is the difference between child selector and descendant selector?

### Answer

Both select elements inside another element, but their behavior differs.

---

## Descendant Selector

Selects all nested elements.

Example:

```css
.container p {
  color: red;
}
```

HTML:

```html
<div class="container">
  <p>Direct</p>

  <section>
    <p>Nested</p>
  </section>
</div>
```

Both paragraphs are selected.

---

## Child Selector

Selects only direct children.

Example:

```css
.container > p {
  color: blue;
}
```

Only:

```html
<p>Direct</p>
```

is selected.

### Comparison

| Descendant         | Child                        |
| ------------------ | ---------------------------- |
| Uses space         | Uses `>`                     |
| Selects all levels | Selects direct children only |

### Interview Tip

Use child selectors when you need strict control.

---

# 180. What are CSS logical properties?

### Answer

CSS logical properties allow styling based on writing direction instead of physical directions.

Instead of:

```css
left

right

top

bottom
```

they use:

```css
inline

block
```

### Examples

Traditional:

```css
margin-left: 20px;
```

Logical:

```css
margin-inline-start: 20px;
```

### Common Logical Properties

```css
margin-inline

padding-block

border-inline

inset-inline
```

### Benefits

- Supports different languages
- Better international layouts
- Cleaner responsive design

### Interview Tip

Logical properties are useful for multilingual websites.

---

# 181. What is the CSS `inherit` value?

### Answer

`inherit` forces an element to take the value of its parent element.

### Example

```css
.child {
  color: inherit;
}
```

The child gets the parent's color.

### Example

```css
.parent {
  color: blue;
}

.child {
  color: inherit;
}
```

Output:

```
Child text is blue
```

### Interview Tip

`inherit` is useful when you want explicit inheritance.

---

# 182. What is the CSS `initial` value?

### Answer

`initial` sets a property back to its default CSS value.

### Example

```css
p {
  display: initial;
}
```

It resets the property to its initial value.

### Example

```css
button {
  color: initial;
}
```

### Interview Tip

`initial` does not mean browser default styles; it means CSS specification default.

---

# 183. What is the CSS `unset` value?

### Answer

`unset` behaves differently depending on whether a property is inherited.

It acts as:

- `inherit` for inherited properties
- `initial` for non-inherited properties

### Example

```css
p {
  color: unset;
}
```

Since color is inherited, it inherits from the parent.

### Interview Tip

`unset` combines the behavior of `inherit` and `initial`.

---

# 184. What is the CSS `all` property?

### Answer

The `all` property resets all CSS properties of an element.

### Values

- initial
- inherit
- unset
- revert

### Example

```css
.box {
  all: unset;
}
```

This removes most applied styles.

### Common Use

Creating clean component styles.

### Interview Tip

Use carefully because it affects almost every property.

---

# 185. What is CSS `object-fit` vs `background-size`?

### Answer

Both control how images fit inside containers, but they work differently.

### object-fit

Used for:

```html
<img />
```

Example:

```css
img {
  object-fit: cover;
}
```

---

### background-size

Used for:

```css
background-image
```

Example:

```css
.box {
  background-size: cover;
}
```

### Comparison

| object-fit                 | background-size            |
| -------------------------- | -------------------------- |
| Works on images/videos     | Works on backgrounds       |
| Controls replaced elements | Controls background images |
| Uses object-position       | Uses background-position   |

### Interview Tip

Use object-fit for content images and background-size for decorative images.

---

# 186. What is CSS clipping?

### Answer

CSS clipping controls which part of an element is visible.

The main property is:

```css
clip-path
```

### Example

```css
.circle {
  clip-path: circle(50%);
}
```

Creates a circular visible area.

### Common Shapes

- circle
- ellipse
- polygon
- inset

### Uses

- Image shapes
- Creative designs
- Masking effects

### Interview Tip

`clip-path` hides parts of elements without changing the layout.

---

# 187. What is CSS `aspect-ratio`?

### Answer

`aspect-ratio` defines the preferred width-to-height ratio of an element.

### Example

```css
.video {
  aspect-ratio: 16 / 9;
}
```

The element maintains:

```
16:9 ratio
```

### Uses

- Videos
- Images
- Cards

### Example

```css
.card {
  width: 300px;

  aspect-ratio: 1;
}
```

Creates a square card.

### Interview Tip

Aspect-ratio reduces the need for fixed heights.

---

# 188. What is CSS containment?

### Answer

CSS containment improves performance by limiting how much the browser needs to calculate when rendering elements.

Property:

```css
contain
```

### Example

```css
.card {
  contain: layout;
}
```

### Types

- size
- layout
- paint
- style

### Benefits

- Better rendering performance
- Improves large applications

### Interview Tip

Containment is useful for optimizing complex interfaces.

---

# 189. What are CSS best practices?

### Answer

Good CSS should be:

- Maintainable
- Reusable
- Scalable
- Easy to understand

### Best Practices

## 1. Use meaningful class names

Good:

```css
.card-title
```

Avoid:

```css
.red-text
```

---

## 2. Avoid deep nesting

Avoid:

```css
.header div ul li a span
```

---

## 3. Use CSS variables

Example:

```css
:root {
  --primary: blue;
}
```

---

## 4. Follow consistent naming

Examples:

- BEM
- Utility classes

---

## 5. Keep styles organized

Separate:

- Components
- Layout
- Utilities

### Interview Tip

Clean CSS improves team collaboration.

---

# 190. How do you organize CSS in large projects?

### Answer

Large projects require a structured CSS approach.

### Common Approaches

---

## 1. Component-Based CSS

Each component has its own styles.

Example:

```
components/

Button/

 Button.jsx

 Button.css
```

---

## 2. CSS Modules

Styles are scoped locally.

Example:

```javascript
import styles from "./Button.module.css";
```

---

## 3. BEM Naming

Example:

```css
.card {
}

.card__title {
}

.card__button {
}
```

---

## 4. Design Tokens

Use variables:

```css
:root {
  --primary-color: #333;

  --spacing: 8px;
}
```

---

## 5. Utility Classes

Reusable small classes.

Example:

```css
.text-center {
}

.mt-20 {
}
```

### Interview Tip

Modern React projects commonly use CSS Modules, Tailwind, styled-components, or component-based CSS.

---
