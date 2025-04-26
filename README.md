# HTML Interview Questions

A curated list of HTML interview questions and answers.

**Note:** This repository is continuously updated with new questions and answers.

<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/1200px-HTML5_logo_and_wordmark.svg.png" alt="HTML5 Logo" width="200">
</div>

## Table of Contents

| No. | Questions                                                                                                                                              |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1   | [What is HTML and what does it stand for?](#1-what-is-html-and-what-does-it-stand-for)                                                                 |
| 2   | [What are the new features in HTML5?](#2-what-are-the-new-features-in-html5)                                                                           |
| 3   | [What is the difference between HTML elements and tags?](#3-what-is-the-difference-between-html-elements-and-tags)                                     |
| 4   | [What is semantic HTML and why is it important?](#4-what-is-semantic-html-and-why-is-it-important)                                                     |
| 5   | [Explain the difference between block and inline elements](#5-explain-the-difference-between-block-and-inline-elements)                                |
| 6   | [What is the purpose of the DOCTYPE declaration?](#6-what-is-the-purpose-of-the-doctype-declaration)                                                   |
| 7   | [What are void elements in HTML?](#7-what-are-void-elements-in-html)                                                                                   |
| 8   | [Explain the importance of the alt attribute for images](#8-explain-the-importance-of-the-alt-attribute-for-images)                                    |
| 9   | [What is the difference between localStorage, sessionStorage, and cookies?](#9-what-is-the-difference-between-localstorage-sessionstorage-and-cookies) |
| 10  | [How do you embed audio and video in a webpage?](#10-how-do-you-embed-audio-and-video-in-a-webpage)                                                    |
| 11  | [Explain the Canvas element and its use cases](#11-explain-the-canvas-element-and-its-use-cases)                                                       |
| 12  | [What are data attributes and how are they useful?](#12-what-are-data-attributes-and-how-are-they-useful)                                              |
| 13  | [What is the purpose of the srcset attribute in images?](#13-what-is-the-purpose-of-the-srcset-attribute-in-images)                                    |
| 14  | [Explain the difference between SVG and Canvas](#14-explain-the-difference-between-svg-and-canvas)                                                     |
| 15  | [What are Web Components?](#15-what-are-web-components)                                                                                                |

## 1. What is HTML and what does it stand for?

HTML stands for **HyperText Markup Language**. It is the standard markup language used to create and structure content on the web. HTML describes the structure of web pages using markup.

HTML elements are represented by tags, which label pieces of content such as "heading", "paragraph", "table", etc.

**Key Points:**

- HTML is not a programming language; it's a markup language
- HTML documents are described by HTML tags
- HTML tags label pieces of content such as "heading", "paragraph", "table", etc.
- Browsers do not display the HTML tags, but use them to render the content of the page

**Example:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Basic HTML Document</title>
  </head>
  <body>
    <header>
      <h1>This is a Heading</h1>
    </header>

    <main>
      <p>This is a paragraph.</p>

      <section>
        <h2>This is a sub-heading</h2>
        <p>
          This is another paragraph with a
          <a href="https://example.com">link</a>.
        </p>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 Example Company</p>
    </footer>
  </body>
</html>
```

HTML was first created by Tim Berners-Lee in 1990. Since then, there have been many versions of HTML. The most recent version is HTML5, which introduced many new semantic elements and APIs.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 2. What are the new features in HTML5?

HTML5 is the latest version of HTML that introduced many new features, APIs, and improvements to make web applications more capable and improve the overall web development experience.

**Key Features:**

1. **Semantic Elements:**

   - `<header>` - Defines a header for a document or a section
   - `<nav>` - Defines navigation links
   - `<section>` - Defines a section in a document
   - `<article>` - Defines an independent, self-contained content
   - `<aside>` - Defines content aside from the content (like a sidebar)
   - `<footer>` - Defines a footer for a document or a section
   - `<figure>` and `<figcaption>` - For illustrations, diagrams, photos, code listings, etc.
   - `<main>` - Specifies the main content of a document

2. **Multimedia Support:**

   - `<audio>` - Embeds sound content
   - `<video>` - Embeds video content
   - `<source>` - Defines multiple media resources for media elements

3. **Graphics:**

   - `<canvas>` - Used to draw graphics via JavaScript
   - Native SVG support - Scalable Vector Graphics can be directly embedded in HTML

4. **Form Enhancements:**

   - New input types: email, url, number, range, date, time, color, etc.
   - New attributes: required, pattern, placeholder, autocomplete, autofocus, etc.

5. **API and JavaScript Enhancements:**
   - localStorage and sessionStorage - For client-side data storage
   - Web Workers - For background processing
   - Geolocation API - For location-aware web applications
   - Drag and Drop API - For drag and drop functionality
   - WebSockets - For real-time communication
   - Server-Sent Events - For one-way server updates
   - History API - For manipulating browser history

**Example:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML5 Features Example</title>
  </head>
  <body>
    <!-- Semantic Structure -->
    <header>
      <h1>Website Title</h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section>
        <h2>HTML5 Video Example</h2>
        <video controls width="400">
          <source src="video.mp4" type="video/mp4" />
          <source src="video.webm" type="video/webm" />
          Your browser does not support the video tag.
        </video>
      </section>

      <section>
        <h2>HTML5 Canvas Example</h2>
        <canvas
          id="myCanvas"
          width="200"
          height="100"
          style="border:1px solid #000;"
        >
          Your browser does not support the canvas element.
        </canvas>
      </section>

      <section>
        <h2>HTML5 Form Elements</h2>
        <form>
          <label for="email">Email:</label>
          <input type="email" id="email" required />

          <label for="date">Date:</label>
          <input type="date" id="date" />

          <label for="range">Range:</label>
          <input type="range" id="range" min="0" max="10" />

          <button type="submit">Submit</button>
        </form>
      </section>
    </main>

    <footer>
      <p>&copy; 2025 Example Company</p>
    </footer>

    <script>
      // Canvas API example
      const canvas = document.getElementById("myCanvas");
      const ctx = canvas.getContext("2d");
      ctx.fillStyle = "#3498db";
      ctx.fillRect(10, 10, 150, 80);

      // LocalStorage example
      localStorage.setItem("username", "visitor");
    </script>
  </body>
</html>
```

**Why HTML5 is Important:**

- Better semantics for improved accessibility and SEO
- Reduced dependency on plugins like Flash
- Native support for rich media content
- Enhanced form validation and user experience
- Better mobile support
- Offline web application capabilities

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 3. What is the difference between HTML elements and tags?

**HTML Elements** and **HTML Tags** are related concepts but have distinct meanings:

**HTML Elements:**

- An HTML element represents the complete structure from opening tag to closing tag, including the content in between
- It consists of an opening tag, content, and usually a closing tag
- Elements define the structure and content of objects within a page
- Example: `<p>This is a paragraph.</p>` - The entire structure is the paragraph element

**HTML Tags:**

- Tags are the markup characters that define the beginning and end of an HTML element
- They are enclosed in angle brackets `< >`
- Opening tags mark the beginning of an element: `<p>`
- Closing tags mark the end and include a forward slash: `</p>`
- Some tags are self-closing (void elements) and don't have a separate closing tag: `<img>`

**Visualization:**

```
<p>This is a paragraph.</p>
↑            ↑          ↑
Opening      Content    Closing
Tag                     Tag
          Element
```

**Example:**

```html
<a href="https://example.com">Visit Example</a>
```

In this example:

- The tags are `<a href="https://example.com">` and `</a>`
- The element is everything: `<a href="https://example.com">Visit Example</a>`
- "Visit Example" is the content
- "href" is an attribute that provides additional information about the element

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 4. What is semantic HTML and why is it important?

**Semantic HTML** refers to the use of HTML markup that conveys the meaning or purpose of the content, rather than just defining its appearance. Semantic elements clearly describe their meaning to both the browser and the developer.

**Examples of semantic elements:**

- `<header>` - Defines a header for a document or section
- `<nav>` - Defines navigation links
- `<main>` - Specifies the main content of a document
- `<article>` - Defines independent, self-contained content
- `<section>` - Defines a section in a document
- `<aside>` - Defines content aside from the main content
- `<footer>` - Defines a footer for a document or section
- `<figure>` and `<figcaption>` - Specifies self-contained content like illustrations, diagrams, photos, etc.

**Non-semantic elements** provide no indication about their content:

- `<div>` - Defines a division or a section
- `<span>` - Used to group inline elements

**Example of non-semantic vs semantic HTML:**

Non-semantic approach:

```html
<div class="header">
  <h1>Website Title</h1>
  <div class="navigation">
    <div class="nav-item"><a href="#home">Home</a></div>
    <div class="nav-item"><a href="#about">About</a></div>
  </div>
</div>
<div class="main-content">
  <div class="article">
    <h2>Article Title</h2>
    <div class="article-content">
      <p>This is an article paragraph.</p>
    </div>
  </div>
</div>
<div class="footer">
  <p>Copyright 2025</p>
</div>
```

Semantic approach:

```html
<header>
  <h1>Website Title</h1>
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
    </ul>
  </nav>
</header>
<main>
  <article>
    <h2>Article Title</h2>
    <p>This is an article paragraph.</p>
  </article>
</main>
<footer>
  <p>Copyright 2025</p>
</footer>
```

**Why Semantic HTML is Important:**

1. **Accessibility**: Screen readers and assistive technologies can better interpret semantic HTML, making websites more accessible to people with disabilities.

2. **SEO**: Search engines better understand the content and context of web pages with semantic markup, potentially improving rankings.

3. **Code Maintainability**: Makes the HTML more readable and easier to maintain, both for the original developer and others.

4. **Consistency**: Provides a consistent structure across websites, making them more predictable for users.

5. **Device Compatibility**: Helps ensure content is correctly displayed across different devices and platforms.

6. **Future-Proofing**: As web technologies evolve, semantic markup is more likely to remain compatible with new standards and browsers.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 5. Explain the difference between block and inline elements

**Block Elements** and **Inline Elements** are two categories of HTML elements that behave differently in terms of display and layout.

### Block Elements

Block-level elements:

- Start on a new line
- Take up the full width available by default
- Create a "block" in the flow of the document
- Can contain other block elements and inline elements
- Height, width, margin, and padding properties can be fully applied

**Common block elements:**

- `<div>`
- `<h1>` to `<h6>`
- `<p>`
- `<section>`
- `<article>`
- `<header>`
- `<footer>`
- `<form>`
- `<ul>`, `<ol>`, `<li>`
- `<table>`
- `<blockquote>`

### Inline Elements

Inline elements:

- Do not start on a new line
- Take only as much width as necessary
- Flow with the surrounding content
- Cannot contain block-level elements
- Height and width properties have no effect
- Vertical margins and paddings have no effect, horizontal ones do

**Common inline elements:**

- `<span>`
- `<a>`
- `<strong>`, `<b>`
- `<em>`, `<i>`
- `<code>`
- `<img>`
- `<input>`
- `<label>`
- `<small>`
- `<br>`

### Inline-Block Elements

There is also a third display type called **inline-block**, which is a hybrid:

- Does not start on a new line (like inline)
- Can have width and height (like block)
- Respects top/bottom margins and paddings (like block)
- Does not force a new line (like inline)

Elements that are typically inline-block:

- `<button>`
- `<input>`
- `<select>`

### Example:

```html
<!-- Block elements example -->
<div style="border: 1px solid red;">
  This div takes up the full width available
</div>
<p style="border: 1px solid blue;">
  This paragraph also takes up the full width available
</p>

<!-- Inline elements example -->
<span style="border: 1px solid green;">This span</span>
<a href="#" style="border: 1px solid purple;">and this link</a>
are inline elements that flow with the text and only take up the width they
need.

<!-- Changing display behavior -->
<div style="display: inline; border: 1px solid orange;">
  This div is displayed inline
</div>
<span style="display: block; border: 1px solid pink;">
  This span is displayed as a block
</span>
```

### Visual Representation:

```
+-----------------------------------------------+
| Block Element                                 |
+-----------------------------------------------+

+-----------------------------------------------+
| Another Block Element                         |
+-----------------------------------------------+

[Inline Element] [Another Inline Element] more text...
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 6. What is the purpose of the DOCTYPE declaration?

The **DOCTYPE declaration** (Document Type Declaration) is an instruction to the web browser about what version of HTML the page is written in. It must be the very first thing in an HTML document, before the `<html>` tag.

### Purpose of DOCTYPE:

1. **Browser Rendering Mode:**

   - Ensures that the browser renders the page in standards mode rather than quirks mode
   - Standards mode follows W3C and WHATWG specifications
   - Quirks mode emulates behavior of older browsers for backward compatibility

2. **Validation:**

   - Allows validators to check the HTML document against the specified HTML version
   - Helps ensure compliance with web standards

3. **Browser Compatibility:**
   - Helps browsers interpret and render the page correctly
   - Different DOCTYPEs trigger different rendering behaviors

### HTML5 DOCTYPE:

```html
<!DOCTYPE html>
```

The HTML5 DOCTYPE is simple and easy to remember. It's case-insensitive but is typically written in lowercase or uppercase.

### Older HTML DOCTYPEs:

**HTML 4.01 Strict:**

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

**HTML 4.01 Transitional:**

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

**XHTML 1.0 Strict:**

```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```

### What happens without a DOCTYPE?

Without a DOCTYPE declaration:

- Browsers will operate in "quirks mode"
- Rendering may be inconsistent across different browsers
- Modern features may not work as expected
- CSS may behave unpredictably
- Validation tools can't effectively check the document

### Example of a Basic HTML5 Document with DOCTYPE:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sample Document</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>This is a properly formatted HTML5 document with DOCTYPE.</p>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 7. What are void elements in HTML?

**Void elements** (also called empty elements or self-closing elements) are HTML elements that cannot have any content inside them and therefore do not have a closing tag. They are "self-closing" by nature.

### Key Characteristics:

- Cannot contain any content
- Do not have a closing tag
- Can have attributes
- Are self-closing
- In HTML5, the trailing slash is optional (e.g., `<img>` or `<img />`)
- In XHTML, the trailing slash is required (e.g., `<img />`)

### Common Void Elements:

- `<img>` - Embeds an image
- `<input>` - Creates an input control
- `<br>` - Line break
- `<hr>` - Horizontal rule (thematic break)
- `<link>` - Links to external resources like CSS
- `<meta>` - Metadata about the document
- `<source>` - Specifies media sources for `<video>` and `<audio>`
- `<area>` - Defines an area inside an image map
- `<base>` - Specifies a base URL for all relative URLs
- `<col>` - Specifies column properties for tables
- `<embed>` - Embeds external content
- `<param>` - Defines parameters for plugins
- `<track>` - Specifies text tracks for media elements
- `<wbr>` - Word break opportunity

### Examples:

```html
<!-- Correct usage of void elements -->
<img src="image.jpg" alt="An example image">
<input type="text" name="username">
<br>
<hr>
<link rel="stylesheet" href="styles.css">
<meta charset="UTF-8">

<!-- Invalid usage (void elements should not have closing tags) -->
<img src="image.jpg" alt="An example image"></img>  <!-- Incorrect -->
<br></br>  <!-- Incorrect -->

<!-- In XHTML, void elements need a trailing slash -->
<img src="image.jpg" alt="An example image" />
<input type="text" name="username" />
<br />
```

### Why This Matters:

1. **Syntax Correctness**: Understanding void elements helps write valid HTML.
2. **Parsing Efficiency**: Browsers can parse HTML more efficiently when it's correctly written.
3. **Cross-Compatibility**: Important for writing HTML that works across all contexts (HTML, XHTML, XML).
4. **Error Prevention**: Prevents unexpected rendering issues that could occur from improperly nested elements.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 8. Explain the importance of the alt attribute for images

The `alt` attribute provides alternative text for an image if the image cannot be displayed or viewed. It is added to the `<img>` tag:

```html
<img src="example.jpg" alt="Description of the image" />
```

### Importance of the alt Attribute:

#### 1. Accessibility

- **Screen Readers**: Enables screen readers to describe images to visually impaired users
- **Text-to-Speech**: Provides content for text-to-speech software to read aloud
- **WCAG Compliance**: Required for Web Content Accessibility Guidelines (WCAG) compliance

#### 2. User Experience

- **Broken Images**: Displays when images fail to load due to network issues, broken links, etc.
- **Slow Connections**: Provides context while images are loading on slow connections
- **Text-Only Browsers**: Some users browse with images turned off or use text-only browsers

#### 3. SEO Benefits

- **Image Search**: Helps search engines understand and index images
- **Context**: Provides additional contextual information about page content
- **Ranking Signals**: Search engines use alt text as a ranking factor

#### 4. Technical Requirements

- **HTML Validation**: Required for valid HTML according to W3C specifications
- **Error Prevention**: Reduces errors in automated testing and validation

### Best Practices for alt Text:

1. **Be Descriptive**: Clearly describe the image content and purpose
2. **Keep It Concise**: Typically 125 characters or less
3. **Context Matters**: Consider the image's role in the surrounding content
4. **Avoid Redundancy**: Don't begin with "picture of" or "image of"
5. **Decorative Images**: Use empty alt text (`alt=""`) for purely decorative images
6. **Functional Images**: Describe the function for images that serve as buttons or links

### Examples:

**Good alt text examples:**

```html
<!-- Informative image -->
<img
  src="chart-sales-2025.png"
  alt="Bar chart showing sales growth of 25% in Q3 2025"
/>

<!-- Image used as a link -->
<a href="home.html">
  <img src="home-icon.png" alt="Home page" />
</a>

<!-- Decorative image -->
<img src="decorative-divider.png" alt="" />
```

**Poor alt text examples:**

```html
<!-- Too vague -->
<img src="graph.png" alt="Graph" />

<!-- Redundant -->
<img src="team.jpg" alt="Image of team members" />

<!-- Keyword stuffing -->
<img
  src="laptop.jpg"
  alt="laptop buy cheap laptop best laptop deals laptop sale"
/>
```

### Testing alt Text:

You can test your alt text by:

- Using a screen reader
- Disabling images in your browser
- Intentionally breaking the image URL
- Using accessibility validation tools

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 9. What is the difference between localStorage, sessionStorage, and cookies?

localStorage, sessionStorage, and cookies are all mechanisms for storing data on the client-side, but they differ in several key aspects:

### Storage Capacity:

- **localStorage**: ~5-10MB (varies by browser)
- **sessionStorage**: ~5-10MB (varies by browser)
- **Cookies**: ~4KB per cookie, typically limited to ~50 cookies per domain

### Lifespan/Persistence:

- **localStorage**: Persists until explicitly deleted by code or user clearing browser data
- **sessionStorage**: Persists for the duration of the page session (until the browser/tab is closed)
- **Cookies**: Can be configured with an expiration date/time (via `expires` or `max-age` attribute)

### Accessibility/Scope:

- **localStorage**: Available across all tabs/windows from the same origin
- **sessionStorage**: Limited to the tab/window that created it
- **Cookies**: Available across all tabs/windows from the same origin (can be restricted with the `path` and `domain` attributes)

### Sent with Requests:

- **localStorage**: Never sent to the server
- **sessionStorage**: Never sent to the server
- **Cookies**: Automatically sent to the server with every HTTP request to the same domain (unless `HttpOnly` flag is set)

### API/Usage:

**localStorage and sessionStorage:**

```javascript
// Storing data
localStorage.setItem("key", "value");
sessionStorage.setItem("key", "value");

// Retrieving data
const value = localStorage.getItem("key");
const value = sessionStorage.getItem("key");

// Removing data
localStorage.removeItem("key");
sessionStorage.removeItem("key");

// Clearing all data
localStorage.clear();
sessionStorage.clear();
```

**Cookies:**

```javascript
// Storing a cookie
document.cookie =
  "username=John; expires=Thu, 18 Dec 2025 12:00:00 UTC; path=/";

// Reading cookies
const allCookies = document.cookie; // Returns all cookies as a string

// Deleting a cookie (set it with a past expiration date)
document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
```

### Security:

- **localStorage & sessionStorage**:

  - Not accessible via cross-origin requests
  - Can be accessed by any JavaScript code on the same origin
  - Not encrypted by default

- **Cookies**:
  - Can be made secure with flags:
    - `Secure`: Only sent over HTTPS
    - `HttpOnly`: Inaccessible to JavaScript
    - `SameSite`: Controls cross-origin sending
  - Still vulnerable to XSS attacks unless `HttpOnly` flag is set

### Best Use Cases:

- **localStorage**:

  - User preferences that persist across sessions
  - Non-sensitive application state
  - Cached data for offline applications

- **sessionStorage**:

  - Form data during a single session
  - Temporary state within a single page visit
  - Per-tab temporary data storage

- **Cookies**:
  - Authentication tokens/sessions (when properly secured)
  - User tracking
  - Server-side preferences
  - When data needs to be accessed by both client and server

### Example Implementation:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Storage Examples</title>
  </head>
  <body>
    <h1>Browser Storage Examples</h1>

    <h2>localStorage</h2>
    <button onclick="setLocalStorage()">Save to localStorage</button>
    <button onclick="getLocalStorage()">Get from localStorage</button>
    <div id="localStorage-output"></div>

    <h2>sessionStorage</h2>
    <button onclick="setSessionStorage()">Save to sessionStorage</button>
    <button onclick="getSessionStorage()">Get from sessionStorage</button>
    <div id="sessionStorage-output"></div>

    <h2>Cookies</h2>
    <button onclick="setCookie()">Save Cookie</button>
    <button onclick="getCookie()">Get Cookie</button>
    <div id="cookie-output"></div>

    <script>
      // localStorage functions
      function setLocalStorage() {
        localStorage.setItem(
          "testData",
          "This data persists across browser sessions - " +
            new Date().toLocaleString()
        );
        alert("Data saved to localStorage");
      }

      function getLocalStorage() {
        const data = localStorage.getItem("testData") || "No data found";
        document.getElementById("localStorage-output").textContent = data;
      }

      // sessionStorage functions
      function setSessionStorage() {
        sessionStorage.setItem(
          "testData",
          "This data persists only for this tab session - " +
            new Date().toLocaleString()
        );
        alert("Data saved to sessionStorage");
      }

      function getSessionStorage() {
        const data = sessionStorage.getItem("testData") || "No data found";
        document.getElementById("sessionStorage-output").textContent = data;
      }

      // Cookie functions
      function setCookie() {
        // Cookie expires in 1 day
        const expiryDate = new Date();
        expiryDate.setDate(expiryDate.getDate() + 1);

        document.cookie = `testCookie=This cookie expires on ${expiryDate.toLocaleString()}; expires=${expiryDate.toUTCString()}; path=/`;
        alert("Cookie saved");
      }

      function getCookie() {
        const cookieValue =
          document.cookie
            .split("; ")
            .find((row) => row.startsWith("testCookie="))
            ?.split("=")[1] || "No cookie found";

        document.getElementById("cookie-output").textContent = cookieValue;
      }
    </script>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 10. How do you embed audio and video in a webpage?

HTML5 introduced native elements for embedding audio and video content without requiring third-party plugins like Flash. These elements are:

- `<audio>` — for sound/music files
- `<video>` — for video playback

---

### 🎵 Audio Embedding

The basic structure of the `<audio>` element:

```html
<audio controls>
  <source src="audio-file.mp3" type="audio/mpeg" />
  <source src="audio-file.ogg" type="audio/ogg" />
  Your browser does not support the audio element.
</audio>
```

#### 🔧 Common Audio Attributes:

| Attribute  | Description                                                                 |
| ---------- | --------------------------------------------------------------------------- |
| `controls` | Displays audio player controls (play, pause, volume)                        |
| `autoplay` | Starts audio automatically when page loads (browser-dependent)              |
| `loop`     | Replays audio continuously                                                  |
| `muted`    | Mutes audio by default                                                      |
| `preload`  | Suggests how much data the browser should load (`auto`, `metadata`, `none`) |
| `src`      | (optional if using `<source>`) Direct path to audio file                    |

#### ✅ Example with Full Attributes:

```html
<audio controls autoplay loop muted preload="auto">
  <source src="audio-file.mp3" type="audio/mpeg" />
  <source src="audio-file.ogg" type="audio/ogg" />
  Your browser does not support the audio element.
</audio>
```

---

### 🎬 Video Embedding

The `<video>` element works similarly but includes width, height, and poster (thumbnail) options:

```html
<video width="640" height="360" controls>
  <source src="video-file.mp4" type="video/mp4" />
  <source src="video-file.webm" type="video/webm" />
  Your browser does not support the video tag.
</video>
```

#### 🔧 Common Video Attributes:

| Attribute          | Description                                   |
| ------------------ | --------------------------------------------- |
| `controls`         | Displays video player controls                |
| `autoplay`         | Starts playing when page loads                |
| `loop`             | Repeats video playback                        |
| `muted`            | Mutes video sound                             |
| `poster`           | Image displayed before the video plays        |
| `preload`          | Preload behavior (`auto`, `metadata`, `none`) |
| `width` / `height` | Sets the display size of the video player     |

#### ✅ Example with All Features:

```html
<video
  controls
  autoplay
  loop
  muted
  poster="thumbnail.jpg"
  width="640"
  height="360"
>
  <source src="video-file.mp4" type="video/mp4" />
  <source src="video-file.webm" type="video/webm" />
  Your browser does not support the video element.
</video>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 11. Explain the `<canvas>` element and its use cases

The HTML5 `<canvas>` element is used to draw graphics, animations, and other visual content on the fly using JavaScript. It acts as a **blank drawing surface** with no predefined content, and everything must be drawn dynamically via code.

---

### 📐 Basic Syntax

```html
<canvas id="myCanvas" width="300" height="150"></canvas>
```

You interact with it using JavaScript like so:

```javascript
const canvas = document.getElementById("myCanvas");
const ctx = canvas.getContext("2d");

ctx.fillStyle = "red";
ctx.fillRect(10, 10, 100, 50); // Draws a red rectangle
```

---

### 🎯 Key Features

- Resolution-independent drawing
- Pixel-based rendering (unlike SVG which is vector-based)
- Provides 2D and WebGL (3D) rendering contexts
- Can export the drawing as an image
- Can be animated and updated frame-by-frame

---

### 💡 Common Use Cases

| Use Case               | Description                                                      |
| ---------------------- | ---------------------------------------------------------------- |
| **Data Visualization** | Drawing charts/graphs manually or with libraries (e.g. Chart.js) |
| **Games**              | 2D/3D games where pixel-level control is needed                  |
| **Image Manipulation** | Applying filters, cropping, or rendering effects                 |
| **Drawing Tools**      | Freehand sketching apps (e.g. whiteboards, paint tools)          |
| **Custom Animations**  | Create complex animations without relying on CSS/DOM             |
| **Simulations**        | Particle effects, physics simulations, real-time rendering       |

---

### 🧠 Example: Drawing a Circle

```html
<canvas id="circleCanvas" width="200" height="200"></canvas>

<script>
  const canvas = document.getElementById("circleCanvas");
  const ctx = canvas.getContext("2d");

  ctx.beginPath();
  ctx.arc(100, 100, 50, 0, 2 * Math.PI); // x, y, radius, startAngle, endAngle
  ctx.fillStyle = "blue";
  ctx.fill();
</script>
```

---

### 🚫 Limitations

- Not SEO-friendly (everything is rendered as pixels)
- Accessibility requires custom implementation
- Requires JavaScript to function — HTML alone cannot render anything on `<canvas>`

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 12. What are data attributes and how are they useful?

### ✅ What Are Data Attributes?

`data-*` attributes are **custom attributes** introduced in HTML5 that allow you to store **extra data** on any HTML element without using JavaScript or altering the structure or appearance of the content.

They follow the format:

```html
data-<name>="value"</name>
```

✅ Example:

```html
<div data-user-id="42" data-role="admin">John Doe</div>
```

- `data-user-id` is a custom attribute.
- `42` is the value associated with it.
- This data is not displayed to the user but can be accessed by JavaScript.

---

### 🧠 Why Are They Useful?

#### 1. **Encapsulating Metadata**

Data attributes let you attach **meta information** to elements — like IDs, states, configuration values — without changing the structure or appearance of the element.

#### 2. **JavaScript Interaction**

You can easily access or manipulate `data-*` attributes using JavaScript via the `.dataset` property.

```javascript
const element = document.querySelector("[data-user-id]");
console.log(element.dataset.userId); // "42"
```

This makes them especially useful when you’re:

- Tracking element states
- Assigning IDs
- Passing info between HTML and JavaScript without complex logic

#### 3. **Clean & Valid HTML**

Unlike using non-standard attributes (e.g. `custom-id`), `data-*` attributes are **100% valid HTML5** and won't cause validation issues.

---

### ✅ Real-world Example: Toggle Button

```html
<button data-toggle-state="off">Toggle</button>

<script>
  const btn = document.querySelector("button");
  btn.addEventListener("click", () => {
    const currentState = btn.dataset.toggleState;
    const newState = currentState === "off" ? "on" : "off";
    btn.dataset.toggleState = newState;
    btn.textContent = `Toggle (${newState})`;
  });
</script>
```

In this example:

- We use `data-toggle-state` to track whether the toggle is "on" or "off".
- No need to maintain state in a separate variable.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 13. What is the purpose of the `srcset` attribute in images?

The `srcset` attribute in HTML allows developers to provide **multiple versions of an image** so that the browser can choose the most appropriate one based on the user's **device resolution** or **viewport size**. This technique is part of **responsive web design**, helping deliver optimized images for different screens — improving both **performance** and **visual quality**.

---

### 🧠 Why Use `srcset`?

Without `srcset`, a single image is served to all users regardless of their device. This can result in:

- **Too large images on small screens** → Wasted bandwidth
- **Too small images on high-res screens** → Blurry visuals

With `srcset`, browsers pick the **best image** automatically.

---

### 🔧 Syntax Example (Using Resolutions)

```html
<img
  src="image-1x.jpg"
  srcset="image-1x.jpg 1x, image-2x.jpg 2x, image-3x.jpg 3x"
  alt="Example Image"
/>
```

- `1x`, `2x`, and `3x` refer to **pixel density** (DPR - device pixel ratio)
- A device with a Retina screen (2x) will use `image-2x.jpg`

---

### 📐 Syntax Example (Using Widths)

```html
<img
  src="image-small.jpg"
  srcset="image-small.jpg 480w, image-medium.jpg 800w, image-large.jpg 1200w"
  sizes="(max-width: 600px) 480px, (max-width: 900px) 800px, 1200px"
  alt="Responsive image by screen width"
/>
```

- `480w`, `800w`, `1200w` specify the **width of each image in pixels**
- `sizes` tells the browser **how wide the image will be displayed**
- The browser selects the most appropriate image **before downloading**, saving bandwidth

---

### ✅ Benefits

- 📱 **Mobile-first** optimization
- 🚀 **Faster load times** on slow connections
- 🔍 **Sharper images** on high-DPI screens
- 🌐 **Better user experience** across devices

---

### 📝 Tip

You should always include a fallback `src` attribute — it’s used by browsers that don’t support `srcset`, and as a default.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 14. Explain the Difference Between SVG and Canvas

When it comes to rendering graphics in web applications, **SVG** and **Canvas** are two important technologies supported natively by modern browsers. Though both are used for drawing graphics, they are fundamentally different in how they work and when you should use them.

---

### 🖼️ What is SVG (Scalable Vector Graphics)?

- **SVG** is an **XML-based vector image format** for defining two-dimensional graphics.
- SVG graphics are made of **shapes (lines, circles, rectangles, paths)**, **text**, and **images**, all described in the DOM.
- Since SVG is **vector-based**, the graphics **scale perfectly** at any resolution without losing quality.

#### Example:

```html
<svg width="200" height="200">
  <circle cx="100" cy="100" r="80" fill="blue" />
</svg>
```

This creates a blue circle inside an SVG canvas.

---

### 🎨 What is Canvas?

- **Canvas** is an **HTML5 element** used for drawing graphics **via scripting (usually JavaScript)**.
- Canvas renders graphics **pixel by pixel** — it's **bitmap-based**.
- Once something is drawn on the canvas, it becomes part of the canvas and **can't be individually manipulated** via the DOM.

#### Example:

```html
<canvas id="myCanvas" width="200" height="200"></canvas>

<script>
  const canvas = document.getElementById("myCanvas");
  const ctx = canvas.getContext("2d");
  ctx.fillStyle = "blue";
  ctx.beginPath();
  ctx.arc(100, 100, 80, 0, Math.PI * 2);
  ctx.fill();
</script>
```

This draws a blue circle inside the canvas.

---

## 🔥 Key Differences Between SVG and Canvas

| Feature             | SVG                                                                                             | Canvas                                                                          |
| :------------------ | :---------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| **Type**            | Vector-based (shapes and paths)                                                                 | Raster-based (pixels)                                                           |
| **DOM Integration** | Each element (rect, circle, path) is part of the DOM and can be styled or scripted individually | Canvas is a single DOM element — graphics are drawn inside it via JavaScript    |
| **Scalability**     | Infinitely scalable without losing quality                                                      | Scaling can cause blurring because it is pixel-based                            |
| **Performance**     | Better for a small number of objects or static graphics                                         | Better for rendering many objects or frequent updates (games, real-time charts) |
| **Interactivity**   | Easier: elements are part of the DOM and respond to CSS and JavaScript events                   | Harder: you must manually track object locations and events                     |
| **Accessibility**   | SVG is accessible (screen readers can interpret SVG content)                                    | Canvas content is not accessible without additional work                        |
| **Use Cases**       | Icons, diagrams, charts, maps                                                                   | Games, particle systems, real-time visualizations                               |

---

## ✅ When to Use SVG

- You need **responsive, scalable graphics** (logos, UI icons).
- You want to **style or animate** parts of the graphic using CSS or JS.
- You need **searchable, accessible graphics**.
- You have a **small or moderate number** of graphic objects.

## ✅ When to Use Canvas

- You’re creating **dynamic, high-performance graphics** (like games or live data visualizations).
- You’re handling **large numbers of objects** or **real-time animations**.
- You don’t need each drawn object to remain accessible or separately addressable.

---

### 📝 Quick Tip

You can actually **combine** SVG and Canvas depending on the situation!  
For example, you can use SVG for static UI elements and Canvas for dynamic animations inside the same application.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 15. What are Web Components?

**Web Components** are a set of modern browser standards that allow developers to create **reusable, encapsulated custom elements** — with their own structure, style, and behavior — that can be used in any web page or app, **without relying on external libraries or frameworks**.

They help in **building UI components** that are **self-contained** and **framework-agnostic**, meaning you can use them across different projects (even between React, Angular, Vue, or plain HTML apps).

---

### 📦 Web Components Are Based on 4 Main Technologies:

| Feature             | Description                                                                                                                 |
| :------------------ | :-------------------------------------------------------------------------------------------------------------------------- |
| **Custom Elements** | Define your own HTML tags with custom behavior (e.g., `<user-profile>`).                                                    |
| **Shadow DOM**      | Provides encapsulated DOM and CSS, so styles/scripts inside a component don’t affect the rest of the page (and vice versa). |
| **HTML Templates**  | Define markup and content for a component using `<template>` and `<slot>`, which are rendered when needed.                  |
| **ES Modules**      | JavaScript modules (`import`/`export`) are used to define and reuse component logic cleanly.                                |

---

### 🔧 Basic Example of a Web Component

```html
<!-- 1. HTML -->
<user-greeting></user-greeting>

<!-- 2. JavaScript -->
<script>
  class UserGreeting extends HTMLElement {
    constructor() {
      super();
      const shadow = this.attachShadow({ mode: "open" });
      shadow.innerHTML = `<p>Hello, Web Components! 🎉</p>`;
    }
  }

  customElements.define("user-greeting", UserGreeting);
</script>
```

✅ Now `<user-greeting>` is a **custom element** — like any native HTML tag!

---

### 🧠 Why Use Web Components?

- **Encapsulation**: Styles and DOM are scoped inside the component (via Shadow DOM).
- **Reusability**: Write once, use anywhere — even across different frameworks.
- **Native Performance**: No extra runtime needed (unlike React, Angular).
- **Interoperability**: Perfect for design systems, micro-frontends, and shared UI libraries.
- **Maintainability**: Components are modular and self-contained.

---

### 🛠️ Key Terms Explained

| Term                | Meaning                                                                                      |
| :------------------ | :------------------------------------------------------------------------------------------- |
| **Custom Elements** | Create custom HTML elements and define their behavior.                                       |
| **Shadow DOM**      | Create a hidden DOM tree inside a component with its own scoped CSS and markup.              |
| **HTML Template**   | Define reusable HTML structures that aren't rendered until used.                             |
| **Slot**            | Placeholder inside a web component where external HTML can be injected (content projection). |

---

### ✅ Real-World Use Cases

- Building a **design system** (button, card, modal components).
- Developing **shared UI libraries** across projects and teams.
- Creating **micro frontends** where different apps contribute components to a single UI.
- Making widgets that can be **embedded** into any site (like Stripe's checkout, YouTube embeds).

---

### 🚨 Browser Support

- Web Components are supported in **modern browsers** (Chrome, Edge, Firefox, Safari).
- For older browsers (like IE11), you can use **polyfills**.

---

### 🔥 Quick Tip

Even though Web Components are **framework-independent**, many modern frameworks (like Angular, Vue, and React) now provide **ways to integrate with Web Components** easily.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>
