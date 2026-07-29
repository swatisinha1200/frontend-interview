# HTML Interview Answers

---

# 1. What is HTML?

### Answer

HTML (HyperText Markup Language) is the standard markup language used to create the structure of web pages.

It defines elements such as headings, paragraphs, images, links, forms, tables, and more. HTML describes **what** appears on the page, while CSS controls **how** it looks and JavaScript controls **how** it behaves.

### Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Page</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>Welcome to HTML.</p>
  </body>
</html>
```

### Interview Tip

> HTML is **not** a programming language.
> It is a **markup language**.

---

# 2. What is HTML5?

### Answer

HTML5 is the latest major version of HTML that introduced new semantic elements, multimedia support, APIs, and better accessibility.

### Features

- Semantic tags
- Audio & Video support
- Canvas
- SVG
- Local Storage
- Session Storage
- Drag & Drop API
- Geolocation API
- Web Workers

### Example

```html
<header>
  <h1>Website</h1>
</header>

<main>
  <article>HTML5 Example</article>
</main>
```

### Interview Tip

HTML5 reduced the need for plugins like Flash.

---

# 3. What are the features of HTML5?

### Answer

Major features include:

- Semantic elements
- Audio support
- Video support
- Canvas
- SVG
- Local Storage
- Session Storage
- Geolocation API
- Drag and Drop
- Web Workers
- Better form validation

### Interview Tip

Semantic HTML and built-in APIs are the biggest improvements over older HTML versions.

---

# 4. What is the basic structure of an HTML document?

### Answer

Every HTML document has a standard structure.

### Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Document</title>
  </head>

  <body></body>
</html>
```

### Explanation

- `<!DOCTYPE html>` → HTML5 declaration
- `<html>` → Root element
- `<head>` → Metadata
- `<body>` → Visible content

---

# 5. What is the purpose of <!DOCTYPE html>?

### Answer

`<!DOCTYPE html>` tells the browser that the document uses HTML5.

It ensures the browser renders the page in **Standards Mode** instead of **Quirks Mode**.

### Example

```html
<!DOCTYPE html>
```

### Interview Tip

Always place it at the very first line.

---

# 6. What are HTML elements?

### Answer

An HTML element consists of:

- Opening tag
- Content
- Closing tag

Example:

```html
<p>Hello World</p>
```

Here,

- Opening tag → `<p>`
- Content → Hello World
- Closing tag → `</p>`

Some elements don't have closing tags.

Example:

```html
<img src="image.jpg" alt="Image" />
```

---

# 7. What are HTML tags?

### Answer

Tags are keywords enclosed within angle brackets (`<>`) that define HTML elements.

### Examples

```html
<h1></h1>

<p></p>

<div></div>

<img />

<a></a>
```

### Interview Tip

Tags create elements.

---

# 8. What is the difference between tags and elements?

### Answer

| Tags                      | Elements                |
| ------------------------- | ----------------------- |
| Opening or closing markup | Complete structure      |
| Written inside `< >`      | Includes tag + content  |
| Example: `<p>`            | Example: `<p>Hello</p>` |

### Example

```html
<p>Hello</p>
```

- `<p>` → Tag
- `</p>` → Closing Tag
- `<p>Hello</p>` → Element

---

# 9. What are HTML attributes?

### Answer

Attributes provide additional information about HTML elements.

They are written inside the opening tag.

### Syntax

```html
<tag attribute="value"></tag>
```

### Example

```html
<img src="cat.jpg" alt="Cat" />

<a href="https://google.com"> Google </a>
```

### Common Attributes

- id
- class
- src
- href
- alt
- title
- style
- disabled
- required
- placeholder

---

# 10. What are global attributes in HTML?

### Answer

Global attributes can be used on almost every HTML element.

### Common Global Attributes

- id
- class
- style
- title
- hidden
- tabindex
- draggable
- lang
- dir
- contenteditable
- data-\*

### Example

```html
<div id="box" class="container" title="Profile" data-user="101">Hello</div>
```

### Interview Tip

`id` should be unique within a page, while `class` can be shared by multiple elements.

---

````md
---

# 11. What is Semantic HTML?

### Answer

Semantic HTML uses elements that clearly describe the purpose and meaning of the content they contain.

Instead of using generic tags like `<div>` everywhere, semantic tags make the structure of a webpage more meaningful to browsers, search engines, and developers.

### Common Semantic Elements

- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<article>`
- `<aside>`
- `<footer>`

### Example

```html
<header>
  <h1>My Blog</h1>
</header>

<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
</nav>

<main>
  <article>
    <h2>HTML Basics</h2>
    <p>Semantic HTML improves readability.</p>
  </article>
</main>

<footer>
  <p>&copy; 2026</p>
</footer>
```

### Benefits

- Better SEO
- Better accessibility
- Easier maintenance
- Cleaner code
- Improved readability

### Interview Tip

Semantic HTML gives **meaning**, not styling.

---

# 12. Why should we use Semantic HTML?

### Answer

Semantic HTML improves the quality and usability of web pages.

### Advantages

- Improves SEO
- Helps screen readers understand content
- Makes code easier to read
- Easier for developers to maintain
- Better browser understanding

### Example

Instead of

```html
<div class="header"></div>
<div class="menu"></div>
<div class="content"></div>
<div class="footer"></div>
```

Use

```html
<header></header>
<nav></nav>
<main></main>
<footer></footer>
```

### Interview Tip

Semantic HTML benefits both users and search engines.

---

# 13. What is the difference between semantic and non-semantic tags?

### Answer

Semantic tags describe the meaning of their content, while non-semantic tags do not.

| Semantic Tags        | Non-semantic Tags    |
| -------------------- | -------------------- |
| Describe purpose     | Generic containers   |
| Better SEO           | No SEO benefit       |
| Better accessibility | Less accessible      |
| Easier to understand | Harder to understand |

### Examples

Semantic

```html
<article>
  <h2>News</h2>
</article>
```

Non-semantic

```html
<div class="news">
  <h2>News</h2>
</div>
```

### Interview Tip

`<div>` is not bad—it should be used only when no semantic element fits.

---

# 14. Explain the following semantic tags

## `<header>`

Represents introductory content or a group of navigation links.

```html
<header>
  <h1>Company</h1>
</header>
```

---

## `<nav>`

Contains navigation links.

```html
<nav>
  <a href="/">Home</a>
  <a href="/contact">Contact</a>
</nav>
```

---

## `<main>`

Represents the primary content of the page.

There should generally be only one `<main>` element per page.

```html
<main>
  <h2>Products</h2>
</main>
```

---

## `<section>`

Represents a thematic grouping of related content.

```html
<section>
  <h2>Services</h2>
  <p>We provide web development.</p>
</section>
```

---

## `<article>`

Represents self-contained content that can stand on its own.

Examples:

- Blog post
- News article
- Forum post
- Product review

```html
<article>
  <h2>JavaScript Tips</h2>
</article>
```

---

## `<aside>`

Contains content related to the main content.

Examples:

- Sidebar
- Advertisements
- Related posts

```html
<aside>
  <h3>Related Articles</h3>
</aside>
```

---

## `<footer>`

Represents footer information.

```html
<footer>
  <p>&copy; 2026 Company</p>
</footer>
```

---

# 15. When should you use `<section>`?

### Answer

Use `<section>` to group related content under a common theme.

Usually, a section has its own heading.

### Example

```html
<section>
  <h2>Our Services</h2>

  <p>Web Development</p>

  <p>UI Design</p>
</section>
```

### Do Not Use

```html
<section>Just some random text.</section>
```

If there is no meaningful grouping, use a `<div>` instead.

### Interview Tip

A `<section>` should generally include a heading.

---

# 16. When should you use `<article>`?

### Answer

Use `<article>` for independent, self-contained content that can be reused or distributed separately.

### Examples

- Blog post
- News article
- Forum post
- Comment
- Product review

### Example

```html
<article>
  <h2>React Interview Questions</h2>

  <p>Today we'll discuss React Hooks...</p>
