
# HTML Basics

> *Click &#9733; if you like the project. Your contributions are heartily ♡ welcome.*

<br/>

## Related Topics

* *[HTML5 Events List](html5-events.md)*
* *[HTML5 Tags](html5-tags.md)*
* *[HTML5 MCQ](html-mcq.md)*
* *[CSS Basics](https://github.com/learning-zone/css-basics)*
* *[JavaScript Basics](https://github.com/learning-zone/javascript-basics)*

<br/>

## Table of Contents

* [Introduction](#-1-introduction)
* [HTML Tags](#-2-html-tags)
* [HTML Events](#-3-html-events)
* [HTML Forms](#-4-html-forms)
* [HTML Tables](#-5-html-tables)
* [HTML Lists](#-6-html-lists)
* [HTML Iframe](#-7-html-iframe)
* [HTML URL](#-8-html-url)
* [HTML SVG](#-9-html-svg)
* [HTML Canvas](#-10-html-canvas)
* [HTML Storage](#-11-html-storage)
* [HTML APIs](#-12-html-apis)
* [HTML Drag and Drop](#-13-html-drag-and-drop)
* [HTML Web Worker](#-14-html-web-worker)
* [HTML Accessibility](#-15-html-accessibility)
* [Miscellaneous](#-16-miscellaneous)
* [HTML Media](#-17-html-media)
* [HTML5 Advanced APIs](#-18-html5-advanced-apis)
* [Service Workers & Web Workers](#-19-service-workers--web-workers)
* [IndexedDB & Advanced Web Storage](#-20-indexeddb--advanced-web-storage)
* [Atomic Design & Pixel Perfect Design](#-21-atomic-design--pixel-perfect-design)
* [SEO Basics & Advanced](#-22-seo-basics--advanced)
* [HTML Performance Optimization](#-23-html-performance-optimization)
* [HTML Tags & Elements (Intermediate)](#-24-html-tags--elements-intermediate)
* [Web Components](#-25-web-components)
* [HTML Security](#-26-html-security)

<br/>

## # 1. Introduction

<br>

## Q. What is the difference between HTML and XHTML?

The Extensible Hypertext Markup Language, or XHTML, has two important notes for front end developers.

1) It needs to be well formed, meaning all elements need to be closed and nested correctly or you will return errors.
2) Since it is more strict than HTML is requires less pre-processing by the browser, which may improve your sites performance.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the building blocks of HTML5?

* **Semantics**: allowing you to describe more precisely what your content is.
* **Connectivity**: allowing you to communicate with the server in new and innovative ways.
* **Offline and storage**: allowing webpages to store data on the client-side locally and operate offline more efficiently.
* **Multimedia**: making video and audio first-class citizens in the Open Web.
* **2D/3D graphics and effects**: allowing a much more diverse range of presentation options.
* **Performance and integration**: providing greater speed optimization and better usage of computer hardware.
* **Device access**: allowing for the usage of various input and output devices.
* **Styling**: letting authors write more sophisticated themes.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the semantic tags available in HTML5?

HTML5 semantic tags define the function and the category of your text, simplifying the work for browsers and search engines, as well as developers.

HTML5 offers new semantic elements to define different parts of a web page:

* `<article>`
* `<aside>`
* `<details>`
* `<figcaption>`
* `<figure>`
* `<footer>`
* `<header>`
* `<main>`
* `<mark>`
* `<nav>`
* `<section>`
* `<summary>`
* `<time>`

**Syntax:**

```html
<!DOCTYPE html> 

<html>  
   <head> 
      <meta charset = "utf-8"/> 
      <title>...</title> 
   </head> 
  
   <body> 
      <header>...</header> 
      <nav>...</nav> 
      
      <article> 
         <section> 
            ... 
         </section> 
      </article> 
      <aside>...</aside> 
      
      <footer>...</footer> 
   </body> 
</html> 
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Why you would like to use semantic tag?

* Search Engine Optimization, accessibility, repurposing, light code. 
* Many visually impaired person rely on browser speech and semantic tag helps to interpret page content clearly.
* Search engine needs to understand page content to rank and semantic tag helps.
* Semantic code aids accessibility. Specially, many people whose eyes are not good rely on speech browsers to read pages to them. These programs cannot interpret pages very well unless they are clearly explained.
* Help Search engines to better understand pages. Search engine need to understand what your content is about when rank you properly on search engines. Semantic code tends to improve your placement on search engines, as it is easier for the "search engine spiders" to understand.
* It\'s easier to read and edit, which saves time and money during maintenance.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What does a `<DOCTYPE html>` do?

A DOCTYPE is always associated to a `DTD` ( **Document Type Definition** ). A DTD defines how documents of a certain type should be structured (i.e. a `button` can contain a `span` but not a `div`), whereas a DOCTYPE declares what DTD a document supposedly respects (i.e. this document respects the HTML DTD). For webpages, the DOCTYPE declaration is required. It is used to tell user agents what version of the HTML specifications your document respects. 

Once a user agent has recognized a correct DOCTYPE, it will trigger the `no-quirks mode` matching this DOCTYPE for reading the document. If a user agent doesn\'t recognize a correct DOCTYPE, it will trigger the `quirks mode`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What happens when DOCTYPE is not given?

The web page is rendered in quirks mode. The web browsers engines use quirks mode to support older browsers which does not follow the **W3C specifications**. In quirks mode CSS class and id names are case insensitive. In standards mode they are case sensitive.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is Character Encoding?

Character encoding is a method of converting bytes into characters. To validate or display an HTML document properly, a program must choose a proper character encoding. This is specified in the tag:

```html
<meta charset="utf-8"/>
```

* **UTF-8**: A Unicode Translation Format that comes in 8-bit units that is, it comes in bytes. A character in UTF8 can be from 1 to 4 bytes long, making UTF8 variable width.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the purpose of meta tags?

The META elements can be used to include name/value pairs describing properties of the HTML document, such as author, expiry date, a list of keywords, document author etc.

```html
<!DOCTYPE html>
<html>
  <head>
        <!--Recommended Meta Tags-->
        <meta charset="utf-8">
        <meta name="language" content="english"> 
        <meta http-equiv="content-type" content="text/html">
        <meta name="author" content="Author Name">
        <meta name="designer" content="Designer Name">
        <meta name="publisher" content="Publisher Name">
        <meta name="no-email-collection" content="name@email.com">
        <meta http-equiv="X-UA-Compatible" content="IE=edge"/>

        <!--Search Engine Optimization Meta Tags-->
        <meta name="description" content="Project Description">
        <meta name="keywords" content="Software Engineer,Product Manager,Project Manager,Data Scientist">
        <meta name="robots" content="index,follow">
        <meta name="revisit-after" content="7 days">
        <meta name="distribution" content="web">
        <meta name="robots" content="noodp">
        
        <!--Optional Meta Tags-->
        <meta name="distribution" content="web">
        <meta name="web_author" content="">
        <meta name="rating" content="">
        <meta name="subject" content="Personal">
        <meta name="title" content=" - Official Website.">
        <meta name="copyright" content="Copyright 2020">
        <meta name="reply-to" content="">
        <meta name="abstract" content="">
        <meta name="city" content="Bangalore">
        <meta name="country" content="INDIA">
        <meta name="distribution" content="">
        <meta name="classification" content="">
    
        <!--Meta Tags for HTML pages on Mobile-->
        <meta name="format-detection" content="telephone=yes"/>
        <meta name="HandheldFriendly" content="true"/> 
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/> 
        <meta name="apple-mobile-web-app-capable" content="yes" />
        
        <!--http-equiv Tags-->
        <meta http-equiv="Content-Style-Type" content="text/css">
        <meta http-equiv="Content-Script-Type" content="text/javascript">
      
    <title>HTML5 Meta Tags</title>
  </head>
  <body>
       ...
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What does async and defer refer in script tag?

**1. Async:**

Downloads the script file during HTML parsing and will pause the HTML parser to execute it when it has finished downloading.

**Example:**

```html
<!-- 
    With async (asynchronous), browser will continue to load the HTML 
    page and render it while the browser load and execute the script at the same time. 
-->
<!-- Google Analytics is usually added like this -->
<script async src="https://google-analytics.com/analytics.js"></script>
```

**2. Defer:**

Defer downloads the script file during HTML parsing and will only execute it after the HTML parser has completed. Not all browsers support this.

**Example:**

```html
<!-- 
    With defer, browser will run your script when the page finished parsing. 
    (not necessary finishing downloading all image files. This is good.) 
-->
<script defer src="myscript.js"></script>
```

The async attribute is used to indicate to the browser that the script file can be executed asynchronously. The HTML parser does not need to pause at the point it reaches the script tag to fetch and execute, the execution can happen whenever the script becomes ready after being fetched in parallel with the document parsing.

The defer attribute tells the browser to only execute the script file once the HTML document has been fully parsed.

**Example:**

```html
<!-- 
    Without async or defer, browser will run your script immediately, 
    before rendering the elements. 
-->
<script src="myscript.js"></script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What does CORS stand for and what issue does it address?

Cross-Origin Resource Sharing (CORS) is a W3C spec that allows cross-domain communication from the browser. By building on top of the XMLHttpRequest object, CORS allows developers to work with the same idioms as same-domain requests. CORS gives web servers cross-domain access controls, which enable secure cross-domain data transfers.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Can you describe the difference between progressive enhancement and graceful degradation?

* Graceful degradation is when you initially serve the best possible user experience, with all modern functionality, but use feature detection to “gracefully degrade” parts of your application with a fallback or polyfill.

* Progressive enhancement ensures a page works at the lowest expected abilities of browsers. So if you have a JavaScript web application that enhances a persons ability to send information to a database with features like ajax – at the very least you need to provide the ability for a person to send that same information without JavaScript enabled. In this case a simple form with full-page refresh will do what you need.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the DOM? How does the DOM work?

The DOM (Document Object Model) is a cross-platform API that treats HTML documents as a tree structure consisting of nodes. These nodes (such as elements and text nodes) are objects that can be programmatically manipulated and any visible changes made to them are reflected live in the document. In a browser, this API is available to JavaScript where DOM nodes can be manipulated to change their styles, contents, placement in the document, or interacted with through event listeners.

* The DOM was designed to be independent of any particular programming language, making the structural representation of the document available from a single, consistent API.

* document.getElementById() and document.querySelector() are common functions for selecting DOM nodes.

* Setting the innerHTML property to a new value runs the string through the HTML parser, offering an easy way to append dynamic HTML content to a node.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How does the browser rendering engine work?

In order to render content the browser has to go through a series of steps:

* Document Object Model(DOM)
* CSS object model(CSSOM)
* Render Tree
* Layout
* Paint

<p align="center">
    <img src="assets/images/layers.png" alt="Browser Rendering Engine" />
</p>

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between standards mode and quirks mode?

In **Quirks mode**, layout emulates nonstandard behavior in Navigator 4 and Internet Explorer 5. This is essential in order to support websites that were built before the widespread adoption of web standards. In **Standards mode**, the behavior is described by the HTML and CSS specifications. 

For HTML documents, browsers use a `<!DOCTYPE html>` in the beginning of the document to decide whether to handle it in quirks mode or standards mode. 
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset=UTF-8>
    <title>Hello World!</title>
  </head>
  <body>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is Critical Rendering Path?

The **Critical Rendering Path (CRP)** is the sequence of steps the browser takes to convert HTML, CSS, and JavaScript into pixels on the screen.

**The 6 steps in order:**

1. **Constructing the DOM Tree** — Browser parses HTML and builds the Document Object Model (tree of nodes)

2. **Constructing the CSSOM Tree** — Browser parses CSS and builds the CSS Object Model (style rules tree)

3. **Running JavaScript** — JS is a **parser-blocking resource**; the browser stops HTML parsing to execute it (unless `async`/`defer` is used)

4. **Creating the Render Tree** — DOM + CSSOM are combined; only visible elements are included (e.g., `display:none` nodes are excluded)

5. **Generating the Layout** — Browser calculates the exact size and position of each element on the screen (also called "reflow")

6. **Painting** — Browser fills in the actual pixels — text, colors, images, borders, shadows

**Why it matters:** Optimizing the CRP improves page load performance. Key techniques include:

- Place `<link>` stylesheets in `<head>` (avoid render blocking)
- Place `<script>` tags at bottom of `<body>`, or use `async`/`defer`
- Minify CSS and JS
- Reduce render-blocking resources

```
HTML → DOM  ─┐
             ├─→ Render Tree → Layout → Paint
CSS → CSSOM ─┘
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the Benefits of Server Side Rendering (SSR) Over Client Side Rendering (CSR)?

**Benefits of SSR over CSR:**

1. **Faster initial page load** — The server sends fully rendered HTML, so the browser displays content immediately without waiting for JavaScript bundles to download and execute.

2. **Better SEO** — Search engine crawlers receive complete HTML content directly, making it easier to index pages accurately. CSR often sends an empty `<body>` that crawlers may not fully process.

3. **No content blocking on slow networks** — In CSR, users on slow connections wait for JS to load before seeing anything. With SSR, content is visible as soon as HTML is parsed.

4. **Co-located API calls are faster** — The server fetches data internally (low latency), renders it, and ships the final HTML — versus CSR where the browser must make separate API calls after JS loads.

**Trade-offs to consider:**

| | SSR | CSR |
|---|---|---|
| Initial load | Faster (content in HTML) | Slower (waits for JS) |
| Subsequent navigation | Slower (full page requests) | Faster (only data fetched) |
| Server load | Higher | Lower |
| SEO | Better out of the box | Requires extra effort |
| Interactivity | Requires hydration step | Immediate after JS loads |

Modern frameworks like Next.js and Nuxt.js combine both approaches — using SSR for the initial load and CSR for subsequent navigation — to get the best of both worlds.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What does the lang attribute in html do?

The `lang` attribute specifies the language of an element\'s content. It is placed on the `<html>` tag to declare the language of the entire page, or on individual elements to override the page language.

```html
<html lang="en">  <!-- English -->
<html lang="fr">  <!-- French -->
<html lang="ar">  <!-- Arabic -->
```

**What it does:**

1. **CSS styling** — Enables the `:lang()` pseudo-class to apply language-specific styles:
```css
p:lang(fr) {
    font-style: italic;
}
```

2. **Spelling & grammar checkers** — Browsers and tools use it to apply the correct dictionary for spell-checking

3. **Search engine language detection** — Helps search engines understand the language of content for accurate indexing and localized results

4. **Screen readers & accessibility** — Assistive technologies use it to select the correct pronunciation and reading rules for text-to-speech

5. **Browser behavior** — Affects automatic translation prompts (e.g., Chrome\'s "Translate this page?")

6. **Quotation marks** — Browsers render `<q>` tag quotes using the correct style for the specified language

**Example:**

```html
<html lang="en">
  <body>
    <p>This is in English.</p>
    <p lang="de">Das ist auf Deutsch.</p>
    <p lang="ja">これは日本語です。</p>
  </body>
</html>
```

It is a **W3C best practice** to always declare `lang` on the `<html>` element for proper accessibility and SEO.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain the difference between layout, painting and compositing?

Compacted conversationThese are the last three steps in the browser\'s rendering pipeline after the Render Tree is built:

**Layout (Reflow)**

Calculates the exact size and position of every element on the screen. Because elements affect each other (e.g., a parent\'s width affects its children), a change to one element can trigger recalculation of the entire tree — making layout the most expensive step to trigger repeatedly.

> Caused by changes to: `width`, `height`, `margin`, `padding`, `font-size`, `top`/`left`, adding/removing DOM elements.

**Paint**

Fills in the actual pixels — text, colors, images, borders, shadows. This is done onto one or more **layers** (surfaces), not directly to the screen.

> Caused by changes to: `color`, `background`, `box-shadow`, `border-color`, `visibility`. Does **not** require a layout recalculation.

**Compositing**

Takes all the separately painted layers and draws them to the screen in the correct order. This matters for overlapping elements — getting the order wrong would render one element on top of another incorrectly.

> CSS properties like `transform` and `opacity` only trigger compositing (skipping layout and paint entirely), which is why they're the most performant to animate.

**Performance hierarchy (fastest → slowest to trigger):**

| Change affects | Steps triggered |
|---|---|
| `transform`, `opacity` | Composite only |
| `color`, `background` | Paint + Composite |
| `width`, `margin`, `top` | Layout + Paint + Composite |

This is why CSS animations using `transform: translateX()` are far smoother than animating `left`/`top` — they bypass layout and paint entirely.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain about HTML Layout Engines used by browsers?

A **layout engine** (also called a rendering engine) is the core software component of a browser responsible for parsing HTML/CSS and rendering the visual output on screen.

**The three active engines today:**

**Blink** (Google, 2013 — forked from WebKit)
- Used by: Chrome, Edge (since 2020), Opera, Brave, Samsung Internet, Vivaldi
- Powers the majority of web traffic today
- Developed by Google + contributors via the Chromium project

**WebKit** (Apple, 2003 — forked from KHTML)
- Used by: Safari on macOS/iOS, and **all** browsers on iOS (Apple mandates WebKit on iOS App Store)
- The original engine Chrome was based on before Google forked it into Blink

**Gecko** (Mozilla, 1998)
- Used by: Firefox, Thunderbird, SeaMonkey, Waterfox
- The only major independent engine not owned by a big tech company
- Uses a separate JS engine called **SpiderMonkey**

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Does the following trigger http request at the time of page load?

```html
<img src="mypic.jpg" style="visibility: hidden" alt="My photo">

<div style="display: none;">
    <img src="mypic.jpg" alt="My photo">
</div>
```

* Yes

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is progressive rendering?

Progressive Rendering is the technique of sequentially rendering portions of a webpage in the server and streaming it to the client in parts without waiting for the whole page to rendered.

It combines the advantages of both CSR (Client Side Rendering) and SSR (Server Side Rendering) (Server Side Rendering).

**1. Client Side Rendering:**

Client Side Rendering (CSR) is a technique in which content is rendered in the browser using JavaScript. Instead of getting all the content from the HTML file itself, the server sends HTML with an empty body and script tags that contain links to JavaScript bundles that the browser will use to render the content.

Typical page load behavior in CSR —

* Browser requests the server for HTML
* Server sends HTML with script tags in head and no content in body
* Browser parses the HTML and makes http requests to load the scripts
* Once the scripts are loaded, the browser parses them and makes API requests and loads all the content asynchronously

Since the all the content starts loading only after loading the initial JavaScript, it takes a longer time to show any content on the page. If the user is on a slow network, the content is blocked for an even longer time due to lower bandwidth and higher latency.

**2. Server Side Rendering:**

When rendering on the server side, the HTML is rendered on the server and sent to the client. The content that we need to display on the screen becomes available immediately after the HTML is parsed; hence, primary rendering of content is faster than CSR.

Typical page load behavior in SSR —

* Browser requests the server for HTML.
* Server makes API requests (usually co-located) and renders the content in the server.
* Once the page is ready, the server sends it to the browser.
* The browser loads and parses the HTML and paints the content on the screen without waiting for the JavaScript bundle(s) to load.
* Once the JavaScript bundle(s) are loaded, the browser hydrates interactivity to DOM elements, which is usually attaching event handlers and other interactive behaviors.

Since the APIs are usually co-located with the server, the content is loaded super fast (faster than CSR) and the HTML is sent to the browser. Initial JavaScript load doesn\'t block content load as the HTML sent by the server already has the content.

<p align="center">
    <img src="assets/images/progressive-rendering.png" alt="Progressive Rendering" width="500px" />
</p>

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you serve a page with content in multiple languages?

The **lang** attribute specifies the language of the element\'s content.

**Example:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>HTML5 Multilanguage Page</title>
  </head>
  <body>
      <h2>English</h2>
      <p lang="en">This is demo text</p>
     
      <h2>French</h2>
      <p lang="fr">Ceci est un texte de démonstration</p>
     
      <h2>Spanish</h2>
      <p lang="es">Este es un texto de demostración</p>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Discuss the differences between an HTML specification and a browser\'s implementation thereof.

**HTML Specification**

An HTML specification (like **HTML5**, maintained by the W3C and WHATWG) is a formal document that defines:

- What elements and attributes are valid
- How browsers **must** parse and render those elements
- How to handle **invalid/malformed** markup
- What APIs and behaviors JavaScript can access


**Browser Implementation**

A browser implementation is the actual code (the rendering engine — Blink, WebKit, Gecko) that **attempts to follow** the specification. The key word is *attempts*.

**Key Differences**

| Aspect | Specification | Browser Implementation |
|---|---|---|
| **Authority** | Defines the standard | Interprets the standard |
| **Completeness** | 100% of features defined | Partial — no browser supports *all* of any spec |
| **Consistency** | Single source of truth | Varies across Chrome, Firefox, Safari, etc. |
| **Invalid HTML** | Defines some error-handling rules | Many edge cases left to browser discretion |
| **Timing** | Features defined before implemented | Implementations lag behind specs |
| **Vendor prefixes** | Not in spec | Browsers add `-webkit-`, `-moz-` for experimental features |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you establish and enforce HTML coding standards across a team?

For a tech lead, ensuring consistent, maintainable HTML across a team requires tooling, documentation, and process — not just guidelines.

**1. Linting with HTMLHint or html-validate:**

```json
// .htmlhintrc
{
  "tagname-lowercase": true,
  "attr-lowercase": true,
  "attr-value-double-quotes": true,
  "doctype-first": true,
  "tag-pair": true,
  "spec-char-escape": true,
  "id-unique": true,
  "src-not-empty": true,
  "alt-require": true,
  "title-require": true,
  "head-script-disabled": true,
  "style-disabled": true
}
```

```bash
# Run as part of CI/CD
npx htmlhint "**/*.html"
npx html-validate "src/**/*.html"
```

**2. Prettier for consistent formatting:**

```json
// .prettierrc
{
  "printWidth": 100,
  "tabWidth": 2,
  "htmlWhitespaceSensitivity": "css",
  "singleAttributePerLine": false
}
```

**3. Accessibility linting:**

```bash
# axe-core for automated a11y checks in CI
npm install -D @axe-core/cli
npx axe http://localhost:3000 --exit
```

**4. Code review checklist for HTML:**

```markdown
## HTML Code Review Checklist

### Structure
- [ ] `<!DOCTYPE html>` declared
- [ ] `<html lang="...">` with correct language code
- [ ] `<meta charset="UTF-8">` as first `<head>` child
- [ ] `<meta name="viewport" content="width=device-width, initial-scale=1">` present
- [ ] Logical heading hierarchy (`h1` → `h2` → `h3`, no skips)
- [ ] Landmark elements used (`<header>`, `<nav>`, `<main>`, `<footer>`)

### Forms
- [ ] Every input has an associated `<label>`
- [ ] `required`, `type`, and validation attributes present
- [ ] `autocomplete` tokens set correctly

### Images
- [ ] All `<img>` have `alt` (empty for decorative)
- [ ] Images have `width` and `height` attributes (prevent layout shift)
- [ ] `loading="lazy"` for below-the-fold images

### Security
- [ ] External scripts use `integrity` + `crossorigin` (SRI)
- [ ] `rel="noopener noreferrer"` on `target="_blank"` links
- [ ] No inline event handlers in templates

### Accessibility
- [ ] Color contrast passes WCAG AA (4.5:1 for text)
- [ ] Focus order is logical
- [ ] Interactive elements are keyboard-operable
- [ ] ARIA used only when native HTML is insufficient
```

**5. Editor integration:** Share `.editorconfig`, Prettier config, and ESLint (for inline scripts) via a shared config package in your monorepo.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you implement HTML-level micro-frontend architecture?

Micro-frontends extend microservices thinking to the frontend — each team owns an independently deployable UI slice. HTML5 provides two primary composition mechanisms:

**1. iframes — strongest isolation, simplest integration:**

```html
<!-- Shell app (host) -->
<div class="layout">
  <header>
    <iframe src="https://team-nav.example.com/navbar" title="Navigation"></iframe>
  </header>
  <main>
    <iframe src="https://team-cart.example.com/app" title="Cart Application"></iframe>
  </main>
</div>
```

- **Pros:** Complete CSS/JS isolation, independent deployment, different frameworks per team
- **Cons:** Hard to share state, poor accessibility, no shared routing, size overhead

**2. Web Components — native browser standard:**

```html
<!-- Each team ships a custom element -->
<script src="https://team-nav.example.com/navbar.js" type="module"></script>
<script src="https://team-cart.example.com/cart.js" type="module"></script>

<body>
  <team-navbar></team-navbar>
  <main>
    <team-cart user-id="123"></team-cart>
  </main>
</body>
```

```js
// team-cart/cart.js — defines the custom element
class TeamCart extends HTMLElement {
  connectedCallback() {
    this.attachShadow({ mode: "open" });
    this.shadowRoot.innerHTML = `<cart-app></cart-app>`;
  }
}
customElements.define("team-cart", TeamCart);
```

- **Pros:** Native browser support, Shadow DOM for CSS isolation, works in any framework
- **Cons:** Shared dependency management, versioning challenges

**3. Module Federation (Webpack/Vite) — runtime composition:**

```html
<!-- host/index.html -->
<div id="nav-container"></div>
<div id="main-app"></div>
<script type="module" src="./bootstrap.js"></script>
```

```js
// bootstrap.js — dynamically loads remote modules
const { NavBar } = await import("nav/NavBar");    // from remote team
const { CartApp } = await import("cart/CartApp"); // from remote team
```

**Cross-micro-frontend communication:**

```js
// CustomEvent — fire and forget
document.dispatchEvent(new CustomEvent("user:loggedin", { detail: { userId: 123 } }));

// Listen in another micro-frontend
document.addEventListener("user:loggedin", ({ detail }) => {
  loadUserCart(detail.userId);
});

// Or use BroadcastChannel for cross-tab/cross-frame
const channel = new BroadcastChannel("mfe-events");
channel.postMessage({ type: "CART_UPDATED", count: 3 });
channel.onmessage = (e) => updateCartBadge(e.data.count);
```

**Tech lead decision guide:**

| Approach | Isolation | Shared State | Complexity | Best For |
|---|---|---|---|---|
| iframe | Strongest | Hard | Low | Legacy or fully independent apps |
| Web Components | CSS isolated | Via events | Medium | Greenfield, framework-agnostic |
| Module Federation | None | Shared | High | Same-framework teams, performance critical |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you implement browser feature detection and handle browser compatibility?

A tech lead must have a clear strategy for handling browser differences — preferring detection over assumption.

**Feature detection vs. User Agent sniffing:**

```js
// BAD — User Agent sniffing (brittle, breaks with new UA strings)
if (navigator.userAgent.includes("Chrome")) {
  useChromePath();
}

// GOOD — Feature detection
if ("IntersectionObserver" in window) {
  useLazyLoading();
} else {
  loadAllImagesImmediately();
}
```

**Modernizr-style manual detection:**

```js
const features = {
  serviceWorker: "serviceWorker" in navigator,
  webp: false,
  webgl: !!document.createElement("canvas").getContext("webgl"),
  touchscreen: "ontouchstart" in window || navigator.maxTouchPoints > 0,
};

// WebP detection (async)
const img = new Image();
img.onload = () => { features.webp = img.width === 1; };
img.onerror = () => { features.webp = false; };
img.src = "data:image/webp;base64,UklGRiQAAABXRUJQVlA4IBgAAAAwAQCdASoBAAEAAgA0JZQCdAEO/gHOAAA=";
```

**CSS `@supports` for feature detection in stylesheets:**

```css
/* Apply only if CSS Grid is supported */
@supports (display: grid) {
  .container { display: grid; grid-template-columns: repeat(3, 1fr); }
}

/* Fallback for older browsers */
.container { display: flex; flex-wrap: wrap; }

@supports (display: grid) {
  .container { display: grid; }
}
```

**Progressive enhancement strategy:**

```html
<!-- Layer 1: Works in all browsers — semantic HTML -->
<form action="/search" method="GET">
  <input type="text" name="q" placeholder="Search...">
  <button type="submit">Search</button>
</form>

<!-- Layer 2: Enhanced with CSS — visual improvements -->
<link rel="stylesheet" href="search.css">

<!-- Layer 3: Enhanced with JS — async search, autocomplete -->
<script type="module" src="search-enhanced.js"></script>
```

**Polyfills and transpilation strategy:**

```js
// browserslist config (.browserslistrc)
// > 0.5%
// last 2 versions
// not dead
// not ie 11
```

```html
<!-- Differential loading: modern browsers get ES modules -->
<script type="module" src="app.modern.js"></script>
<!-- Legacy browsers get transpiled bundle -->
<script nomodule src="app.legacy.js"></script>
```

**Key tools for a tech lead\'s compatibility workflow:**

| Tool | Purpose |
|---|---|
| [caniuse.com](https://caniuse.com) | Check feature browser support |
| Browserslist | Define target browsers consistently |
| Babel | Transpile modern JS for older browsers |
| PostCSS / Autoprefixer | Add CSS vendor prefixes automatically |
| Polyfill.io | Serve polyfills based on the request UA |
| BrowserStack / Percy | Cross-browser visual testing |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 2. HTML Tags

<br>

## Q. What is difference between `span` tag and `div` tag?

The primary difference between div and span tag is their default behavior. By default, a `<div>` is a **block-level-element** and a `<span>` is an **inline element**.

* `<div>` is a block level element which means it will render it on it\'s own line with a width of a 100% of the parent element.
* `<span>` is an inline element which means it will render on the same line as the previous element, if it is also an inline element, and it\'s width will be determined by it\'s content.

```html
<div>Demo Text, with <span>some other</span> text.</div>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are optional closing tag?

In HTML, **optional closing tags** are tags where the browser automatically closes them when it encounters a new tag, so the end tag is not required.

Common examples: `<p>`, `<li>`, `<td>`, `<tr>`, `<th>`, `<html>`, `<body>`

The full list of optional tags includes:

| Tag | Tag | Tag |
|-----|-----|-----|
| `<area>` | `<head>` | `<option>` |
| `<base>` | `<hr>` | `<p>` |
| `<body>` | `<html>` | `<param>` |
| `<br>` | `<img>` | `<rp>` |
| `<caption>` | `<input>` | `<rt>` |
| `<col>` | `<li>` | `<source>` |
| `<colgroup>` | `<link>` | `<tbody>` |
| `<dd>` | `<meta>` | `<td>` |
| `<dt>` | `<optgroup>` | `<tfoot>` |
| `<embed>` | | `<th>`, `<thead>`, `<tr>`, `<track>`, `<wbr>` |

For example, both of these are valid:

```html
<!-- With closing tag -->
<p>Hello World</p>
<p>Second paragraph</p>

<!-- Without closing tag — browser closes <p> automatically -->
<p>Hello World
<p>Second paragraph
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is a self closing tag?

In HTML5 it is not strictly necessary to close certain HTML tags. The tags that aren\'t required to have specific closing tags are called “self closing” tags.

An example of a self closing tag is something like a line break (`<br />`) or the meta tag (`<meta>`). This means that the following are both acceptable:

```html
<meta charset="UTF-8">
...
<meta charset="UTF-8" />
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain the difference between block elements and inline elements?

* block elements `<h1>, <p>, <ul>, <ol>, <li>`,
* inline elements `<span>, <a>, <strong>, <i>, <img>`

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are semantic and non-semantic elements?

* **Semantic elements**: clearly describes its meaning to both the browser and the developer.
For example: `<form>`, `<table>`,  `<article>`, `<aside>`, `<details>`, `<figcaption>`, `<figure>`, `<footer>`, `<header>`, `<main>`, `<mark>`, `<nav>`, `<section>`, `<summary>`, `<time>` clearly defines its content.
  
* **Non-semantic elements**: `<div>` and `<span>` tells nothing about its content.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the purpose of `main` element?

The HTML `<main>` element represents the dominant content of the `<body>` of a document. The main content area consists of content that is directly related to or expands upon the central topic of a document, or the central functionality of an application.

```html
<main role="main">
    <p>Geckos are a group of usually small, usually nocturnal lizards. 
       They are found on every continent except Australia.</p>
    <p>Many species of gecko have adhesive toe pads which enable them to climb walls and even windows.</p>
</main>
```

*Note: A document mustn\'t have more than one `<main>` element that doesn\'t have the hidden attribute specified.*

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the semantic meanings for `<section>, <article>, <aside>, <nav>, <header>, <footer>` and how should each be used in structuring html markup?

* `<header>` is used to contain introductory and navigational information about a section of the page. This can include the section heading, the author\'s name, time and date of publication, table of contents, or other navigational information.

* `<article>` is meant to house a self-contained composition that can logically be independently recreated outside of the page without losing it\'s meaning. Individual blog posts or news stories are good examples.

* `<section>` is a flexible container for holding content that shares a common informational theme or purpose.

* `<footer>` is used to hold information that should appear at the end of a section of content and contain additional information about the section. Author\'s name, copyright information, and related links are typical examples of such content.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. When should you use `section`, `div` or `article`?

* `<section>`, group of content inside is related to a single theme, and should appear as an entry in an outline of the page. It\'s a chunk of related content, like a subsection of a long article, a major part of the page (eg the news section on the homepage), or a page in a webapp\'s tabbed interface. A section normally has a heading (title) and maybe a footer too.

* `<article>`, represents a complete, or self-contained, composition in a document, page, application, or site and that is, in principle, independently distributable or reusable, e.g. in syndication. This could be a forum post, a magazine or newspaper article, a blog entry, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.

* `<div>`, on the other hand, does not convey any meaning, aside from any found in its class, lang and title attributes.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Can a web page contain multiple `<header>` elements? What about `<footer>` elements?

Yes, header elements can be used multiple times in documents. A `<header>` tag must be present for all articles, sections, and pages, although a `<footer>` tag is not necessary.

**From W3C standards**

```html
A header element is intended to usually contain the section\'s heading (an h1–h6 element or an hgroup 
element), but this is not required. The header element can also be used to wrap a section\'s table of 
contents, a search form, or any relevant logos.
```

```html
The footer element represents a footer for its nearest ancestor sectioning content or sectioning root 
element. A footer typically contains information about its section such as who wrote it, links to related 
documents, copyright data, and the like.
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the physical tags and logical tags in HTML?

**1. Physical Tags:**

Physical tags are used to indicate how a particular character is to be formatted. Any physical style tag may contain any item allowed in text, including conventional text, images, line breaks, etc.

**Example:**

|Tags      | Description                                                      |
|----------|------------------------------------------------------------------|
|`<sup>`   |Superscript is usually used for showing elements above base-line |
|`<sub>`   |The subscript is used for alternate baseline.|
|`<i>`     |An Italic tag is used to define a text with a special meaning. |
|`<big>`   |Big tag increase the font size by 1 (Note: You can not use the big tag in HTML 5)|
|`<small>` |A small tag defines the small text, and it is used while writing copyright.|
|`<b>`     |Bold increases the importance of the text because bold tag covert the text into bold size.|
|`<u>`     |It is used to underline the text.|
|`<tt>`    |Teletype text gives the default font-family which is monospace.|
|`<strike>`|It is an editing markup that tells the reader to ignore the text passage.|

**2. Logical Tags:**

Logical tags are used to tell the browser what kind of text is written inside the tags. Logical tags are also known as Structural tags because they specify the structure of the document. Logical tags are used to indicate to the visually impaired person that there is something more important in the text or to emphasize the text ie, logical tags can be used for styling purposes as well as to give special importance to text content.

**Example:**

|Tags       | Description                     |
|-----------|---------------------------------|
|`<abbr>`   |Defines the abbreviation of text.|
|`<acronym>`|Defines the acronym.|
|`<address>`|Contact information of a person or an organization.|
|`<cite>`   |Defines citation. It displays the text in italic format.|
|`<code>`   |Defines the piece of computer code.|
|`<blockquote>`|Defines a long quotation.|
|`<del>`    |Defines the deleted text and is used to mark a portion of text which has been deleted from the document.|
|`<dfn>`    |Defines the definition element and is used to representing a defining instance in HTML.|
|`<ins>`    |Defines inserted text.|
|`<kbd>`    |Defines keyboard input text.|
|`<pre>`    |Defines the block of preformatted text which preserves the text spaces, line breaks, tabs, and other formatting characters which are ignored by web browsers.|
|`<q>`      |Defines the short quotation.|
|`<samp>`   |Defines the sample output text from a computer program.|
|`<strong>` |Defines strong text i.e. show the importance of the text.|
|`<var>`    |Defines the variable in a mathematical equation or in the computer program.|

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How can you highlight text in HTML?

The `<mark>` HTML element represents text which is marked or highlighted for reference or notation purposes, due to the marked passage\'s relevance or importance in the enclosing context.

**Example:**

```html
<p>Search results for "salamander":</p>
<p>Several species of <mark>salamander</mark> inhabit the Pacific Northwest.</p>
```

**Note**:

By default, browsers render `<mark>` with a yellow background.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between an "attribute" and a "property" in HTML?

Attributes are defined by HTML. Properties are accessed from DOM (Document Object Model) nodes.

**Example:**

```html
<input id="inputId" type="text" value="Hello World!" />
```

The **value** property reflects the current text-content inside the input box, whereas the **value** attribute contains the initial text-content of the **value** attribute from the HTML source code

**Difference between HTML attributes and DOM properties:**

|Attribute                               |Property                |
|----------------------------------------|------------------------|
|Attributes are defined by HTML.         |Properties are defined by the DOM.|
|The value of an attribute is constant.  |The value of a property is variable.|
|These are used to initialize the DOM properties.| No such job defined.|

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is an optional tag?

An **optional tag** is an HTML tag whose closing (or sometimes opening) tag can be omitted because the browser automatically closes it when it encounters the next element.

**Example**:

```html
<!-- Both of these are valid HTML -->

<!-- With closing tags -->
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<!-- Without closing tags — browser auto-closes <li> -->
<ul>
  <li>Item 1
  <li>Item 2
</ul>
```

**Common optional tags**

| Tag | When it auto-closes |
|---|---|
| `<p>` | When another block element starts |
| `<li>` | When another `<li>` or parent closes |
| `<td>`, `<th>` | When another cell or row starts |
| `<tr>` | When another `<tr>` starts |
| `<html>`, `<body>`, `<head>` | Always optional |

**Full list of optional tags**

`<area>`, `<base>`, `<body>`, `<br>`, `<caption>`, `<col>`, `<colgroup>`, `<dd>`, `<dt>`, `<embed>`, `<head>`, `<hr>`, `<html>`, `<img>`, `<input>`, `<li>`, `<link>`, `<meta>`, `<optgroup>`, `<option>`, `<p>`, `<param>`, `<rp>`, `<rt>`, `<source>`, `<tbody>`, `<td>`, `<tfoot>`, `<th>`, `<thead>`, `<tr>`, `<track>`, `<wbr>`

> **Note:** While omitting these tags is technically valid per the HTML spec, it\'s generally considered best practice to include closing tags for readability and consistency, especially in team environments.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is an HTML preprocessor? Have you used different HTML templating languages before?

An **HTML preprocessor** is a tool that lets you write HTML in an extended syntax with features like variables, loops, conditionals, and mixins — then compiles it down to standard HTML that browsers can read.

**Why Use One?**

- **Avoid repetition** — define layouts/partials once, reuse everywhere
- **Dynamic content** — inject server-side data (from DB, API, etc.) into templates
- **Cleaner syntax** — less boilerplate than raw HTML
- **Inheritance** — extend base layouts with child templates


**Popular HTML Templating Languages**

* Pug (formerly Jade)
* Haml
* ERB (Embedded Ruby)
* Handlebars
* Jinja2
* Liquid

The key distinction from plain HTML is **server-side rendering of dynamic data** — the preprocessor fills in variables, loops through data, and outputs fully-formed HTML before it ever reaches the browser.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you change the direction of html text?

The default text direction in HTML is left-to-right. However, when developing web content and applications, we may need to set it to right-to-left, for instance, to cater for languages such as Arabic, Hebrew, Pashto, Persian, Urdu, and Sindhi.

We can set text direction in HTML in one of two ways:

* With the HTML **dir** attribute
* With the CSS **direction** property

**Example:**

```html
<!-- Syntax -->
<element dir="ltr|rtl|auto">

<!-- Example -->
<textarea dir="rtl"></textarea>
```

**Attribute Values:**

|Value          |Description                |
|---------------|---------------------------|
|ltr            |Default. Left-to-right text direction|
|rtl            |Right-to-left text direction|
|auto           |Let the browser figure out the text direction, based on the content|

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. When is it appropriate to use the small element?

The `<small>` HTML element represents side-comments and small print, like copyright and legal text, independent of its styled presentation. By default, it renders text within it one font-size smaller, such as from `small` to `x-small`.

**Example:**

```html
<!DOCTYPE html>
<html>
  <head>
      <title>Small Element</title>
  </head>
  <style>
    small {
      font-size: .7em
    }
  </style>
  <body>
    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</p>
    <hr>
    <p><small>The content is licensed under a W3C License.</small></p>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `<section>` and `<div>`?

The `<section>` tag creates independent sections within a webpage having logically connected content. And the `<div>` tag is an empty container specifying a division or a section.

**The `<section>` Element**

According to the W3C specification, the `<section>` tag means that the content inside this element is grouped. In other words, the content relates to a single theme. It must be an entry in the outline of the page.

**Example:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Section Tag Example</title>
  </head>
  <body>
    <h1>W3Docs</h1>
    <section>
      <h2>W3Docs Sections</h2>
      <ul>
        <li>Books</li>
        <li>Quizzes</li>
        <li>Snippets</li>
      </ul>
    </section>
    <section>
      <h3>Books</h3>
      <p>Learn HTML</p>
      <p>Learn CSS</p>
      <p>Learn Javascript</p>
    </section>
  </body>
</html>
```

**The `<div>` Element**

The `<div>` element only represents its child elements and doesn\'t have a special meaning. It can be used with the `lang`, `title`, and `class` attributes to add semantics that is common to a group of consecutive elements. This element can also be used in a `<dl>` tag and wrap groups of `<dt>` and `<dd>` elements.

**Example:**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Div Tag Example</title>
    <style>
      div {
        background-color: #87f5b3
      }
    </style>
  </head>
  <body>
    <h1>Example</h1>
    <div>
      <h2>A heading in a <div> tag.</h2>
      <p>Some text in a <div> tag.</p>
    </div>
    <p>Here is some other text in a <p> tag.</p>
  </body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 3. HTML Events

<br>

## Q. What are HTML events?

HTML events are actions or occurrences that happen in the browser — triggered by the user or by the browser itself. JavaScript can listen for these events and execute code in response.

Events can originate from:
- **User interaction** — mouse clicks, key presses, form input
- **Browser lifecycle** — page load, resize, scroll
- **Media** — video play/pause/end
- **Network** — online/offline state changes

**How to handle events:**

**1. Inline HTML attribute (not recommended):**
```html
<button onclick="alert('Clicked!')">Click Me</button>
```

**2. DOM property:**
```html
<button id="btn">Click Me</button>
<script>
  document.getElementById("btn").onclick = function() {
    alert("Clicked!");
  };
</script>
```

**3. `addEventListener` (recommended):**
```html
<button id="btn">Click Me</button>
<script>
  document.getElementById("btn").addEventListener("click", function(event) {
    console.log("Button clicked!", event);
  });
</script>
```

`addEventListener` is preferred because it allows multiple listeners on the same element and provides cleaner separation of concerns.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the categories of HTML events?

HTML events are grouped into the following categories:

| Category | Events |
|---|---|
| **Mouse Events** | `click`, `dblclick`, `mousedown`, `mouseup`, `mousemove`, `mouseover`, `mouseout`, `mouseenter`, `mouseleave`, `contextmenu` |
| **Keyboard Events** | `keydown`, `keyup`, `keypress` (deprecated) |
| **Form Events** | `submit`, `reset`, `change`, `input`, `focus`, `blur`, `focusin`, `focusout` |
| **Window / Document Events** | `load`, `DOMContentLoaded`, `unload`, `beforeunload`, `resize`, `scroll` |
| **Clipboard Events** | `copy`, `cut`, `paste` |
| **Drag & Drop Events** | `dragstart`, `drag`, `dragenter`, `dragover`, `dragleave`, `drop`, `dragend` |
| **Media Events** | `play`, `pause`, `ended`, `volumechange`, `timeupdate`, `canplay` |
| **Touch Events** | `touchstart`, `touchmove`, `touchend`, `touchcancel` |
| **Pointer Events** | `pointerdown`, `pointermove`, `pointerup`, `pointerenter`, `pointerleave` |
| **Animation Events** | `animationstart`, `animationend`, `animationiteration` |
| **Transition Events** | `transitionstart`, `transitionend` |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is event bubbling and event capturing in HTML?

When an event occurs on a nested element, it propagates through the DOM in two phases:

**1. Capturing phase (top → target)**
The event travels from the `document` root down to the target element.

**2. Bubbling phase (target → top)**
After reaching the target, the event bubbles back up through its ancestors.

```
Capturing:  document → html → body → div → button
Bubbling:   button → div → body → html → document
```

**Example:**
```html
<div id="parent">
  <button id="child">Click Me</button>
</div>

<script>
  document.getElementById("parent").addEventListener("click", () => {
    console.log("Parent clicked");
  });

  document.getElementById("child").addEventListener("click", () => {
    console.log("Child clicked");
  });
  // Output on button click:
  // "Child clicked"
  // "Parent clicked"  ← bubbles up
</script>
```

**Controlling propagation:**

```js
// Stop the event from bubbling further
event.stopPropagation();

// Stop bubbling AND prevent other listeners on the same element
event.stopImmediatePropagation();
```

**Using capturing phase** (pass `true` as the third argument):
```js
element.addEventListener("click", handler, true); // capturing
element.addEventListener("click", handler, false); // bubbling (default)
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is event delegation in HTML?

**Event delegation** is a technique where a single event listener is attached to a **parent element** instead of adding listeners to each child element individually. It leverages event bubbling to handle events from child elements.

**Why use it:**
- Fewer event listeners → better memory performance
- Works for dynamically added elements
- Cleaner code

**Example without delegation (inefficient):**
```html
<ul id="list">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<script>
  // Attaches a listener to EVERY li
  document.querySelectorAll("li").forEach(li => {
    li.addEventListener("click", () => console.log(li.textContent));
  });
</script>
```

**Example with delegation (efficient):**
```html
<ul id="list">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<script>
  // One listener on the parent handles all li clicks
  document.getElementById("list").addEventListener("click", function(event) {
    if (event.target.tagName === "LI") {
      console.log(event.target.textContent);
    }
  });
</script>
```

Dynamic elements also work because the parent listener is already in place when new `<li>` elements are added.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `event.preventDefault()` and `event.stopPropagation()`?

| Method | Purpose |
|---|---|
| `event.preventDefault()` | Prevents the browser\'s **default action** for the event |
| `event.stopPropagation()` | Prevents the event from **bubbling up** (or capturing down) the DOM |

**`preventDefault()` examples:**
```js
// Prevent form submission
form.addEventListener("submit", function(event) {
  event.preventDefault();
  // validate before submitting
});

// Prevent link navigation
link.addEventListener("click", function(event) {
  event.preventDefault();
  // handle navigation manually
});

// Prevent right-click context menu
document.addEventListener("contextmenu", function(event) {
  event.preventDefault();
});
```

**`stopPropagation()` example:**
```js
document.getElementById("child").addEventListener("click", function(event) {
  event.stopPropagation(); // parent\'s click listener will NOT fire
  console.log("Child only");
});
```

> They are independent — calling one does not affect the other. You can call both if needed.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `mouseenter` and `mouseover` events?

Both fire when the mouse cursor enters an element, but they differ in how they handle **child elements**:

| Event | Fires on child hover? | Bubbles? |
|---|---|---|
| `mouseover` | Yes — re-fires when entering a child | Yes |
| `mouseenter` | No — fires only when entering the element itself | No |

**Example:**
```html
<div id="parent" style="padding: 20px; background: lightblue;">
  Parent
  <span id="child" style="background: coral; padding: 5px;">Child</span>
</div>

<script>
  document.getElementById("parent").addEventListener("mouseover", () => {
    console.log("mouseover fired"); // fires when entering parent AND child
  });

  document.getElementById("parent").addEventListener("mouseenter", () => {
    console.log("mouseenter fired"); // fires ONLY when entering parent
  });
</script>
```

Moving the cursor from the parent into the child element:
- `mouseover` fires again (because it bubbles from the child)
- `mouseenter` does **not** fire again

Similarly, `mouseleave` (no bubbling) vs `mouseout` (bubbles).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `DOMContentLoaded` and `load` events?

| Event | Fires when |
|---|---|
| `DOMContentLoaded` | HTML is fully parsed and DOM is ready (CSS, images, and subframes may still be loading) |
| `load` | **Everything** on the page has fully loaded — HTML, CSS, images, scripts, iframes |

**Example:**
```html
<script>
  // DOM is ready — safe to query elements
  document.addEventListener("DOMContentLoaded", function() {
    console.log("DOM ready");
    document.getElementById("btn").style.color = "red";
  });

  // All resources fully loaded
  window.addEventListener("load", function() {
    console.log("Page fully loaded");
    // image dimensions are now available, etc.
  });
</script>
```

**When to use which:**
- Use `DOMContentLoaded` for most DOM manipulation scripts — it fires earlier, making the page feel faster.
- Use `load` only when you need fully loaded resources (e.g., reading image dimensions, third-party widgets).

> Placing `<script>` tags at the bottom of `<body>` is an alternative to `DOMContentLoaded` that achieves a similar result.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `event` object and what are its commonly used properties?

When an event fires, the browser automatically passes an **event object** to the handler. It contains details about the event and the element it occurred on.

**Commonly used properties:**

| Property / Method | Description |
|---|---|
| `event.type` | The event type (e.g., `"click"`, `"keydown"`) |
| `event.target` | The element that **triggered** the event |
| `event.currentTarget` | The element the listener is **attached to** |
| `event.bubbles` | `true` if the event bubbles |
| `event.cancelable` | `true` if `preventDefault()` can stop the default action |
| `event.timeStamp` | Time (ms) when the event was created |
| `event.preventDefault()` | Cancels the default browser action |
| `event.stopPropagation()` | Stops event from bubbling/capturing further |

**Mouse event properties:**

| Property | Description |
|---|---|
| `event.clientX / clientY` | Cursor position relative to the viewport |
| `event.pageX / pageY` | Cursor position relative to the page |
| `event.button` | Mouse button pressed (0=left, 1=middle, 2=right) |

**Keyboard event properties:**

| Property | Description |
|---|---|
| `event.key` | The key value (e.g., `"Enter"`, `"a"`) |
| `event.code` | Physical key code (e.g., `"KeyA"`, `"ArrowUp"`) |
| `event.shiftKey / ctrlKey / altKey` | Modifier key state |

**Example:**
```js
document.addEventListener("keydown", function(event) {
  console.log("Key pressed:", event.key);
  console.log("Ctrl held:", event.ctrlKey);
  if (event.key === "Enter") {
    console.log("Enter was pressed");
  }
});
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `focus` and `focusin`, and `blur` and `focusout` events?

| Event | Bubbles? | Description |
|---|---|---|
| `focus` | No | Fires when an element **gains** focus |
| `focusin` | Yes | Fires when an element **gains** focus (bubbles) |
| `blur` | No | Fires when an element **loses** focus |
| `focusout` | Yes | Fires when an element **loses** focus (bubbles) |

**Example:**
```html
<form id="form">
  <input id="username" type="text" placeholder="Username">
  <input id="password" type="password" placeholder="Password">
</form>

<script>
  // focus/blur: attach to each input individually (does not bubble)
  document.getElementById("username").addEventListener("focus", () => {
    console.log("Username focused");
  });

  // focusin/focusout: attach to parent to catch all children (bubbles)
  document.getElementById("form").addEventListener("focusin", (event) => {
    console.log("Focus moved to:", event.target.id);
  });

  document.getElementById("form").addEventListener("focusout", (event) => {
    console.log("Focus left:", event.target.id);
  });
</script>
```

Use `focusin`/`focusout` with event delegation on a parent element; use `focus`/`blur` when listening directly on a specific element.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `input` and `change` events on form elements?

| Event | Fires when |
|---|---|
| `input` | Immediately on every value change (each keystroke, paste, etc.) |
| `change` | When the element **loses focus** after its value has changed (or on selection for `<select>`) |

**Example:**
```html
<input id="textbox" type="text">
<select id="dropdown">
  <option value="a">Option A</option>
  <option value="b">Option B</option>
</select>

<script>
  const box = document.getElementById("textbox");

  box.addEventListener("input", (event) => {
    console.log("input:", event.target.value); // fires on every keystroke
  });

  box.addEventListener("change", (event) => {
    console.log("change:", event.target.value); // fires on blur after change
  });

  // For <select>, change fires immediately on selection
  document.getElementById("dropdown").addEventListener("change", (event) => {
    console.log("Selected:", event.target.value);
  });
</script>
```

Use `input` for real-time feedback (e.g., live search, character counters); use `change` for validation after the user finishes editing.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 4. HTML Forms

<br>

## Q. What is an HTML form and what is it used for?

An HTML `<form>` element is used to collect user input and send it to a server for processing. It acts as a container for interactive controls like text fields, checkboxes, radio buttons, dropdowns, and submit buttons.

**Basic structure:**

```html
<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <button type="submit">Submit</button>
</form>
```

**Key `<form>` attributes:**

| Attribute | Description |
|---|---|
| `action` | URL where form data is sent on submission |
| `method` | HTTP method: `GET` (data in URL) or `POST` (data in body) |
| `enctype` | Encoding type for form data (important for file uploads) |
| `novalidate` | Disables browser\'s built-in validation |
| `autocomplete` | Enables/disables browser autocomplete (`on`/`off`) |
| `target` | Where to display the response (`_self`, `_blank`, etc.) |

**GET vs POST:**

| | `GET` | `POST` |
|---|---|---|
| Data location | Appended to URL as query string | Sent in request body |
| Visibility | Visible in URL | Not visible |
| Max data size | Limited (~2000 chars) | No practical limit |
| Use case | Search, filtering | Login, registration, file upload |
| Bookmarkable | Yes | No |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are all the input types available in HTML?

HTML provides a wide range of `<input>` types to collect different kinds of data:

**Text & Data Entry:**

| Type | Description |
|---|---|
| `text` | Single-line plain text (default) |
| `password` | Masked text input |
| `email` | Email address (with basic format validation) |
| `number` | Numeric input with optional min/max/step |
| `tel` | Telephone number |
| `url` | URL with format validation |
| `search` | Search query field |

**Date & Time:**

| Type | Description |
|---|---|
| `date` | Date picker (yyyy-mm-dd) |
| `time` | Time picker (hh:mm) |
| `datetime-local` | Date and time (no timezone) |
| `month` | Month and year picker |
| `week` | Week picker |

**Selection & Choice:**

| Type | Description |
|---|---|
| `checkbox` | Boolean toggle (can select multiple) |
| `radio` | Single choice from a group |
| `range` | Slider for a numeric range |
| `color` | Color picker |

**File & Action:**

| Type | Description |
|---|---|
| `file` | File upload control |
| `submit` | Submits the form |
| `reset` | Resets all fields to default values |
| `button` | Generic button (no default action) |
| `hidden` | Hidden field (not shown to user, value sent with form) |

**Example:**

```html
<input type="text" name="username" placeholder="Enter username">
<input type="email" name="email" placeholder="Enter email">
<input type="password" name="password" placeholder="Enter password">
<input type="number" name="age" min="1" max="120">
<input type="date" name="dob">
<input type="checkbox" name="agree" value="yes"> I agree
<input type="radio" name="gender" value="male"> Male
<input type="file" name="avatar" accept="image/*">
<input type="range" name="volume" min="0" max="100" step="5">
<input type="color" name="favorite_color">
<input type="hidden" name="csrf_token" value="abc123">
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is HTML form validation and what are the built-in validation attributes?

HTML5 provides **client-side form validation** without JavaScript, using built-in validation attributes. The browser checks these constraints before submitting.

**Built-in validation attributes:**

| Attribute | Applies to | Description |
|---|---|---|
| `required` | Most inputs | Field must not be empty |
| `minlength` / `maxlength` | `text`, `email`, `password`, etc. | Min/max character count |
| `min` / `max` | `number`, `date`, `range` | Min/max value |
| `step` | `number`, `range`, `date` | Valid value increments |
| `pattern` | `text`, `email`, `url`, `tel` | Must match a regex |
| `type` | `<input>` | Validates format (e.g., `email`, `url`, `number`) |

**Example:**

```html
<form>
  <input type="text" name="username" required>
  <input type="text" name="bio" minlength="10" maxlength="200">
  <input type="number" name="age" min="18" max="100">
  <!-- Pattern: 5-digit US zip code -->
  <input type="text" name="zip" pattern="[0-9]{5}" title="5-digit zip code">
  <input type="email" name="email">
  <button type="submit">Submit</button>
</form>
```

**CSS pseudo-classes for validation state:**

```css
input:valid   { border-color: green; }
input:invalid { border-color: red; }
input:required { background: lightyellow; }
```

**Disabling validation:**

```html
<form novalidate>...</form>
<button type="submit" formnovalidate>Save Draft</button>
```

> Client-side validation improves UX but must **never replace server-side validation** — it can always be bypassed.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `name` and `id` attributes on form elements?

| Attribute | Purpose | Required for forms? |
|---|---|---|
| `id` | Uniquely identifies the element in the DOM; used by CSS/JS and `<label for="">` | No |
| `name` | Identifies the field\'s key when form data is submitted to the server | **Yes** — without it, the field\'s value is NOT sent |

**Example:**

```html
<form action="/submit" method="POST">
  <label for="email">Email:</label>
  <input type="email" id="email" name="user_email">
  <!-- id="email"       → links the <label> to this input (accessibility) -->
  <!-- name="user_email" → the key sent to server: user_email=value -->
  <button type="submit">Submit</button>
</form>
```

Submitted data: `user_email=john@example.com`

**Key rule:** `id` must be unique per page. Multiple elements can share the same `name` (e.g., radio buttons and checkboxes in a group).

```html
<!-- Radio group: same name, different values -->
<input type="radio" name="gender" id="male" value="male">
<label for="male">Male</label>

<input type="radio" name="gender" id="female" value="female">
<label for="female">Female</label>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How does the `<label>` element improve HTML forms?

The `<label>` element provides a text description for a form control. It improves both **accessibility** and **usability**.

**Two ways to associate a label with an input:**

**1. Using `for` + `id` (explicit — recommended):**

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

**2. Wrapping the input (implicit):**

```html
<label>
  Username:
  <input type="text" name="username">
</label>
```

**Benefits:**

1. **Accessibility** — Screen readers announce the label text when the input receives focus.
2. **Larger click target** — Clicking the label text also focuses/activates the input, especially helpful for checkboxes and radio buttons on mobile.

```html
<!-- Clicking "I agree" checks the checkbox -->
<input type="checkbox" id="agree" name="agree">
<label for="agree">I agree to the terms</label>
```

3. **WCAG compliance** — Associating labels with inputs is a WCAG 2.1 Level A requirement.

> Always use `<label>` for every form control. Placeholder text is **not** a substitute — it disappears when the user starts typing.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<fieldset>` and `<legend>` element in HTML forms?

`<fieldset>` groups related form controls together, and `<legend>` provides a caption for that group. They improve both structure and accessibility.

**Example:**

```html
<form>
  <fieldset>
    <legend>Personal Information</legend>
    <label for="fname">First Name:</label>
    <input type="text" id="fname" name="fname" required>

    <label for="lname">Last Name:</label>
    <input type="text" id="lname" name="lname" required>
  </fieldset>

  <fieldset>
    <legend>Shipping Address</legend>
    <label for="street">Street:</label>
    <input type="text" id="street" name="street">

    <label for="city">City:</label>
    <input type="text" id="city" name="city">
  </fieldset>

  <button type="submit">Submit</button>
</form>
```

**Benefits:**

- **Accessibility** — Screen readers announce the `<legend>` text before each field in the group, giving context to users.
- **Visual grouping** — Browsers render a box around the group by default.
- **Disabling a group** — Adding `disabled` to `<fieldset>` disables all controls inside it.

```html
<fieldset disabled>
  <legend>Payment (currently unavailable)</legend>
  <input type="text" name="card">
</fieldset>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the different button types in HTML forms?

The `<button>` element has three `type` values that control its behavior inside a form:

| Type | Behavior |
|---|---|
| `type="submit"` | Submits the form (default when inside a `<form>`) |
| `type="reset"` | Resets all form fields to their initial values |
| `type="button"` | No default action — used with JavaScript event handlers |

**Example:**

```html
<form id="myForm" action="/submit" method="POST">
  <input type="text" name="username" placeholder="Username">

  <button type="submit">Submit</button>
  <button type="reset">Clear</button>
  <button type="button" onclick="previewForm()">Preview</button>
</form>
```

**Important:** Always specify `type` explicitly. If `type` is omitted and the button is inside a `<form>`, it defaults to `type="submit"` — which can cause accidental form submissions.

```html
<!-- This button inside a form will accidentally submit it! -->
<button onclick="toggleMenu()">Menu</button>

<!-- Fix: explicitly set type="button" -->
<button type="button" onclick="toggleMenu()">Menu</button>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `autocomplete` attribute in HTML forms?

The `autocomplete` attribute controls whether the browser should automatically fill in form field values based on the user\'s previously entered data.

**Values:**

| Value | Description |
|---|---|
| `on` | Browser may autocomplete (default for most inputs) |
| `off` | Browser should not autocomplete |
| Named tokens | Tells browser what kind of data to fill in |

**Example:**

```html
<!-- Disable autocomplete for entire form -->
<form autocomplete="off">
  <input type="text" name="otp" placeholder="One-time code">
</form>

<!-- Enable specific autocomplete hints -->
<form autocomplete="on">
  <input type="text" name="fname" autocomplete="given-name" placeholder="First name">
  <input type="text" name="lname" autocomplete="family-name" placeholder="Last name">
  <input type="email" name="email" autocomplete="email" placeholder="Email">
  <input type="tel" name="phone" autocomplete="tel" placeholder="Phone">
  <input type="text" name="address" autocomplete="street-address" placeholder="Street address">
</form>
```

**Common autocomplete tokens:**

`name`, `given-name`, `family-name`, `email`, `username`, `new-password`, `current-password`, `tel`, `street-address`, `postal-code`, `country`, `cc-number`, `bday`

> Use `autocomplete="new-password"` on password creation fields to prevent password managers from filling in the current password.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the new form elements in HTML5?

There are five new form elements in the HTML5 forms specification: `<datalist>`, `<output>`, `<progress>`, and `<meter>`. 

**1. Datalist Tag**

Allows to attach a list of suggestions to a text input element. As soon as the user begins to type in the text field, the list of suggestions appears and the user can choose from the suggestions with the mouse.

```html
<p>Enter your favorite browser name:</p>
<input type="text" list="browsers" name="favorite_browser">
<datalist id="browsers">
    <option value="Firefox">
    <option value="Chrome">    
    <option value="Internet Explorer">
    <option value="Opera">
    <option value="Safari">
</datalist>
```

**2. Meter Tag**

Indicates a numeric value that falls within a range. The tag supports a number of attributes:
value: If you don\'t specify a value, the first numeric value inside the `<meter></meter>` pair becomes the value.

* **max**: The maximum possible value of the item.
* **min**: The minimum possible value of the item.
* **high**: If the value can be defined as a range, this is the high end of the range.
* **low**: If the value can defined as a range, this is the low end of that range.
* **optimum**: The optimal value of the element. 

```html
<p>Disk Usage: <meter value="0.2">20%</meter></p>

<p>Total Score: <meter value="6" min="0" max="10">6 out of 10</meter></p>

<p>Pollution Level: <meter low="60" high="80" max="100" value="85">Very High</meter></p>
```

**3. Output Tag**

It indicates a section of the page that can be modified by a script (usually JavaScript).

```html
<form oninput="result.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" value="50"> +
  <input type="number" id="b" value="100"> =
  <output name="result" for="a b"></output>
</form>
```

**4. Progress Tag**

Indicates how much of a task has been completed (often marked as a percentage). It is expected to be modified through JavaScript code.

```html
 
<p>Progress: <progress id="bar" value="0" max="100"><span>0</span>%</progress></p>

<script type="text/javascript">
    var i = 0;
    var progressBar = document.getElementById("bar");
    
    function countNumbers() {
      if(i < 100) {
        i = i + 1;
        progressBar.value = i;
        // For browsers that don\'t support progress tag
        progressBar.getElementsByTagName("span")[0].textContent = i;
      }

      // Wait for sometime before running this script again
      setTimeout("countNumbers()", 100);
    }
    countNumbers();
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How many new form elements are introduced in html5?

|Sl.No| Element     | Description   |
|-----|-------------|---------------------------|
| 01. |color        |Gives the end user a native color picker to choose a color.|
| 02. |date         |Offers a datepicker.|
| 03. |datetime     |An element to choose both date and time.|
| 04. |datetime-local |An element to choose both date and time, with local settings support.|
| 05. |email        |A field for entering e-mail address(es).|
| 06. |month       |Choose a full month.|
| 07. |number       |Picking a number.|
| 08. |range        |Offers a slider to set to a certain value/position.|
| 09. |search       |A field for search queries.|
| 10. |tel          |Choosing a telephone number.|
| 11. |time         |Input a certain time.|
| 12. |url          |Entering a URL.|
| 13. |week         |Picking a specific week.|


**Example:**

```html
<input type="color" value="#b97a57">

<input type="date" value="2020-06-08">

<input type="datetime" value="2020-06-09T20:35:34.32">

<input type="datetime-local" value="2020-06-09T22:41">

<input type="email" value="robert@robertnyman.com">

<input type="month" value="2020-06">

<input type="number" value="4">

<input type="range" value="15">

<!-- Note: If not set, default attribute values are min="0", max="100", step="1". -->

<input type="search" value="[Any search text]">

<input type="tel" value="[Any numeric value]">

<!-- Note: Most web browsers seem to let through any value at this time. -->

<input type="time" value="22:38">

<input type="url" value="https://www.google.com/">

<!-- Note: requires a protocol like http://, ftp:// etc in the beginning. -->


<input type="week" value="2020-W24">
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Create a HTML form with below constraints?

   * Accept User Name, Email, Country and Subject
   * Validate the fields
   * Store data into local Storage
   * Fetch user data and display on right side of the page

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
  body {font-family: Arial, Helvetica, sans-serif;}
  * {box-sizing: border-box;}
  
  input[type=text], input[type=email], select, textarea {
    width: 100%;
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
  }
  
  input[type=submit] {
    background-color: #0e8af7;
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  input[type=submit]:hover {
    background-color: #1181e3;
  }
  
  .container {
    border-radius: 5px;
    background-color: #f2f2f2;
    padding: 20px;
  }
</style>
</head>
<body>

<h3>Contact Form</h3>

<div class="container">
  <form name="contactForm" onsubmit="return validateForm()" method="post">
    <label for="fname">Name</label>
    <input type="text" id="user_name" name="user_name" placeholder="Your name.." required>

    <label for="lname">Email ID</label>
    <input type="email" id="email" name="email" placeholder="Your Email Address.." required>

    <label for="country">Country</label>
    <select id="country" name="country" required>
      <option value="">--- SELECT ---</option>
      <option value="australia">Australia</option>
      <option value="canada">Canada</option>
      <option value="india">India</option>
      <option value="usa">USA</option>
    </select>

    <label for="subject">Subject</label>
    <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>

    <input type="submit" value="Submit">
  </form>
</div>
<script>
    function validateForm() {
      let name = document.forms["contactForm"]["user_name"].value;
      let email = document.forms["contactForm"]["email"].value;
      let country = document.forms["contactForm"]["country"].value;
      let subject = document.forms["contactForm"]["subject"].value;

      if (name === "" || email === "" || country === "") {
        alert("All the fields are mandatory");
        return false;
      } else { 
        // Create a JSON Object
        const userData = {
          name: name,
          email: email,
          country: country,
          subject: subject
        };

        // Store the object into storage
        localStorage.setItem("userData", JSON.stringify(userData));

        // Retrieve the object from the storage
        const data = localStorage.getItem("userData");
        console.log("data: ", JSON.parse(data));
        
        return false;
      }
    }
</script>
</body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What does `enctype='multipart/form-data'` mean?

The enctype attribute specifies how the form-data should be encoded when submitting it to the server.

**Example:** 01

```html
<form action="fileupload.php" method="post" enctype="multipart/form-data"> 
    <p>Please select the file you would like to upload.</p> 
    <input type="file" name="upload"> 
    <br> 
    <input type="submit" value="Upload File">
</form>
```

**Example:** 02

```html
<form action="/urlencoded?token=A87412B" method="POST" enctype="application/x-www-form-urlencoded">
    <input type="text" name="username" value=""/>
    <input type="text" name="password" value=""/>
    <input type="submit" value="Submit" />
</form>
```

**Example:** 03

```html
<form action="action.do" method="get" enctype="text/plain">
    Name: <input type="text" name="name" />
    Phone: <input type="number" name="phone" />
    <input type="submit" value="Submit" />
</form>
```

|Sl.No|Value	                |Description                        |
|-----|-------------------------|-----------------------------------|
| 01. |application/x-www-form-urlencoded  |	Default. All characters are encoded before sent (spaces are converted to "+" symbols, and special characters are converted to ASCII HEX values)|
| 02. |multipart/form-data	    |No characters are encoded. This value is required when you are using forms that have a file upload control |
| 03.  |text/plain	            |Spaces are converted to "+" symbols, but no special characters are encoded|

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is difference between Select and Datalist?

For the select element, the user is required to select one of the options you\'ve given. For the datalist element, it is suggested that the user select one of the options you\'ve given, but he can actually enter anything he wants in the input.

**1. Select:**

```html
<select name="browser">
  <option value="firefox">Firefox</option>
  <option value="ie">IE</option>
  <option value="chrome">Chrome</option>
  <option value="opera">Opera</option>
  <option value="safari">Safari</option>
</select>
```

**2. Datalist:**

```html
<input type="text" list="browsers">
<datalist id="browsers">
  <option value="Firefox">
  <option value="IE">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 5. HTML Tables

<br>

## Q. What are the basic HTML table elements and their purpose?

An HTML table is created using the `<table>` element along with a set of related tags to define rows, headers, and data cells.

**Core table elements:**

| Element | Description |
|---|---|
| `<table>` | The root container for the table |
| `<thead>` | Groups header rows — rendered at the top |
| `<tbody>` | Groups the main body rows |
| `<tfoot>` | Groups footer rows — rendered at the bottom |
| `<tr>` | Defines a table row |
| `<th>` | Defines a header cell (bold + centered by default) |
| `<td>` | Defines a standard data cell |
| `<caption>` | Provides a title/description for the table |
| `<colgroup>` | Groups columns for applying styles |
| `<col>` | Specifies properties for one or more columns within `<colgroup>` |

**Example:**

```html
<table>
  <caption>Employee List</caption>
  <thead>
    <tr>
      <th>Name</th>
      <th>Department</th>
      <th>Salary</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>Engineering</td>
      <td>$95,000</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>Marketing</td>
      <td>$75,000</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="2">Total</td>
      <td>$170,000</td>
    </tr>
  </tfoot>
</table>
```

**Why use `<thead>`, `<tbody>`, `<tfoot>`?**

- Browsers can scroll `<tbody>` independently while keeping headers/footers fixed
- Screen readers use them to better announce table structure
- When printing, the browser can repeat `<thead>` and `<tfoot>` on every page

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `<th>` and `<td>` in HTML tables?

Both `<th>` and `<td>` define cells in a table row, but they have distinct purposes:

| | `<th>` (Table Header) | `<td>` (Table Data) |
|---|---|---|
| **Purpose** | Header cell — labels a column or row | Data cell — contains actual data |
| **Default style** | Bold, centered | Normal weight, left-aligned |
| **Accessibility** | Semantically marks up heading content | Contains content only |
| **`scope` attribute** | Supports `scope` to define what it headers | Does not use `scope` |
| **Usage** | Inside `<thead>` rows, or as row headers in `<tbody>` | Inside `<tbody>` and `<tfoot>` rows |

**Example:**

```html
<table>
  <thead>
    <tr>
      <!-- Column headers -->
      <th scope="col">Product</th>
      <th scope="col">Price</th>
      <th scope="col">Stock</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <!-- Row header -->
      <th scope="row">Widget A</th>
      <td>$10.00</td>
      <td>50</td>
    </tr>
    <tr>
      <th scope="row">Widget B</th>
      <td>$25.00</td>
      <td>12</td>
    </tr>
  </tbody>
</table>
```

**`scope` attribute values for `<th>`:**

| Value | Description |
|---|---|
| `col` | Header for its column |
| `row` | Header for its row |
| `colgroup` | Header for a group of columns |
| `rowgroup` | Header for a group of rows |

> Always use `<th>` for header cells and add the `scope` attribute for accessibility — screen readers use it to correctly associate headers with data cells.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do `colspan` and `rowspan` attributes work in HTML tables?

`colspan` and `rowspan` allow a cell to span across multiple columns or rows respectively.

**`colspan`** — merges cells horizontally across columns:

```html
<table border="1">
  <tr>
    <!-- This cell spans 3 columns -->
    <th colspan="3">Full Name</th>
  </tr>
  <tr>
    <td>Title</td>
    <td>First Name</td>
    <td>Last Name</td>
  </tr>
  <tr>
    <td>Mr.</td>
    <td>John</td>
    <td>Smith</td>
  </tr>
</table>
```

**`rowspan`** — merges cells vertically across rows:

```html
<table border="1">
  <tr>
    <th>Day</th>
    <th>Time</th>
    <th>Activity</th>
  </tr>
  <tr>
    <!-- This cell spans 2 rows -->
    <td rowspan="2">Monday</td>
    <td>9:00 AM</td>
    <td>Meeting</td>
  </tr>
  <tr>
    <!-- No "Day" cell here — it\'s covered by the rowspan above -->
    <td>11:00 AM</td>
    <td>Workshop</td>
  </tr>
</table>
```

**Combining both:**

```html
<table border="1">
  <tr>
    <td colspan="2" rowspan="2">Top-left 2×2 block</td>
    <td>Top-right</td>
  </tr>
  <tr>
    <td>Middle-right</td>
  </tr>
  <tr>
    <td>Bottom-left</td>
    <td>Bottom-middle</td>
    <td>Bottom-right</td>
  </tr>
</table>
```

> **Key rule:** When a cell spans multiple rows or columns, the cells it covers must be **omitted** from the HTML markup — the browser fills them automatically.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<caption>` element in HTML tables and why is it important?

The `<caption>` element provides a **title or description** for an HTML table. It must be the first child of `<table>`.

**Example:**

```html
<table>
  <caption>Q1 2025 Sales Report</caption>
  <thead>
    <tr>
      <th scope="col">Region</th>
      <th scope="col">Revenue</th>
      <th scope="col">Growth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>North</td>
      <td>$120,000</td>
      <td>+8%</td>
    </tr>
    <tr>
      <td>South</td>
      <td>$95,000</td>
      <td>+3%</td>
    </tr>
  </tbody>
</table>
```

**Why it matters:**

1. **Accessibility** — Screen readers announce the caption before reading the table, giving users context about what data follows. This is especially important for complex tables.
2. **Discoverability** — Users who navigate by tables (using AT shortcuts) see the caption first, helping them decide whether to enter the table.
3. **SEO** — Provides semantic meaning to search engines about the table\'s content.

**Caption positioning with CSS:**

```css
/* Default: caption above the table */
caption { caption-side: top; }

/* Move caption below the table */
caption { caption-side: bottom; }
```

> For complex tables, consider also using the `summary` attribute (HTML4) or `aria-describedby` (modern approach) to provide a more detailed description of the table\'s structure.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you use `<colgroup>` and `<col>` to style table columns?

`<colgroup>` and `<col>` allow you to apply styles to entire columns without repeating styles on each cell.

**Syntax:**

```html
<table>
  <colgroup>
    <col style="width: 40%;">
    <col style="width: 30%; background-color: #f0f8ff;">
    <col style="width: 30%;">
  </colgroup>
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
      <th>Salary</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>Engineer</td>
      <td>$95,000</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>Designer</td>
      <td>$80,000</td>
    </tr>
  </tbody>
</table>
```

**Using `span` to target multiple columns at once:**

```html
<colgroup>
  <!-- First column -->
  <col style="background: #fffde7;">
  <!-- Next 2 columns share the same style -->
  <col span="2" style="background: #e8f5e9;">
</colgroup>
```

**CSS properties that work on `<col>`:**

Only a limited subset of CSS applies to `<col>`:
- `width`
- `background` / `background-color`
- `border`
- `visibility`

> Most other CSS properties (like `text-align`, `padding`) must still be applied to `<td>` / `<th>` directly.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you create an accessible HTML table?

An accessible table ensures screen reader users can understand the relationship between headers and data cells.

**Key techniques:**

**1. Use `<th>` with `scope` for all header cells:**

```html
<table>
  <caption>Monthly Budget</caption>
  <thead>
    <tr>
      <th scope="col">Category</th>
      <th scope="col">Planned</th>
      <th scope="col">Actual</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">Rent</th>
      <td>$1,200</td>
      <td>$1,200</td>
    </tr>
    <tr>
      <th scope="row">Groceries</th>
      <td>$400</td>
      <td>$375</td>
    </tr>
  </tbody>
</table>
```

**2. Use `id` + `headers` for complex tables with merged cells:**

```html
<table>
  <tr>
    <th id="name" scope="col">Name</th>
    <th id="q1" scope="col">Q1</th>
    <th id="q2" scope="col">Q2</th>
  </tr>
  <tr>
    <th id="alice" scope="row">Alice</th>
    <td headers="alice q1">$10k</td>
    <td headers="alice q2">$12k</td>
  </tr>
</table>
```

**3. Always include `<caption>` for a meaningful title.**

**4. Avoid using tables for layout** — use CSS Grid or Flexbox instead. Layout tables confuse screen readers that expect tabular data.

**5. Don\'t use empty header cells** — if a corner cell has no content, use `<td>` instead of `<th>`, or add visually hidden text:

```html
<th scope="col"><span class="sr-only">Name</span></th>
```

**Accessibility checklist:**

- [ ] `<caption>` present
- [ ] All column headers use `<th scope="col">`
- [ ] Row headers use `<th scope="row">` where applicable
- [ ] Complex tables use `id`/`headers` association
- [ ] No empty `<th>` cells
- [ ] Table used for data, not layout

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you make an HTML table responsive?

By default, HTML tables don\'t adapt well to small screens. Here are the common techniques to make them responsive:

**1. Horizontal scrolling wrapper (simplest approach):**

```html
<div style="overflow-x: auto;">
  <table>
    <thead>...</thead>
    <tbody>...</tbody>
  </table>
</div>
```

```css
.table-wrapper {
  overflow-x: auto;
  -webkit-overflow-scrolling: touch; /* smooth scroll on iOS */
}
```

**2. Stacked layout using CSS (cards approach):**

Transform each row into a card on small screens using `data-*` attributes for labels:

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
      <th>Salary</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td data-label="Name">Alice</td>
      <td data-label="Role">Engineer</td>
      <td data-label="Salary">$95,000</td>
    </tr>
  </tbody>
</table>
```

```css
@media (max-width: 600px) {
  table, thead, tbody, th, td, tr {
    display: block;
  }

  thead tr {
    display: none; /* hide original headers */
  }

  td {
    position: relative;
    padding-left: 50%;
  }

  td::before {
    content: attr(data-label);
    position: absolute;
    left: 0;
    font-weight: bold;
  }
}
```

**3. Hide less important columns on small screens:**

```css
@media (max-width: 600px) {
  .optional-col {
    display: none;
  }
}
```

```html
<th class="optional-col">Phone</th>
<td class="optional-col">555-1234</td>
```

> For data-heavy applications, consider using a JavaScript table library (like AG Grid or DataTables) that provides built-in responsive features.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you style an HTML table with CSS?

Modern HTML tables should be styled entirely with CSS rather than deprecated HTML attributes like `border`, `cellpadding`, `cellspacing`, and `bgcolor`.

**Basic table styling:**

```css
/* Remove default spacing between cells */
table {
  border-collapse: collapse; /* or separate */
  width: 100%;
  font-family: Arial, sans-serif;
}

th, td {
  padding: 12px 16px;
  text-align: left;
  border-bottom: 1px solid #ddd;
}

th {
  background-color: #4a90d9;
  color: white;
  font-weight: bold;
}

/* Zebra striping */
tbody tr:nth-child(even) {
  background-color: #f5f5f5;
}

/* Hover highlight */
tbody tr:hover {
  background-color: #e8f0fe;
}

/* Caption styling */
caption {
  font-size: 1.2em;
  font-weight: bold;
  margin-bottom: 8px;
  text-align: left;
}
```

**`border-collapse` values:**

| Value | Description |
|---|---|
| `collapse` | Adjacent cells share a single border (most common) |
| `separate` | Each cell has its own border with a gap between them |

**With `border-separate`, use `border-spacing` to control the gap:**

```css
table {
  border-collapse: separate;
  border-spacing: 4px 8px; /* horizontal vertical */
}
```

**Full styled example:**

```html
<style>
  table { border-collapse: collapse; width: 100%; }
  th { background: #2c3e50; color: white; padding: 10px; }
  td { padding: 10px; border: 1px solid #ccc; }
  tr:nth-child(even) td { background: #f9f9f9; }
  tr:hover td { background: #eaf4fb; }
</style>

<table>
  <caption>Product Inventory</caption>
  <thead>
    <tr><th>Product</th><th>Category</th><th>Price</th><th>Stock</th></tr>
  </thead>
  <tbody>
    <tr><td>Widget A</td><td>Tools</td><td>$10</td><td>50</td></tr>
    <tr><td>Widget B</td><td>Tools</td><td>$25</td><td>12</td></tr>
    <tr><td>Gadget X</td><td>Electronics</td><td>$99</td><td>8</td></tr>
  </tbody>
</table>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 6. HTML Lists

<br>

## Q. What are the types of lists available in HTML?

HTML provides three main types of lists to organize content:

| List Type | Element | Description |
|---|---|---|
| **Unordered list** | `<ul>` | Bulleted list — order does not matter |
| **Ordered list** | `<ol>` | Numbered list — order matters |
| **Description list** | `<dl>` | Term–description pairs (glossaries, metadata) |

**1. Unordered List (`<ul>`):**

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

Output: bullet points (•) by default.

**2. Ordered List (`<ol>`):**

```html
<ol>
  <li>Install Node.js</li>
  <li>Create a project folder</li>
  <li>Run npm init</li>
</ol>
```

Output: numbered 1, 2, 3 by default.

**3. Description List (`<dl>`):**

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language — the structure of web pages.</dd>

  <dt>CSS</dt>
  <dd>Cascading Style Sheets — the presentation of web pages.</dd>
</dl>
```

- `<dt>` — description term
- `<dd>` — description detail (indented by default)

> All list item content goes inside `<li>` elements for `<ul>` and `<ol>`. Description lists use `<dt>` and `<dd>` instead.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the attributes of the `<ol>` element?

The `<ol>` element supports several attributes to control numbering style and starting value:

| Attribute | Description |
|---|---|
| `type` | Sets the numbering style |
| `start` | Sets the starting number (integer) |
| `reversed` | Counts down instead of up |

**`type` values:**

| Value | Output |
|---|---|
| `1` | 1, 2, 3 … (default) |
| `a` | a, b, c … |
| `A` | A, B, C … |
| `i` | i, ii, iii … |
| `I` | I, II, III … |

**Examples:**

```html
<!-- Start from 5 -->
<ol start="5">
  <li>Fifth item</li>
  <li>Sixth item</li>
</ol>

<!-- Alphabetical -->
<ol type="A">
  <li>Option A</li>
  <li>Option B</li>
  <li>Option C</li>
</ol>

<!-- Reversed countdown -->
<ol reversed>
  <li>Bronze</li>
  <li>Silver</li>
  <li>Gold</li>
</ol>
<!-- Outputs: 3. Bronze, 2. Silver, 1. Gold -->

<!-- Roman numerals from 4 -->
<ol type="i" start="4">
  <li>Step four</li>
  <li>Step five</li>
</ol>
```

**Overriding a specific item\'s value with `value`:**

```html
<ol>
  <li>First</li>
  <li value="10">Tenth</li>
  <li>Eleventh</li>
</ol>
```

> Prefer CSS `list-style-type` for purely visual changes; use HTML attributes when the numbering is semantically meaningful.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you customize list markers with CSS?

CSS provides several ways to control or replace the default bullet/number markers on lists.

**1. `list-style-type` — change the marker style:**

```css
ul { list-style-type: disc; }        /* default bullet */
ul { list-style-type: circle; }
ul { list-style-type: square; }
ul { list-style-type: none; }        /* remove markers */

ol { list-style-type: decimal; }     /* 1, 2, 3 */
ol { list-style-type: lower-alpha; } /* a, b, c */
ol { list-style-type: upper-roman; } /* I, II, III */
ol { list-style-type: lower-greek; } /* α, β, γ */
```

**2. `list-style-image` — use a custom image as a bullet:**

```css
ul {
  list-style-image: url('checkmark.png');
}
```

**3. `list-style-position` — control marker placement:**

```css
ul { list-style-position: outside; } /* default — marker outside text box */
ul { list-style-position: inside; }  /* marker inside text flow */
```

**4. Shorthand `list-style`:**

```css
ul {
  list-style: square inside url('bullet.png');
  /* type | position | image */
}
```

**5. Custom markers with `::marker` pseudo-element (modern):**

```css
li::marker {
  content: "✓ ";
  color: green;
  font-size: 1.2em;
}
```

**6. Fully custom styling (remove default, use padding + pseudo-elements):**

```css
ul {
  list-style: none;
  padding: 0;
}

ul li::before {
  content: "→ ";
  color: #4a90d9;
  font-weight: bold;
}
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you create a nested list in HTML?

A nested list is created by placing a `<ul>` or `<ol>` element inside an `<li>` element of a parent list.

**Example — nested unordered list:**

```html
<ul>
  <li>Frontend
    <ul>
      <li>HTML</li>
      <li>CSS
        <ul>
          <li>Flexbox</li>
          <li>Grid</li>
        </ul>
      </li>
      <li>JavaScript</li>
    </ul>
  </li>
  <li>Backend
    <ul>
      <li>Node.js</li>
      <li>Python</li>
    </ul>
  </li>
</ul>
```

**Example — mixed ordered and unordered:**

```html
<ol>
  <li>Plan the project
    <ul>
      <li>Define requirements</li>
      <li>Create wireframes</li>
    </ul>
  </li>
  <li>Build the project</li>
  <li>Test and deploy</li>
</ol>
```

**Important rules:**

- The nested list must be placed **inside an `<li>` element**, not directly inside `<ul>`/`<ol>`
- Browsers apply different default markers at each nesting level (disc → circle → square for `<ul>`)

```css
/* Customize nested list indentation */
ul ul, ol ol {
  margin-left: 1.5em;
  padding-left: 1em;
}
```

> Avoid deep nesting (more than 3 levels) for readability. Consider restructuring content or using headings instead.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is a description list in HTML and when should you use it?

A **description list** (`<dl>`) is used to present a list of term–description pairs. It is ideal for glossaries, metadata, FAQs, and key-value data.

**Elements:**

| Element | Description |
|---|---|
| `<dl>` | Container for the description list |
| `<dt>` | Description **term** (the key/word being defined) |
| `<dd>` | Description **detail** (the definition or value) |

**Example — glossary:**

```html
<dl>
  <dt>HTTP</dt>
  <dd>HyperText Transfer Protocol — used to transfer data on the web.</dd>

  <dt>DNS</dt>
  <dd>Domain Name System — translates domain names to IP addresses.</dd>

  <dt>API</dt>
  <dd>Application Programming Interface — a way for applications to communicate.</dd>
</dl>
```

**One term, multiple descriptions:**

```html
<dl>
  <dt>JavaScript</dt>
  <dd>A scripting language for the web.</dd>
  <dd>Runs in the browser and on the server (Node.js).</dd>
</dl>
```

**Multiple terms, one description:**

```html
<dl>
  <dt>UK</dt>
  <dt>United Kingdom</dt>
  <dd>A country in northwestern Europe.</dd>
</dl>
```

**When to use `<dl>` vs `<ul>`:**

| Use `<dl>` | Use `<ul>` |
|---|---|
| Key-value pairs (term: definition) | Simple list of items |
| Glossaries, FAQs | Navigation menus |
| Metadata (author, date, category) | Feature lists |
| Contact information | Tag lists |

> `<dl>` is often misused for layout indentation. Use it only when the content is genuinely a set of term–description pairs.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you create a navigation menu using an HTML list?

Unordered lists are the standard semantic structure for navigation menus. Screen readers and search engines recognize `<nav>` + `<ul>` as a navigation pattern.

**Basic horizontal nav bar:**

```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
    <li><a href="/services">Services</a></li>
    <li><a href="/contact">Contact</a></li>
  </ul>
</nav>
```

```css
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  gap: 24px;
  background: #2c3e50;
}

nav ul li a {
  display: block;
  padding: 12px 16px;
  color: white;
  text-decoration: none;
}

nav ul li a:hover {
  background: #4a90d9;
}
```

**Dropdown menu (nested list):**

```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li>
      <a href="/products">Products ▾</a>
      <ul class="dropdown">
        <li><a href="/products/widgets">Widgets</a></li>
        <li><a href="/products/gadgets">Gadgets</a></li>
      </ul>
    </li>
    <li><a href="/contact">Contact</a></li>
  </ul>
</nav>
```

```css
li { position: relative; }

.dropdown {
  display: none;
  position: absolute;
  top: 100%;
  left: 0;
  background: white;
  box-shadow: 0 2px 8px rgba(0,0,0,0.15);
  min-width: 160px;
}

li:hover .dropdown { display: block; }
```

**Accessibility for nav menus:**

- Use `<nav>` to wrap the list for landmark navigation
- Add `aria-label="Main navigation"` if there are multiple `<nav>` elements on the page
- Mark the current page link with `aria-current="page"`

```html
<li><a href="/" aria-current="page">Home</a></li>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 7. HTML Iframe

<br>

## Q. What is an iframe and how it works?

The `<iframe>` HTML element represents a nested browsing context, embedding another HTML page into the current one. Each embedded browsing context has its own **session history** and **document**. The browsing context that embeds the others is called the parent browsing context. The topmost browsing context — the one with no parent — is usually the browser window, represented by the **Window** object.

**Example**

```html
<!DOCTYPE html>
<html>
  <head>
    <title>HTML5 iframe</title>
  </head>
  <style type="text/css">
  iframe {
    border: 1px solid #333;
    width: 50%;
  }
  .output {
    background: #eee;
  }
  </style>
  <body>
    <p>The Inline iFrame Example</p>
    <iframe id="inlineFrameId"
      title="Inline iFrame Example"
      width="300"
      height="200"
      src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik">
        Sorry your browser does not support inline frames.
    </iframe>
  </body>
</html>
```

**The Iframe Tag Attributes:**

|Attribute       | Description                |
|----------------|----------------------------|
|allow           |indicates what features the iframe is allowed to use (e.g. fullscreen, camera, autoplay)|
|allowfullscreen |grants or denies permission for the iframe to appear in full-screen mode|
|height           |sets the height of the iframe (if not specified, the default height is 150 pixels)|
|loading         |sets lazy loading or eager loading for the iframe|
|referrerpolicy  |sets what referrer information should be sent in the request for the iframe|
|src             |the address of the resource included in the iframe|
|width           |sets the width of the iframe (if not specified, the default width is 300 pixels)|

*Note: Because each browsing context is a complete document environment, every `<iframe>` in a page requires increased memory and other computing resources.*

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How does cross-origin communication work with iframes using `postMessage`?

The `window.postMessage()` API is the **safe, standard mechanism** for cross-origin communication between a parent page and an embedded iframe (or between browser windows/tabs).

**Syntax:**

```js
targetWindow.postMessage(message, targetOrigin);
```

**Sending a message from the parent to the iframe:**

```html
<!-- parent.html (https://parent.com) -->
<iframe id="myFrame" src="https://child.com/frame.html"></iframe>

<script>
  const iframe = document.getElementById("myFrame");

  // Wait for iframe to load, then send
  iframe.addEventListener("load", () => {
    iframe.contentWindow.postMessage(
      { type: "GREETING", text: "Hello from parent!" },
      "https://child.com"  // targetOrigin — NEVER use "*" with sensitive data
    );
  });
</script>
```

**Receiving the message in the iframe:**

```js
// frame.html (https://child.com)
window.addEventListener("message", (event) => {
  // ALWAYS validate the origin
  if (event.origin !== "https://parent.com") return;

  console.log("Received:", event.data);

  // Send a reply back
  event.source.postMessage({ type: "REPLY", text: "Hello back!" }, event.origin);
});
```

**Receiving the reply in the parent:**

```js
window.addEventListener("message", (event) => {
  if (event.origin !== "https://child.com") return;
  console.log("Reply from iframe:", event.data);
});
```

**Security rules:**

| Rule | Why |
|---|---|
| Always validate `event.origin` | Prevents messages from malicious pages |
| Never use `targetOrigin: "*"` for sensitive data | Any page could intercept it |
| Validate the message shape/type | Prevents processing malformed payloads |
| Do not use `innerHTML` with received data | XSS risk |

> `postMessage` is the building block for micro-frontend communication, embedded widgets, payment iframes (Stripe, PayPal), and OAuth popup flows.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the performance considerations when using iframes?

Iframes have significant performance implications because each one is a **fully independent browsing context** with its own DOM, CSSOM, JavaScript engine instance, and resource pipeline.

**Performance costs:**

| Cost | Detail |
|---|---|
| **Memory** | Each iframe has its own JS heap, DOM tree, and style system |
| **Network** | A fresh HTTP pipeline per iframe; no connection sharing with parent |
| **CPU** | Separate render pipeline and JS execution context |
| **Load blocking** | Synchronous iframes (no `loading="lazy"`) block `window.onload` |
| **Third-party scripts** | Ads/analytics in iframes may load dozens of sub-resources |

**Optimization techniques:**

**1. Lazy load iframes:**

```html
<!-- Browser only fetches iframe when it enters the viewport -->
<iframe src="https://maps.example.com/embed" loading="lazy" title="Map"></iframe>
```

**2. Defer non-critical iframes with JavaScript:**

```html
<!-- Don\'t set src on page load -->
<iframe id="chat-widget" data-src="https://chat.example.com/widget" title="Chat"></iframe>

<script>
  // Load only after page is interactive
  window.addEventListener("load", () => {
    const frame = document.getElementById("chat-widget");
    frame.src = frame.dataset.src;
  });
</script>
```

**3. Use `allow` and `sandbox` to restrict capabilities:**

Restricting permissions slightly reduces the iframe\'s resource footprint and prevents unneeded feature loading.

```html
<iframe
  src="https://video.example.com/embed"
  allow="autoplay; fullscreen"
  sandbox="allow-scripts allow-same-origin"
></iframe>
```

**4. Avoid iframes in the critical rendering path.** Place them below the fold or load them after `DOMContentLoaded`.

**5. Prefer native embedding when available.** YouTube\'s `<lite-youtube>` web component, for example, avoids loading the full YouTube iframe until user interaction.

> As a tech lead, audit your page\'s iframe usage with Chrome DevTools Performance tab and Network tab. Check for blocking iframes and excessive sub-resource loads from third-party widgets.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `allow` attribute on iframes and how does it relate to Permissions Policy?

The `allow` attribute on `<iframe>` controls which browser features the embedded content is permitted to use. It is the iframe-level enforcement of the **Permissions Policy** (formerly Feature Policy).

**Syntax:**

```html
<iframe
  src="https://example.com/embed"
  allow="camera 'none'; microphone 'none'; geolocation 'self'; fullscreen"
></iframe>
```

**Common feature tokens:**

| Token | Description |
|---|---|
| `autoplay` | Media autoplay |
| `camera` | Camera access |
| `microphone` | Microphone access |
| `geolocation` | Geolocation API |
| `fullscreen` | Fullscreen API |
| `payment` | Payment Request API |
| `display-capture` | Screen sharing |
| `usb` | WebUSB access |
| `clipboard-read` / `clipboard-write` | Clipboard API |

**Origin values:**

| Value | Meaning |
|---|---|
| `'self'` | Allowed only for the same origin as the iframe\'s `src` |
| `'none'` | Blocked entirely |
| `'src'` | Allowed for the origin specified in `src` (default) |
| `https://trusted.com` | Allowed for that specific origin |

**Example — video embed that can go fullscreen but not access camera:**

```html
<iframe
  src="https://video.example.com/player"
  allow="fullscreen; autoplay; picture-in-picture"
  title="Video player"
></iframe>
```

> The `allow` attribute is distinct from `sandbox` — `sandbox` restricts browser behavior (scripting, forms), while `allow` controls access to device/browser features. Both can be used together for defense-in-depth.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 8. HTML URL

<br>

## Q. What is a URL and what are its components?

A **URL (Uniform Resource Locator)** is the complete address used to access a resource on the web. It tells the browser the protocol to use, the server to contact, and the path to the resource.

**URL Structure:**

```
scheme://username:password@host:port/path?query#fragment
```

**Example:**

```
https://www.example.com:443/products/shoes?color=blue&size=10#reviews
│      │               │   │              │                  │
scheme  host           port path          query string       fragment
```

**Components breakdown:**

| Component | Example | Description |
|---|---|---|
| **Scheme / Protocol** | `https` | Protocol to use (`http`, `https`, `ftp`, `mailto`, `file`) |
| **Host** | `www.example.com` | Domain name or IP address of the server |
| **Port** | `443` | Server port (optional; defaults: `80` for HTTP, `443` for HTTPS) |
| **Path** | `/products/shoes` | Location of the resource on the server |
| **Query String** | `?color=blue&size=10` | Key-value pairs sent to the server (starts with `?`, separated by `&`) |
| **Fragment** | `#reviews` | Anchor pointing to a section within the page (processed by browser only, not sent to server) |

**URL encoding:** Spaces and special characters in URLs must be percent-encoded:

```
Space   → %20
#       → %23
&       → %26
https://example.com/search?q=hello%20world
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between absolute and relative URLs?

**Absolute URL**

Contains the full address including protocol, host, and path. Works regardless of where the current page is located.

```html
<a href="https://www.example.com/about">About Us</a>
<img src="https://cdn.example.com/images/logo.png" alt="Logo">
```

**Relative URL**

Specifies the path relative to the current page\'s location. The browser constructs the full URL by combining the current page\'s base with the relative path.

| Relative URL | Current Page | Resolves To |
|---|---|---|
| `about.html` | `https://example.com/blog/` | `https://example.com/blog/about.html` |
| `./about.html` | `https://example.com/blog/` | `https://example.com/blog/about.html` |
| `../about.html` | `https://example.com/blog/` | `https://example.com/about.html` |
| `/about.html` | `https://example.com/blog/` | `https://example.com/about.html` |

**Types of relative URLs:**

```html
<!-- Same directory -->
<a href="contact.html">Contact</a>

<!-- Child directory -->
<a href="docs/guide.html">Guide</a>

<!-- Parent directory -->
<a href="../index.html">Home</a>

<!-- Root-relative (starts from domain root) -->
<a href="/about">About</a>

<!-- Protocol-relative (uses same scheme as current page) -->
<script src="//cdn.example.com/library.js"></script>
```

**When to use which:**
- Use **absolute URLs** for external resources and canonical links
- Use **root-relative URLs** (`/path`) for internal links in large sites — they don\'t break when pages move between directories

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<base>` tag in HTML and how does it affect URLs?

The `<base>` element specifies the **base URL** for all relative URLs in a document. It must be placed inside `<head>` and there can only be one per page.

**Syntax:**

```html
<head>
  <base href="https://www.example.com/images/" target="_blank">
</head>
```

**How it affects relative URLs:**

```html
<head>
  <base href="https://www.example.com/">
</head>
<body>
  <!-- Resolves to: https://www.example.com/about -->
  <a href="about">About</a>

  <!-- Resolves to: https://www.example.com/images/logo.png -->
  <img src="images/logo.png" alt="Logo">

  <!-- Fragment links still work — browser looks for #section on current page -->
  <a href="#section">Jump to section</a>
</body>
```

**`target` attribute on `<base>`:** Sets the default target for all links on the page:

```html
<!-- All links open in a new tab by default -->
<base href="https://example.com/" target="_blank">
```

**Important caveats:**
- Fragment-only links (`href="#id"`) are affected — they resolve relative to the base URL, not the current page. To avoid this, use full URLs for fragment links when `<base>` is set.
- Only one `<base>` tag is allowed per document.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `href` and `src` attributes?

Both specify a URL, but they serve different purposes and trigger different browser behavior:

| | `href` | `src` |
|---|---|---|
| **Stands for** | Hypertext Reference | Source |
| **Used on** | `<a>`, `<link>`, `<base>`, `<area>` | `<img>`, `<script>`, `<iframe>`, `<audio>`, `<video>`, `<input>` |
| **Purpose** | Points to a **linked** resource | Points to an **embedded** resource |
| **Browser behavior** | Does not stop HTML parsing | `<script src>` **blocks** HTML parsing until downloaded & executed (unless `async`/`defer`) |
| **Relationship** | Navigational — the resource supplements the document | Replacement — the resource is placed **into** the document |

**Examples:**

```html
<!-- href: links to a stylesheet (loaded in parallel, not blocking) -->
<link rel="stylesheet" href="styles.css">

<!-- href: navigation link -->
<a href="/about">About</a>

<!-- src: embeds an image into the document -->
<img src="logo.png" alt="Logo">

<!-- src: embeds and executes script (blocks parsing by default) -->
<script src="app.js"></script>

<!-- src: embeds another page inside the document -->
<iframe src="https://example.com"></iframe>
```

> Using `src` on a `<script>` tag embeds and executes the file. Using `href` on a `<link>` tag fetches the resource and applies it as a relationship (e.g., stylesheet).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the `target` attribute values for anchor tags?

The `target` attribute on `<a>`, `<form>`, `<area>`, and `<base>` specifies **where** to open the linked resource.

| Value | Behavior |
|---|---|
| `_self` | Opens in the **same** browsing context (default) |
| `_blank` | Opens in a **new** tab or window |
| `_parent` | Opens in the **parent** browsing context (relevant for iframes) |
| `_top` | Opens in the **full body** of the window, breaking out of all frames |
| `framename` | Opens in the named `<iframe>` or `<frame>` |

**Example:**

```html
<!-- Opens in the same tab (default) -->
<a href="/about" target="_self">About</a>

<!-- Opens in a new tab -->
<a href="https://example.com" target="_blank" rel="noopener noreferrer">External</a>

<!-- Opens inside a named iframe -->
<a href="/content.html" target="myFrame">Load Here</a>
<iframe name="myFrame" src="/default.html"></iframe>
```

**Security note:** Always add `rel="noopener noreferrer"` when using `target="_blank"` to prevent the opened page from accessing `window.opener` and potentially redirecting the parent page.

```html
<!-- Secure way to open external links in a new tab -->
<a href="https://external.com" target="_blank" rel="noopener noreferrer">
  Visit External Site
</a>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is URL encoding and when is it required?

**URL encoding** (also called percent-encoding) converts characters that are not allowed or have special meaning in URLs into a `%` followed by two hexadecimal digits representing the character\'s ASCII code.

**Characters that must be encoded:**

| Character | Encoded | Reason |
|---|---|---|
| Space | `%20` (or `+` in query strings) | Not allowed in URLs |
| `#` | `%23` | Reserved (fragment identifier) |
| `&` | `%26` | Reserved (query param separator) |
| `=` | `%3D` | Reserved (key=value separator) |
| `+` | `%2B` | Has special meaning in query strings |
| `/` | `%2F` | Reserved (path separator) |
| `?` | `%3F` | Reserved (query string start) |
| `@` | `%40` | Reserved |

**JavaScript encoding functions:**

```js
// encodeURIComponent: encodes everything except A-Z a-z 0-9 - _ . ! ~ * ' ( )
// Use for encoding individual query parameter values
const query = encodeURIComponent("hello world & more");
console.log(query); // "hello%20world%20%26%20more"

// encodeURI: encodes everything except characters valid in a complete URL
// Use for encoding a full URL
const url = encodeURI("https://example.com/search?q=hello world");
console.log(url); // "https://example.com/search?q=hello%20world"

// Decoding
console.log(decodeURIComponent("hello%20world")); // "hello world"
```

**Example in practice:**

```js
const baseUrl = "https://api.example.com/search";
const params = new URLSearchParams({
  q: "JavaScript & HTML",
  page: 1,
  sort: "date desc"
});
const fullUrl = `${baseUrl}?${params.toString()}`;
// https://api.example.com/search?q=JavaScript+%26+HTML&page=1&sort=date+desc
```

> Use `URLSearchParams` to safely build query strings without manual encoding.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain the use of rel="nofollow", rel="noreferrer", rel="noopener" attribute? 

**1. rel="nofollow"**

When `rel="nofollow"` tag is used, it instruct the search engines not to pass any PageRank from one page to the other. It does not allow it to pass the authority to the specific website. The main advantage of using this attribute is to control the spam attack.

There may be times, when you do not have control over what people publish on your websites, for example some blog comments and some kind of forum posting.

**Example:**

```html
<a href="https://www.website.com" rel="nofollow">Link</a>
```

**2. rel="noreferrer"**

Noreferrer is related to analytics and tracking. The referrer value shows the previous page where a user came from. By using the noreferrer attribute on a link, you are preventing other pages from seeing that traffic came from a click on your link.

**Example:**

```html
<a href="https://www.website.com" rel="noreferrer">Link</a>
```

**3. rel="noopener"**

It prevents the new page from being able to access the `window.opener` property and will make it run in a separate process. noopener tag works as a security fix which prevents malicious links to take control over an opened tab.

**Example:**

```html
<a href="https://www.website.com" target="_blank" rel="noopener">Link</a>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 9. HTML SVG

<br>

## Q. What is difference between SVG and Canvas?

**1. SVG:**

The Scalable Vector Graphics (SVG) is an XML-based image format that is used to define two-dimensional vector based graphics for the web. Unlike raster image (e.g. .jpg, .gif, .png, etc.), a vector image can be scaled up or down to any extent without losing the image quality.

There are following advantages of using SVG over other image formats like JPEG, GIF, PNG, etc.

* SVG images can be searched, indexed, scripted, and compressed.
* SVG images can be created and modified using JavaScript in real time.
* SVG images can be printed with high quality at any resolution.
* SVG content can be animated using the built-in animation elements.
* SVG images can contain hyperlinks to other documents.

**Example:**

```html
<!DOCTYPE html>
<html>
   <head>
      <style>
         #svgelem {
            position: relative;
            left: 50%;
            -webkit-transform: translateX(-20%);
            -ms-transform: translateX(-20%);
            transform: translateX(-20%);
         }
      </style>
      <title>HTML5 SVG</title>
   </head>
   <body>
      <h2 align="center">HTML5 SVG Circle</h2>
      <svg id="svgelem" height="200" xmlns="http://www.w3.org/2000/svg">
         <circle id="bluecircle" cx="60" cy="60" r="50" fill="blue" />
      </svg>
   </body>
</html>
```

**2. Canvas:**

Canvas is a HTML element is used to draw graphics on a web page. It is a  bitmap with an “immediate mode” graphics application programming interface (API) for drawing on it. The `<canvas>` element is only a container for graphics. In order to draw the graphics, you are supposed to use a script. Canvas has several strategies when it comes to drawing paths, boxes, circles, text & adding images.

**Example:**

```html
<!DOCTYPE html>
<html>
   <head>
      <title>HTML5 Canvas Tag</title>
   </head>
   <body>
      <canvas id="newCanvas" width="200" height="100" style="border:1px solid #000000;"></canvas>
      <script>
         var c = document.getElementById('newCanvas');
         var ctx = c.getContext('2d');
         ctx.fillStyle = '#7cce2b';
         ctx.fillRect(0,0,300,100);
      </script>
   </body>
</html>
```

**Differences:**

|SVG	                |Canvas                                         |
|-----------------------|-----------------------------------------------|
|Vector based (composed of shapes)	|Raster based (composed of pixel)
|Multiple graphical elements, which become the part of the page\'s DOM tree|	Single element similar to <img> in behavior. Canvas diagram can be saved to PNG or JPG format|
|Modified through script and CSS	|Modified through script only
|Good text rendering capabilities	|Poor text rendering capabilities
|Give better performance with smaller number of objects or larger surface, or both	|Give better performance with larger number of objects or smaller surface, or both|
|Better scalability. Can be printed with high quality at any resolution. Pixelation does not occur	|Poor scalability. Not suitable for printing on higher resolution. Pixelation may occur |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the different ways to embed SVG in HTML and when should you use each?

SVG can be included in HTML using four different methods, each with different capabilities and trade-offs:

**1. Inline SVG — embed directly in HTML:**

```html
<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100">
  <circle cx="50" cy="50" r="40" fill="steelblue" />
</svg>
```

- Full CSS and JavaScript access to SVG elements
- Can be styled with external CSS and animated
- No extra HTTP request
- Increases HTML payload; can\'t be cached separately

**2. `<img>` tag:**

```html
<img src="icon.svg" alt="Icon description" width="100" height="100">
```

- Simple, cacheable
- No JS/CSS access to SVG internals
- Can\'t modify fill color with CSS unless `currentColor` is used in the SVG

**3. CSS `background-image`:**

```css
.icon {
  background-image: url('icon.svg');
  width: 100px;
  height: 100px;
}
```

- Good for decorative icons
- No DOM access; can\'t be interactive

**4. `<object>` or `<embed>` (legacy):**

```html
<object type="image/svg+xml" data="chart.svg" width="400" height="300">
  Fallback content
</object>
```

- Allows JS access to the SVG document via `contentDocument`
- Rarely used in modern development

**Decision guide:**

| Need | Best method |
|---|---|
| Style with CSS (colors, hover) | Inline SVG |
| Icon in content (accessible alt text) | `<img>` |
| Decorative background | CSS `background-image` |
| Interactive / animated SVG | Inline SVG |
| Cacheable, unmodified asset | `<img>` or CSS |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you make SVG accessible?

SVG accessibility requires explicit markup because browsers don\'t always expose SVG semantics to assistive technologies the same way as HTML.

**1. Informative SVG (conveys meaning) — use `<title>` and `<desc>`:**

```html
<svg
  xmlns="http://www.w3.org/2000/svg"
  role="img"
  aria-labelledby="chart-title chart-desc"
  width="400" height="200"
>
  <title id="chart-title">Monthly Sales 2025</title>
  <desc id="chart-desc">
    Bar chart showing sales from January to June. June had the highest sales at $95,000.
  </desc>
  <!-- chart shapes -->
</svg>
```

**2. Decorative SVG — hide from screen readers:**

```html
<!-- Inline decorative icon -->
<svg aria-hidden="true" focusable="false" ...>
  <!-- icon path -->
</svg>

<!-- If used as <img> -->
<img src="decorative-divider.svg" alt="" role="presentation">
```

**3. Interactive SVG elements:**

```html
<svg ...>
  <!-- Make a shape a button -->
  <g role="button" tabindex="0" aria-label="Play video"
     onclick="playVideo()" onkeypress="handleKey(event)">
    <circle cx="50" cy="50" r="40" fill="green"/>
    <polygon points="40,30 70,50 40,70" fill="white"/>
  </g>
</svg>
```

**4. SVG in `<img>` tags — always provide `alt` text:**

```html
<!-- Informative -->
<img src="logo.svg" alt="Acme Corp logo">

<!-- Decorative -->
<img src="divider.svg" alt="">
```

**Key rules summary:**

- Add `role="img"` to standalone SVGs
- Use `<title>` (short) + `<desc>` (long) for informative SVGs
- Add `aria-hidden="true"` to decorative SVGs
- Ensure interactive SVG elements have `tabindex` and keyboard handlers
- Don\'t rely on SVG `title` tooltip for accessibility — use `aria-label` or `aria-labelledby`

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you animate SVG and what are the different animation techniques?

SVG supports three animation techniques, each with different trade-offs:

**1. CSS animations (recommended for most use cases):**

```html
<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100">
  <circle id="dot" cx="50" cy="50" r="20" fill="steelblue"/>
</svg>
```

```css
#dot {
  animation: pulse 1.5s ease-in-out infinite;
  transform-origin: 50px 50px; /* SVG uses element coordinates */
}

@keyframes pulse {
  0%, 100% { r: 20; opacity: 1; }
  50% { r: 30; opacity: 0.6; }
}
```

- Best performance (GPU-accelerated for `transform` and `opacity`)
- Familiar syntax

**2. JavaScript animations (for complex/data-driven animation):**

```js
const circle = document.getElementById("dot");
let frame;
let r = 20;
let growing = true;

function animate() {
  r = growing ? r + 0.5 : r - 0.5;
  if (r >= 35) growing = false;
  if (r <= 20) growing = true;
  circle.setAttribute("r", r);
  frame = requestAnimationFrame(animate);
}

animate();
// To stop: cancelAnimationFrame(frame);
```

- Full control for data-driven or interactive animations
- Use `requestAnimationFrame` for smooth, 60fps updates
- Libraries: GreenSock (GSAP), Anime.js, D3.js

**3. SMIL animations (deprecated — avoid in new code):**

```html
<circle cx="50" cy="50" r="20" fill="steelblue">
  <animate attributeName="r" from="20" to="35" dur="1s" repeatCount="indefinite"/>
</circle>
```

- Inline SVG animations
- Deprecated in Chrome; not recommended

**Performance tip:** Animate only `transform` and `opacity` on SVG elements — these are GPU-accelerated and bypass layout and paint steps, just like in HTML.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 10. HTML Canvas

<br>

## Q. Explain about HTML Canvas?

**canvas** is an HTML element which can be used to draw graphics via JavaScript. This can, for instance, be used to draw graphs, combine photos, or create animations.

**1. Colors, Styles, and Shadows:**

|  Property    |	Description                                                                 |
|--------------|--------------------------------------------------------------------------------|
|fillStyle	   | Sets or returns the color, gradient, or pattern used to fill the drawing       |
|strokeStyle   | Sets or returns the color, gradient, or pattern used for strokes               |
|shadowColor   | Sets or returns the color to use for shadows                                   |
|shadowBlur	   | Sets or returns the blur level for shadows                                     |
|shadowOffsetX | Sets or returns the horizontal distance of the shadow from the shape           |
|shadowOffsetY | Sets or returns the vertical distance of the shadow from the shape             |

**2. Line Styles:**

|Property	 |  Description                                                   |
|------------|----------------------------------------------------------------|
|lineCap	 |Sets or returns the style of the end caps for a line            |
|lineJoin	 |Sets or returns the type of corner created, when two lines meet |
|lineWidth	 |Sets or returns the current line width                          |
|miterLimit	 |Sets or returns the maximum miter length                        |

**3. Rectangles:**
  
|Method	        |Description                                          |
|---------------|-----------------------------------------------------|
|rect()	        |Creates a rectangle                                  |
|fillRect()	    |Draws a "filled" rectangle                           |
|strokeRect()	|Draws a rectangle (no fill)                          |
|clearRect()	|Clears the specified pixels within a given rectangle |

**4. Paths:**

| Method	      |   Description                                                                                 |
|-----------------|---------------------------------------------------------------------------------------------- |
|fill()	          |Fills the current drawing (path)                                                               |
|stroke()	      |Actually draws the path you have defined                                                       |
|beginPath()	  |Begins a path, or resets the current path                                                      |
|moveTo()	      |Moves the path to the specified point in the canvas, without creating a line                   |
|closePath()	  |Creates a path from the current point back to the starting point                               |
|lineTo()	      |Adds a new point and creates a line to that point from the last specified point in the canvas  |
|clip()	          |Clips a region of any shape and size from the original canvas                                  |
|arc()	          |Creates an arc/curve (used to create circles, or parts of circles)                             |
|arcTo()	      |Creates an arc/curve between two tangents                                                      |

**5. Transformations:**

|Method	        |Description                                                                |
|---------------|-------------------------------------------------------------------------- |
|scale()	    |Scales the current drawing bigger or smaller                               |
|rotate()	    |Rotates the current drawing                                                |
|translate()	|Remaps the (0,0) position on the canvas                                    |
|transform()	|Replaces the current transformation matrix for the drawing                 |
|setTransform()	|Resets the current transform to the identity matrix. Then runs transform() |

**6. Text:**

|Property	    |Description                                                       |
|---------------|----------------------------------------------------------------- |
|font	        |Sets or returns the current font properties for text content      |
|textAlign	    |Sets or returns the current alignment for text content            |
|textBaseline	|Sets or returns the current text baseline used when drawing text  |
|fillText()	    |Draws "filled" text on the canvas                                 |
|strokeText()	|Draws text on the canvas (no fill)                                |
|measureText()	|Returns an object that contains the width of the specified text   |

**Example 01:** HTML5 Canvas for Text

```html
<div>Text</div>
<canvas id="text" width="200" height="100" ></canvas>

<script type="text/javascript">
    // Text with style
    var canvas = document.getElementById('text');
    var context = canvas.getContext('2d');
    context.font = '20pt Calibri';
    context.fillStyle = 'blue';
    context.fillText('Hello World!', 50, 50);
</script>
```

**Example 02:** HTML5 Canvas for Straight Line

```html
<div>Straight Line</div>
<canvas id="line" width="300" height="0" style="border: 1px solid #333;"></canvas>

<script type="text/javascript">
    // Straight Line
    var canvas = document.getElementById("line");
    var context = canvas.getContext("2d");
    context.moveTo(50, 150);
    context.lineTo(250, 50);
    context.stroke();
</script>
```

**Example 03:** HTML5 Canvas for Rectangle

```html
<div>Rectangle with Style</div>
<canvas id="rectangle" width="300" height="200" style="border: 1px solid #999;"></canvas>

<script type="text/javascript">
    // Rectange with style
    var canvas = document.getElementById("rectangle");
    var context = canvas.getContext("2d");
    context.fillStyle = "#FF0000";
    context.fillRect(0, 0, 300, 200);
</script>
```

**Example 04:** HTML5 Canvas for Circle

```html
<div>Circle</div>
<canvas id="circle">This browser does not support Canvas!</canvas>

<script type="text/javascript">
    // Circle
    var canvas = document.getElementById("circle");
    var context = canvas.getContext("2d");
    context.beginPath();
    context.arc(95, 50, 40, 0, 2 * Math.PI);
    context.stroke();
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 11. HTML Storage

<br>

## Q. What is local storage in html5?

**localStorage** is a web storage API in HTML5 that allows you to store key-value pairs in the browser with **no expiration** — data persists across browser sessions until explicitly cleared.

**Key characteristics:**
- Storage capacity: ~5MB per domain
- Data is never sent to the server
- Accessible from any window/tab on the same origin
- Stores data as strings

**Basic API:**

```js
// Store data
localStorage.setItem("name", "John");

// Retrieve data
localStorage.getItem("name"); // "John"

// Remove a specific item
localStorage.removeItem("name");

// Clear all items
localStorage.clear();
```

**Storing objects** (must be serialized):

```js
const user = { name: "John", age: 30 };

// Store
localStorage.setItem("user", JSON.stringify(user));

// Retrieve
const data = JSON.parse(localStorage.getItem("user"));
```

**Error handling** — throws `QuotaExceededError` when storage limit is reached:

```js
try {
    localStorage.setItem("key", "value");
} catch(e) {
    console.log("Storage limit exceeded");
}
```

**Comparison with related storage types:**

| Feature | `localStorage` | `sessionStorage` | `cookie` |
|---------|---------------|-----------------|---------|
| Expiry | Never | On tab close | Manually set |
| Capacity | 5MB | 5MB | 4KB |
| Sent to server | No | No | Yes |
| Scope | Any window | Same tab only | Any window |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is session storage in html5?

The **sessionStorage** object is equal to the localStorage object, except that it stores the data for only one session. The data is deleted when the user closes the specific browser tab.

**Example:**

```js
// Save data to sessionStorage
sessionStorage.setItem('key', 'value');

// Get saved data from sessionStorage
let data = sessionStorage.getItem('key');

// Remove saved data from sessionStorage
sessionStorage.removeItem('key');

// Remove all saved data from sessionStorage
sessionStorage.clear();
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is cookies in html5?

A cookie is an amount of information that persists between a server-side and a client-side. A web browser stores this information at the time of browsing.

A cookie contains the information as a string generally in the form of a name-value pair separated by semi-colons. It maintains the state of a user and remembers the user\'s information among all the web pages.

**Example 01:** Create a Cookies

```js
// create a cookie
document.cookie = "username=Anjali Batta";

// cookie with expiry date
document.cookie = "username=Anjali Batta; expires=Thu, 18 Dec 2022 12:00:00 UTC";
```

**Example 02:** Cookie with expiry date

```js
// cookie with expiry date
document.cookie = "username=Anjali Batta; expires=Thu, 18 Dec 2022 12:00:00 UTC";
```

**Example 03:** Read Cookie

```js
let myCookies = document.cookie;

console.log(myCookies);
```

**Example 04:** Update Cookie

```js
document.cookie = "username=John Smith; expires=Thu, 18 Dec 2022 12:00:00 UTC; path=/";
```

**Example 05:** Delete Cookie

```js
document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC; path=/;";
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Describe the difference between a cookie, sessionStorage and localStorage?

|      | `cookie`  | `localStorage` | `sessionStorage` |
|------|-----------|----------------|------------------|
| Initiator        | Client or server. Server can use `Set-Cookie` header     | Client         | Client           |
| Expiry           | Manually set                                             | Forever        | On tab close     |
| Persistent across browser sessions | Depends on whether expiration is set | Yes            | No   | | Sent to server with every HTTP request | Cookies are automatically being sent via `Cookie` header | No    | No               |
| Capacity (per domain) | 4kb        | 5MB            | 5MB              |
| Accessibility  | Any window        | Any window     | Same tab         |

*Note: If the user decides to clear browsing data via whatever mechanism provided by the browser, this will clear out any `cookie`, `localStorage`, or `sessionStorage` stored. It\'s important to keep this in mind when designing for local persistance, especially when comparing to alternatives such as server side storing in a database or similar (which of course will persist despite user actions).*

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Does localStorage throw error after reaches maximum limits?

Yes - **QuotaExceededError**

**Example:**

```html
<!DOCTYPE HTML>
<html>
   <head>
         <title>HTML5 localStorage</title>
   </head>
   <body>
      <script type="text/javascript">
        try{
            if(window.localStorage){ // Check if the localStorage object exists
            
                var result = "";
                var characters  = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
                var charactersLength = characters.length;
                for(var i = 0; i < 10000; i++){
                    result += characters.charAt(Math.floor(Math.random() * charactersLength));
                    localStorage.setItem("key"+i, result);
                }  
            } else {
                alert("Sorry, your browser do not support localStorage.");
            }
        } catch(e) {
            console.log('Exception: '+e);
        }
      </script>
   </body>
</html>
```

Output

```js
Exception: QuotaExceededError: Failed to execute 'setItem' on 'Storage': 
           Setting the value of 'key3230' exceeded the quota.
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the purpose of cache busting and how can you achieve it?

Browsers have a cache to temporarily store files on websites so they don\'t need to be re-downloaded again when switching between pages or reloading the same page. The server is set up to send headers that tell the browser to store the file for a given amount of time. This greatly increases website speed and preserves bandwidth.

However, it can cause problems when the website has been changed by developers because the user\'s cache still references old files. This can either leave them with old functionality or break a website if the cached CSS and JavaScript files are referencing elements that no longer exist, have moved or have been renamed.

**Cache busting** is the process of forcing the browser to download the new files. This is done by naming the file something different to the old file.

A common technique to force the browser to re-download the file is to append a query string to the end of the file.

```html
<!-- src="js/script.js" => src="js/script.js?v=2" -->
<script src="js/script.js?v=2"></script>
```

The browser considers it a different file but prevents the need to change the file name.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 12. HTML APIs

<br>

## Q. List the API available in HTML5?

**1. High Resolution Time API**

The High Resolution Time API provides the current time in sub-millisecond resolution and such that it is not subject to system clock skew or adjustments.

It exposes only one method, that belongs to the `window.performance` object, called `now()`. It returns a `DOMHighResTimeStamp` representing the current time in milliseconds. The timestamp is very accurate, with precision to a thousandth of a millisecond, allowing for accurate tests of the performance of our code.

```javascript
var time = performance.now();
```

**2. User Timing API**

It allows us to accurately measure and report the performance of a section of JavaScript code. It deals with two main concepts: mark and measure. The former represents an instant (timestamp), while the latter represents the time elapsed between two marks.

```javascript
performance.mark("startFoo");
// A time consuming function
foo();
performance.mark("endFoo");

performance.measure("durationFoo", "startFoo", "endFoo");
```

**3. Network Information API**

This API belongs to the connection property of the `window.navigator` object. It exposes two read-only properties: `bandwidth` and `metered`. The former is a number representing an estimation of the current bandwidth, while the latter is a Boolean whose value is true if the user\'s connection is subject to limitation and bandwidth usage, and false otherwise.

|Sl.No| API                            | Description
|-----|--------------------------------|--------------------------------------------------------------------|
| 01. |navigator.connection.type       |Network Type                               |
| 02. |navigator.connection.downlink   |Effective bandwidth estimate ( downlink )                               |
| 03. |navigator.connection.rtt        |Effective round-trip time estimate ( rtt )                                |
| 04. |navigator.connection.downlinkMax|Upper bound on the downlink speed of the first network hop ( downlinkMax )|
| 05. |navigator.connection.effectiveType|Effective connection type  |
| 06. |navigator.connection.saveData   |True if the user has requested a reduced data usage mode from the user agent ( saveData )|

**4. Vibration API**

It exposes only one method, `vibrate()`, that belongs to the `window.navigator` object. This method accepts one parameter specifying the duration of the vibration in milliseconds. The parameter can be either an integer or an array of integers. In the second case, it\'s interpreted as alternating vibration times and pauses.

```javascript
// Vibrate once for 2 seconds
navigator.vibrate(2000);
```

**5. Battery Status API**

The Battery Status API exposes four properties (`charging`, `chargingTime`, `discharingTime`, and `level`) and four events. The properties specify if the battery is in charge, the seconds remaining until the battery is fully charged, the seconds remaining until the battery is fully discharged, and the current level of the battery. These properties belongs to the `battery` property of the `window.navigator` object.

```javascript
// Retrieves the percentage of the current level of the device\'s battery
var percentageLevel = navigator.battery.level * 100;
```

**6. Page Visibility API**

The Page Visibility API enables us to determine the current visibility state of the page. The Page Visibility API is especially useful for saving resources and improving performance by letting a page avoid performing unnecessary tasks when the document isn\'t visible.

```javascript
//document.hidden retuns true if page is not visible.
console.log('Page Visibility: '+document.hidden); 
```

**7. Fullscreen API**

The Fullscreen API provides a way to request fullscreen display from the user, and exit this mode when desired. This API exposes two methods, `requestFullscreen()` and `exitFullscreen()`, allowing us to request an element to become fullscreen and to exit fullscreen.

```javascript
document.addEventListener("keypress", function(e) {
    if (e.keyCode === 13) { // Enter Key
        toggleFullScreen();
    }
}, false);

function toggleFullScreen() {
    if (!document.fullscreenElement) {
        document.documentElement.requestFullscreen();
    } else {
        if (document.exitFullscreen) {
        document.exitFullscreen(); 
        }
    }
}
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How geolocation api works in html5?

The Geolocation API allows the user to provide their location to web applications if they so desire. For privacy reasons, the user is asked for permission to report location information.

The Geolocation API is published through the `navigator.geolocation` object.

```javascript
if ("geolocation" in navigator) {
  /* geolocation API is available */
} 
```

**Example**

```html
<!DOCTYPE html>
<html>
    <head>
         <title>Geolocation</title>
    </head>
   <body>
    <p><button onclick="geoFindMe()">Show my location</button></p>
    <div id="out"></div>
</body>

<script type="text/javascript">
    /**
        The Geolocation API allows the user to provide their location to web applications 
        if they so desire. For privacy reasons, the user is asked for permission to report 
        location information.
    **/
    function geoFindMe() {
        var output = document.getElementById("out");

        if (!navigator.geolocation){
            output.innerHTML = "<p>Geolocation is not supported by your browser</p>";
            return;
        }

        function success(position) {
            var latitude  = position.coords.latitude;
            var longitude = position.coords.longitude;

            output.innerHTML = '<p>Latitude is ' + latitude + '° <br>Longitude is ' + longitude + '°</p>';

            var img = new Image();
            img.src = "https://maps.googleapis.com/maps/api/staticmap?center=" + latitude + "," + longitude + "&zoom=13&size=300x300&sensor=false";

            output.appendChild(img);
        }

        function error() {
            output.innerHTML = "Unable to retrieve your location";
        }

        output.innerHTML = "<p>Locating…</p>";

        navigator.geolocation.getCurrentPosition(success, error); //function to get the current position of the device
    }
</script>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the use of WebSocket API?

The **WebSocket API** is an advanced technology that makes it possible to open a two-way interactive communication session between the user\'s browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.

**Interfaces:**  

|Sl.No|   API      | Description    |
|-----|------------|----------------|
| 01. |WebSocket   |The primary interface for connecting to a WebSocket server and then sending and receiving data on the connection.|   
| 02. |CloseEvent  |The event sent by the WebSocket object when the connection closes.   |
| 03. |MessageEvent|The event sent by the WebSocket object when a message is received from the server.|

**Example**

```javascript
const socket = new WebSocket('ws://localhost:8080/');

// Connection established
socket.addEventListener('open', (event) => {
    socket.send('Hello Server!');
});

// Message received from server
socket.addEventListener('message', (event) => {
    console.log('Received:', event.data);
});

// Connection closed
socket.addEventListener('close', (event) => {
    console.log('Connection closed:', event.code);
});

// Error occurred
socket.addEventListener('error', (error) => {
    console.error('WebSocket error:', error);
});

// Close connection manually
socket.close();
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the MutationObserver API and when should you use it?

`MutationObserver` is a built-in browser API that lets you **watch for changes to the DOM** — additions/removals of nodes, attribute changes, and text content changes — and react asynchronously.

**Basic usage:**

```js
// Select the target node to observe
const target = document.getElementById("app");

// Create an observer instance with a callback
const observer = new MutationObserver((mutationsList) => {
  for (const mutation of mutationsList) {
    if (mutation.type === "childList") {
      console.log("Child nodes changed:", mutation.addedNodes, mutation.removedNodes);
    } else if (mutation.type === "attributes") {
      console.log(`Attribute "${mutation.attributeName}" changed`);
    } else if (mutation.type === "characterData") {
      console.log("Text content changed:", mutation.target.data);
    }
  }
});

// Start observing
observer.observe(target, {
  childList: true,      // Watch for added/removed child nodes
  subtree: true,        // Watch all descendants, not just direct children
  attributes: true,     // Watch for attribute changes
  attributeFilter: ["class", "data-state"], // Only these attributes
  characterData: true,  // Watch text node changes
});

// Stop observing when done (prevents memory leaks)
observer.disconnect();
```

**`MutationRecord` properties:**

| Property | Description |
|---|---|
| `type` | `"childList"`, `"attributes"`, or `"characterData"` |
| `target` | The node that changed |
| `addedNodes` | NodeList of added nodes |
| `removedNodes` | NodeList of removed nodes |
| `attributeName` | Changed attribute name (for `attributes` type) |
| `oldValue` | Previous value (if `attributeOldValue`/`characterDataOldValue` enabled) |

**When to use MutationObserver:**

- **Third-party DOM changes** — React when a library or extension modifies the DOM
- **Custom element lifecycle** — Detect when a component is added/removed
- **Lazy-init widgets** — Initialize a plugin when a container appears in DOM
- **Polling replacement** — Avoid `setInterval` DOM checks

```js
// Example: auto-initialize tooltips when data-tooltip is added
const observer = new MutationObserver((mutations) => {
  mutations.forEach(({ addedNodes }) => {
    addedNodes.forEach((node) => {
      if (node.nodeType === 1 && node.dataset.tooltip) {
        initTooltip(node);
      }
    });
  });
});

observer.observe(document.body, { childList: true, subtree: true });
```

> **Performance note:** MutationObserver callbacks are batched and run as microtasks after each rendering cycle — they're efficient and don\'t block the main thread.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the ResizeObserver API and how is it different from the `resize` window event?

`ResizeObserver` observes size changes on **individual elements**, whereas the `resize` window event only fires when the **browser window** itself resizes.

**Basic usage:**

```js
const observer = new ResizeObserver((entries) => {
  for (const entry of entries) {
    const { width, height } = entry.contentRect;
    console.log(`Element resized: ${width}px × ${height}px`);

    // Access border-box size (more accurate with padding/border)
    const [boxSize] = entry.borderBoxSize;
    console.log(`Border box: ${boxSize.inlineSize} × ${boxSize.blockSize}`);
  }
});

// Observe a specific element
observer.observe(document.getElementById("sidebar"));

// Unobserve when done
observer.unobserve(document.getElementById("sidebar"));

// Disconnect all observations
observer.disconnect();
```

**`ResizeObserverEntry` properties:**

| Property | Description |
|---|---|
| `target` | The observed element |
| `contentRect` | `DOMRectReadOnly` with `width`, `height`, `x`, `y` |
| `contentBoxSize` | Content box dimensions (array) |
| `borderBoxSize` | Border box dimensions (includes padding+border) |
| `devicePixelContentBoxSize` | Pixel-perfect device size |

**Use cases:**

```js
// Responsive chart — redraw when container changes size
const chartObserver = new ResizeObserver(([entry]) => {
  const { width } = entry.contentRect;
  redrawChart(width);
});
chartObserver.observe(document.getElementById("chart-container"));

// Container queries (before CSS container queries were widely supported)
const cardObserver = new ResizeObserver(([entry]) => {
  const el = entry.target;
  el.classList.toggle("compact", entry.contentRect.width < 300);
});
cardObserver.observe(document.querySelector(".card"));
```

**Difference from `window.resize`:**

| | `window.resize` event | `ResizeObserver` |
|---|---|---|
| Scope | Entire viewport | Any individual element |
| Trigger | Window resize only | Any size change (CSS, DOM, font changes) |
| Element level | No | Yes |
| Performance | Needs debouncing | Batched by browser automatically |

> Use `ResizeObserver` in modern apps instead of manual window resize + element dimension polling.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is `requestAnimationFrame` and why should you use it for animations?

`requestAnimationFrame` (rAF) tells the browser to call your function **just before the next repaint**, synchronized with the display refresh rate (typically 60Hz = ~16.7ms per frame). It\'s the correct tool for JavaScript-driven animations and visual updates.

**Basic usage:**

```js
let animationId;
let position = 0;
const box = document.getElementById("box");

function animate() {
  position += 2;
  box.style.transform = `translateX(${position}px)`;

  if (position < 400) {
    animationId = requestAnimationFrame(animate); // schedule next frame
  }
}

// Start
animationId = requestAnimationFrame(animate);

// Stop at any time
cancelAnimationFrame(animationId);
```

**Why rAF beats `setInterval`/`setTimeout` for animations:**

| | `setInterval` / `setTimeout` | `requestAnimationFrame` |
|---|---|---|
| Timing | Fixed timer — may not align with screen refresh | Synchronized with display refresh (60fps) |
| Background tabs | Continues running, wastes CPU | **Paused automatically** when tab is hidden |
| Frame skips | Can fire multiple times per frame or miss frames | Fires exactly once per frame |
| Battery drain | Higher | Lower — browser can optimize |
| Smooth animation | No — may cause jank | Yes — synchronized with rendering cycle |

**Timestamp argument for delta-time animations:**

```js
let start = null;
const duration = 1000; // 1 second
const distance = 300;

function animate(timestamp) {
  if (!start) start = timestamp;
  const elapsed = timestamp - start;
  const progress = Math.min(elapsed / duration, 1);

  box.style.transform = `translateX(${progress * distance}px)`;

  if (progress < 1) {
    requestAnimationFrame(animate);
  }
}

requestAnimationFrame(animate);
```

**`requestIdleCallback` — for non-visual background work:**

```js
// Run low-priority tasks when browser is idle (between frames)
requestIdleCallback((deadline) => {
  while (deadline.timeRemaining() > 0 && tasks.length > 0) {
    processTask(tasks.shift());
  }
}, { timeout: 2000 }); // Force run after 2s if still idle
```

> Use rAF for all visual/DOM updates, and `requestIdleCallback` for analytics, pre-computation, and non-urgent tasks to avoid blocking the main thread.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 13. HTML Drag and Drop

<br>

## Q. Explain Drag and Drop in HTML5?

HTML5 drag-and-drop uses the `DOM event model` and `drag events` inherited from `mouse events`. A typical drag operation begins when a user selects a draggable element, drags the element to a droppable element, and then releases the dragged element.

|Event	        |Description                                                            |
|---------------|-----------------------------------------------------------------------|
|Drag	        |It fires every time when the mouse is moved while the object is being dragged.|
|Dragstart	    |It is a very initial stage. It fires when the user starts dragging object.|
|Dragenter	    |It fires when the user moves his/her mouse cursur over the target element.|
|Dragover	    |This event is fired when the mouse moves over an element.|
|Dragleave	    |This event is fired when the mouse leaves an element.|
|Drop	        |Drop It fires at the end of the drag operation.|
|Dragend	    |It fires when user releases the mouse button to complete the drag operation.|

Example

```html
<!DOCTYPE HTML>
<html>
   <head>
   <script>
        function allowDrop(ev) {
            ev.preventDefault();
        }

        function drag(ev) {
            ev.dataTransfer.setData("text", ev.target.id);
        }

        function drop(ev) {
            ev.preventDefault();
            var data = ev.dataTransfer.getData("text");
            ev.target.appendChild(document.getElementById(data));
        }
    </script>
</head>
<body>
  <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
  <img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69">
</body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the DataTransfer object and how do you use it in drag and drop?

The `DataTransfer` object carries data during a drag-and-drop operation. It is available on `DragEvent` objects and allows you to store, retrieve, and control what data is being transferred.

**Key properties and methods:**

| Member | Description |
|---|---|
| `dataTransfer.setData(format, data)` | Store data with a MIME type key |
| `dataTransfer.getData(format)` | Retrieve stored data |
| `dataTransfer.clearData([format])` | Remove stored data |
| `dataTransfer.effectAllowed` | Defines allowed operations: `"copy"`, `"move"`, `"link"`, `"none"`, `"all"` |
| `dataTransfer.dropEffect` | The actual effect during dragover: `"copy"`, `"move"`, `"link"`, `"none"` |
| `dataTransfer.files` | `FileList` of files being dragged (from OS) |
| `dataTransfer.items` | `DataTransferItemList` for multi-item data |
| `dataTransfer.setDragImage(element, x, y)` | Set a custom drag image |

**Complete sortable list example:**

```html
<ul id="sortable">
  <li draggable="true" data-id="1">Item 1</li>
  <li draggable="true" data-id="2">Item 2</li>
  <li draggable="true" data-id="3">Item 3</li>
</ul>

<script>
  let draggedId;

  document.querySelectorAll("li[draggable]").forEach(item => {
    item.addEventListener("dragstart", (e) => {
      draggedId = e.target.dataset.id;
      e.dataTransfer.effectAllowed = "move";
      e.dataTransfer.setData("text/plain", draggedId);
      e.target.classList.add("dragging");
    });

    item.addEventListener("dragend", (e) => {
      e.target.classList.remove("dragging");
    });

    item.addEventListener("dragover", (e) => {
      e.preventDefault();               // Required to allow drop
      e.dataTransfer.dropEffect = "move";
    });

    item.addEventListener("drop", (e) => {
      e.preventDefault();
      const sourceId = e.dataTransfer.getData("text/plain");
      const target = e.currentTarget;
      const source = document.querySelector(`[data-id="${sourceId}"]`);
      if (source !== target) {
        target.parentNode.insertBefore(source, target);
      }
    });
  });
</script>
```

**Custom drag image:**

```js
element.addEventListener("dragstart", (e) => {
  const ghost = document.createElement("div");
  ghost.textContent = "Dragging...";
  ghost.style.cssText = "position:absolute;top:-1000px;background:#4a90d9;color:white;padding:8px;border-radius:4px;";
  document.body.appendChild(ghost);
  e.dataTransfer.setDragImage(ghost, 0, 0);
  // Clean up ghost after drag
  setTimeout(() => document.body.removeChild(ghost), 0);
});
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you handle file drag and drop in HTML5?

HTML5\'s drag-and-drop API combined with the File API allows users to drag files from the OS directly onto a web page for upload.

**Example — drag files onto a drop zone:**

```html
<div id="dropzone"
     style="width:300px;height:150px;border:2px dashed #aaa;display:flex;
            align-items:center;justify-content:center;font-family:sans-serif;">
  Drop files here
</div>
<ul id="file-list"></ul>

<script>
  const dropzone = document.getElementById("dropzone");
  const fileList = document.getElementById("file-list");

  // Prevent default browser behavior (open file in browser)
  ["dragenter", "dragover", "dragleave", "drop"].forEach(event => {
    dropzone.addEventListener(event, (e) => e.preventDefault());
    document.body.addEventListener(event, (e) => e.preventDefault());
  });

  // Visual feedback
  dropzone.addEventListener("dragover", () => {
    dropzone.style.borderColor = "#4a90d9";
    dropzone.style.background = "#e8f0fe";
  });

  dropzone.addEventListener("dragleave", () => {
    dropzone.style.borderColor = "#aaa";
    dropzone.style.background = "";
  });

  // Handle drop
  dropzone.addEventListener("drop", (e) => {
    dropzone.style.borderColor = "#aaa";
    dropzone.style.background = "";

    const files = e.dataTransfer.files; // FileList
    fileList.innerHTML = "";

    for (const file of files) {
      const li = document.createElement("li");
      li.textContent = `${file.name} (${(file.size / 1024).toFixed(1)} KB) — ${file.type}`;
      fileList.appendChild(li);
    }

    // Upload with FormData
    const formData = new FormData();
    for (const file of files) {
      formData.append("files[]", file);
    }
    // fetch("/upload", { method: "POST", body: formData });
  });
</script>
```

**Checking file types:**

```js
dropzone.addEventListener("drop", (e) => {
  const allowedTypes = ["image/jpeg", "image/png", "image/webp"];
  const files = Array.from(e.dataTransfer.files).filter(f =>
    allowedTypes.includes(f.type)
  );
  if (files.length === 0) {
    alert("Only JPEG, PNG, and WebP images are accepted.");
    return;
  }
  handleFiles(files);
});
```

> Always validate file type and size on the **server side** as well — client-side checks can be bypassed.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 14. HTML Web Worker

<br>

## Q. What is an HTML Web Worker and why is it needed?

A **Web Worker** is a JavaScript script that runs in a **background thread**, separate from the main browser thread. It allows long-running or CPU-intensive tasks to execute without blocking the UI — keeping the page responsive.

**The problem Web Workers solve:**

JavaScript is single-threaded. Any heavy computation runs on the main thread, which also handles rendering and user interactions. Long tasks freeze the UI:

```js
// Without Web Worker — blocks the UI
function heavyCalculation() {
  let result = 0;
  for (let i = 0; i < 10_000_000_000; i++) {
    result += i;
  }
  return result; // UI is frozen during this entire loop
}
```

**With a Web Worker — UI stays responsive:**

```js
// main.js
const worker = new Worker("worker.js");

worker.postMessage({ limit: 10_000_000_000 });

worker.onmessage = function(event) {
  console.log("Result:", event.data.result); // received when done
};
```

```js
// worker.js
self.onmessage = function(event) {
  let result = 0;
  for (let i = 0; i < event.data.limit; i++) {
    result += i;
  }
  self.postMessage({ result }); // send result back to main thread
};
```

**What Web Workers can and cannot do:**

| Can do | Cannot do |
|---|---|
| Perform heavy computations | Access the DOM |
| Make `fetch` / `XMLHttpRequest` calls | Access `window`, `document`, `parent` |
| Use `setTimeout` / `setInterval` | Manipulate UI elements directly |
| Use `IndexedDB` | Use `localStorage` (synchronous) |
| Import scripts via `importScripts()` | Use `alert()` / `confirm()` |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you create and communicate with a Web Worker?

Communication between the main thread and a Web Worker happens exclusively through **message passing** using `postMessage()` and `onmessage`.

**Step 1 — Create the worker file (`worker.js`):**

```js
// worker.js
self.onmessage = function(event) {
  const { numbers } = event.data;

  // Perform heavy work
  const sum = numbers.reduce((acc, n) => acc + n, 0);

  // Send result back to main thread
  self.postMessage({ sum });
};
```

**Step 2 — Use the worker in the main script:**

```js
// main.js
const worker = new Worker("worker.js");

// Send data to the worker
worker.postMessage({ numbers: [1, 2, 3, 4, 5] });

// Receive result from the worker
worker.onmessage = function(event) {
  console.log("Sum:", event.data.sum); // 15
};

// Handle errors
worker.onerror = function(error) {
  console.error("Worker error:", error.message);
};

// Terminate the worker when done
worker.terminate();
```

**Using `addEventListener` (alternative syntax):**

```js
worker.addEventListener("message", (event) => {
  console.log("Received:", event.data);
});

worker.addEventListener("error", (error) => {
  console.error("Error:", error);
});
```

**Inline worker using a Blob (no separate file needed):**

```js
const workerCode = `
  self.onmessage = function(e) {
    const result = e.data * 2;
    self.postMessage(result);
  };
`;

const blob = new Blob([workerCode], { type: "application/javascript" });
const worker = new Worker(URL.createObjectURL(blob));

worker.postMessage(21);
worker.onmessage = (e) => console.log(e.data); // 42
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the types of Web Workers?

There are three types of Web Workers, each serving a different use case:

**1. Dedicated Worker**

The most common type. Created with `new Worker()` and can only be accessed by the script that created it.

```js
const worker = new Worker("worker.js");
worker.postMessage("start");
```

**2. Shared Worker**

Can be accessed by **multiple scripts** across different windows, iframes, or tabs from the same origin. Uses a `port` for communication.

```js
// main.js (can be used in multiple tabs)
const sharedWorker = new SharedWorker("shared-worker.js");

sharedWorker.port.start();
sharedWorker.port.postMessage("hello");

sharedWorker.port.onmessage = (event) => {
  console.log("From shared worker:", event.data);
};
```

```js
// shared-worker.js
self.onconnect = function(event) {
  const port = event.ports[0];
  port.onmessage = function(e) {
    port.postMessage("Shared worker received: " + e.data);
  };
};
```

**3. Service Worker**

Acts as a **proxy between the browser and the network**. Used for caching, offline support, push notifications, and background sync. Registered separately and has a distinct lifecycle.

```js
// Register a service worker
if ("serviceWorker" in navigator) {
  navigator.serviceWorker.register("/sw.js")
    .then(() => console.log("Service Worker registered"))
    .catch((err) => console.error("Registration failed:", err));
}
```

**Comparison:**

| | Dedicated Worker | Shared Worker | Service Worker |
|---|---|---|---|
| Scope | Single page/script | Multiple tabs/windows | All pages on origin |
| Use case | Background computation | Shared state across tabs | Caching, offline, push |
| Communication | `postMessage` | Port-based `postMessage` | `fetch` events, `postMessage` |
| Lifecycle | Tied to creating page | Tied to connected pages | Persistent (independent) |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the lifecycle of a Web Worker?

A Web Worker goes through several stages from creation to termination:

**1. Creation**

A worker is created when the main script calls `new Worker("worker.js")`. The browser downloads, parses, and starts executing the worker script in a background thread.

```js
const worker = new Worker("worker.js"); // Worker created
```

**2. Running**

The worker listens for messages and processes tasks:

```js
// worker.js
self.onmessage = function(event) {
  // Process incoming messages
  const result = processData(event.data);
  self.postMessage(result);
};
```

**3. Termination**

A worker can be terminated in two ways:

**From the main thread:**
```js
worker.terminate(); // Immediately stops the worker
```

**From inside the worker itself:**
```js
// worker.js
self.close(); // Worker shuts itself down
```

**4. Error handling**

```js
// Catch errors in the main thread
worker.onerror = function(event) {
  console.error(`Error in ${event.filename}, line ${event.lineno}: ${event.message}`);
};
```

**Worker lifecycle summary:**

```
new Worker("worker.js")
        ↓
  Script downloaded
        ↓
  Script parsed & executed
        ↓
  Listening for messages  ←──────────────┐
        ↓                                │
  Receives message via onmessage         │
        ↓                                │
  Processes task                         │
        ↓                                │
  Sends result via postMessage() ────────┘
        ↓
  worker.terminate() or self.close()
        ↓
  Worker stopped & memory freed
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between a Web Worker and a Service Worker?

Both run in background threads but serve fundamentally different purposes:

| | Web Worker | Service Worker |
|---|---|---|
| **Primary purpose** | Offload CPU-intensive computation from the main thread | Act as a network proxy for caching, offline support, and push notifications |
| **Scope** | Tied to a single page | Registered for an entire origin (`/`) |
| **Lifecycle** | Lives as long as the page is open | Persists independently; can run after page is closed |
| **DOM access** | No | No |
| **Network interception** | No | Yes — intercepts `fetch` requests |
| **Cache API access** | Limited | Yes — primary use case |
| **Push notifications** | No | Yes |
| **Created with** | `new Worker()` | `navigator.serviceWorker.register()` |
| **Communication** | `postMessage` directly | `postMessage` via `navigator.serviceWorker` |

**Web Worker example (computation):**
```js
// Offload sorting a large dataset
const worker = new Worker("sort-worker.js");
worker.postMessage({ data: largeArray });
worker.onmessage = (e) => renderResults(e.data.sorted);
```

**Service Worker example (caching):**
```js
// sw.js — intercept all fetch requests
self.addEventListener("fetch", (event) => {
  event.respondWith(
    caches.match(event.request).then((cached) => {
      return cached || fetch(event.request);
    })
  );
});
```

**When to use which:**
- Use a **Web Worker** when you need to run JavaScript computation without freezing the UI (parsing, encryption, image processing).
- Use a **Service Worker** when you need offline support, background sync, or push notifications.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 15. HTML Accessibility

<br>

## Q. What ARIA and screenreaders are, and how to make a website accessible?

Screen readers are software programs that  provide assistive technologies that allow people with disabilities (such as no sight, sound or mouse-ing ability) to use web applications. You can make your sites more accessible by following ARIA standards such as semantic HTML, alt attributes and using [role=button] in the expected ways

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is accessibility & ARIA role means in a web application?

**Web Accessibility**

Web accessibility means designing and building websites so that people with disabilities can **perceive, understand, navigate, and interact** with them. This includes users who rely on:

- **Screen readers** (e.g., NVDA, JAWS, VoiceOver) — read page content aloud
- **Keyboard-only navigation** — no mouse
- **Switch devices** — for users with motor impairments
- **Braille displays**

**ARIA**

**ARIA (Accessible Rich Internet Applications)** is a set of HTML attributes defined by W3C\'s WAI-ARIA specification. It adds semantic meaning to elements so assistive technologies can understand them — especially for **dynamic content and custom widgets** that plain HTML doesn\'t describe well.

> ARIA does **not** change visual appearance or browser behavior. It only adds an extra layer of information for assistive technologies.

**Golden rule:** Use native semantic HTML first. Only add ARIA when HTML alone is insufficient.

**Example:**

```html
<!-- Prefer this (native semantics) -->
<button>Submit</button>

<!-- Over this (requires ARIA to be accessible) -->
<div role="button" tabindex="0">Submit</div>
```

**The Three Types of ARIA Attributes**

**1. Roles — What an element *is***

**Example:**

```html
<div role="navigation">...</div>
<div role="dialog">...</div>
<div role="alert">Error: Invalid input</div>
<span role="button" tabindex="0">Click me</span>
```

**2. Properties — Describe characteristics (static)**

**Example:**

```html
<!-- Labels the element -->
<input aria-label="Search" type="text">

<!-- Points to another element that labels this one -->
<h2 id="title">Login</h2>
<form aria-labelledby="title">...</form>

<!-- Describes with additional context -->
<input aria-describedby="hint">
<span id="hint">Must be at least 8 characters</span>

<!-- Marks required fields -->
<input aria-required="true">
```

**3. States — Dynamic values changed by JavaScript**

**Example:**

```html
<!-- Expanded/collapsed (accordion, dropdown) -->
<button aria-expanded="false">Menu</button>

<!-- Checkbox state -->
<div role="checkbox" aria-checked="true">Accept terms</div>

<!-- Hidden from screen readers -->
<div aria-hidden="true">Decorative icon</div>

<!-- Invalid form field -->
<input aria-invalid="true">

<!-- Disabled element -->
<button aria-disabled="true">Submit</button>
```

**ARIA Role Categories**

**1. Landmark Roles — Page regions for navigation**

**Example:**

```html
<header role="banner">...</header>
<nav role="navigation" aria-label="Main menu">...</nav>
<main role="main">...</main>
<aside role="complementary">...</aside>
<footer role="contentinfo">...</footer>
<form role="search">...</form>
```

**2. Widget Roles — Interactive UI components**

| Role | Use case |
|---|---|
| `button` | Clickable action element |
| `checkbox` | Toggleable input |
| `dialog` | Modal window |
| `tab` / `tabpanel` | Tab interface |
| `slider` | Range input |
| `progressbar` | Loading/progress indicator |
| `alert` | Important time-sensitive message |
| `tooltip` | Hover/focus hint |

**3. Live Region — Announce dynamic content changes**

**Example:**

```html
<!-- Screen reader announces changes automatically -->
<div aria-live="polite" aria-atomic="true">
  Cart updated: 3 items
</div>

<!-- For urgent alerts (interrupts current reading) -->
<div role="alert">
  Error: Session expired
</div>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is tabindex attribute and how does it affect keyboard navigation?

The `tabindex` attribute controls the order in which elements receive focus when the user navigates using the **Tab** key. It can be applied to any HTML element.

| Value | Behavior |
|---|---|
| `tabindex="0"` | Element is focusable in natural DOM order |
| `tabindex="-1"` | Focusable via JavaScript only (`element.focus()`), excluded from Tab sequence |
| `tabindex="n"` (positive) | Focused before elements with lower or no tabindex (avoid — breaks natural order) |

**Example:**

```html
<!-- Custom button accessible by keyboard -->
<div role="button" tabindex="0" onclick="doAction()">Click Me</div>

<!-- Skip link — focused programmatically, not via Tab -->
<a href="#main" tabindex="-1" id="skip">Skip to content</a>
```

**Best practice:** Use `tabindex="0"` to make custom interactive elements keyboard-accessible. Avoid positive tabindex values as they break the natural reading order for keyboard and screen reader users.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are skip navigation links and why are they important?

**Skip navigation links** (or "skip links") are hidden anchor links placed at the very top of a page that allow keyboard and screen reader users to jump past repetitive navigation blocks directly to the main content.

Without a skip link, keyboard users must Tab through every navigation item on every page load before reaching the content — a significant accessibility barrier.

**Implementation:**

```html
<!-- Place as the first element inside <body> -->
<a href="#main-content" class="skip-link">Skip to main content</a>

<nav>
  <!-- ...many nav links... -->
</nav>

<main id="main-content" tabindex="-1">
  <h1>Page Title</h1>
  <!-- page content -->
</main>
```

```css
.skip-link {
  position: absolute;
  left: -9999px;
  top: auto;
  width: 1px;
  height: 1px;
  overflow: hidden;
}

/* Become visible when focused */
.skip-link:focus {
  position: static;
  width: auto;
  height: auto;
}
```

*Note: `tabindex="-1"` on `<main>` ensures it can receive programmatic focus when the skip link is activated.*

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are ARIA live regions and when should you use them?

**ARIA live regions** announce dynamic content changes to screen reader users without requiring them to navigate to the changed area. This is critical for alerts, notifications, status messages, and any content that updates without a page reload.

**`aria-live` values:**

| Value | Behavior |
|---|---|
| `off` | No announcements (default) |
| `polite` | Announces after the user finishes current activity — does **not** interrupt |
| `assertive` | Interrupts the user immediately — use sparingly |

**Basic example:**

```html
<!-- Status messages (polite) -->
<div aria-live="polite" aria-atomic="true" id="status-message">
  <!-- Content injected here by JS will be announced -->
</div>

<button onclick="saveForm()">Save</button>

<script>
  function saveForm() {
    // ... save logic
    document.getElementById("status-message").textContent = "Form saved successfully.";
  }
</script>
```

**For errors/urgent alerts (assertive):**

```html
<div role="alert" aria-live="assertive" aria-atomic="true" id="error-message">
  <!-- Error messages here -->
</div>
```

> `role="alert"` implicitly sets `aria-live="assertive"` and `aria-atomic="true"`.

**`aria-atomic` and `aria-relevant`:**

```html
<!-- aria-atomic="true" → read the entire region, not just the changed part -->
<div aria-live="polite" aria-atomic="true">
  <span id="count">3</span> items in cart
</div>

<!-- aria-relevant: what changes trigger announcements -->
<!-- additions | removals | text | all (default: "additions text") -->
<div aria-live="polite" aria-relevant="additions removals">
  <!-- log of events -->
</div>
```

**Common roles that imply live regions:**

| Role | Equivalent live behavior |
|---|---|
| `role="alert"` | `aria-live="assertive"`, `aria-atomic="true"` |
| `role="status"` | `aria-live="polite"`, `aria-atomic="true"` |
| `role="log"` | `aria-live="polite"`, `aria-relevant="additions"` |
| `role="timer"` | `aria-live="off"` (announcements on demand) |
| `role="marquee"` | `aria-live="off"` |

**Best practices:**

1. Inject the live region into the DOM on page load (empty) — don\'t inject it dynamically when you need to announce.
2. Use `polite` by default; only use `assertive` for error messages and time-sensitive alerts.
3. Announce meaningful, concise messages — screen readers read exactly what\'s in the region.

```html
<!-- GOOD: Live region present in page from start -->
<div role="status" id="notification"></div>

<!-- Then update content dynamically -->
<script>
  document.getElementById("notification").textContent = "Your changes have been saved.";
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you manage focus in Single Page Applications (SPAs)?

In traditional multi-page apps, the browser automatically moves focus to the top of the page on navigation. SPAs update content without a page load, so focus management becomes the developer\'s responsibility — without it, keyboard and screen reader users get lost.

**The problem:**

```js
// User clicks "Go to About page" link
// SPA updates the DOM with new content
// But focus stays on the clicked link (which may now be gone or irrelevant)
// Screen reader doesn\'t know the page has changed
```

**Solution 1 — Focus the new page heading:**

```js
function navigateTo(pageId) {
  loadPage(pageId);

  // After DOM update, move focus to the main heading
  requestAnimationFrame(() => {
    const heading = document.querySelector("main h1");
    if (heading) {
      heading.setAttribute("tabindex", "-1");
      heading.focus();
    }
  });
}
```

**Solution 2 — Use a route announcement region:**

```html
<!-- Visually hidden, but announced by screen readers -->
<div role="status" aria-live="polite" class="sr-only" id="route-announcer"></div>
```

```js
function navigateTo(route) {
  loadPage(route);

  document.getElementById("route-announcer").textContent = `Navigated to ${route.title}`;
}
```

React Router, Next.js App Router, and Angular CDK Router all provide built-in focus management — but you may need to configure them explicitly.

**Solution 3 — Focus the main content container:**

```html
<main id="main-content" tabindex="-1">
  <!-- page content -->
</main>
```

```js
// After navigation
document.getElementById("main-content").focus();
```

**Focus management for modals and dialogs:**

```js
function openModal(modal) {
  modal.removeAttribute("hidden");

  // Save the element that triggered the modal
  previouslyFocused = document.activeElement;

  // Move focus into modal (first focusable element or close button)
  modal.querySelector("button, [tabindex]").focus();
}

function closeModal(modal) {
  modal.setAttribute("hidden", "");

  // Restore focus to the triggering element
  previouslyFocused?.focus();
}
```

**Focus trap for modals (keep Tab within modal while open):**

```js
function trapFocus(modal) {
  const focusable = modal.querySelectorAll(
    'a, button, input, select, textarea, [tabindex]:not([tabindex="-1"])'
  );
  const first = focusable[0];
  const last = focusable[focusable.length - 1];

  modal.addEventListener("keydown", (e) => {
    if (e.key !== "Tab") return;
    if (e.shiftKey && document.activeElement === first) {
      e.preventDefault();
      last.focus();
    } else if (!e.shiftKey && document.activeElement === last) {
      e.preventDefault();
      first.focus();
    }
  });
}
```

> For production SPA accessibility, use the `@angular/cdk/a11y` FocusTrap, React\'s `focus-trap-react`, or the `<dialog>` element (which manages focus natively in modern browsers).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 16. Miscellaneous

<br>

## Q. How to use data- attribute in html5?

Any attribute on any element whose attribute name starts with **data-** is a data attribute. The data-* attributes gives us the ability to embed custom data attributes on all HTML elements. The stored (custom) data can then be used in the page\'s JavaScript to create a more engaging user experience.

**Example:**

```html
<article
  id="electric-cars"
  data-columns="10"
  data-index-number="100"
  data-parent="cars"
>
  <h1>Electric Cars</h1>
</article>
```

```js
/**
 * Access data attribute
 */
const article = document.getElementById("electric-cars");

article.dataset.columns; // "10"
article.dataset.indexNumber; // "100"
article.dataset.parent; // "cars"
```

**&#9885; [Try this example on CodeSandbox](https://codesandbox.io/s/html-data-attribute-llxlkn?file=/script.js)**

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the purpose of the `alt` attribute on images?

The `alt` attribute provides alternative information for an image if a user cannot view it. The `alt` attribute should be used to describe any images except those which only serve a decorative purposes, in which case it should be left empty.

```html
<img src="pancakes.png" alt="Stack of blueberry pancakes with powdered sugar">
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain some of the pros and cons for CSS animations versus JavaScript animations?

Regarding optimization and responsiveness the debate bounces back and forth but, the concept is:

* CSS animations allows the browser to choose where the animation processing is done, CPU or the GPU. (Central or Graphics Processing Unit)

* That said, adding many layers to a document will eventually have a performance hit.

* JS animation means more code for the user to download and for the developer to maintain.

* Applying multiple animation types on an element is harder with CSS since all transforming power is in one property transform

* CSS animations being declarative are not programmable therefore limited in capability.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to improve the page load?

Here are the key techniques to improve page load performance:

**Reduce HTTP Requests**
- Combine JS files into one, CSS files into one
- Use CSS sprites to merge multiple images into a single file
- Remove duplicate scripts

**Assets & Delivery**
- Use a **CDN** — serves content from servers geographically closer to users
- **Gzip** compression — reduces HTTP response size by ~70%
- Minify JavaScript and CSS
- Make JS and CSS external so browsers can cache them

**Script & Style Placement**
- Put `<link>` stylesheets in `<head>` — enables progressive rendering
- Put `<script>` tags at the bottom of `<body>`, or use `async`/`defer`

```html
<script defer src="myscript.js"></script>   <!-- executes after HTML parsed -->
<script async src="analytics.js"></script>  <!-- loads in parallel -->
```

**Caching**
- Set `Expires` / `Cache-Control` headers on static assets
- Use `localStorage` to cache data client-side
- Configure ETags
- Use **cache busting** (`script.js?v=2`) when assets change

**Images**
- Compress and optimize images
- Don\'t scale images in HTML (serve correct size)
- Use lazy loading for off-screen images

**Network & DNS**
- Use `dns-prefetch` to resolve domains early:
```html
<link rel="dns-prefetch" href="//example.com">
```
- Reduce DNS lookups
- Avoid redirects
- Eliminate 404 errors (wasted HTTP requests)
- Keep cookie size small
- Use GET instead of POST for AJAX (single TCP packet)

**DOM**
- Reduce the number of DOM elements
- Minimize DOM access in JavaScript
- Minimize number of iframes

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to improve website performance?

Here\'s a comprehensive breakdown of ways to improve website performance:

**1. Minimize HTTP Requests**
- Combine multiple JS files into one, CSS files into one
- Use **CSS Sprites** — merge background images into a single image, use `background-position` to display segments
- Remove duplicate scripts

**2. Use a CDN (Content Delivery Network)**
- Serves content from geographically closer servers to users, significantly improving load times

**3. Optimize Images**
- Reduce resolution/quality to lower file size
- Compress images
- Crop to remove unnecessary areas
- Don\'t scale images in HTML — serve the correct size
- Optimize CSS sprites
- Make `favicon.ico` small and cacheable
- Avoid empty `src` attributes on `<img>`

**4. Script & Stylesheet Placement**
- Put stylesheets in `<head>` — enables progressive rendering
- Put scripts at the bottom of `<body>`, or use `async`/`defer`
- Avoid CSS expressions

**5. Caching & Compression**
- Add `Expires` or `Cache-Control` headers to make components cacheable
- Enable **Gzip** compression — reduces response size by ~70%
- Configure ETags
- Make Ajax cacheable

**6. JavaScript & CSS**
- Use external JS/CSS files (cached by browser vs. re-downloaded inline each time)
- Minify JavaScript and CSS
- Use **GET** for AJAX requests (single TCP packet vs. POST\'s two-step process)

**7. Network**
- Reduce DNS lookups
- Avoid redirects
- Eliminate 404 errors (wasted HTTP round-trips)
- Reduce cookie size (cookies sent with every HTTP request)

**8. Loading Strategy**
- Post-load non-critical components
- Preload components needed for next navigation
- Reduce number of DOM elements
- Minimize iframes
- Minimize DOM access in JavaScript

**Quick reference summary:**

| Category | Technique |
|---|---|
| Network | CDN, DNS prefetch, avoid redirects |
| Assets | Minify, Gzip, cache headers |
| Images | Compress, correct size, sprites |
| Scripts | `defer`/`async`, external files, bottom of body |
| Requests | Combine files, remove 404s, reduce cookies |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is desktop first and mobile first design approach?

Both are responsive design strategies that differ in **which screen size you design for first** and how you write your CSS media queries.

**Desktop First**

Start by designing for large desktop screens, then use `max-width` media queries to scale down for smaller devices.

```css
/* Default styles target desktop */
.container {
    width: 1200px;
    display: flex;
}

/* Override for smaller screens */
@media screen and (max-width: 768px) {
    .container {
        width: 100%;
        flex-direction: column;
    }
}
```

**Mobile First**

Start by designing for small mobile screens, then use `min-width` media queries to enhance the layout for larger screens.

```css
/* Default styles target mobile */
.container {
    width: 100%;
    flex-direction: column;
}

/* Override for larger screens */
@media screen and (min-width: 768px) {
    .container {
        width: 1200px;
        flex-direction: row;
    }
}
```

**Key Differences:**

| | Desktop First | Mobile First |
|---|---|---|
| Default styles target | Large screens | Small screens |
| Media query type | `max-width` | `min-width` |
| CSS loaded on mobile | Full desktop CSS + overrides | Only what\'s needed |
| Performance on mobile | Worse | Better |
| Industry preference | Legacy approach | Modern standard |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are `data-` attributes good for?

`data-*` attributes let you store custom data directly on HTML elements without using non-standard attributes or extra DOM properties.

**When to use them:**
- When you need to store extra information on an element that has no appropriate HTML attribute
- To pass data from server-rendered HTML to JavaScript without extra API calls
- To drive behavior in JavaScript/CSS without polluting class names

**HTML syntax:**
```html
<button
  data-user-id="42"
  data-role="admin"
  data-action="delete"
>
  Delete User
</button>
```

**Access in JavaScript via `dataset`:**
```js
const btn = document.querySelector("button");

btn.dataset.userId;   // "42"      (note: camelCase)
btn.dataset.role;     // "admin"
btn.dataset.action;   // "delete"
```

**Access in CSS:**
```css
/* Style based on data attribute value */
[data-role="admin"] {
    background-color: red;
}

/* Use content in pseudo-elements */
button::after {
    content: attr(data-action);
}
```

**Common use cases:**

| Use case | Example |
|---|---|
| Store IDs for JS operations | `data-product-id="123"` |
| Configuration for widgets | `data-toggle="modal"` |
| Track state | `data-expanded="true"` |
| Pass server data to JS | `data-api-url="/api/users"` |
| Analytics tracking | `data-track-event="click"` |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to make page responsive?

Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones).

**1. Viewport meta tag:**

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

**2. Responsive Images:**

If the CSS width property is set to 100%, the image will be responsive and scale up and down

```html
<!-- Scales with container -->
<img src="photo.jpg" style="max-width: 100%; height: auto;">

<!-- Serve different image per screen size -->
<picture>
  <source srcset="small.jpg" media="(max-width: 600px)">
  <source srcset="large.jpg" media="(min-width: 601px)">
  <img src="large.jpg" alt="Photo">
</picture>
```

**3. Fluid layouts:**

Use `%`, `vw`, `fr` units instead of fixed `px`:

```css
.column { width: 48%; }        /* percentage */
.hero   { width: 100vw; }      /* viewport width */
```

**4. Media Queries:**

Using media queries you can define completely different styles for different browser sizes.

```css
/* Mobile first: base styles for small screens */
.container { width: 100%; }

/* Tablet and up */
@media (min-width: 768px) {
    .container { width: 750px; }
}

/* Desktop and up */
@media (min-width: 1024px) {
    .container { width: 960px; }
}
```

**5. CSS Flexbox and Grid**

Built-in responsiveness with minimal media queries:

```css
/* Flexbox — wraps automatically */
.row { display: flex; flex-wrap: wrap; }

/* Grid — auto-fills columns based on available space */
.grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); }
```
<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Explain Microdata in HTML5?

Microdata is a standardized way to provide additional semantics in web pages. Microdata lets you define your own customized elements and start embedding custom properties in your web pages. At a high level, microdata consists of a group of name-value pairs.

The groups are called **items**, and each name-value pair is a **property**. Items and properties are represented by regular elements. Search engines benefit greatly from direct access to this structured data because it allows search engines to understand the information on web pages and provide more 
relevant results to users.

At a high level, microdata consists of a group of name-value pairs
* **itemscope**:- To create an item
* **itemprop**:- To add a property to an item

Example

```html
<div itemscope>
    <p>My name is <span itemprop="name">Elizabeth</span>.</p>
</div>

<div itemscope>
    <p>My name is <span itemprop="name">Daniel</span>.</p>
</div>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How can I get indexed better by search engines?

HTML tags are used to influence the way our pages appear in search results. With the help of certain tags, we can turn regular search snippets into rich snippets, and maybe even into featured snippets. And, as our search snippets get more advanced, they are able to secure better **Search Engine Results Pages (SERP)** positions and attract more traffic.

Here are all the HTML tags that still matter:

**1. Title tag:**

Title tags are used by search engines to determine the subject of a page and display it in SERP. As a rule of thumb, titles that are under 60 characters long will fit on most screens. In HTML, a title tag looks like this:

```html
<title>Your Title Goes Here</title>
```

**2. Meta description tag:**

Meta description is a short paragraph of text used to describe your page in search results. The function of meta description is similar to the title. It provides a little more detail about your page and it helps users decide whether to visit your page or not. In HTML, a meta description tag looks like this:

```html
<meta name="description" content="Your description goes here">
```

**3. Heading tags:**

Headings (h1-h6) are used to split your page into sections or chapters. Each heading is like a small title within the page. In HTML, a heading looks like this:

```html
<h1>Your heading goes here</h1>
```

**4. Image `alt` attribute:**

The `alt` text attribute is a part of an image tag, and it provides a description for an image. Alt text plays a major role in image optimization. It makes your images accessible both to search engines (by telling them what a particular image means) and to people (by displaying an alternative text in case a particular image cannot be loaded or by helping screen readers convey images). In HTML it may look like this:

```html
<img src="url" alt="Your image description goes here">
```

**5. Open Graph tags:**

Open Graph (OG) tags are placed in the `<head>` section of a page and allow any webpage to become a rich object in social networks. OG tags let you control how the information about your page is represented when shared via social channels. This possibility may help you enhance the performance of your links on social media, thus driving more click-throughs and increasing conversions. In HTML, it can look like this:

```html
<meta property="og:title" content="Your Page Title">
<meta property="og:description" content="Page description">
```

**6. Robots meta tag:**

A robots meta tag is an element in the HTML of a page that informs search engines which pages on your site should be indexed and which should not. Its functions are similar to robots.txt, but robots.txt gives suggestions. Whereas robots tags give instructions. In HTML, it can look like this:

```html
<meta name="robots" content="index, follow">
```

**7. Canonical tag:**

A canonical tag is a way of telling search engines that a specific URL represents the master copy of a page. Using the canonical tag prevents problems caused by identical or "duplicate" content appearing on multiple URLs. Practically speaking, the canonical tag tells search engines which version of a URL you want to appear in search results. In HTML, it may look like this:

```html
<link rel="canonical" href="https://example.com/page">
```

**8. HTML5 semantic tags:**

One of the most important features of HTML5 is its semantics tags. Semantic tags refers to syntax that makes the HTML more comprehensible by better defining the different sections and layout of web pages. It makes web pages more informative and adaptable, allowing browsers and search engines to better interpret content. For example, instead of using `<div id="header"></div>` you can use a `<header></hrader>` tag.

<p align="center">
    <img src="assets/images/semantic-tags.png" alt="HTML5 semantic tags" width="300px" />
</p>

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Why you would use a srcset attribute in an image tag?

The `srcset` attribute allows to define a list of different image resources along with size information so that browser can pick the most appropriate image based on the actual device\'s resolution.

`srcset` lets you provide multiple image versions and let the browser pick the best one for the current device automatically.

The Two Ways to Use `srcset`

**1. Using display density descriptor(`x`):**

`srcset` provides a comma-separated list of image resources along with display density it should be used, for example1x, 2x etc.

**Example:**

```html
<img 
  src="logo.png"
  srcset="logo.png 1x,
          logo@2x.png 2x,
          logo@3x.png 3x"
  alt="Logo"
>
```

| Descriptor | Meaning |
|---|---|
| `1x` | Standard screen (96 DPI) |
| `2x` | Retina/HiDPI screen (192 DPI) |
| `3x` | Very high-density screen (e.g., some Android phones) |

**2. Using Width Descriptor(`w`):**

The syntax is similar to the display density descriptor, but instead of display density values, we provide the actual width of the image.

**Example:**

```html
<img
  src="photo-800.jpg"
  srcset="photo-400.jpg 400w,
          photo-800.jpg 800w,
          photo-1200.jpg 1200w"
  sizes="(max-width: 600px) 100vw,
         (max-width: 1024px) 50vw,
         800px"
  alt="A landscape photo"
>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. Create a traffic signal light in html?

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Traffic Signal</title>
  <style>
    .container { 
      background: #333; 
      padding: 10px; 
      width: fit-content; 
      border-radius: 10px; 
    }
    .signal {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      margin: 10px;
      opacity: 0.2; /* Dim by default */
      transition: opacity 0.3s;
    }
    /* Only full brightness when active */
    .red.active    { background-color: red;    opacity: 1; box-shadow: 0 0 20px red; }
    .yellow.active { background-color: yellow; opacity: 1; box-shadow: 0 0 20px yellow; }
    .green.active  { background-color: green;  opacity: 1; box-shadow: 0 0 20px green; }
  </style>
</head>
<body>

  <div class="container">
    <div id="red"    class="signal red"></div>
    <div id="yellow" class="signal yellow"></div>
    <div id="green"  class="signal green"></div>
  </div>

  <script>
    const signals = {
      red:    document.getElementById("red"),
      yellow: document.getElementById("yellow"),
      green:  document.getElementById("green")
    };

    // Helper to wait
    const wait = (ms) => new Promise(resolve => setTimeout(resolve, ms));

    async function startTrafficCycle() {
      while (true) { // Infinite loop
        // Green
        setLight('green');
        await wait(5000);

        // Yellow
        setLight('yellow');
        await wait(2000);

        // Red
        setLight('red');
        await wait(5000);
      }
    }

    function setLight(color) {
      // Remove 'active' from everyone, add to the target
      Object.values(signals).forEach(el => el.classList.remove('active'));
      signals[color].classList.add('active');
    }

    startTrafficCycle();
  </script>
</body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 17. HTML Media

<br/>

## Q. How to use the HTML5 `<video>` element?

The `<video>` element embeds a media player that supports video playback directly in the browser without requiring any plugin.

**Attributes:**

| Attribute | Description |
|---|---|
| `src` | URL of the video file |
| `controls` | Show browser\'s built-in play/pause/volume controls |
| `autoplay` | Start playback automatically (requires `muted` in most browsers) |
| `muted` | Mute audio by default |
| `loop` | Restart video when it ends |
| `poster` | Image to show before the video plays |
| `preload` | `none` / `metadata` / `auto` — hints how much to preload |
| `width` / `height` | Dimensions in pixels |

**Example — Basic video with fallback sources:**

```html
<video width="640" height="360" controls poster="thumbnail.jpg">
  <source src="video.mp4"  type="video/mp4">
  <source src="video.webm" type="video/webm">
  <source src="video.ogv"  type="video/ogg">
  <p>Your browser does not support HTML5 video. 
     <a href="video.mp4">Download the video</a>.
  </p>
</video>
```

**Example — Autoplay muted loop (common for hero videos):**

```html
<video autoplay muted loop playsinline>
  <source src="hero.mp4" type="video/mp4">
</video>
```

**Controlling via JavaScript:**

```js
const video = document.getElementById("myVideo");

video.play();          // Start playback
video.pause();         // Pause
video.currentTime = 0; // Seek to start
video.volume = 0.5;    // Set volume (0–1)
video.playbackRate = 2; // 2× speed

// Events
video.addEventListener("ended", () => console.log("Video finished"));
video.addEventListener("timeupdate", () => console.log(video.currentTime));
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to use the HTML5 `<audio>` element?

The `<audio>` element embeds sound content such as music, podcasts, or sound effects.

**Attributes:**

| Attribute | Description |
|---|---|
| `src` | URL of the audio file |
| `controls` | Show browser\'s built-in controls |
| `autoplay` | Start playback automatically |
| `muted` | Mute audio by default |
| `loop` | Repeat when finished |
| `preload` | `none` / `metadata` / `auto` |

**Supported formats:**

| Format | MIME type | Browser support |
|---|---|---|
| MP3 | `audio/mpeg` | All modern browsers |
| OGG | `audio/ogg` | Firefox, Chrome, Opera |
| WAV | `audio/wav` | All modern browsers |
| AAC | `audio/aac` | Chrome, Edge, Safari |
| WebM | `audio/webm` | Chrome, Firefox, Edge |

**Example — with multiple fallback sources:**

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  <source src="audio.ogg" type="audio/ogg">
  <source src="audio.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>
```

**Controlling via JavaScript:**

```js
const audio = new Audio("audio.mp3");

audio.play();
audio.pause();
audio.volume = 0.8;

audio.addEventListener("ended", () => {
  console.log("Audio finished");
});
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<picture>` element and how does it work?

The `<picture>` element provides multiple image sources so the browser can choose the most appropriate one based on screen size, resolution, or format support. It is the recommended way to serve **art-directed** or **format-switched** responsive images.

**Syntax:**

```html
<picture>
  <source media="..." srcset="...">
  <source type="..."  srcset="...">
  <img src="fallback.jpg" alt="Description">
</picture>
```

The `<img>` inside is **required** — it serves as the fallback for browsers that don\'t support `<picture>`.

**Use Case 1 — Art direction (different crop per screen):**

```html
<picture>
  <!-- Wide landscape crop for desktop -->
  <source media="(min-width: 1024px)" srcset="hero-wide.jpg">
  <!-- Square crop for tablet -->
  <source media="(min-width: 600px)"  srcset="hero-square.jpg">
  <!-- Tight portrait crop for mobile (fallback) -->
  <img src="hero-mobile.jpg" alt="Team photo">
</picture>
```

**Use Case 2 — Modern format with fallback:**

```html
<picture>
  <source srcset="photo.avif" type="image/avif">
  <source srcset="photo.webp" type="image/webp">
  <img src="photo.jpg" alt="Photo" loading="lazy">
</picture>
```

The browser uses the first `<source>` it supports — e.g., AVIF → WebP → JPEG.

**Difference between `<picture>` and `srcset`:**

| | `srcset` on `<img>` | `<picture>` |
|---|---|---|
| Purpose | Resolution/density switching | Art direction + format switching |
| Browser picks | Best resolution match | First supported `<source>` |
| Control | Browser decides | Developer specifies conditions |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to add subtitles and captions to an HTML5 video?

The `<track>` element is used inside `<video>` to provide timed text tracks such as subtitles, captions, chapters, and metadata.

**Attributes of `<track>`:**

| Attribute | Description |
|---|---|
| `src` | URL of the `.vtt` (WebVTT) or `.srt` subtitle file |
| `kind` | `subtitles` / `captions` / `descriptions` / `chapters` / `metadata` |
| `srclang` | Language of the track (e.g., `en`, `fr`) |
| `label` | Human-readable label shown in the browser UI |
| `default` | Enables this track by default |

**Difference between subtitles and captions:**
- **Subtitles** — translate dialogue for users who don\'t speak the language
- **Captions** — include dialogue + sound effects for deaf/hard-of-hearing users

**Example:**

```html
<video controls width="640">
  <source src="movie.mp4" type="video/mp4">

  <track src="subtitles-en.vtt" kind="subtitles" srclang="en" label="English" default>
  <track src="subtitles-fr.vtt" kind="subtitles" srclang="fr" label="Français">
  <track src="captions-en.vtt"  kind="captions"  srclang="en" label="English Captions">
</video>
```

**Sample WebVTT file (`subtitles-en.vtt`):**

```
WEBVTT

00:00:01.000 --> 00:00:04.000
Hello, welcome to the tutorial.

00:00:05.000 --> 00:00:09.500
In this video we will cover HTML5 media elements.
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 18. HTML5 Advanced APIs

<br/>

## Q. What is the Server-Sent Events (SSE) API?

**Server-Sent Events (SSE)** is a server push technology that enables a server to send real-time updates to the browser over a single, long-lived HTTP connection. Unlike WebSockets, SSE is **one-directional** — server to client only — and automatically reconnects if the connection is lost.

**When to use SSE vs WebSockets:**

| | SSE | WebSocket |
|---|---|---|
| Direction | Server → Client only | Full duplex (both directions) |
| Protocol | HTTP/HTTPS | ws:// / wss:// |
| Auto-reconnect | Yes (built-in) | No (must implement manually) |
| Format | Text (UTF-8) | Text or binary |
| Use case | Live feeds, notifications, dashboards | Chat, gaming, collaboration |

**Client-side (browser):**

```js
const source = new EventSource("/api/stream");

// Listen for default message events
source.onmessage = (event) => {
  console.log("Data:", event.data);
};

// Listen for named custom events
source.addEventListener("update", (event) => {
  console.log("Update received:", event.data);
});

// Handle errors
source.onerror = (error) => {
  console.error("SSE error:", error);
  // Browser will automatically retry
};

// Close connection
source.close();
```

**Server-side (Node.js example):**

```js
const http = require("http");

http.createServer((req, res) => {
  if (req.url === "/api/stream") {
    res.writeHead(200, {
      "Content-Type":  "text/event-stream",
      "Cache-Control": "no-cache",
      "Connection":    "keep-alive"
    });

    // Send a message every second
    const interval = setInterval(() => {
      const data = JSON.stringify({ time: new Date().toISOString() });
      res.write(`data: ${data}\n\n`);
    }, 1000);

    // Clean up when client disconnects
    req.on("close", () => clearInterval(interval));
  }
}).listen(3000);
```

**SSE message format:**

```
data: Hello World\n\n          ← simple message

event: update\n                ← named event
data: {"value": 42}\n\n

id: 1\n                        ← message ID (used for reconnect)
data: Message with ID\n\n

retry: 5000\n\n                ← ask client to retry after 5s
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the Intersection Observer API?

The **Intersection Observer API** provides an asynchronous way to observe changes in the intersection (visibility) of a target element with its ancestor or the viewport. It is the recommended approach for implementing lazy loading, infinite scrolling, and animation triggers — replacing expensive scroll event listeners.

**Core concepts:**

- **root** — the ancestor element used as the viewport (defaults to browser viewport)
- **rootMargin** — margin around the root (like CSS `margin`)
- **threshold** — percentage of the target visible before the callback fires (0.0 to 1.0)

**Example — Lazy load images:**

```html
<img data-src="photo.jpg" alt="Photo" class="lazy">
```

```js
const observer = new IntersectionObserver((entries, observer) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      const img = entry.target;
      img.src = img.dataset.src;       // Load the actual image
      img.classList.remove("lazy");
      observer.unobserve(img);         // Stop observing once loaded
    }
  });
}, {
  root: null,        // browser viewport
  rootMargin: "0px",
  threshold: 0.1     // trigger when 10% of image is visible
});

document.querySelectorAll(".lazy").forEach(img => observer.observe(img));
```

**Example — Animate elements on scroll:**

```js
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add("animate");
    }
  });
}, { threshold: 0.2 });

document.querySelectorAll(".fade-in").forEach(el => observer.observe(el));
```

**Benefits over scroll event listeners:**

| | Scroll Event | Intersection Observer |
|---|---|---|
| Performance | Fires on every scroll tick (main thread) | Async, off main thread |
| Throttling | Must implement manually | Built-in |
| Viewport detection | Complex calculations needed | Built-in |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the History API in HTML5?

The **History API** (`window.history`) enables JavaScript to manipulate the browser\'s session history — adding or modifying history entries — without reloading the page. This is the foundation of **Single Page Applications (SPAs)**.

**Key methods:**

| Method | Description |
|---|---|
| `history.pushState(state, title, url)` | Add a new history entry |
| `history.replaceState(state, title, url)` | Replace the current history entry |
| `history.back()` | Go back one step (same as browser back button) |
| `history.forward()` | Go forward one step |
| `history.go(n)` | Jump `n` steps (`-1` = back, `2` = forward two) |
| `history.length` | Number of entries in the session history |

**Example — SPA-style navigation:**

```js
// Navigate to /users without page reload
history.pushState({ page: "users" }, "Users", "/users");

// Navigate to /users/42
history.pushState({ page: "user", id: 42 }, "User 42", "/users/42");

// Replace current URL (no new history entry)
history.replaceState({ page: "home" }, "Home", "/");
```

**Handling the browser back/forward button:**

```js
// popstate fires when user clicks back/forward
window.addEventListener("popstate", (event) => {
  console.log("State:", event.state); // { page: "users" }
  // Render the correct content based on event.state or location.pathname
  renderPage(event.state);
});
```

**Example — Complete SPA routing pattern:**

```js
function navigate(path, state = {}) {
  history.pushState(state, "", path);
  renderPage(path);
}

window.addEventListener("popstate", (e) => {
  renderPage(location.pathname);
});

function renderPage(path) {
  switch (path) {
    case "/":       document.getElementById("app").innerHTML = "<h1>Home</h1>"; break;
    case "/about":  document.getElementById("app").innerHTML = "<h1>About</h1>"; break;
    default:        document.getElementById("app").innerHTML = "<h1>404</h1>";
  }
}
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the Notification API?

The **Notification API** allows web applications to display system-level notifications to the user outside the browser tab — even when the browser is minimized, as long as it is running.

**Permission lifecycle:**

```js
// 1. Request permission (must be triggered by user gesture)
Notification.requestPermission().then(permission => {
  console.log(permission); // "granted" | "denied" | "default"
});

// 2. Check current permission
console.log(Notification.permission); // "granted" | "denied" | "default"
```

**Creating a notification:**

```js
if (Notification.permission === "granted") {
  const notification = new Notification("New Message!", {
    body:  "You have a new message from Alice.",
    icon:  "/icons/chat.png",
    badge: "/icons/badge.png",
    tag:   "message-1",        // Replaces previous notification with same tag
    silent: false,
    requireInteraction: true   // Stays until user dismisses it
  });

  // Events
  notification.onclick = () => {
    window.focus();
    notification.close();
  };

  notification.onclose = () => console.log("Notification closed");
  notification.onerror = (e) => console.error("Error:", e);

  // Auto-close after 5 seconds
  setTimeout(() => notification.close(), 5000);
}
```

**Full example with permission request:**

```js
async function sendNotification(title, options) {
  if (!("Notification" in window)) {
    console.log("Browser does not support notifications");
    return;
  }

  let permission = Notification.permission;

  if (permission === "default") {
    permission = await Notification.requestPermission();
  }

  if (permission === "granted") {
    new Notification(title, options);
  }
}

sendNotification("Hello!", { body: "Welcome back.", icon: "/logo.png" });
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the File API in HTML5?

The **File API** provides a way to read and interact with files that users select via `<input type="file">` or drag-and-drop, entirely on the client side — without uploading to a server.

**Key interfaces:**

| Interface | Description |
|---|---|
| `File` | Represents a single file; extends `Blob` |
| `FileList` | Array-like list of `File` objects from an `<input>` |
| `FileReader` | Reads the content of a `File` or `Blob` asynchronously |
| `Blob` | Raw binary data; `File` is a specialized `Blob` |

**Example — Read a text file:**

```html
<input type="file" id="fileInput" accept=".txt">
```

```js
document.getElementById("fileInput").addEventListener("change", (event) => {
  const file = event.target.files[0];

  if (!file) return;

  console.log("Name:", file.name);
  console.log("Size:", file.size, "bytes");
  console.log("Type:", file.type);
  console.log("Last modified:", new Date(file.lastModified));

  const reader = new FileReader();

  reader.onload = (e) => {
    console.log("Content:", e.target.result);
  };

  reader.onerror = () => console.error("Error reading file");

  reader.readAsText(file);         // Read as text
  // reader.readAsDataURL(file);   // Read as base64 Data URL (for images)
  // reader.readAsArrayBuffer(file); // Read as binary ArrayBuffer
});
```

**Example — Preview an uploaded image:**

```html
<input type="file" id="imageInput" accept="image/*">
<img id="preview" src="" alt="Preview">
```

```js
document.getElementById("imageInput").addEventListener("change", (event) => {
  const file = event.target.files[0];
  if (!file) return;

  const reader = new FileReader();
  reader.onload = (e) => {
    document.getElementById("preview").src = e.target.result;
  };
  reader.readAsDataURL(file);
});
```

**FileReader methods:**

| Method | Returns |
|---|---|
| `readAsText(file)` | String (UTF-8 by default) |
| `readAsDataURL(file)` | Base64 data URL string |
| `readAsArrayBuffer(file)` | ArrayBuffer (raw binary) |
| `readAsBinaryString(file)` | Binary string (deprecated) |
| `abort()` | Cancel the read |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is MathML and how is it used in HTML5?

**MathML (Mathematical Markup Language)** is an XML-based markup language for describing mathematical notation. It is natively supported inside HTML5 using the `<math>` element, allowing mathematical expressions to be rendered by the browser without images or JavaScript libraries.

**Two types of MathML:**

1. **Presentation MathML** — controls how math *looks* (most commonly used)
2. **Content MathML** — describes the mathematical *meaning*

**Example — Inline math (within text):**

```html
<p>The quadratic formula is 
  <math>
    <mrow>
      <mi>x</mi>
      <mo>=</mo>
      <mfrac>
        <mrow>
          <mo>-</mo><mi>b</mi>
          <mo>&#xB1;</mo>
          <msqrt>
            <mrow>
              <msup><mi>b</mi><mn>2</mn></msup>
              <mo>-</mo>
              <mn>4</mn><mi>a</mi><mi>c</mi>
            </mrow>
          </msqrt>
        </mrow>
        <mrow><mn>2</mn><mi>a</mi></mrow>
      </mfrac>
    </mrow>
  </math>
</p>
```

**Common MathML elements:**

| Element | Description | Example |
|---|---|---|
| `<math>` | Root element | `<math>...</math>` |
| `<mi>` | Identifier (variable) | `<mi>x</mi>` → *x* |
| `<mn>` | Number | `<mn>42</mn>` → 42 |
| `<mo>` | Operator | `<mo>+</mo>` → + |
| `<mrow>` | Horizontal group | Groups subexpressions |
| `<mfrac>` | Fraction | numerator / denominator |
| `<msqrt>` | Square root | √ |
| `<mroot>` | nth root | ∜ |
| `<msup>` | Superscript | x² |
| `<msub>` | Subscript | x₁ |
| `<msubsup>` | Both sub and superscript | xₙᵏ |

**Display attribute:**

```html
<!-- Inline formula -->
<math display="inline"><mi>E</mi><mo>=</mo><mi>mc</mi><msup><mi></mi><mn>2</mn></msup></math>

<!-- Block (centered) formula -->
<math display="block">
  <mrow>
    <msup><mi>a</mi><mn>2</mn></msup>
    <mo>+</mo>
    <msup><mi>b</mi><mn>2</mn></msup>
    <mo>=</mo>
    <msup><mi>c</mi><mn>2</mn></msup>
  </mrow>
</math>
```

**Browser support & fallback:** MathML is natively supported in Firefox and Safari. For Chrome/Edge, use a polyfill like [MathJax](https://www.mathjax.org/) for maximum compatibility.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 19. Service Workers & Web Workers

<br/>

## Q. What is a Web Worker in HTML5?

A **Web Worker** runs JavaScript in a **background thread**, separate from the main UI thread. This allows CPU-intensive computations to run without freezing or blocking the user interface.

**Key characteristics:**
- Runs in an isolated thread (no access to DOM, `window`, or `document`)
- Communicates with the main thread via `postMessage()` / `onmessage`
- Has access to `fetch`, `XMLHttpRequest`, `IndexedDB`, `WebSockets`
- **Dedicated worker** — owned by one script only
- **Shared worker** — shared across multiple scripts/tabs on the same origin

**Example — Dedicated Worker:**

`worker.js`:
```js
// Runs in the worker thread
self.onmessage = (event) => {
  const { data } = event;
  let result = 0;
  for (let i = 0; i < data; i++) result += i; // Heavy computation
  self.postMessage(result);
};
```

`main.js` (in the page):
```js
const worker = new Worker("worker.js");

// Send data to worker
worker.postMessage(1_000_000);

// Receive result
worker.onmessage = (event) => {
  console.log("Result:", event.data);
};

worker.onerror = (error) => {
  console.error("Worker error:", error.message);
};

// Terminate worker when done
worker.terminate();
```

**What Web Workers can and cannot access:**

| Can Access | Cannot Access |
|---|---|
| `fetch` / `XMLHttpRequest` | `document` |
| `setTimeout` / `setInterval` | `window` |
| `WebSockets` | `DOM elements` |
| `IndexedDB` | `localStorage` / `sessionStorage` |
| `crypto` | `alert()` / `confirm()` |
| `postMessage` | Parent page variables |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is a Service Worker?

A **Service Worker** is a script that the browser runs in the background, separate from a web page, enabling features that don\'t require a web page or user interaction. It acts as a **programmable network proxy** between the browser and the server.

**Core capabilities:**
- Intercept and cache network requests (offline support)
- Background sync
- Push notifications
- Periodic background sync

**Service Worker lifecycle:**

```
Register → Install → Activate → Idle → Fetch/Push/Sync events
```

**Example — Register and install a Service Worker:**

`main.js`:
```js
if ("serviceWorker" in navigator) {
  navigator.serviceWorker.register("/sw.js")
    .then(reg => console.log("SW registered:", reg.scope))
    .catch(err => console.error("SW registration failed:", err));
}
```

`sw.js` (Service Worker file):
```js
const CACHE_NAME = "my-app-v1";
const ASSETS = ["/", "/index.html", "/styles.css", "/app.js", "/logo.png"];

// Install: pre-cache static assets
self.addEventListener("install", (event) => {
  event.waitUntil(
    caches.open(CACHE_NAME).then(cache => cache.addAll(ASSETS))
  );
  self.skipWaiting(); // Activate immediately
});

// Activate: clean up old caches
self.addEventListener("activate", (event) => {
  event.waitUntil(
    caches.keys().then(keys =>
      Promise.all(keys.filter(k => k !== CACHE_NAME).map(k => caches.delete(k)))
    )
  );
  self.clients.claim();
});

// Fetch: serve from cache, fallback to network
self.addEventListener("fetch", (event) => {
  event.respondWith(
    caches.match(event.request).then(cached => cached || fetch(event.request))
  );
});
```

**Caching strategies:**

| Strategy | Description | Best for |
|---|---|---|
| Cache First | Serve from cache; fetch if not cached | Static assets, fonts |
| Network First | Fetch from network; fallback to cache | API data, dynamic content |
| Stale-While-Revalidate | Serve cache immediately, update in background | News feeds, user profiles |
| Cache Only | Never go to network | Pre-cached offline assets |
| Network Only | Always fetch from network | Non-cacheable real-time data |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between Web Workers and Service Workers?

Both run JavaScript off the main thread, but they have very different purposes and lifetimes.

| Feature | Web Worker | Service Worker |
|---|---|---|
| **Purpose** | CPU-intensive background computation | Network proxy, offline support, push notifications |
| **Scope** | Tied to the page that created it | Registered to an origin/scope, independent of any page |
| **Lifetime** | Lives as long as the creating page | Persists beyond page close (in background) |
| **DOM access** | No | No |
| **Network interception** | No | Yes (via `fetch` event) |
| **Cache API access** | No | Yes |
| **Push notifications** | No | Yes |
| **Background sync** | No | Yes |
| **Multiple instances** | One per `new Worker()` call | One per scope |
| **Communication** | `postMessage` with the creating page | `postMessage` with all controlled clients |
| **Requires HTTPS** | No | Yes (except localhost) |
| **Types** | Dedicated, Shared | Single type |

**Simple analogy:**
- **Web Worker** = a calculator in the background (compute things for me)
- **Service Worker** = a local post office (intercept all mail going in/out, cache deliveries, deliver even when the recipient is away)

**When to use each:**

Use **Web Workers** for:
- Image/video processing
- Parsing large JSON or CSV files
- Complex mathematical computations
- Encryption/decryption operations

Use **Service Workers** for:
- Offline-first Progressive Web Apps (PWA)
- Caching static and dynamic content
- Background push notifications
- Background sync (send data when back online)

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 20. IndexedDB & Advanced Web Storage

<br/>

## Q. What is IndexedDB in HTML5?

**IndexedDB** is a low-level, NoSQL, client-side database built into the browser. It stores large amounts of structured data — including files and blobs — and supports indexes for high-performance queries. It is asynchronous and uses a transaction-based model.

**Key characteristics:**
- Storage capacity: typically hundreds of MBs to GBs (browser/OS dependent)
- Stores JavaScript objects, files, binary data (Blob, ArrayBuffer)
- Supports indexes for efficient querying
- Fully asynchronous (Promise or event-based)
- Scoped per origin (same-origin policy)
- Data persists across sessions (until cleared)

**Core concepts:**

| Concept | Description |
|---|---|
| **Database** | Container for object stores; has a name and version |
| **Object Store** | Like a table in SQL; stores records as key-value pairs |
| **Index** | Secondary key for querying by properties other than the primary key |
| **Transaction** | All operations happen inside a transaction (read or read/write) |
| **Cursor** | Iterator for traversing multiple records |

**Example — Store and retrieve data:**

```js
// 1. Open the database (creates it if it doesn\'t exist)
const request = indexedDB.open("MyDatabase", 1);

// 2. Create schema on first creation or version upgrade
request.onupgradeneeded = (event) => {
  const db = event.target.result;

  // Create an object store with auto-incrementing key
  const store = db.createObjectStore("users", {
    keyPath: "id",
    autoIncrement: true
  });

  // Create an index on the "email" property
  store.createIndex("email", "email", { unique: true });
};

request.onsuccess = (event) => {
  const db = event.target.result;

  // 3. Add a record
  const tx = db.transaction("users", "readwrite");
  const store = tx.objectStore("users");

  store.add({ name: "Alice", email: "alice@example.com", age: 30 });

  tx.oncomplete = () => console.log("User added");

  // 4. Read a record by primary key
  const getTx = db.transaction("users", "readonly");
  const getStore = getTx.objectStore("users");
  const getReq = getStore.get(1);

  getReq.onsuccess = () => console.log("User:", getReq.result);

  // 5. Query by index
  const indexTx = db.transaction("users", "readonly");
  const emailIndex = indexTx.objectStore("users").index("email");
  const indexReq = emailIndex.get("alice@example.com");

  indexReq.onsuccess = () => console.log("Found:", indexReq.result);
};

request.onerror = (event) => console.error("DB error:", event.target.error);
```

**Comparison with other storage options:**

| | `localStorage` | `sessionStorage` | `Cookie` | `IndexedDB` |
|---|---|---|---|---|
| Capacity | ~5 MB | ~5 MB | ~4 KB | Hundreds of MB |
| Data types | String only | String only | String only | Any JS object |
| Async | No (sync) | No (sync) | No (sync) | Yes |
| Indexes | No | No | No | Yes |
| Transactions | No | No | No | Yes |
| Works in SW | No | No | No | Yes |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is WebSQL?

**WebSQL** is a deprecated browser API that provided a relational database using a variant of **SQLite** directly in the browser. It allowed web pages to use SQL queries (`SELECT`, `INSERT`, `UPDATE`, `DELETE`) on a local client-side database.

**Status: Deprecated and removed**  
WebSQL was never standardized by the W3C. It was rejected in favor of IndexedDB and was **removed from Chrome in 2024** and has not been supported in Firefox or Edge for many years.

**Basic WebSQL usage (historical reference):**

```js
// Open (or create) a database
const db = openDatabase(
  "myDB",     // name
  "1.0",      // version
  "My DB",    // display name
  2 * 1024 * 1024  // size (2 MB)
);

// Create a table
db.transaction((tx) => {
  tx.executeSql("CREATE TABLE IF NOT EXISTS users (id INTEGER PRIMARY KEY, name TEXT, email TEXT)");
});

// Insert data
db.transaction((tx) => {
  tx.executeSql("INSERT INTO users (name, email) VALUES (?, ?)", ["Alice", "alice@example.com"]);
});

// Query data
db.transaction((tx) => {
  tx.executeSql("SELECT * FROM users", [], (tx, results) => {
    for (let i = 0; i < results.rows.length; i++) {
      console.log(results.rows.item(i));
    }
  });
});
```

**Why WebSQL was deprecated:**
1. It was based on SQLite, which tied the spec to a specific SQL dialect
2. No browser other than WebKit-based browsers implemented it
3. The W3C stopped working on it in 2010
4. IndexedDB was chosen as the standard replacement

**Migration path:** Use **IndexedDB** (with a library like [Dexie.js](https://dexie.org/) or [idb](https://github.com/jakearchibald/idb) for a friendlier API) instead of WebSQL.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 21. Atomic Design & Pixel Perfect Design

<br/>

## Q. What is Atomic Design Pattern?

**Atomic Design** is a methodology for creating design systems by composing UI components in a hierarchy inspired by chemistry. It was introduced by Brad Frost.

The five levels are:

**1. Atoms**  
The smallest, indivisible UI building blocks — single HTML elements that cannot be broken down further without losing their functionality.

```html
<!-- Atom: A button -->
<button class="btn btn-primary">Submit</button>

<!-- Atom: An input -->
<input type="text" placeholder="Enter email">

<!-- Atom: A label -->
<label for="email">Email Address</label>
```

**2. Molecules**  
Simple groups of atoms functioning together as a unit.

```html
<!-- Molecule: A search form (input + button atoms) -->
<form class="search-form">
  <input type="search" placeholder="Search...">
  <button type="submit">Go</button>
</form>
```

**3. Organisms**  
Relatively complex components composed of molecules and/or atoms, forming distinct sections of an interface.

```html
<!-- Organism: A site header -->
<header class="site-header">
  <a class="logo" href="/">Brand</a>
  <nav class="main-nav">
    <a href="/about">About</a>
    <a href="/blog">Blog</a>
  </nav>
  <form class="search-form">
    <input type="search" placeholder="Search...">
    <button type="submit">Go</button>
  </form>
</header>
```

**4. Templates**  
Page-level structures that arrange organisms into a layout. They define the content structure without real content (using placeholder/lorem ipsum).

```html
<!-- Template: Blog page layout -->
<div class="blog-template">
  <header class="site-header">...</header>
  <main class="content">
    <article class="post-grid">...</article>
    <aside class="sidebar">...</aside>
  </main>
  <footer class="site-footer">...</footer>
</div>
```

**5. Pages**  
Specific instances of templates with real, representative content. This is what users actually see.

```html
<!-- Page: Blog post with actual content -->
<div class="blog-template">
  <header><!-- real nav --></header>
  <main>
    <article>
      <h1>10 Tips for Responsive Design</h1>
      <img src="real-photo.jpg" alt="...">
      <p>Real article content...</p>
    </article>
  </main>
</div>
```

**Benefits of Atomic Design:**

| Benefit | Description |
|---|---|
| Reusability | Components built once, used everywhere |
| Consistency | Unified UI language across the entire product |
| Maintainability | Change an atom and all molecules/organisms update |
| Scalability | Easy to extend and add new components |
| Better collaboration | Shared vocabulary between designers and developers |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to achieve pixel perfect design in HTML/CSS?

**Pixel perfect design** means implementing a UI that matches the designer\'s mockup precisely — every margin, padding, font size, color, and spacing aligns exactly with the design specification.

**1. Use the correct base styles**

Reset browser defaults to eliminate inconsistencies across browsers:

```css
/* Modern CSS reset */
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

**2. Match the design\'s spacing system**

Use a consistent spacing scale (e.g., 4px or 8px grid):

```css
:root {
  --space-1: 4px;
  --space-2: 8px;
  --space-3: 16px;
  --space-4: 24px;
  --space-5: 32px;
  --space-6: 48px;
}
```

**3. Use exact font settings from the design**

```css
.heading {
  font-family: "Inter", sans-serif;
  font-size: 32px;
  font-weight: 700;
  line-height: 1.25;       /* = 40px */
  letter-spacing: -0.5px;
  color: #1A1A2E;
}
```

**4. Match colors exactly**

Copy hex/rgba values directly from design tools (Figma, Sketch, XD):

```css
:root {
  --color-primary:    #3B82F6;
  --color-secondary:  #8B5CF6;
  --color-text:       #111827;
  --color-muted:      #6B7280;
  --color-background: #F9FAFB;
}
```

**5. Use a design overlay extension**

Browser extensions (e.g., **PerfectPixel** for Chrome/Firefox) let you overlay the design mockup directly on top of the browser — you can adjust opacity to compare pixel by pixel.

**6. Inspect with browser DevTools**

- Right-click → Inspect → use the **Box Model** diagram to verify margins and padding
- Use the **ruler tool** and **element measurement** (Shift+click in DevTools)

**7. Handle sub-pixel rendering**

```css
/* Prevent blurry sub-pixel text */
body {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-rendering: optimizeLegibility;
}
```

**8. Use rem/em consistently for scaling**

```css
html { font-size: 16px; } /* 1rem = 16px */

.card {
  padding: 1.5rem;     /* 24px */
  border-radius: 0.5rem; /* 8px */
}
```

**9. Match border-radius, shadows exactly**

```css
.card {
  /* Figma shows: shadow x=0, y=4, blur=16, spread=0, color=#00000014 */
  box-shadow: 0 4px 16px 0 rgba(0, 0, 0, 0.08);
  border-radius: 12px;
  border: 1px solid #E5E7EB;
}
```

**10. Verify at multiple viewport sizes**

Test at the exact breakpoints defined in the design (e.g., 375px mobile, 768px tablet, 1440px desktop) and compare against the design mockup.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 22. SEO Basics & Advanced

<br/>

## Q. What are Core Web Vitals?

**Core Web Vitals** are a set of real-world performance metrics defined by Google that measure user experience on the web. They are official Google Search ranking signals as of 2021.

**The three Core Web Vitals:**

**1. Largest Contentful Paint (LCP)**
Measures **loading performance** — the time it takes for the largest visible content element (image, video, or block of text) to fully render.

| Score | Threshold |
|---|---|
| Good | ≤ 2.5 seconds |
| Needs Improvement | 2.5s – 4.0s |
| Poor | > 4.0 seconds |

**How to improve LCP:**
- Optimize and compress large images
- Use `<link rel="preload">` for the hero image
- Use a CDN
- Remove render-blocking CSS/JS
- Use `loading="eager"` on above-the-fold images

**2. Interaction to Next Paint (INP)** *(replaced FID in March 2024)*
Measures **interactivity** — the latency of all user interactions (clicks, taps, keyboard input) throughout the page\'s lifetime.

| Score | Threshold |
|---|---|
| Good | ≤ 200 ms |
| Needs Improvement | 200ms – 500ms |
| Poor | > 500 ms |

**How to improve INP:**
- Minimize long tasks on the main thread
- Use Web Workers for heavy computation
- Avoid unnecessary re-renders
- Defer non-critical JavaScript

**3. Cumulative Layout Shift (CLS)**
Measures **visual stability** — how much the page layout unexpectedly shifts during loading.

| Score | Threshold |
|---|---|
| Good | ≤ 0.1 |
| Needs Improvement | 0.1 – 0.25 |
| Poor | > 0.25 |

**How to improve CLS:**
- Always specify `width` and `height` on images and videos
- Reserve space for ads and embeds
- Avoid inserting content above existing content
- Use `font-display: optional` or preload fonts

**Measurement tools:**
- Google PageSpeed Insights (`pagespeed.web.dev`)
- Chrome DevTools → Lighthouse
- Chrome User Experience Report (CrUX)
- `web-vitals` JavaScript library

```js
import { getLCP, getINP, getCLS } from "web-vitals";

getLCP(console.log);
getINP(console.log);
getCLS(console.log);
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is structured data and JSON-LD for SEO?

**Structured data** is a standardized format for providing explicit information about a page\'s content so that search engines can better understand it and display **rich results** (also called rich snippets) in search engine results pages (SERPs).

**JSON-LD (JavaScript Object Notation for Linked Data)** is Google\'s recommended format for embedding structured data in a `<script>` tag, using vocabulary from [Schema.org](https://schema.org).

**Benefits of structured data:**
- Eligibility for rich results (star ratings, FAQ boxes, breadcrumbs, product carousels)
- Improved click-through rate (CTR) from search results
- Better understanding of content by search engines

**Example — Article schema:**

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "Top 10 HTML5 Interview Questions",
  "author": {
    "@type": "Person",
    "name": "John Doe"
  },
  "datePublished": "2024-01-15",
  "dateModified": "2024-04-01",
  "image": "https://example.com/article-image.jpg",
  "publisher": {
    "@type": "Organization",
    "name": "HTML Basics",
    "logo": {
      "@type": "ImageObject",
      "url": "https://example.com/logo.png"
    }
  }
}
</script>
```

**Example — FAQ schema (creates FAQ dropdowns in SERPs):**

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is HTML5?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "HTML5 is the latest version of HyperText Markup Language..."
      }
    },
    {
      "@type": "Question",
      "name": "What are semantic HTML elements?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Semantic elements clearly describe their meaning to the browser..."
      }
    }
  ]
}
</script>
```

**Example — Product schema:**

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "Laptop Pro 15",
  "image": "https://example.com/laptop.jpg",
  "description": "High-performance laptop for developers.",
  "brand": { "@type": "Brand", "name": "TechBrand" },
  "offers": {
    "@type": "Offer",
    "price": "1299.99",
    "priceCurrency": "USD",
    "availability": "https://schema.org/InStock"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.8",
    "reviewCount": "245"
  }
}
</script>
```

**Popular Schema.org types:**

| Type | Rich result |
|---|---|
| `Article` | Article appearance |
| `FAQPage` | FAQ accordion in SERPs |
| `Product` | Price, availability, reviews |
| `BreadcrumbList` | Breadcrumb navigation |
| `Organization` | Knowledge panel |
| `LocalBusiness` | Business info with map |
| `Recipe` | Recipe cards with ratings |
| `Event` | Event details |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are hreflang tags and when should you use them?

**`hreflang`** is an HTML attribute used to tell search engines which language and/or geographic region a page is intended for. It helps Google serve the correct regional or language variant to users.

**When to use:**
- Your site has content in multiple languages (e.g., English, French, Spanish)
- Your site has region-specific versions (e.g., `en-US`, `en-GB`, `en-AU`)
- Your site has translated pages with different URLs

**Syntax:**

```html
<!-- In the <head> of each page: -->

<!-- English (default, all regions) -->
<link rel="alternate" hreflang="en" href="https://example.com/en/page">

<!-- French -->
<link rel="alternate" hreflang="fr" href="https://example.com/fr/page">

<!-- Spanish (all regions) -->
<link rel="alternate" hreflang="es" href="https://example.com/es/page">

<!-- English for US -->
<link rel="alternate" hreflang="en-US" href="https://example.com/en-us/page">

<!-- English for UK -->
<link rel="alternate" hreflang="en-GB" href="https://example.com/en-gb/page">

<!-- Fallback for all other regions/languages -->
<link rel="alternate" hreflang="x-default" href="https://example.com/page">
```

**Rules:**
1. Every page in the set must reference all other pages, including itself
2. The `x-default` tag indicates the fallback page when no language match is found
3. Language codes follow IETF BCP 47 format (e.g., `en`, `en-GB`, `zh-Hant`)
4. Hreflang can also be set in the HTTP header or XML sitemap

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between crawling and indexing in SEO?

**Crawling** and **indexing** are two separate steps search engines perform before a page can appear in search results.

**Crawling**

Crawling is the process by which search engine bots (called **crawlers** or **spiders**, e.g., Googlebot) discover and download web pages by following links.

- Googlebot starts from a list of known URLs and follows hyperlinks
- Pages are added to a crawl queue based on PageRank, update frequency, and site authority
- **Robots.txt** controls which paths crawlers are allowed or forbidden to access:

```
# robots.txt
User-agent: *
Disallow: /admin/
Disallow: /private/
Allow: /public/

Sitemap: https://example.com/sitemap.xml
```

**Indexing**

Indexing is the process of analyzing and storing crawled content in the search engine\'s database (index) so it can be retrieved in response to a search query.

- After crawling, Google processes the page\'s content, HTML, images, metadata
- If the page is deemed indexable, it enters the index
- The `<meta name="robots" content="noindex">` tag prevents a page from being indexed

```html
<!-- Allow both crawling and indexing (default) -->
<meta name="robots" content="index, follow">

<!-- Prevent indexing but allow link following -->
<meta name="robots" content="noindex, follow">

<!-- Prevent crawling of links -->
<meta name="robots" content="index, nofollow">

<!-- Prevent both indexing and link following -->
<meta name="robots" content="noindex, nofollow">
```

**Key differences:**

| | Crawling | Indexing |
|---|---|---|
| **What happens** | Bot discovers and downloads the page | Page is analyzed and stored in the index |
| **Controlled by** | `robots.txt`, crawl budget | `<meta name="robots">`, `X-Robots-Tag` |
| **Outcome** | Page is fetched | Page can appear in search results |
| **Can be blocked** | Yes, via `Disallow` in robots.txt | Yes, via `noindex` directive |
| **Order** | Always first | Happens after crawling |

*Note: Blocking crawling (robots.txt) also prevents indexing. But `noindex` only blocks indexing — the page can still be crawled.*

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 23. HTML Performance Optimization

<br/>

## Q. What are resource hints in HTML5?

**Resource hints** are HTML link directives that tell the browser to perform certain network operations early — before they are needed — to speed up page load. They are set in the `<head>` using `<link>` tags.

**1. `dns-prefetch` — Resolve DNS early**

Resolves the DNS lookup for a domain before any resource from it is requested. Cheap and broadly supported.

```html
<!-- Resolve DNS for external font/analytics domains -->
<link rel="dns-prefetch" href="//fonts.googleapis.com">
<link rel="dns-prefetch" href="//www.google-analytics.com">
```

**2. `preconnect` — Establish connection early**

Opens a TCP connection (and TLS handshake for HTTPS) to an origin before it is needed. Stronger than dns-prefetch — use for critical third-party origins.

```html
<!-- Critical: fonts will be loaded from here -->
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="preconnect" href="https://api.example.com">
```

**3. `preload` — Fetch a resource immediately**

Tells the browser to download a resource as soon as possible (high priority) because it will be needed very soon. Does **not** execute it — just downloads it.

```html
<!-- Preload the hero image (above the fold) -->
<link rel="preload" href="hero.jpg" as="image">

<!-- Preload critical font to avoid FOUT -->
<link rel="preload" href="/fonts/inter.woff2" as="font" type="font/woff2" crossorigin>

<!-- Preload a JS module needed right after parse -->
<link rel="preload" href="/app.js" as="script">

<!-- Preload critical CSS -->
<link rel="preload" href="/critical.css" as="style">
```

**The `as` attribute values:**

| `as` value | Resource type |
|---|---|
| `image` | Image files |
| `font` | Web fonts (must add `crossorigin`) |
| `script` | JavaScript |
| `style` | CSS stylesheet |
| `fetch` | `fetch()` / `XHR` requests |
| `document` | HTML documents (iframes) |

**4. `prefetch` — Download for future navigation**

Fetches a resource at **low priority** in the browser\'s idle time — for resources that will likely be needed on the **next page** (not the current one).

```html
<!-- User is likely to go to the dashboard next -->
<link rel="prefetch" href="/dashboard.html">
<link rel="prefetch" href="/dashboard.css">
```

**5. `prerender` — Render a whole page in the background**

Fetches and renders the entire next page in a hidden tab — the fastest possible experience when users navigate to it.

```html
<link rel="prerender" href="https://example.com/next-page">
```

**Comparison:**

| Hint | Timing | Priority | Use for |
|---|---|---|---|
| `dns-prefetch` | Current page | Low | DNS only, third-party domains |
| `preconnect` | Current page | Medium | Critical third-party origins |
| `preload` | Current page | High | Critical current-page resources |
| `prefetch` | Next navigation | Idle (low) | Resources for next page |
| `prerender` | Next navigation | Idle | Entire next page |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How to implement lazy loading in HTML?

**Lazy loading** defers loading of off-screen resources (images, iframes) until the user scrolls near them, reducing initial page load time and saving bandwidth.

**1. Native lazy loading (HTML attribute — recommended)**

Supported in all modern browsers natively:

```html
<!-- Lazy load an image -->
<img src="photo.jpg" alt="Photo" loading="lazy" width="800" height="600">

<!-- Lazy load an iframe -->
<iframe src="https://www.youtube.com/embed/video" loading="lazy"></iframe>
```

**Always specify `width` and `height`** to prevent layout shifts (CLS) when the image loads.

`loading` attribute values:
- `lazy` — defer loading until near the viewport
- `eager` — load immediately (default for above-the-fold images)
- `auto` — browser decides

**2. JavaScript lazy loading with Intersection Observer**

```js
const images = document.querySelectorAll("img[data-src]");

const observer = new IntersectionObserver((entries, observer) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      const img = entry.target;
      img.src = img.dataset.src;

      if (img.dataset.srcset) {
        img.srcset = img.dataset.srcset;
      }

      img.removeAttribute("data-src");
      observer.unobserve(img);
    }
  });
}, {
  rootMargin: "0px 0px 200px 0px" // Start loading 200px before entering viewport
});

images.forEach(img => observer.observe(img));
```

```html
<!-- Use data-src instead of src -->
<img data-src="photo.jpg"
     data-srcset="photo-400.jpg 400w, photo-800.jpg 800w"
     src="placeholder.svg"
     alt="Photo"
     width="800"
     height="600">
```

**3. Lazy loading background images (CSS + JS)**

```css
.lazy-bg {
  background-image: none;
  background-color: #eee; /* placeholder */
}

.lazy-bg.loaded {
  background-image: url("hero.jpg");
}
```

```js
const bgEls = document.querySelectorAll(".lazy-bg");
const bgObserver = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add("loaded");
      bgObserver.unobserve(entry.target);
    }
  });
});

bgEls.forEach(el => bgObserver.observe(el));
```

**Best practices:**
- Never lazy load the LCP (Largest Contentful Paint) image — use `loading="eager"` or `<link rel="preload">` for it
- Always provide `width` and `height` to prevent layout shift
- Use `loading="lazy"` for all below-the-fold images as a baseline

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `async` and `defer` in `<script>` and when to use each?

Both `async` and `defer` allow the browser to **download** the script without blocking HTML parsing. The difference is **when the script executes**.

**Without `async` or `defer` (default behavior):**

```html
<script src="script.js"></script>
```

1. HTML parsing stops
2. Script is downloaded
3. Script executes
4. HTML parsing resumes

**With `async`:**

```html
<script async src="analytics.js"></script>
```

1. HTML parsing continues in parallel while script downloads
2. As soon as download completes, HTML parsing **pauses** and script executes immediately
3. HTML parsing resumes after execution
4. **Order of execution is NOT guaranteed** when multiple async scripts are used

**With `defer`:**

```html
<script defer src="app.js"></script>
```

1. HTML parsing continues in parallel while script downloads
2. Script executes **after the HTML is fully parsed** (before `DOMContentLoaded`)
3. **Order of execution IS guaranteed** — scripts execute in document order

**Visual comparison:**

```
Default:  |----HTML parsing----|[pause]|--download--|--execute--|[resume]|---HTML---|
async:    |----HTML parsing----|--download--|[pause]|--execute--|[resume]-------------|
defer:    |----HTML parsing---(downloads in background)---|--execute--|DOMContentLoaded|
```

**Decision guide:**

| Use case | Attribute |
|---|---|
| Script has no dependencies and order doesn\'t matter (e.g., analytics, ads) | `async` |
| Script depends on the DOM being fully parsed | `defer` |
| Script depends on other scripts being loaded first | `defer` (respects order) |
| Small inline script | Neither (inline scripts can\'t use these attributes) |
| Module scripts (`type="module"`) | `defer` by default |

```html
<!-- Example: proper script loading strategy -->
<head>
  <!-- Critical styles: no defer/async needed -->
  <link rel="stylesheet" href="styles.css">

  <!-- Analytics: async (no dependencies, order doesn\'t matter) -->
  <script async src="https://www.google-analytics.com/analytics.js"></script>

  <!-- App code: defer (needs DOM ready, must run in order) -->
  <script defer src="vendor.js"></script>
  <script defer src="app.js"></script>
</head>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is Content Security Policy (CSP) and how is it configured in HTML?

**Content Security Policy (CSP)** is a browser security mechanism that helps prevent **Cross-Site Scripting (XSS)**, clickjacking, and other code injection attacks by declaring which sources of content are trusted.

**How it works:** The server sends a `Content-Security-Policy` HTTP header (or a `<meta>` tag) telling the browser to only execute/load resources from the approved sources.

**Via HTTP header (recommended):**

```
Content-Security-Policy: default-src 'self'; script-src 'self' https://cdn.example.com; style-src 'self' 'unsafe-inline'; img-src 'self' data: https:; font-src 'self' https://fonts.gstatic.com
```

**Via HTML `<meta>` tag (limited — cannot use `report-uri`):**

```html
<meta http-equiv="Content-Security-Policy"
      content="default-src 'self'; script-src 'self' https://trusted-cdn.com; style-src 'self';">
```

**Common CSP directives:**

| Directive | Controls |
|---|---|
| `default-src` | Fallback for all resource types |
| `script-src` | JavaScript sources |
| `style-src` | CSS sources |
| `img-src` | Image sources |
| `font-src` | Font sources |
| `connect-src` | AJAX, WebSocket, fetch targets |
| `frame-src` | `<iframe>` sources |
| `media-src` | `<audio>` and `<video>` sources |
| `form-action` | `<form action>` targets |
| `upgrade-insecure-requests` | Upgrade HTTP to HTTPS |

**Common source values:**

| Value | Meaning |
|---|---|
| `'self'` | Same origin only |
| `'none'` | No sources allowed |
| `'unsafe-inline'` | Allow inline `<script>` and `<style>` (avoid when possible) |
| `'unsafe-eval'` | Allow `eval()` (avoid when possible) |
| `'nonce-xxxxx'` | Allow specific inline script with matching nonce |
| `https:` | Any HTTPS source |
| `https://cdn.example.com` | Specific origin |

**Nonce-based approach (preferred over `unsafe-inline`):**

```html
<!-- Server generates a unique nonce per request -->
<script nonce="abc123xyz">
  // This inline script is allowed
  console.log("Trusted inline script");
</script>
```

```
Content-Security-Policy: script-src 'nonce-abc123xyz'
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the purpose of `<link rel="preload">` and how does it improve performance?

`<link rel="preload">` is a **declarative fetch directive** that tells the browser to download a resource as soon as possible (at high priority) because it will be needed shortly — without delaying the current render. It eliminates the "late discovery" problem where the browser only discovers critical resources after parsing deep into the HTML or CSS.

**Why it matters:**

Without preload, fonts are typically discovered only after:
1. HTML is parsed
2. CSS is downloaded and parsed
3. `@font-face` rule is encountered

This causes **Flash of Invisible Text (FOIT)** or **Flash of Unstyled Text (FOUT)**. Preloading the font starts the download immediately.

**Common use cases and examples:**

```html
<head>
  <!-- 1. Preload hero image (above the fold = LCP element) -->
  <link rel="preload" href="/images/hero.webp" as="image">

  <!-- 2. Preload critical web font -->
  <link rel="preload" href="/fonts/inter-400.woff2" as="font" type="font/woff2" crossorigin>

  <!-- 3. Preload a critical JavaScript module -->
  <link rel="preload" href="/js/app.js" as="script">

  <!-- 4. Preload critical CSS (then apply it) -->
  <link rel="preload" href="/css/critical.css" as="style" onload="this.onload=null;this.rel='stylesheet'">
  <noscript><link rel="stylesheet" href="/css/critical.css"></noscript>

  <!-- 5. Preload an API response used immediately on page load -->
  <link rel="preload" href="/api/user/profile" as="fetch" crossorigin>
</head>
```

**Key rules:**
- Always include the `as` attribute — without it, the resource is fetched at low priority and may be downloaded twice
- Fonts require `crossorigin` even if same-origin (due to CORS requirements for font loading)
- Don\'t over-preload — preloading too many resources competes for bandwidth and can slow down other resources

**Preload vs Prefetch:**

| | `preload` | `prefetch` |
|---|---|---|
| Priority | High (current page) | Low (future page, idle time) |
| Purpose | Critical resources needed now | Resources for next navigation |
| Browser behavior | Downloads immediately | Downloads during idle time |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are WCAG guidelines and accessibility levels?

**WCAG (Web Content Accessibility Guidelines)** is the international standard for web accessibility, developed by the W3C\'s Web Accessibility Initiative (WAI). The current version is **WCAG 2.2** (2023), with WCAG 3.0 in development.

**The four WCAG principles (POUR):**

**1. Perceivable** — Information and UI components must be presentable to all users.
- Provide text alternatives for non-text content (`alt` attributes)
- Provide captions and transcripts for audio/video
- Ensure sufficient color contrast
- Don\'t rely on color alone to convey information

**2. Operable** — UI components must be operable by all users.
- All functionality must be accessible via keyboard
- Provide enough time for users to read content
- No content that flashes more than 3 times per second (seizure risk)
- Provide skip links and descriptive page titles

**3. Understandable** — Information and UI operation must be understandable.
- Identify the language of the page (`lang` attribute)
- Make pages behave predictably
- Provide clear error messages and instructions

**4. Robust** — Content must be robust enough to be interpreted by assistive technologies.
- Use valid, semantic HTML
- Ensure name, role, and value of components are exposed to assistive tech

**Conformance levels:**

| Level | Description | Requirement |
|---|---|---|
| **A** | Minimum accessibility | Must satisfy (basic barriers removed) |
| **AA** | Standard accessibility target | Should satisfy (legal requirement in many countries) |
| **AAA** | Highest accessibility | May satisfy (aspirational, not required for all content) |

**Key AA requirements:**
- Minimum color contrast ratio: **4.5:1** for normal text, **3:1** for large text (18pt+)
- All functionality operable by keyboard
- Error identification: identify field in error and describe it in text
- Consistent navigation across pages
- No time limit on user tasks (or user can extend it)

**HTML implementation examples:**

```html
<!-- Perceivable: meaningful alt text -->
<img src="chart.png" alt="Sales increased 40% from Q1 to Q2 2024">

<!-- Operable: keyboard-accessible custom button -->
<div role="button" tabindex="0" 
     onkeydown="if(event.key==='Enter'||event.key===' ')this.click()"
     onclick="doAction()">
  Custom Button
</div>

<!-- Understandable: form with clear error -->
<label for="email">Email <span aria-hidden="true">*</span></label>
<input type="email" id="email" 
       aria-required="true" 
       aria-describedby="email-error"
       aria-invalid="true">
<span id="email-error" role="alert">Please enter a valid email address.</span>

<!-- Robust: landmark roles -->
<header role="banner">
  <nav role="navigation" aria-label="Main navigation">...</nav>
</header>
<main role="main" id="main-content">...</main>
<footer role="contentinfo">...</footer>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 24. HTML Tags & Elements (Intermediate)

<br/>

## Q. What is the difference between `<strong>` and `<b>`, `<em>` and `<i>`?

Both pairs look visually similar but differ in semantic meaning:

| Tag | Type | Meaning |
|---|---|---|
| `<b>` | Presentational | Bold text — no semantic weight |
| `<strong>` | Semantic | **Important** content; screen readers may stress it |
| `<i>` | Presentational | Italic text — no semantic meaning |
| `<em>` | Semantic | **Emphasized** content; screen readers change tone |

```html
<!-- Presentational (avoid for meaningful content) -->
<b>Warning</b>
<i>Technical term</i>

<!-- Semantic (preferred) -->
<strong>Warning: Do not proceed without authorization.</strong>
<em>This step is critical.</em>
```

Use `<strong>` and `<em>` when the emphasis carries meaning. Use `<b>` and `<i>` only for purely stylistic formatting (e.g., keywords in a document, foreign words, technical terms without added importance).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the `<details>` and `<summary>` elements?

The `<details>` element creates a native browser disclosure widget — content that is hidden by default and revealed when the user toggles it. The `<summary>` element provides the visible label/heading for the widget.

**Example:**

```html
<details>
  <summary>What is the capital of France?</summary>
  <p>The capital of France is <strong>Paris</strong>.</p>
</details>
```

**Key attributes:**

| Attribute | Description |
|---|---|
| `open` | If present, the content is shown by default |

```html
<details open>
  <summary>System Requirements</summary>
  <ul>
    <li>OS: Windows 10 or later</li>
    <li>RAM: 8 GB minimum</li>
    <li>Storage: 20 GB free disk space</li>
  </ul>
</details>
```

**Why it matters:** No JavaScript required. Screen readers expose the state (`expanded`/`collapsed`) automatically via ARIA. Commonly used in FAQs, accordions, and progressive disclosure patterns.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are the `<figure>` and `<figcaption>` elements?

`<figure>` represents self-contained content (images, diagrams, code blocks, charts) that is referenced from the main content but could be moved without affecting the document flow. `<figcaption>` provides a caption for the figure.

**Example:**

```html
<figure>
  <img src="architecture-diagram.png" alt="Microservices architecture showing 5 services">
  <figcaption>Fig. 1 — Microservices architecture of the payment platform.</figcaption>
</figure>

<!-- Also valid with code -->
<figure>
  <pre><code>const sum = (a, b) => a + b;</code></pre>
  <figcaption>Arrow function example in JavaScript</figcaption>
</figure>
```

**Why it matters:** `<figure>` + `<figcaption>` creates an accessible, semantic association between a visual/media element and its description — something `<img>` + `<p>` does not do structurally.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<time>` element and why is it useful?

The `<time>` element represents a specific date, time, or duration. The `datetime` attribute provides a machine-readable format while the element\'s text content can be human-readable.

**Syntax:**

```html
<!-- Date -->
<time datetime="2025-04-28">April 28, 2025</time>

<!-- Date and time -->
<time datetime="2025-04-28T09:00">9:00 AM on April 28</time>

<!-- Duration -->
<time datetime="PT2H30M">2 hours 30 minutes</time>

<!-- In context -->
<p>The conference starts on <time datetime="2025-06-15">June 15</time>.</p>
<p>Article published <time datetime="2025-04-28T12:00Z">today at noon UTC</time>.</p>
```

**Why it matters:** Search engines (Google\'s Knowledge Graph, schema.org microdata) use the `datetime` attribute to accurately index events, articles, and schedules. Screen readers can interpret the date format correctly regardless of how it\'s displayed.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between the `hidden` attribute and `display: none`?

Both hide an element visually, but they differ in semantics and behavior:

| | `hidden` attribute | `display: none` |
|---|---|---|
| Type | HTML boolean attribute | CSS rule |
| Semantic | Element is **not relevant** to the current state | No semantic meaning |
| Override | CSS can override it (e.g., `display: block` overrides `hidden`) | Cannot be overridden by `hidden` |
| JavaScript toggle | `el.hidden = true/false` | `el.style.display = 'none'/'block'` |
| Accessibility | Excluded from accessibility tree | Excluded from accessibility tree |

```html
<!-- Hidden attribute -->
<div hidden>This content is not relevant right now.</div>

<!-- Toggle with JS -->
<script>
  document.getElementById("panel").hidden = false; // Reveal
</script>
```

**Best practice:** Use `hidden` when the content is semantically not applicable in the current state (e.g., a step in a wizard). Use `display: none` when hiding for pure visual/layout reasons.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<base>` element in HTML?

The `<base>` element specifies a **base URL** for all relative URLs in a document and/or a default `target` for all links. It must be placed in `<head>` and there can only be one per document.

**Syntax:**

```html
<head>
  <base href="https://www.example.com/projects/" target="_blank">
</head>

<body>
  <!-- Resolved as: https://www.example.com/projects/overview.html -->
  <a href="overview.html">Overview</a>

  <!-- Resolved as: https://www.example.com/projects/assets/logo.png -->
  <img src="assets/logo.png" alt="Logo">
</body>
```

**Caveats:**
- Affects **all** relative URLs on the page including `<link>`, `<script>`, `<img>`, and `<a>` tags
- Fragment identifiers (`#section`) are also resolved relative to the base URL, which can break in-page anchor links
- Single-Page Applications (SPAs) using the History API often set `<base href="/">` to ensure correct asset resolution after deep-link navigations

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<dialog>` element in HTML?

The `<dialog>` element is a native HTML modal/dialog box. It provides built-in accessibility (focus trapping, `role="dialog"`, ARIA attributes) without any JavaScript libraries.

**Example:**

```html
<dialog id="confirmDialog">
  <h2>Confirm Delete</h2>
  <p>Are you sure you want to delete this item?</p>
  <button id="confirmBtn">Yes, Delete</button>
  <button id="cancelBtn">Cancel</button>
</dialog>

<button id="openBtn">Delete Item</button>

<script>
  const dialog = document.getElementById("confirmDialog");

  document.getElementById("openBtn").addEventListener("click", () => {
    dialog.showModal(); // Opens as a modal (blocks background)
  });

  document.getElementById("cancelBtn").addEventListener("click", () => {
    dialog.close(); // Closes the dialog
  });

  document.getElementById("confirmBtn").addEventListener("click", () => {
    // perform delete action
    dialog.close("confirmed");
  });

  // Listen for close event
  dialog.addEventListener("close", () => {
    console.log("Return value:", dialog.returnValue);
  });
</script>
```

**Key methods:**

| Method | Description |
|---|---|
| `show()` | Opens as a non-modal (no backdrop) |
| `showModal()` | Opens as a modal with a backdrop, traps focus |
| `close(returnValue)` | Closes dialog, optionally sets `returnValue` |

**Why it matters over `div`-based modals:**
- Native focus trapping (keyboard users can\'t escape to background)
- Backdrop via `::backdrop` pseudo-element
- Escape key closes it automatically
- Proper ARIA semantics out of the box

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<noscript>` element?

The `<noscript>` element defines fallback content to display when JavaScript is **disabled** in the browser or when the browser does not support scripting.

**In `<head>`** — used to inject alternative `<meta>` or `<link>` tags:

```html
<head>
  <noscript>
    <meta http-equiv="refresh" content="0; url=no-js-version.html">
  </noscript>
</head>
```

**In `<body>`** — used to show fallback UI:

```html
<body>
  <noscript>
    <p>This application requires JavaScript. Please enable it to continue.</p>
  </noscript>

  <div id="app"></div>
  <script src="app.js"></script>
</body>
```

**Common use cases:**
- Displaying a meaningful message for users with JS disabled
- Providing a server-rendered fallback for JS-driven SPAs
- Inserting no-JS tracking pixels (`<img>` inside `<noscript>`) for analytics

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `src` and `href` attributes?

Both attributes link to external resources, but they are used differently:

| | `src` | `href` |
|---|---|---|
| Full form | Source | Hypertext Reference |
| Purpose | **Embeds** the resource into the current document | **Links** to the resource (creates a relationship) |
| Blocks rendering? | Yes — browser pauses parsing to fetch and execute | No — fetched in parallel |
| Used on | `<img>`, `<script>`, `<iframe>`, `<video>`, `<audio>` | `<a>`, `<link>`, `<base>` |

```html
<!-- src: resource is embedded and parsed immediately -->
<img src="logo.png" alt="Logo">
<script src="app.js"></script>
<iframe src="widget.html"></iframe>

<!-- href: document navigates to or includes a relationship -->
<a href="https://example.com">Visit</a>
<link rel="stylesheet" href="styles.css">
```

**Key insight:** When a browser encounters `<script src="app.js">`, it **stops HTML parsing** to download and execute the script. When it encounters `<link href="styles.css">`, it downloads the CSS in parallel with HTML parsing (though it does block rendering until CSS is processed).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between `innerHTML`, `textContent`, and `innerText`?

All three access or modify element content but behave differently:

| | `innerHTML` | `textContent` | `innerText` |
|---|---|---|---|
| Returns | HTML markup as a string | Raw text of all nodes (including hidden) | Rendered text (respects CSS, no hidden elements) |
| Parses HTML on set | Yes | No (treats input as plain text) | No |
| XSS risk | **Yes** — can execute injected scripts | **No** — safe | **No** — safe |
| Performance | Slower (triggers reflow/repaint) | Faster | Slower than `textContent` |
| `display:none` nodes | Included | Included | **Excluded** |

```html
<div id="el">Hello <span style="display:none">hidden</span> <b>World</b></div>

<script>
  const el = document.getElementById("el");

  console.log(el.innerHTML);     // 'Hello <span style="display:none">hidden</span> <b>World</b>'
  console.log(el.textContent);   // 'Hello hidden World'
  console.log(el.innerText);     // 'Hello World'  (hidden span excluded)

  // XSS risk with innerHTML:
  el.innerHTML = userInput;       // DANGEROUS if userInput is untrusted
  el.textContent = userInput;     // SAFE — renders as plain text
</script>
```

**Best practice:** Always use `textContent` when setting plain text from user input. Only use `innerHTML` with sanitized, trusted content.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are HTML entities and when do you use them?

HTML entities are special character codes used to represent characters that have a reserved meaning in HTML (like `<`, `>`, `&`) or that are not easily typeable.

**Syntax:** `&name;` or `&#number;` (decimal) or `&#xHEX;` (hex)

**Common entities:**

| Character | Entity Name | Entity Number | Use case |
|---|---|---|---|
| `<` | `&lt;` | `&#60;` | Less-than (HTML tag delimiter) |
| `>` | `&gt;` | `&#62;` | Greater-than (HTML tag delimiter) |
| `&` | `&amp;` | `&#38;` | Ampersand (entity start character) |
| `"` | `&quot;` | `&#34;` | Quote inside attribute values |
| `'` | `&apos;` | `&#39;` | Apostrophe inside attribute values |
| ` ` (non-breaking space) | `&nbsp;` | `&#160;` | Prevent line break between words |
| `©` | `&copy;` | `&#169;` | Copyright symbol |
| `®` | `&reg;` | `&#174;` | Registered trademark |
| `→` | `&rarr;` | `&#8594;` | Right arrow |

**Example:**

```html
<!-- Without entity: browser treats < as start of a tag -->
<p>Use <code>&lt;div&gt;</code> for block-level containers.</p>

<!-- Non-breaking space: keeps "10 km" on one line -->
<p>The distance is 10&nbsp;km.</p>

<!-- Copyright footer -->
<footer>&copy; 2025 Acme Corp. All rights reserved.</footer>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `contenteditable` attribute?

The `contenteditable` attribute makes any HTML element directly editable by the user in the browser, similar to a text field but with rich-text capabilities.

**Values:**

| Value | Behavior |
|---|---|
| `true` or empty string | Element is editable |
| `false` | Element is not editable (overrides inherited editability) |
| `plaintext-only` | Editable but pasting formatted content is stripped to plain text |

**Example:**

```html
<!-- Editable div -->
<div contenteditable="true" style="border: 1px solid #ccc; padding: 10px; min-height: 100px;">
  Click here to start editing...
</div>

<!-- Read current content via JS -->
<script>
  const editor = document.querySelector('[contenteditable]');

  editor.addEventListener('input', () => {
    console.log('Content:', editor.innerHTML);      // HTML content
    console.log('Plain text:', editor.innerText);   // Plain text
  });
</script>
```

**Key characteristics:**
- Supports copy/paste, undo/redo, and spell-checking natively
- Used as the foundation for rich text editors (e.g., Medium, Notion, Quill.js, Slate.js)
- Content can be retrieved via `innerHTML` or `innerText`
- Does **not** submit with `<form>` — use a hidden `<input>` to capture the value on submit
- Always sanitize `innerHTML` output before persisting to avoid XSS

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is HTML5 native form validation and what are constraint validation attributes?

HTML5 provides built-in client-side form validation without JavaScript, using **constraint validation attributes** on form controls. The browser validates automatically on submit and shows native error messages.

**Key attributes:**

| Attribute | Applies to | Description |
|---|---|---|
| `required` | All inputs | Field must not be empty |
| `minlength` / `maxlength` | `text`, `email`, `password`, `textarea` | Min/max character count |
| `min` / `max` | `number`, `date`, `range` | Min/max value |
| `pattern` | `text`, `email`, `tel`, `url` | RegExp the value must match |
| `type` | `<input>` | `email`, `url`, `number` validate format automatically |
| `step` | `number`, `date`, `range` | Valid value intervals |

**Example:**

```html
<form>
  <label for="username">Username (3–20 chars, alphanumeric):</label>
  <input
    type="text"
    id="username"
    name="username"
    required
    minlength="3"
    maxlength="20"
    pattern="[a-zA-Z0-9]+"
    title="Only letters and numbers allowed"
  >

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>

  <label for="age">Age (18–99):</label>
  <input type="number" id="age" name="age" min="18" max="99" required>

  <button type="submit">Submit</button>
</form>
```

**Custom validation via JavaScript:**

```js
const input = document.getElementById("username");

input.addEventListener("input", () => {
  if (input.validity.patternMismatch) {
    input.setCustomValidity("Only alphanumeric characters are allowed.");
  } else {
    input.setCustomValidity(""); // Clear error
  }
});
```

**Constraint Validation API properties on `input.validity`:**

| Property | True when |
|---|---|
| `valueMissing` | `required` field is empty |
| `typeMismatch` | Value doesn\'t match `type` (e.g., invalid email) |
| `patternMismatch` | Value doesn\'t match `pattern` |
| `tooShort` / `tooLong` | Below `minlength` / above `maxlength` |
| `rangeUnderflow` / `rangeOverflow` | Below `min` / above `max` |
| `valid` | All constraints pass |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the difference between GET and POST methods in HTML forms?

| | `GET` | `POST` |
|---|---|---|
| Data location | Appended to URL as query string (`?key=value`) | Sent in the HTTP request body |
| Visibility | Visible in URL / browser history / server logs | Not visible in URL |
| Bookmarkable | Yes | No |
| Idempotent | Yes — repeated requests produce same result | No — can cause side effects |
| Data limit | ~2000 characters (URL length limit) | No practical limit |
| Caching | Browsers and proxies can cache | Not cached by default |
| Security | Less secure — data in URL | More secure for sensitive data |
| Use case | Search queries, filters, read-only operations | Login forms, file upload, data submission |

```html
<!-- GET: search query visible in URL -->
<form action="/search" method="get">
  <input type="text" name="q" placeholder="Search...">
  <button type="submit">Search</button>
</form>
<!-- Result: /search?q=html+interview -->

<!-- POST: login credentials in request body -->
<form action="/login" method="post">
  <input type="text" name="username" placeholder="Username">
  <input type="password" name="password" placeholder="Password">
  <button type="submit">Login</button>
</form>
```

**Note:** HTML forms natively support only `GET` and `POST`. `PUT`, `PATCH`, and `DELETE` require JavaScript (`fetch` / `XMLHttpRequest`) or a workaround like a hidden `_method` field.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 25. Web Components

<br/>

## Q. What is Shadow DOM and how does it work?

**Shadow DOM** is a browser API that allows you to attach an **encapsulated, isolated DOM subtree** to an element — separate from the main document DOM. Styles and scripts inside the shadow DOM do not leak out, and external styles cannot accidentally affect it.

**Key concepts:**

| Term | Description |
|---|---|
| Shadow host | The regular DOM element that the shadow DOM is attached to |
| Shadow root | The root node of the shadow tree (`attachShadow()` returns this) |
| Shadow tree | The DOM subtree inside the shadow root |
| Light DOM | The regular document DOM (as opposed to the shadow DOM) |

**Example:**

```js
// Attach shadow DOM to an element
const host = document.getElementById("my-widget");
const shadow = host.attachShadow({ mode: "open" }); // "open" = accessible via JS

// Build shadow DOM content
shadow.innerHTML = `
  <style>
    /* This style ONLY applies inside the shadow DOM */
    p { color: red; font-weight: bold; }
  </style>
  <p>This text is styled in isolation.</p>
`;
```

```html
<div id="my-widget"></div>
```

**`mode` option:**

| Mode | Description |
|---|---|
| `"open"` | Shadow root accessible via `element.shadowRoot` |
| `"closed"` | Shadow root is not accessible externally |

**Why Shadow DOM matters:**
- Scoped CSS — no class name collisions between components
- Encapsulated DOM — child nodes hidden from `querySelector` on the main document
- Foundation for Web Components and frameworks like Lit, Stencil, and native browser UI elements (`<input>`, `<video>`)

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What are Custom Elements in HTML5 (Web Components)?

**Custom Elements** allow developers to define new HTML tags with their own behavior and lifecycle callbacks. They are one of the four Web Components standards (Custom Elements, Shadow DOM, HTML Templates, ES Modules).

**Two types:**

1. **Autonomous custom elements** — extend `HTMLElement` directly, create a brand-new tag
2. **Customized built-in elements** — extend an existing HTML element (e.g., `HTMLButtonElement`)

**Example — Autonomous Custom Element:**

```js
class UserCard extends HTMLElement {
  // Called when element is added to the DOM
  connectedCallback() {
    const name = this.getAttribute("name");
    const role = this.getAttribute("role");

    this.innerHTML = `
      <div class="card">
        <h3>${name}</h3>
        <p>${role}</p>
      </div>
    `;
  }

  // Called when element is removed from the DOM
  disconnectedCallback() {
    console.log("UserCard removed");
  }

  // Called when a watched attribute changes
  static get observedAttributes() {
    return ["name", "role"];
  }

  attributeChangedCallback(name, oldValue, newValue) {
    console.log(`Attribute "${name}" changed from ${oldValue} to ${newValue}`);
    this.connectedCallback(); // Re-render on attribute change
  }
}

// Register the custom element
customElements.define("user-card", UserCard);
```

```html
<!-- Use like any HTML element -->
<user-card name="Alice Johnson" role="Senior Engineer"></user-card>
<user-card name="Bob Smith" role="Product Manager"></user-card>
```

**Lifecycle callbacks:**

| Callback | When it fires |
|---|---|
| `connectedCallback` | Element is inserted into the DOM |
| `disconnectedCallback` | Element is removed from the DOM |
| `attributeChangedCallback` | A watched attribute changes |
| `adoptedCallback` | Element is moved to a new document |

**Why it matters:** Custom Elements allow creation of reusable, framework-independent components that work in any HTML page without React, Angular, or Vue.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<template>` element in HTML?

The `<template>` element holds **inert HTML markup** that is not rendered or executed when the page loads. Its content is only activated (cloned and inserted) via JavaScript. It is a key part of the Web Components standard.

**Key properties:**
- Content inside `<template>` is **parsed** but not rendered
- Scripts inside do not execute, images do not load, styles have no effect
- Accessible via `template.content` which returns a `DocumentFragment`

**Example:**

```html
<template id="product-card-template">
  <div class="card">
    <img class="card-img" src="" alt="">
    <h3 class="card-title"></h3>
    <p class="card-price"></p>
    <button class="add-to-cart">Add to Cart</button>
  </div>
</template>

<div id="product-list"></div>

<script>
  const template = document.getElementById("product-card-template");
  const container = document.getElementById("product-list");

  const products = [
    { title: "Laptop", price: "$999", img: "laptop.jpg" },
    { title: "Phone",  price: "$499", img: "phone.jpg" }
  ];

  products.forEach(product => {
    // Clone the template content
    const clone = template.content.cloneNode(true);

    clone.querySelector(".card-title").textContent = product.title;
    clone.querySelector(".card-price").textContent = product.price;
    clone.querySelector(".card-img").src = product.img;
    clone.querySelector(".card-img").alt = product.title;

    container.appendChild(clone);
  });
</script>
```

**Advantages over `innerHTML`:**
- Parsed once by the browser (efficient)
- No XSS risk from template structure itself
- Works with `DocumentFragment`, which is faster to manipulate than live DOM

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `<slot>` element in Web Components?

The `<slot>` element is a **placeholder inside a Shadow DOM** where users of the component can inject their own content (called "light DOM"). Slots enable content composition in Web Components.

**Default slot — accepts any light DOM content:**

```js
class InfoBox extends HTMLElement {
  connectedCallback() {
    const shadow = this.attachShadow({ mode: "open" });
    shadow.innerHTML = `
      <style>
        .box { border: 2px solid #007bff; padding: 12px; border-radius: 4px; }
        .title { font-weight: bold; color: #007bff; }
      </style>
      <div class="box">
        <p class="title"><slot name="title">Default Title</slot></p>
        <slot></slot>
      </div>
    `;
  }
}
customElements.define("info-box", InfoBox);
```

```html
<!-- Light DOM content fills the slots -->
<info-box>
  <span slot="title">Important Notice</span>
  <p>Your session will expire in 5 minutes.</p>
</info-box>
```

**Named vs default slots:**

| Type | Definition | Usage |
|---|---|---|
| Default slot | `<slot></slot>` | Any unassigned light DOM children |
| Named slot | `<slot name="header"></slot>` | `<el slot="header">` in light DOM |

**Why slots matter:** They allow component authors to control the **structure and styling** while users control the **content** — similar to Angular `ng-content` or React `props.children`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## # 26. HTML Security

<br/>

## Q. What is Subresource Integrity (SRI) and how is it used?

**Subresource Integrity (SRI)** is a security feature that allows browsers to verify that files loaded from third-party sources (CDNs) have not been tampered with. The browser computes a cryptographic hash of the downloaded file and compares it to the expected hash in the `integrity` attribute. If they don\'t match, the resource is blocked.

**Syntax:**

```html
<!-- CSS from CDN with SRI -->
<link
  rel="stylesheet"
  href="https://cdn.example.com/bootstrap.min.css"
  integrity="sha384-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
  crossorigin="anonymous"
>

<!-- Script from CDN with SRI -->
<script
  src="https://cdn.example.com/jquery.min.js"
  integrity="sha384-XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
  crossorigin="anonymous"
></script>
```

**Generating the hash:**

```bash
# Generate SHA-384 hash of a file
openssl dgst -sha384 -binary jquery.min.js | openssl base64 -A
```

Or use [srihash.org](https://www.srihash.org/) to generate hashes online.

**Why `crossorigin="anonymous"` is required:** SRI requires the resource to be served with CORS headers. The `crossorigin="anonymous"` attribute tells the browser to make a CORS request without sending credentials.

**Why it matters for security:**
- Prevents **CDN compromise attacks** — if an attacker modifies a CDN-hosted file, browsers will refuse to load it
- Mitigates supply-chain attacks for third-party scripts
- Recommended by OWASP as a best practice for third-party resource inclusion

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is the `sandbox` attribute on `<iframe>` and how does it enhance security?

The `sandbox` attribute on `<iframe>` applies a set of **extra restrictions** to the content of the iframe. By default, `sandbox` with no value restricts almost everything. You can selectively allow capabilities by adding specific token values.

**Default behavior with `sandbox` (no values) — ALL of these are blocked:**
- Script execution
- Form submission
- Popups and new windows
- Access to parent frame (`window.parent`)
- Same-origin access (treated as a different origin)
- Plugin loading

**Selective allow tokens:**

| Token | Allows |
|---|---|
| `allow-scripts` | JavaScript execution |
| `allow-forms` | Form submission |
| `allow-same-origin` | Same-origin access (use with caution) |
| `allow-popups` | `window.open()`, `target="_blank"` links |
| `allow-top-navigation` | Frame can navigate the top-level window |
| `allow-modals` | `alert()`, `confirm()`, `prompt()` |
| `allow-downloads` | File download triggers |

**Examples:**

```html
<!-- Maximum restriction: no scripts, no forms, no nothing -->
<iframe src="untrusted-content.html" sandbox></iframe>

<!-- Allow only scripts (no same-origin — common for ad widgets) -->
<iframe src="ad-widget.html" sandbox="allow-scripts"></iframe>

<!-- Allow scripts and form submission (e.g., embedded payment form) -->
<iframe
  src="https://payments.example.com/checkout"
  sandbox="allow-scripts allow-forms allow-same-origin"
></iframe>
```

**Security warning:** Never combine `allow-scripts` and `allow-same-origin` on untrusted content — this effectively removes the sandbox protection because the script can remove the `sandbox` attribute via DOM access.

**Why it matters:** Sandboxed iframes are critical for embedding third-party content (ads, widgets, user-generated content) without allowing it to compromise the host page.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. How do you prevent Cross-Site Scripting (XSS) in HTML?

**Cross-Site Scripting (XSS)** is an attack where malicious scripts are injected into a trusted web page and executed in a victim\'s browser. HTML is a primary attack surface.

**1. Never set `innerHTML` with untrusted data:**

```js
// VULNERABLE
element.innerHTML = userInput;  // Executes <script> or event handlers in input

// SAFE alternatives
element.textContent = userInput;       // Renders as plain text
element.setAttribute("data-x", val);   // For attributes
```

**2. Use Content Security Policy (CSP) headers:**

```html
<!-- Meta tag CSP (limited; HTTP header preferred) -->
<meta http-equiv="Content-Security-Policy"
      content="default-src 'self'; script-src 'self' https://trusted.cdn.com">
```

CSP blocks inline scripts and restricts which domains can serve scripts, eliminating entire classes of XSS.

**3. Sanitize HTML when rich text is needed:**

```js
// Use a library like DOMPurify
const clean = DOMPurify.sanitize(userInput);
element.innerHTML = clean;  // Safe — dangerous tags/attributes stripped
```

**4. Encode output in templates:**

Always HTML-encode user-controlled values in templates:

| Character | Encode as |
|---|---|
| `<` | `&lt;` |
| `>` | `&gt;` |
| `"` | `&quot;` |
| `'` | `&#x27;` |
| `&` | `&amp;` |

**5. Avoid dangerous patterns:**

```js
// DANGEROUS — executes string as code
eval(userInput);
setTimeout(userInput, 0);
new Function(userInput)();

// DANGEROUS attributes — avoid with user input
element.setAttribute("onclick", userInput);
element.href = "javascript:" + userInput;
```

**6. Use `httpOnly` and `Secure` cookie flags** to prevent XSS from stealing session cookies:

```http
Set-Cookie: session=abc123; HttpOnly; Secure; SameSite=Strict
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## Q. What is Clickjacking and how do you prevent it in HTML?

**Clickjacking** is a UI redressing attack where a malicious page embeds your website inside a transparent or hidden `<iframe>` and tricks users into clicking on elements of your site while thinking they are clicking on the attacker\'s page.

**Example scenario:**
1. Attacker creates a page with an attractive button: "Click to win a prize!"
2. Your bank\'s "Transfer Funds" button is overlaid invisibly via a transparent iframe
3. User clicks the "prize" button, unknowingly triggering the fund transfer

**Prevention — HTTP Header (preferred):**

```http
X-Frame-Options: DENY
# or
X-Frame-Options: SAMEORIGIN
```

**Prevention — Content Security Policy `frame-ancestors`:**

```http
Content-Security-Policy: frame-ancestors 'none';
# or allow same origin only
Content-Security-Policy: frame-ancestors 'self';
# or allow specific domains
Content-Security-Policy: frame-ancestors 'self' https://trusted-partner.com;
```

**Prevention — HTML meta tag (limited effectiveness):**

```html
<!-- Note: X-Frame-Options via meta is NOT supported by most browsers -->
<!-- Always set it as an HTTP response header instead -->
```

**JavaScript frame-busting (legacy fallback):**

```js
// Prevent being embedded in an iframe
if (window.top !== window.self) {
  window.top.location = window.self.location;
}
```

**Comparison:**

| Method | Effectiveness | Recommended |
|---|---|---|
| `X-Frame-Options: DENY` header | High | Yes (legacy support) |
| `CSP: frame-ancestors 'none'` | Highest | Yes (modern, more flexible) |
| JavaScript frame-busting | Low (easily bypassed with `sandbox`) | No (use as last resort) |

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>