</article>
```

### Interview Tip

If the content makes sense on its own, use `<article>`.

---

# 17. Difference between `<section>` and `<article>`?

### Answer

| `<section>`            | `<article>`                 |
| ---------------------- | --------------------------- |
| Groups related content | Independent content         |
| Part of a page         | Can stand alone             |
| Organizes information  | Represents complete content |

### Example

```html
<section>
  <h2>Latest News</h2>

  <article>
    <h3>React 20 Released</h3>
  </article>

  <article>
    <h3>JavaScript Updates</h3>
  </article>
</section>
```

### Interview Tip

Think of a newspaper:

- Newspaper = `<section>`
- Individual news story = `<article>`

---

# 18. Difference between `<header>` and `<head>`?

### Answer

| `<head>`                    | `<header>`                         |
| --------------------------- | ---------------------------------- |
| Contains metadata           | Visible page content               |
| Not displayed               | Displayed on the page              |
| Only once per HTML document | Can appear multiple times          |
| Includes title, meta, CSS   | Includes logo, heading, navigation |

### Example

```html
<head>
  <title>My Website</title>
</head>

<body>
  <header>
    <h1>Welcome</h1>
  </header>
</body>
```

### Interview Tip

A very common interview question.

Remember:

- `<head>` → Browser information
- `<header>` → User-visible content

---

# 19. Difference between `<nav>` and `<menu>`?

### Answer

`<nav>` defines a section of navigation links.

```html
<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
</nav>
```

`<menu>` represents a list of commands or actions. It is rarely used in modern websites.

```html
<menu>
  <button>Save</button>
  <button>Delete</button>
</menu>
```

### Interview Tip

Use `<nav>` for website navigation.

Most production websites rarely use `<menu>`.

---

# 20. Why is Semantic HTML important for SEO?

### Answer

Search engines analyze semantic elements to better understand the structure and content of a webpage.

### Benefits

- Better page indexing
- Improved search rankings
- Easier crawling
- Rich search results
- Better user experience

### Example

```html
<article>
  <h1>HTML Interview Questions</h1>

  <section>
    <h2>Semantic HTML</h2>
    <p>...</p>
  </section>
</article>
```

This clearly tells search engines:

- Main article
- Topic heading
- Related section

### Interview Tip

Semantic HTML **does not directly increase rankings**, but it helps search engines understand your content, which can improve SEO when combined with good content and other best practices.

---
````

---

# 21. What is the difference between `<div>` and `<span>`?

### Answer

Both `<div>` and `<span>` are non-semantic HTML elements used to group content. The main difference is how they behave in the document.

| `<div>`                       | `<span>`                           |
| ----------------------------- | ---------------------------------- |
| Block-level element           | Inline element                     |
| Starts on a new line          | Does not start on a new line       |
| Takes full available width    | Takes only the required width      |
| Used to group larger sections | Used to style small pieces of text |

### Example

```html
<div class="card">
  <h2>Product</h2>
  <p>Description</p>
</div>

<p>
  Price:
  <span class="price">$99</span>
</p>
```

### Interview Tip

Neither `<div>` nor `<span>` has any semantic meaning.

---

# 22. What are block-level elements?

### Answer

Block-level elements always begin on a new line and occupy the full width available by default.

### Common Block Elements

- `<div>`
- `<p>`
- `<h1>` to `<h6>`
- `<section>`
- `<article>`
- `<header>`
- `<footer>`
- `<main>`
- `<nav>`
- `<ul>`
- `<ol>`
- `<li>`

### Example

```html
<h1>Heading</h1>

<p>This is a paragraph.</p>

<div>Container</div>
```

Each element appears on a separate line.

### Interview Tip

Think of block elements as creating "blocks" in the page layout.

---

# 23. What are inline elements?

### Answer

Inline elements do not start on a new line. They only occupy as much width as their content requires.

### Common Inline Elements

- `<span>`
- `<a>`
- `<strong>`
- `<em>`
- `<img>`
- `<label>`
- `<code>`
- `<small>`

### Example

```html
<p>
  Learn
  <strong>HTML</strong>
  and
  <em>CSS</em>.
</p>
```

The inline elements remain within the same line.

### Interview Tip

Inline elements are commonly used for formatting text within block elements.

---

# 24. Difference between block and inline elements?

### Answer

| Block Elements                                                   | Inline Elements                                 |
| ---------------------------------------------------------------- | ----------------------------------------------- |
| Start on a new line                                              | Stay in the same line                           |
| Take full available width                                        | Take only required width                        |
| Can contain block and inline elements (depending on the element) | Generally contain text or other inline elements |
| Used for layout                                                  | Used for text formatting                        |

### Example

```html
<div>
  <span>Hello</span>
  <span>World</span>
</div>
```

Output

```
Hello World
```

The `<div>` creates a block, while the `<span>` elements remain inline.

### Interview Tip

This is one of the most frequently asked HTML interview questions.

---

# 25. What is the `<pre>` tag?

### Answer

The `<pre>` element displays preformatted text.

It preserves:

- Spaces
- Tabs
- Line breaks

exactly as written in the HTML source.

### Example

```html
<pre>
Name: Swati
Age : 31
City: Hyderabad
</pre>
```

Output

```
Name: Swati
Age : 31
City: Hyderabad
```

### Common Uses

- Displaying code
- ASCII art
- Logs
- Configuration files

### Interview Tip

Browsers normally collapse multiple spaces. `<pre>` prevents this behavior.

---

# 26. What is the `<code>` tag?

### Answer

The `<code>` tag represents a fragment of computer code.

It is semantic and often displayed in a monospace font.

### Example

```html
<p>
  Use
  <code>console.log()</code>
  to print output.
</p>
```

### Combining with `<pre>`

```html
<pre>
<code>
function greet() {
  console.log("Hello");
}
</code>
</pre>
```

### Interview Tip

`<code>` identifies code, while `<pre>` preserves formatting. They are often used together.

---

# 27. Difference between `<strong>` and `<b>`?

### Answer

Both typically appear bold, but they have different meanings.

| `<strong>`               | `<b>`                   |
| ------------------------ | ----------------------- |
| Semantic                 | Non-semantic            |
| Indicates importance     | Only changes appearance |
| Better for accessibility | Purely visual           |

### Example

```html
<p>
  <strong>Warning:</strong>
  Save your work.
</p>

<p>
  <b>Product Name</b>
</p>
```

### Interview Tip

Prefer `<strong>` when the text is important, not just bold.

---

# 28. Difference between `<em>` and `<i>`?

### Answer

Both usually appear italic, but they serve different purposes.

| `<em>`                      | `<i>`                 |
| --------------------------- | --------------------- |
| Semantic                    | Non-semantic          |
| Adds emphasis               | Visual styling only   |
| Screen readers emphasize it | No additional meaning |

### Example

```html
<p>
  Please
  <em>read carefully</em>.
</p>

<p>
  <i>Scientific Name</i>
</p>
```

### Interview Tip

Use `<em>` when the emphasis changes the meaning of the sentence.

---

# 29. Difference between `<br>` and `<hr>`?

### Answer

`<br>` inserts a line break, while `<hr>` creates a thematic break between sections.

### `<br>` Example

```html
Address:<br />
Hyderabad<br />
India
```

### `<hr>` Example

```html
<h2>Chapter 1</h2>

<hr />

<h2>Chapter 2</h2>
```

### Comparison

| `<br>`           | `<hr>`                                  |
| ---------------- | --------------------------------------- |
| Line break       | Horizontal rule                         |
| No visible line  | Displays a horizontal line (by default) |
| Used within text | Separates sections                      |

### Interview Tip

Use `<br>` sparingly. Avoid using it to create page spacing—use CSS instead.

---

# 30. Difference between `<ol>` and `<ul>`?

### Answer

`<ol>` creates an ordered (numbered) list, while `<ul>` creates an unordered (bulleted) list.

### Ordered List

```html
<ol>
  <li>Install Node.js</li>
  <li>Create Project</li>
  <li>Run Application</li>
</ol>
```

Output

```
1. Install Node.js
2. Create Project
3. Run Application
```

### Unordered List

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

Output

```
• HTML
• CSS
• JavaScript
```

### Interview Tip

Use `<ol>` when the order matters (steps, rankings, instructions).

Use `<ul>` when the order does not matter (features, skills, categories).

---

---

# 31. What is the anchor (`<a>`) tag?

### Answer

The `<a>` (anchor) tag is used to create hyperlinks that allow users to navigate between web pages, sections of the same page, email addresses, phone numbers, or downloadable files.

### Syntax

```html
<a href="URL">Link Text</a>
```

### Example

```html
<a href="https://www.google.com">Visit Google</a>
```

### Other Examples

Open in a new tab:

```html
<a href="https://openai.com" target="_blank"> OpenAI </a>
```

Email link:

```html
<a href="mailto:abc@example.com"> Send Email </a>
```

Phone link:

```html
<a href="tel:+911234567890"> Call Us </a>
```

### Interview Tip

The `href` attribute is required to make an anchor a hyperlink.

---

# 32. Difference between Absolute URL and Relative URL?

### Answer

A URL specifies the location of a resource.

### Absolute URL

Contains the complete web address including protocol and domain.

```html
<a href="https://www.google.com">Google</a>
```

### Relative URL

Contains the path relative to the current website.

```html
<a href="/about">About</a>

<a href="contact.html">Contact</a>
```

### Comparison

| Absolute URL               | Relative URL                 |
| -------------------------- | ---------------------------- |
| Complete address           | Partial address              |
| Includes protocol          | No protocol                  |
| Used for external websites | Used within the same website |

### Interview Tip

Use relative URLs for internal navigation and absolute URLs for external websites.

---

# 33. What is the `target` attribute?

### Answer

The `target` attribute specifies where the linked document should open.

### Common Values

| Value     | Description                      |
| --------- | -------------------------------- |
| `_self`   | Opens in the same tab (default)  |
| `_blank`  | Opens in a new tab               |
| `_parent` | Opens in the parent frame        |
| `_top`    | Opens in the full browser window |

### Example

```html
<a href="https://github.com" target="_blank"> GitHub </a>
```

### Interview Tip

When using `target="_blank"`, also use `rel="noopener noreferrer"` for security.

---

# 34. Why use `rel="noopener noreferrer"`?

### Answer

When opening a link in a new tab using `target="_blank"`, the newly opened page can potentially access the original page using `window.opener`.

Using

```html
rel="noopener noreferrer"
```

prevents this security risk.

### Example

```html
<a href="https://google.com" target="_blank" rel="noopener noreferrer">
  Google
</a>
```

### Benefits

- Improves security
- Prevents reverse tabnabbing attacks
- Improves performance by preventing access to `window.opener`

### Interview Tip

Most companies expect this whenever you use `target="_blank"`.

---

# 35. Difference between `<img>` and `<picture>`?

### Answer

`<img>` displays a single image.

`<picture>` allows multiple image sources so the browser can choose the best one based on screen size or image format.

### `<img>` Example

```html
<img src="car.jpg" alt="Car" />
```

### `<picture>` Example

```html
<picture>
  <source media="(min-width:768px)" srcset="large.jpg" />

  <source media="(min-width:480px)" srcset="medium.jpg" />

  <img src="small.jpg" alt="Car" />
</picture>
```

### Comparison

| `<img>`       | `<picture>`                |
| ------------- | -------------------------- |
| Single image  | Multiple image sources     |
| Simpler       | Responsive images          |
| Less flexible | Browser chooses best image |

### Interview Tip

Use `<picture>` for responsive images and modern image formats like WebP or AVIF.

---

# 36. What is the `<picture>` element?

### Answer

The `<picture>` element is a container that provides multiple versions of an image.

The browser selects the most appropriate image based on:

- Screen size
- Device resolution
- Supported image format

### Example

```html
<picture>
  <source srcset="image.webp" type="image/webp" />

  <source srcset="image.jpg" type="image/jpeg" />

  <img src="image.jpg" alt="Landscape" />
</picture>
```

### Benefits

- Responsive images
- Better performance
- Modern image formats
- Browser compatibility

### Interview Tip

Always include an `<img>` element as the fallback inside `<picture>`.

---

# 37. What are Responsive Images?

### Answer

Responsive images automatically adapt to different screen sizes and device resolutions.

This helps improve:

- Performance
- User experience
- Loading speed

### Methods

Using `srcset`

```html
<img
  src="small.jpg"
  srcset="small.jpg 480w, medium.jpg 768w, large.jpg 1200w"
  alt="Mountain"
/>
```

Using `<picture>`

```html
<picture>
  <source media="(min-width:768px)" srcset="desktop.jpg" />

  <img src="mobile.jpg" alt="Mountain" />
</picture>
```

### Interview Tip

Responsive images reduce unnecessary downloads on smaller devices.

---

# 38. Difference between SVG and Canvas?

### Answer

Both are used to display graphics but work differently.

### SVG

- Vector graphics
- XML-based
- Easily scalable
- Individual elements can be styled with CSS and manipulated with JavaScript

Example

```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" fill="blue" />
</svg>
```

### Canvas

- Pixel-based
- Drawn using JavaScript
- Better for animations and games

Example

```html
<canvas id="canvas"></canvas>
```

```javascript
const canvas = document.getElementById("canvas");
const ctx = canvas.getContext("2d");

ctx.fillRect(20, 20, 100, 60);
```

### Comparison

| SVG                      | Canvas                        |
| ------------------------ | ----------------------------- |
| Vector                   | Raster                        |
| Scalable                 | Pixel-based                   |
| DOM elements             | Single drawing surface        |
| Best for icons and logos | Best for games and animations |

### Interview Tip

SVG is ideal for icons, logos, and charts.

Canvas is ideal for games, image editing, and complex animations.

---

# 39. What is an `<iframe>`?

### Answer

An `<iframe>` (Inline Frame) is used to embed another HTML document inside the current webpage.

### Common Uses

- YouTube videos
- Google Maps
- External websites
- PDF viewers

### Example

```html
<iframe
  src="https://example.com"
  width="600"
  height="400"
  title="Example Website"
>
</iframe>
```

### Important Attributes

- `src`
- `width`
- `height`
- `title`
- `loading`
- `allowfullscreen`

### Interview Tip

Always provide a meaningful `title` attribute for accessibility.

---

# 40. Advantages and Disadvantages of `<iframe>`

### Advantages

- Embed external websites
- Display videos
- Embed maps
- Display PDFs
- Isolates embedded content

### Disadvantages

- Can slow page loading
- SEO benefits are limited for embedded content
- Security concerns with untrusted sources
- Difficult to style embedded content from another domain due to the Same-Origin Policy

### Example

Embedding a YouTube video

```html
<iframe
  width="560"
  height="315"
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="YouTube Video"
  allowfullscreen
>
</iframe>
```

### Interview Tip

Use iframes only when necessary. Avoid embedding untrusted websites, and use attributes like `loading="lazy"` when appropriate to improve performance.

---

---

# 41. What is a form?

### Answer

An HTML form is used to collect user input and send it to a server for processing.

Forms are commonly used for:

- Login
- Registration
- Contact forms
- Search
- Feedback
- Checkout

### Syntax

```html
<form action="/submit" method="post"></form>
```

### Example

```html
<form action="/register" method="post">
  <label for="name">Name</label>
  <input type="text" id="name" name="name" />

  <button type="submit">Register</button>
</form>
```

### Important Attributes

- `action`
- `method`
- `autocomplete`
- `novalidate`

### Interview Tip

The `<form>` element itself does not collect data—it acts as a container for form controls.

---

# 42. Explain GET vs POST.

### Answer

GET and POST are HTTP methods used to submit form data.

### GET

- Sends data in the URL
- Visible in browser address bar
- Can be bookmarked
- Has URL length limitations
- Suitable for searching and fetching data

Example

```html
<form method="get"></form>
```

URL after submission

```
https://example.com/search?q=html
```

---

### POST

- Sends data in the request body
- Data is not visible in the URL
- Better for sensitive information
- No practical URL length limit
- Used for creating or updating data

Example

```html
<form method="post"></form>
```

### Comparison

| GET               | POST                                     |
| ----------------- | ---------------------------------------- |
| Data in URL       | Data in request body                     |
| Less secure       | More secure (especially with HTTPS)      |
| Can be bookmarked | Cannot be bookmarked with submitted data |
| Used for fetching | Used for submitting                      |

### Interview Tip

Passwords should **never** be sent using GET.

---

# 43. Difference between `id` and `name`?

### Answer

Although they may contain the same value, they serve different purposes.

### `id`

- Uniquely identifies an element
- Used by CSS
- Used by JavaScript
- Used with `<label for="">`

Example

```html
<input id="email" />
```

---

### `name`

- Used when submitting form data
- Sent to the server
- Required if you want the field's value included in the form submission

Example

```html
<input id="email" name="email" />
```

### Comparison

| id               | name                                                |
| ---------------- | --------------------------------------------------- |
| Must be unique   | Can be repeated in some cases (e.g., radio buttons) |
| Used by CSS & JS | Used for form submission                            |
| Not submitted    | Submitted with the form                             |

### Interview Tip

Without a `name` attribute, an input's value is generally **not included** in the submitted form data.

---

# 44. What is the `<label>` tag?

### Answer

The `<label>` tag provides a text description for a form control.

Clicking the label focuses or activates the associated input.

### Example

```html
<label for="email"> Email </label>

<input id="email" type="email" />
```

### Benefits

- Better accessibility
- Larger clickable area
- Better user experience

### Interview Tip

Always associate a label with every form field whenever possible.

---

# 45. Why should every input have a label?

### Answer

Labels improve both usability and accessibility.

### Benefits

- Helps screen readers identify inputs
- Makes forms easier to understand
- Clicking the label focuses the input
- Improves user experience

### Example

❌ Poor

```html
<input type="text" />
```

✅ Better

```html
<label for="username"> Username </label>

<input id="username" type="text" />
```

### Interview Tip

Using placeholders alone is **not** a replacement for labels.

---

# 46. Difference between `readonly` and `disabled`?

### Answer

Both restrict user interaction, but they behave differently.

### `readonly`

- User cannot edit the value
- Value is submitted with the form
- Element can receive focus

Example

```html
<input type="text" value="Swati" readonly />
```

---

### `disabled`

- User cannot interact with the element
- Value is **not** submitted
- Cannot receive focus

Example

```html
<input type="text" value="Swati" disabled />
```

### Comparison

| readonly     | disabled     |
| ------------ | ------------ |
| Editable ❌  | Editable ❌  |
| Submitted ✅ | Submitted ❌ |
| Focusable ✅ | Focusable ❌ |

### Interview Tip

This is a very common frontend interview question.

---

# 47. Difference between `required` and `pattern`?

### Answer

### `required`

Makes a field mandatory.

```html
<input type="text" required />
```

---

### `pattern`

Validates the entered value using a regular expression.

```html
<input type="text" pattern="[A-Za-z]{3,}" />
```

The above accepts only letters with a minimum length of 3.

### Comparison

| required                 | pattern                        |
| ------------------------ | ------------------------------ |
| Checks if input is empty | Checks the format of the value |
| Mandatory field          | Validation rule                |

### Interview Tip

They are often used together.

```html
<input required pattern="[A-Za-z]{3,}" />
```

---

# 48. Difference between radio and checkbox?

### Answer

Both allow users to make selections, but they are used in different scenarios.

### Radio Button

- Only one option can be selected within the same `name` group.

```html
<input type="radio" name="gender" />

<input type="radio" name="gender" />
```

---

### Checkbox

- Multiple options can be selected.

```html
<input type="checkbox" />

<input type="checkbox" />
```

### Comparison

| Radio                      | Checkbox               |
| -------------------------- | ---------------------- |
| One selection              | Multiple selections    |
| Same `name` groups options | Independent selections |
| Circular UI                | Square UI              |

### Interview Tip

Radio buttons in the same group must share the same `name` attribute.

---

# 49. Difference between button, submit and reset?

### Answer

The `<button>` element can have different behaviors based on its `type` attribute.

### `type="button"`

Does nothing by default.

Used with JavaScript.

```html
<button type="button">Click</button>
```

---

### `type="submit"`

Submits the form.

```html
<button type="submit">Submit</button>
```

---

### `type="reset"`

Resets all form fields to their initial values.

```html
<button type="reset">Reset</button>
```

### Comparison

| Type   | Purpose                   |
| ------ | ------------------------- |
| button | Custom JavaScript actions |
| submit | Submit the form           |
| reset  | Restore initial values    |

### Interview Tip

Inside a `<form>`, a `<button>` without a `type` attribute defaults to `type="submit"`.

---

# 50. What are HTML5 input types?

### Answer

HTML5 introduced several new input types that provide built-in validation and better user experiences.

### Common Input Types

- text
- password
- email
- number
- tel
- url
- search
- date
- time
- datetime-local
- month
- week
- color
- range
- file
- checkbox
- radio
- hidden

### Example

```html
<input type="email" />

<input type="date" />

<input type="color" />

<input type="range" />

<input type="file" />
```

### Benefits

- Built-in validation
- Better mobile keyboards
- Improved user experience
- Less JavaScript required

### Interview Tip

Use the most appropriate input type instead of always using `type="text"`.

For example:

- `type="email"` validates email format.
- `type="number"` accepts numeric input.
- `type="date"` displays a date picker in supported browsers.

---

---

# 51. What is Web Storage?

### Answer

Web Storage is a feature of HTML5 that allows websites to store data directly in the user's browser.

Unlike cookies, Web Storage stores larger amounts of data and is **not sent to the server** with every HTTP request.

### Types of Web Storage

- localStorage
- sessionStorage

### Benefits

- Stores data in the browser
- Faster than cookies for client-side data
- Stores more data (typically around 5–10 MB depending on the browser)
- Easy to use with JavaScript

### Example

```javascript
localStorage.setItem("name", "Swati");

sessionStorage.setItem("theme", "dark");
```

### Interview Tip

Web Storage is only accessible through JavaScript.

---

# 52. What is localStorage?

### Answer

`localStorage` stores data in the browser with **no expiration time**.

The data remains available even after:

- Closing the browser
- Restarting the computer

It is removed only when:

- The user clears browser data
- JavaScript removes it

### Example

Store Data

```javascript
localStorage.setItem("username", "Swati");
```

Retrieve Data

```javascript
const user = localStorage.getItem("username");
```

Remove One Item

```javascript
localStorage.removeItem("username");
```

Clear All Data

```javascript
localStorage.clear();
```

### Common Uses

- Dark mode preference
- Language selection
- Shopping cart
- User preferences

### Interview Tip

localStorage stores **only strings**.

To store objects:

```javascript
const user = {
  name: "Swati",
  age: 31,
};

localStorage.setItem("user", JSON.stringify(user));
```

Retrieve

```javascript
const data = JSON.parse(localStorage.getItem("user"));
```

---

# 53. What is sessionStorage?

### Answer

`sessionStorage` stores data only for the current browser tab or window.

The data is automatically removed when the tab or browser is closed.

### Example

Store

```javascript
sessionStorage.setItem("theme", "dark");
```

Retrieve

```javascript
sessionStorage.getItem("theme");
```

Remove

```javascript
sessionStorage.removeItem("theme");
```

Clear

```javascript
sessionStorage.clear();
```

### Common Uses

- Multi-step forms
- Temporary user data
- Session-specific information

### Interview Tip

Opening a new tab creates a new session with its own `sessionStorage`.

---

# 54. Difference between localStorage and sessionStorage?

### Answer

| localStorage                          | sessionStorage                      |
| ------------------------------------- | ----------------------------------- |
| No expiration                         | Exists only for the current session |
| Shared across tabs of the same origin | Limited to one tab/window           |
| Persists after browser restart        | Cleared when the tab is closed      |
| Suitable for long-term storage        | Suitable for temporary storage      |

### Example

```javascript
localStorage.setItem("theme", "dark");

sessionStorage.setItem("currentPage", "dashboard");
```

### Interview Tip

Remember:

- **localStorage → Long-term**
- **sessionStorage → Temporary**

---

# 55. What are Cookies?

### Answer

Cookies are small pieces of data stored in the browser.

Unlike Web Storage, cookies are automatically sent to the server with every HTTP request to the same domain.

### Uses

- Authentication
- Session management
- Remember Me functionality
- Tracking user preferences

### Example

```javascript
document.cookie = "username=Swati";
```

Read Cookie

```javascript
console.log(document.cookie);
```

### Interview Tip

Cookies can have an expiration date.

If no expiration is set, they become **session cookies**.

---

# 56. Cookies vs localStorage?

### Answer

| Cookies                         | localStorage                       |
| ------------------------------- | ---------------------------------- |
| Sent with every HTTP request    | Never sent automatically           |
| Small storage (~4 KB)           | Larger storage (typically 5–10 MB) |
| Can expire                      | No expiration unless removed       |
| Used for authentication/session | Used for client-side data          |

### Example

Cookie

```javascript
document.cookie = "theme=dark";
```

localStorage

```javascript
localStorage.setItem("theme", "dark");
```

### Interview Tip

Do **not** store sensitive information like passwords in either cookies or localStorage.

---

# 57. Cookies vs sessionStorage?

### Answer

| Cookies                      | sessionStorage                      |
| ---------------------------- | ----------------------------------- |
| Sent to server automatically | Not sent to server                  |
| Can persist beyond a session | Cleared when the tab closes         |
| About 4 KB storage           | Typically 5–10 MB storage           |
| Used for authentication      | Used for temporary client-side data |

### Example

Cookie

```javascript
document.cookie = "language=en";
```

sessionStorage

```javascript
sessionStorage.setItem("step", "2");
```

### Interview Tip

Use:

- Cookies → Authentication/session management
- sessionStorage → Temporary UI state

---

# 58. What are meta tags?

### Answer

Meta tags provide information (metadata) about a web page.

They are placed inside the `<head>` element and are not displayed on the page.

### Common Meta Tags

- charset
- viewport
- description
- keywords (largely ignored by modern search engines)
- author
- robots

### Example

```html
<head>
  <meta charset="UTF-8" />

  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <meta name="description" content="HTML Interview Questions" />
</head>
```

### Interview Tip

Meta tags help browsers and search engines understand your page.

---

# 59. Why is the viewport meta tag important?

### Answer

The viewport meta tag controls how a web page is displayed on different screen sizes.

Without it, mobile browsers may render the page as if it were designed for a much wider desktop screen.

### Syntax

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### Meaning

- `width=device-width` → Match the device's screen width.
- `initial-scale=1.0` → Set the initial zoom level.

### Benefits

- Responsive design
- Better mobile experience
- Proper scaling

### Interview Tip

This meta tag is essential for responsive websites.

---

# 60. What is charset?

### Answer

The `charset` meta tag specifies the character encoding used by the HTML document.

The recommended encoding is **UTF-8**, which supports most languages and symbols.

### Example

```html
<meta charset="UTF-8" />
```

### Benefits

- Displays special characters correctly
- Supports multiple languages
- Avoids character encoding issues

### Interview Tip

Always use UTF-8 unless you have a specific reason to use another encoding.

---

---

# 61. What is the description meta tag?

### Answer

The **description** meta tag provides a brief summary of a webpage's content.

Search engines often use this description in search results below the page title (though they may choose a different snippet).

### Syntax

```html
<meta
  name="description"
  content="Learn HTML interview questions with detailed answers and examples."
/>
```

### Benefits

- Improves SEO
- Increases click-through rate (CTR)
- Helps users understand the page before visiting

### Best Practices

- Keep it around **150–160 characters**
- Make it unique for every page
- Include important keywords naturally
- Write for users, not just search engines

### Interview Tip

The description meta tag is **not a direct ranking factor**, but a good description can improve CTR.

---

# 62. What is the robots meta tag?

### Answer

The `robots` meta tag tells search engine crawlers how to index and follow links on a webpage.

### Syntax

```html
<meta name="robots" content="index, follow" />
```

### Common Values

| Value       | Description                |
| ----------- | -------------------------- |
| `index`     | Allow indexing             |
| `noindex`   | Don't index the page       |
| `follow`    | Follow links               |
| `nofollow`  | Don't follow links         |
| `noarchive` | Don't store cached version |
| `nosnippet` | Don't show search snippet  |

### Example

Prevent indexing

```html
<meta name="robots" content="noindex, nofollow" />
```

### Interview Tip

Use `noindex` for pages like admin panels or thank-you pages that shouldn't appear in search results.

---

# 63. What is a Canonical URL?

### Answer

A canonical URL tells search engines which version of a webpage is the preferred (original) version.

It helps prevent duplicate content issues.

### Syntax

```html
<link rel="canonical" href="https://example.com/products" />
```

### Example

Suppose both URLs show the same page:

```
https://example.com/products

https://example.com/products?sort=price
```

The canonical URL should be:

```html
<link rel="canonical" href="https://example.com/products" />
```

### Benefits

- Prevents duplicate content
- Consolidates SEO value
- Improves indexing

### Interview Tip

Every important page should have a canonical URL pointing to its preferred version.

---

# 64. What is Open Graph metadata?

### Answer

Open Graph (OG) metadata controls how a webpage appears when shared on social media platforms like Facebook, LinkedIn, and many messaging apps.

### Example

```html
<meta property="og:title" content="Frontend Interview Questions" />

<meta
  property="og:description"
  content="100 HTML interview questions with answers."
/>

<meta property="og:image" content="cover.jpg" />

<meta property="og:url" content="https://example.com" />

<meta property="og:type" content="website" />
```

### Benefits

- Rich social media previews
- Better user engagement
- Professional appearance

### Interview Tip

Without Open Graph tags, social platforms may choose random images or text.

---

# 65. What is SEO?

### Answer

SEO (Search Engine Optimization) is the process of improving a website so it can be found more easily in search engine results.

The goal is to increase organic (non-paid) traffic.

### SEO Includes

- Semantic HTML
- Quality content
- Fast loading pages
- Mobile-friendly design
- Accessibility
- Good page structure

### Example

Instead of

```html
<div>About Us</div>
```

Use

```html
<h1>About Us</h1>
```

### Interview Tip

SEO is not only about keywords. Good HTML structure and user experience are also important.

---

# 66. How does HTML improve SEO?

### Answer

Proper HTML helps search engines understand your content more effectively.

### Good HTML Practices

- Use semantic elements
- Use heading tags correctly
- Add descriptive `alt` text to images
- Write meaningful page titles
- Add meta descriptions
- Use descriptive link text
- Create a logical page hierarchy

### Example

```html
<article>
  <h1>React Interview Questions</h1>

  <section>
    <h2>Hooks</h2>

    <p>...</p>
  </section>
</article>
```

### Benefits

- Better crawling
- Better indexing
- Improved accessibility
- Better user experience

### Interview Tip

Search engines understand semantic HTML much better than pages built entirely with generic `<div>` elements.

---

# 67. What are the best SEO practices in HTML?

### Answer

### Best Practices

- Use semantic HTML
- Write descriptive page titles
- Add meta descriptions
- Use proper heading hierarchy (`h1` → `h6`)
- Add `alt` text to images
- Use descriptive URLs
- Use canonical URLs
- Optimize images
- Use responsive design
- Improve page loading speed

### Example

```html
<header>
  <h1>HTML Interview Questions</h1>
</header>

<main>
  <article>
    <img src="html.png" alt="HTML Logo" />
  </article>
</main>
```

### Interview Tip

SEO is a combination of:

- Good HTML
- High-quality content
- Website performance
- Accessibility

---

# 68. What is Accessibility (a11y)?

### Answer

Accessibility (often abbreviated as **a11y**) is the practice of designing websites that everyone can use, including people with disabilities.

Examples include users who:

- Have visual impairments
- Have hearing impairments
- Cannot use a mouse
- Use screen readers
- Have cognitive disabilities

### Benefits

- Better user experience
- Wider audience
- Improved SEO
- Legal compliance in many regions

### Example

```html
<button>Submit</button>
```

Using a real button is more accessible than styling a generic `<div>` to behave like one.

### Interview Tip

Accessibility should be considered from the beginning of development, not added later.

---

# 69. Why is accessibility important?

### Answer

Accessibility ensures that websites can be used by as many people as possible.

### Advantages

- Supports users with disabilities
- Improves usability
- Better SEO
- Better keyboard navigation
- Better screen reader support
- Often required for legal compliance

### Example

Accessible image

```html
<img src="profile.jpg" alt="Profile photo of Swati" />
```

Poor example

```html
<img src="profile.jpg" />
```

### Interview Tip

Many accessibility best practices also improve SEO and overall user experience.

---

# 70. What is ARIA?

### Answer

ARIA stands for **Accessible Rich Internet Applications**.

ARIA provides additional information to assistive technologies when standard HTML semantics are not sufficient.

### Example

```html
<button aria-label="Close">✖</button>
```

Here, the screen reader announces:

```
Close button
```

instead of just reading the symbol "✖".

### Common ARIA Attributes

- `aria-label`
- `aria-labelledby`
- `aria-describedby`
- `aria-hidden`
- `aria-expanded`
- `aria-live`
- `role`

### Interview Tip

**Use semantic HTML first.** Add ARIA only when native HTML cannot provide the required accessibility information.

---

---

# 71. What are ARIA attributes?

### Answer

ARIA (Accessible Rich Internet Applications) attributes provide additional information to assistive technologies, such as screen readers, making web applications more accessible.

### Common ARIA Attributes

| Attribute          | Purpose                                            |
| ------------------ | -------------------------------------------------- |
| `aria-label`       | Provides a label when no visible label exists      |
| `aria-labelledby`  | References another element as the label            |
| `aria-describedby` | References another element as a description        |
| `aria-hidden`      | Hides an element from screen readers               |
| `aria-expanded`    | Indicates whether content is expanded or collapsed |
| `aria-live`        | Announces dynamic content updates                  |
| `aria-disabled`    | Indicates an element is disabled                   |
| `aria-current`     | Indicates the current item (page, step, etc.)      |

### Example

```html
<button aria-label="Close Menu">✖</button>
```

### Example

```html
<button aria-expanded="false">Menu</button>
```

### Interview Tip

Use ARIA only when native HTML elements cannot provide the required accessibility.

---

# 72. Difference between `alt` and `title`?

### Answer

Although both provide additional information, they serve different purposes.

### Comparison

| `alt`                            | `title`                                                       |
| -------------------------------- | ------------------------------------------------------------- |
| Used for images                  | Can be used on many elements                                  |
| Improves accessibility           | Provides additional information as a tooltip in many browsers |
| Read by screen readers           | Not a replacement for `alt`                                   |
| Displayed if image fails to load | Usually shown on hover                                        |

### Example

```html
<img src="logo.png" alt="OpenAI Logo" title="Company Logo" />
```

### Interview Tip

Never leave the `alt` attribute empty unless the image is purely decorative.

---

# 73. What makes a form accessible?

### Answer

An accessible form can be used easily by everyone, including people using screen readers or keyboard navigation.

### Best Practices

- Use `<label>` for every input
- Associate labels using `for` and `id`
- Use semantic HTML
- Show clear error messages
- Group related controls using `<fieldset>` and `<legend>`
- Ensure keyboard accessibility
- Use appropriate input types
- Don't rely only on placeholders

### Example

```html
<form>
  <fieldset>
    <legend>Login</legend>

    <label for="email"> Email </label>

    <input id="email" type="email" />
  </fieldset>
</form>
```

### Interview Tip

A placeholder should **never** replace a label.

---

# 74. Why should images have `alt` text?

### Answer

The `alt` attribute provides alternative text for images.

It is used when:

- The image cannot be loaded
- A screen reader reads the page
- The image is unavailable

### Example

```html
<img src="cat.jpg" alt="White cat sitting on a sofa" />
```

Poor Example

```html
<img src="cat.jpg" alt="image" />
```

### Benefits

- Better accessibility
- Better SEO
- Improved user experience

### Interview Tip

Write descriptive `alt` text that explains the image's purpose.

If the image is decorative, use:

```html
alt=""
```

---

# 75. How do semantic tags improve accessibility?

### Answer

Semantic HTML gives meaning to page content, allowing assistive technologies to understand the page structure.

### Example

Instead of

```html
<div class="navigation"></div>
```

Use

```html
<nav></nav>
```

Instead of

```html
<div class="footer"></div>
```

Use

```html
<footer></footer>
```

### Benefits

- Better screen reader navigation
- Better keyboard navigation
- Easier page understanding
- Improved SEO

### Interview Tip

Semantic HTML should always be your first choice before adding ARIA.

---

# 76. What is keyboard accessibility?

### Answer

Keyboard accessibility means users can navigate and interact with a website using only the keyboard.

Many users cannot use a mouse and rely on:

- Tab
- Shift + Tab
- Enter
- Space
- Arrow keys
- Escape

### Example

```html
<button>Save</button>
```

A native `<button>` is keyboard accessible by default.

### Bad Example

```html
<div onclick="save()">Save</div>
```

The `<div>` is not keyboard accessible without additional code.

### Interview Tip

Use native HTML elements whenever possible because they include built-in keyboard support.

---

# 77. What is `tabindex`?

### Answer

The `tabindex` attribute controls whether an element can receive keyboard focus and the order in which it receives focus when navigating with the Tab key.

### Common Values

| Value          | Meaning                                                                         |
| -------------- | ------------------------------------------------------------------------------- |
| `0`            | Element participates in the natural tab order                                   |
| `-1`           | Element can receive focus programmatically but is skipped during Tab navigation |
| Positive value | Sets a custom tab order (generally discouraged)                                 |

### Example

```html
<div tabindex="0">Focusable Div</div>
```

### Interview Tip

Avoid positive `tabindex` values. Use the natural tab order whenever possible.

---

# 78. What is the difference between `id` and `class`?

### Answer

Both `id` and `class` are global attributes used to identify HTML elements, but they are intended for different purposes.

### Comparison

| `id`                           | `class`                                                        |
| ------------------------------ | -------------------------------------------------------------- |
| Must be unique within a page   | Can be shared by multiple elements                             |
| Used for unique elements       | Used for grouping similar elements                             |
| Selected with `#` in CSS       | Selected with `.` in CSS                                       |
| Accessed by `getElementById()` | Accessed by `getElementsByClassName()` or `querySelectorAll()` |

### Example

```html
<h1 id="title">Welcome</h1>

<p class="text">Paragraph 1</p>

<p class="text">Paragraph 2</p>
```

### Interview Tip

Use `id` for unique elements and `class` for reusable styles.

---

# 79. Can multiple elements have the same `id`?

### Answer

**No.**

According to HTML standards, an `id` value should be unique within a document.

### Incorrect

```html
<div id="box"></div>

<div id="box"></div>
```

### Correct

```html
<div id="box1"></div>

<div id="box2"></div>
```

Or use a class if multiple elements share the same styling.

```html
<div class="box"></div>

<div class="box"></div>
```

### Why It Matters

Duplicate IDs can cause:

- CSS conflicts
- JavaScript selecting the wrong element
- Accessibility issues

### Interview Tip

If multiple elements need the same style or behavior, use a `class`, not an `id`.

---

# 80. What is the `data-*` attribute?

### Answer

The `data-*` attribute allows you to store custom data on HTML elements without using non-standard attributes.

These attributes are intended for use by JavaScript.

### Syntax

```html
<div data-user-id="101" data-role="admin"></div>
```

### Access in JavaScript

```javascript
const element = document.querySelector("div");

console.log(element.dataset.userId);

console.log(element.dataset.role);
```

### Common Uses

- Store IDs
- Product information
- User roles
- Status values
- Configuration settings

### Interview Tip

Avoid storing sensitive information in `data-*` attributes because users can view them in the browser's developer tools.

---

---

# 81. What are custom data attributes used for?

### Answer

Custom data attributes (`data-*`) are used to store extra information directly inside HTML elements.

They allow developers to attach custom data that can later be accessed using JavaScript.

### Example

```html
<button data-product-id="101" data-price="499">Buy Now</button>
```

Access using JavaScript:

```javascript
const button = document.querySelector("button");

console.log(button.dataset.productId);
console.log(button.dataset.price);
```

### Common Uses

- Storing product IDs
- Storing user information
- Passing data between HTML and JavaScript
- Adding configuration values
- Handling UI interactions

### Interview Tip

`data-*` attributes are for non-sensitive client-side data only.

---

# 82. What is the difference between `defer` and `async`?

### Answer

Both `defer` and `async` are attributes used with the `<script>` tag to control JavaScript loading behavior.

### Normal Script

```html
<script src="app.js"></script>
```

The browser:

1. Stops HTML parsing
2. Downloads JavaScript
3. Executes JavaScript
4. Continues parsing HTML

---

# async

The script downloads while HTML parsing continues.

Execution happens immediately after download.

```html
<script src="app.js" async></script>
```

### Behavior

```
HTML Parsing
     |
     |---- Download Script
     |
     |---- Execute Script
     |
Continue HTML Parsing
```

### Use Cases

- Analytics scripts
- Ads
- Independent scripts

---

# defer

The script downloads while HTML parsing continues but executes after HTML parsing is complete.

```html
<script src="app.js" defer></script>
```

### Behavior

```
HTML Parsing
     |
     |---- Download Script
     |
HTML Completed
     |
Execute Script
```

### Comparison

| async                          | defer                             |
| ------------------------------ | --------------------------------- |
| Executes as soon as downloaded | Executes after HTML parsing       |
| Order is not guaranteed        | Maintains script order            |
| Good for independent scripts   | Good for main application scripts |

### Interview Tip

For most frontend applications, `defer` is preferred for external scripts that depend on the DOM.

---

# 83. What happens when HTML is parsed?

### Answer

HTML parsing is the process where the browser converts HTML code into the DOM (Document Object Model).

### Process

1. Browser receives HTML
2. HTML parser reads the document
3. Browser creates DOM tree
4. CSS is loaded and CSSOM is created
5. DOM + CSSOM create the Render Tree
6. Browser paints the page

### Example

HTML:

```html
<h1>Hello</h1>
```

DOM representation:

```
Document
   |
 html
   |
 body
   |
 h1
   |
 Hello
```

### Interview Tip

JavaScript can block HTML parsing if it is loaded without `async` or `defer`.

---

# 84. What is DOM?

### Answer

DOM stands for **Document Object Model**.

It is a programming interface that represents an HTML document as a tree of objects.

JavaScript uses the DOM to:

- Read HTML
- Modify content
- Change styles
- Add or remove elements
- Handle events

### Example HTML

```html
<h1 id="title">Hello</h1>
```

JavaScript:

```javascript
document.getElementById("title").innerHTML = "Welcome";
```

### DOM Tree

```
Document
 |
 html
 |
 body
 |
 h1
 |
 Hello
```

### Interview Tip

DOM is not HTML itself. It is the browser's object representation of HTML.

---

# 85. What is BOM?

### Answer

BOM stands for **Browser Object Model**.

It allows JavaScript to interact with the browser window and browser features.

### Common BOM Objects

- window
- navigator
- location
- history
- screen

### Example

Get browser size:

```javascript
console.log(window.innerWidth);
```

Change URL:

```javascript
window.location.href = "https://google.com";
```

Go back:

```javascript
window.history.back();
```

### Interview Tip

DOM works with the webpage.

BOM works with the browser.

---

# 86. Difference between DOM and HTML?

### Answer

HTML is the markup language used to create a webpage.

DOM is the browser-created object model of that HTML.

### Comparison

| HTML                          | DOM                              |
| ----------------------------- | -------------------------------- |
| Source code                   | Browser representation           |
| Static document               | Dynamic object structure         |
| Written by developers         | Created by browser               |
| Cannot directly change itself | Can be modified using JavaScript |

### Example

HTML:

```html
<p>Hello</p>
```

JavaScript changes DOM:

```javascript
document.querySelector("p").textContent = "Welcome";
```

Updated page:

```html
<p>Welcome</p>
```

### Interview Tip

When JavaScript changes a webpage, it modifies the DOM, not the original HTML file.

---

# 87. What is Progressive Enhancement?

### Answer

Progressive Enhancement is a development approach where you first build a basic working website, then add advanced features for modern browsers.

### Layers

1. Basic HTML → Content works everywhere
2. CSS → Better design
3. JavaScript → Advanced interactions

### Example

Basic:

```html
<form>
  <input type="email" />
  <button>Submit</button>
</form>
```

Enhanced:

```javascript
// Client-side validation
```

### Benefits

- Works on all devices
- Better accessibility
- Better reliability
- Improved user experience

### Interview Tip

HTML is the foundation of progressive enhancement.

---

# 88. What is Graceful Degradation?

### Answer

Graceful Degradation means building a fully-featured website first and ensuring it still works when advanced features are unavailable.

### Example

Modern browser:

```
Animation + JavaScript + CSS
```

Older browser:

```
Basic functionality still works
```

### Comparison

| Progressive Enhancement     | Graceful Degradation            |
| --------------------------- | ------------------------------- |
| Start simple, add features  | Start advanced, remove features |
| Mobile-first approach       | Desktop-first approach          |
| Focus on core functionality | Focus on fallback               |

### Interview Tip

Modern web development usually prefers progressive enhancement.

---

# 89. What are data attributes?

### Answer

Data attributes are custom HTML attributes that start with `data-`.

They allow developers to store extra information inside HTML elements.

### Syntax

```html
<div data-id="123">Product</div>
```

### Access using JavaScript

```javascript
const product = document.querySelector("div");

console.log(product.dataset.id);
```

### Naming Rules

HTML:

```html
data-user-name="Swati"
```

JavaScript:

```javascript
element.dataset.userName;
```

### Interview Tip

Data attributes are automatically available through the `dataset` property.

---

# 90. What are void elements?

### Answer

Void elements are HTML elements that do not have closing tags.

They cannot contain child elements.

### Examples

```html
<img />

<br />

<hr />

<input />

<meta />

<link />
```

### Example

```html
<img src="logo.png" alt="Logo" />
```

Correct:

```html
<img src="image.jpg" />
```

Incorrect:

```html
<img>
</img>
```

### Interview Tip

HTML5 does not require a `/` at the end.

Both:

```html
<img />
```

and

```html
<img />
```

are accepted, but HTML style usually uses the first form.

---

---

# 91. Why would you choose `<button>` instead of `<a>`?

### Answer

`<button>` and `<a>` have different purposes.

Use:

- `<button>` for actions
- `<a>` for navigation

### Use `<button>` when:

- Submitting a form
- Opening a modal
- Triggering JavaScript actions
- Changing UI state

Example:

```html
<button onclick="openModal()">Open Profile</button>
```

---

### Use `<a>` when:

- Navigating to another page
- Opening a URL
- Downloading a file

Example:

```html
<a href="/profile"> View Profile </a>
```

### Comparison

| Button                  | Anchor              |
| ----------------------- | ------------------- |
| Performs an action      | Navigates somewhere |
| Uses click events       | Uses URLs           |
| Used for UI interaction | Used for links      |

### Interview Tip

Do not use `<div>` or `<span>` as a replacement for buttons.

---

# 92. Why shouldn't you use `<div>` for everything?

### Answer

`<div>` is a generic container and has no semantic meaning.

Using only `<div>` makes the structure harder for:

- Search engines
- Screen readers
- Developers

### Bad Example

```html
<div>Header</div>

<div>Navigation</div>

<div>Main Content</div>

<div>Footer</div>
```

### Better Example

```html
<header>Header</header>

<nav>Navigation</nav>

<main>Main Content</main>

<footer>Footer</footer>
```

### Benefits of Semantic Tags

- Better accessibility
- Better SEO
- Cleaner code
- Easier maintenance

### Interview Tip

Use `<div>` only when no semantic element is suitable.

---

# 93. How do you build an accessible form?

### Answer

An accessible form should be usable by all users, including users who use screen readers or keyboard navigation.

### Best Practices

## 1. Use Labels

```html
<label for="email"> Email </label>

<input id="email" type="email" />
```

---

## 2. Use Proper Input Types

```html
<input type="email" />

<input type="tel" />

<input type="date" />
```

---

## 3. Use Required Attributes

```html
<input type="password" required />
```

---

## 4. Provide Error Messages

Example:

```html
<p role="alert">Invalid email address</p>
```

---

## 5. Support Keyboard Navigation

Avoid clickable elements like:

```html
<div onclick="submitForm()">Submit</div>
```

Use:

```html
<button>Submit</button>
```

### Interview Tip

A good form should work without a mouse.

---

# 94. How would you optimize HTML for SEO?

### Answer

HTML optimization helps search engines understand and index content correctly.

### Techniques

### 1. Use Semantic HTML

```html
<header>
  <nav>
    <main>
      <article>
        <footer></footer>
      </article>
    </main>
  </nav>
</header>
```

---

### 2. Use Proper Heading Structure

```html
<h1>Main Topic</h1>

<h2>Section</h2>

<h3>Subsection</h3>
```

---

### 3. Add Meta Information

```html
<meta name="description" content="Frontend interview preparation" />
```

---

### 4. Optimize Images

```html
<img src="html.png" alt="HTML Logo" />
```

---

### 5. Use Meaningful Links

Good:

```html
<a href="/react-hooks"> React Hooks Guide </a>
```

Bad:

```html
<a href="/react-hooks"> Click Here </a>
```

---

### 6. Improve Performance

- Minimize unnecessary HTML
- Optimize images
- Use lazy loading

Example:

```html
<img src="image.jpg" loading="lazy" />
```

### Interview Tip

SEO starts with good HTML structure.

---

# 95. How do you create a responsive image?

### Answer

Responsive images adjust according to different screen sizes and device resolutions.

### Method 1: Using `srcset`

```html
<img
  src="small.jpg"
  srcset="small.jpg 480w, medium.jpg 768w, large.jpg 1200w"
  alt="Mountain"
/>
```

The browser chooses the best image.

---

### Method 2: Using `<picture>`

```html
<picture>
  <source media="(min-width:768px)" srcset="desktop.jpg" />

  <img src="mobile.jpg" alt="Mountain" />
</picture>
```

### Method 3: CSS

```css
img {
  max-width: 100%;
  height: auto;
}
```

### Benefits

- Faster loading
- Better mobile experience
- Saves bandwidth

### Interview Tip

Use `srcset` and `<picture>` for performance optimization.

---

# 96. How would you embed another website?

### Answer

Use the `<iframe>` element.

### Example

```html
<iframe src="https://example.com" width="600" height="400" title="Example">
</iframe>
```

### Common Uses

- YouTube videos
- Google Maps
- Payment widgets
- External tools

### Security Considerations

- Avoid untrusted websites
- Use sandbox when needed

Example:

```html
<iframe src="page.html" sandbox> </iframe>
```

### Interview Tip

Always provide a `title` attribute for accessibility.

---

# 97. How would you improve page loading?

### Answer

HTML can be optimized to improve website performance.

### Techniques

## 1. Use Lazy Loading

Images:

```html
<img src="image.jpg" loading="lazy" />
```

---

## 2. Optimize Images

- Compress images
- Use modern formats like WebP
- Use responsive images

---

## 3. Load Scripts Properly

Use:

```html
<script src="app.js" defer></script>
```

---

## 4. Use Proper HTML Structure

Avoid unnecessary nested elements.

---

## 5. Preload Important Resources

Example:

```html
<link rel="preload" href="style.css" as="style" />
```

### Interview Tip

Performance improvements should reduce unnecessary browser work.

---

# 98. How would you structure a blog page semantically?

### Answer

A blog page should use semantic HTML elements to describe its structure.

### Example

```html
<header>
  <h1>My Blog</h1>
</header>

<nav>Navigation Links</nav>

<main>
  <article>
    <header>
      <h2>HTML Interview Questions</h2>
    </header>

    <section>Blog Content</section>

    <footer>Author Information</footer>
  </article>
</main>

<aside>Related Posts</aside>

<footer>Copyright</footer>
```

### Structure

- Header → Website title
- Nav → Navigation
- Main → Main content
- Article → Blog post
- Aside → Related information
- Footer → Additional details

### Interview Tip

Semantic structure improves accessibility and SEO.

---

# 99. What are common HTML interview mistakes?

### Answer

Common mistakes developers make:

### 1. Using `<div>` everywhere

Instead of:

```html
<div>Navigation</div>
```

Use:

```html
<nav>Navigation</nav>
```

---

### 2. Missing `alt` attributes

Wrong:

```html
<img src="logo.png" />
```

Correct:

```html
<img src="logo.png" alt="Company Logo" />
```

---

### 3. Incorrect heading order

Wrong:

```html
<h1>
  <h4>
    <h2></h2>
  </h4>
</h1>
```

Correct:

```html
<h1>
  <h2>
    <h3></h3>
  </h2>
</h1>
```

---

### 4. Using placeholders instead of labels

Wrong:

```html
<input placeholder="Email" />
```

Better:

```html
<label>Email</label> <input />
```

---

### 5. Not closing elements properly

Example:

```html
<p>Hello</p>
```

Correct:

```html
<p>Hello</p>
```

---

### Interview Tip

Good HTML is semantic, accessible, and maintainable.

---

# 100. Top HTML interview tips

### Answer

To prepare for HTML interviews:

## 1. Understand Semantic HTML

Know:

- header
- nav
- main
- article
- section
- footer

---

## 2. Master Forms

Understand:

- input types
- validation
- GET vs POST
- accessibility

---

## 3. Learn Browser Concepts

Know:

- DOM
- BOM
- HTML parsing
- rendering process

---

## 4. Focus on Accessibility

Understand:

- ARIA
- labels
- keyboard navigation
- semantic tags

---

## 5. Practice Writing HTML

Build:

- Forms
- Landing pages
- Blog layouts
- Portfolio pages

---

## 6. Know SEO Basics

Understand:

- Meta tags
- Heading structure
- Alt text
- Semantic markup

---

## Final Interview Checklist

✅ Semantic HTML  
✅ Forms  
✅ Accessibility  
✅ SEO  
✅ Browser rendering  
✅ Storage APIs  
✅ Responsive images  
✅ DOM basics

### Interview Tip

A frontend developer is expected to write HTML that is:

- Meaningful
- Accessible
- SEO-friendly
- Easy to maintain

---
