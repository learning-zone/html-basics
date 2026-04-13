# HTML5 Scenario-Based MCQ

> Scenario-based multiple choice questions covering core HTML5 topics.  

<br>

## Table of Contents

1. [Semantic Elements](#1-semantic-elements)
2. [Forms & Validation Attributes](#2-forms--validation-attributes)
3. [HTML5 Input Types](#3-html5-input-types)
4. [Media — Audio, Video & Canvas](#4-media--audio-video--canvas)
5. [Browser Storage](#5-browser-storage)
6. [Accessibility](#6-accessibility)
7. [Semantics (Advanced)](#7-semantics-advanced)
8. [Responsive Images](#8-responsive-images)
9. [Web APIs](#9-web-apis)
10. [Custom Data Attributes](#10-custom-data-attributes)
11. [Meta & Document Head](#11-meta--document-head)
12. [SVG](#12-svg)
13. [WebSocket API](#13-websocket-api)
14. [IFrame & Sandbox](#14-iframe--sandbox)
15. [Progress, Meter, Time & Dialog](#15-progress-meter-time--dialog)

<br>

## 1. Semantic Elements

**Q1.** You are building a news website. The page has a site-wide navigation bar at the top, a main article in the centre, a sidebar with related links, and a copyright notice at the bottom. Which combination of semantic elements best structures this page?

- A) `<div id="nav">`, `<div id="main">`, `<div id="sidebar">`, `<div id="footer">`
- B) `<nav>`, `<main>`, `<aside>`, `<footer>`
- C) `<navigation>`, `<article>`, `<sidebar>`, `<footer>`
- D) `<nav>`, `<section>`, `<div>`, `<footer>`

> **Answer: B**  
> `<nav>`, `<main>`, `<aside>`, and `<footer>` are the correct HTML5 semantic elements for site navigation, primary content, supplementary content, and page footer respectively.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q2.** A developer renders a blog post that contains a heading, body text, and a publication date. Which element should wrap the entire blog post so that search engines and screen readers correctly identify it as a self-contained piece of content?

- A) `<section>`
- B) `<div>`
- C) `<article>`
- D) `<main>`

> **Answer: C**  
> `<article>` represents a self-contained, independently distributable piece of content such as a blog post, news story, or forum entry.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q3.** While reviewing a teammate's code you notice:

```html
<section>
  <p>Copyright © 2026 Acme Corp. All rights reserved.</p>
</section>
```

What is the most semantically correct replacement for `<section>` here?

- A) `<div>`
- B) `<footer>`
- C) `<aside>`
- D) `<small>`

> **Answer: B**  
> `<footer>` is the appropriate semantic element for copyright information, contact details, and other footer content associated with its nearest sectioning ancestor.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q4.** A documentation site groups related topics under expandable headings. Each group has a visible title and hidden details that toggle on click. Without any JavaScript, which HTML5 element pair enables this behaviour natively?

- A) `<div>` and `<span>`
- B) `<summary>` inside `<details>`
- C) `<caption>` inside `<table>`
- D) `<legend>` inside `<fieldset>`

> **Answer: B**  
> The `<details>` / `<summary>` element pair provides a native browser-controlled disclosure widget — no JavaScript required.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q5.** A recipe website uses the same header (logo + nav) on every page and the same footer (links + copyright). A developer wraps each in `<header>` and `<footer>` tags respectively. A junior colleague says this is wrong because only one `<header>` and one `<footer>` is allowed per page. Who is correct?

- A) The junior colleague — only one `<header>` and one `<footer>` are allowed.
- B) The developer — `<header>` and `<footer>` can appear multiple times, including inside `<article>` or `<section>`.
- C) Neither — `<banner>` and `<contentinfo>` should be used instead.
- D) The developer, but only `<footer>` can repeat, not `<header>`.

> **Answer: B**  
> `<header>` and `<footer>` are not limited to one per page. They can appear inside any sectioning element (`<article>`, `<section>`, `<aside>`, `<nav>`).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 2. Forms & Validation Attributes

**Q6.** A registration form has an email field that must be filled in before submission. The field should also show a custom error message "Please enter a valid company email" when invalid. Which markup achieves both requirements using only HTML5 attributes?

- A) `<input type="email" required placeholder="Please enter a valid company email">`
- B) `<input type="email" required title="Please enter a valid company email">`
- C) `<input type="email" mandatory title="Please enter a valid company email">`
- D) `<input type="email" validate="true" message="Please enter a valid company email">`

> **Answer: B**  
> `required` enforces a non-empty value and `title` provides the tooltip/hint text that browsers display as the validation message. (For fully custom messages `setCustomValidity()` is used in JS, but `title` is the HTML-only approach.)

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q7.** A password field must be between 8 and 20 characters and contain only alphanumeric characters. Which HTML5 attributes enforce these constraints without JavaScript?

- A) `minlength="8" maxlength="20" type="password"`
- B) `min="8" max="20" pattern="[a-zA-Z0-9]+" type="password"`
- C) `minlength="8" maxlength="20" pattern="[a-zA-Z0-9]+" type="password"`
- D) `size="8-20" regex="[a-zA-Z0-9]+" type="password"`

> **Answer: C**  
> `minlength` and `maxlength` control character count, while `pattern` applies a regex constraint. `min`/`max` apply to numeric/date inputs, not text.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q8.** A checkout form has multiple sections: personal info, shipping address, and payment. The designer wants the browser's autofill to correctly distinguish between the "billing email" and the "shipping email" fields. Which attribute enables this?

- A) `name`
- B) `id`
- C) `autocomplete`
- D) `placeholder`

> **Answer: C**  
> The `autocomplete` attribute with values like `billing email` and `shipping email` tells the browser exactly what data each field expects, enabling accurate autofill.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q9.** A developer writes the following form:

```html
<form>
  <input type="text" name="city">
  <button type="button">Submit</button>
</form>
```

A tester reports the form never validates even though `required` was added to the input. What is the cause?

- A) `type="text"` does not support `required`.
- B) The `<button>` has `type="button"` instead of `type="submit"`, so form validation is never triggered.
- C) The form is missing an `action` attribute.
- D) `required` only works inside a `<fieldset>`.

> **Answer: B**  
> `type="button"` does not submit the form and therefore never triggers HTML5 constraint validation. It must be `type="submit"` (or omit `type`, which defaults to `submit`).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q10.** A survey form has a "Rating" field that accepts only whole numbers from 1 to 10, in steps of 1. Which input correctly enforces this?

- A) `<input type="number" min="1" max="10" step="1">`
- B) `<input type="range" min="1" max="10" step="1">`
- C) `<input type="text" pattern="[1-9]|10">`
- D) Both A and B

> **Answer: D**  
> Both `type="number"` (text-entry with spinner) and `type="range"` (slider) accept `min`, `max`, and `step`. The right choice depends on UX preference, but both enforce the constraint.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 3. HTML5 Input Types

**Q11.** A travel booking site needs a field where users enter their departure date. The field should display a native date-picker on supported browsers and store the value in `YYYY-MM-DD` format. Which input type should be used?

- A) `<input type="text" placeholder="YYYY-MM-DD">`
- B) `<input type="datetime">`
- C) `<input type="date">`
- D) `<input type="calendar">`

> **Answer: C**  
> `type="date"` renders a native date-picker and stores the value in `YYYY-MM-DD` format. `type="datetime"` is not a valid HTML5 input type (`datetime-local` is).

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q12.** An e-commerce site lets users pick a product colour. The developer wants the browser's native colour-picker widget with no extra libraries. Which input type should be used?

- A) `<input type="text" pattern="#[0-9A-Fa-f]{6}">`
- B) `<input type="color">`
- C) `<input type="hex">`
- D) `<input type="rgb">`

> **Answer: B**  
> `type="color"` invokes the OS/browser native colour-picker and returns a hex colour string.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q13.** A fitness app collects data via a mobile form. For the "Weight (kg)" field, the developer wants the numeric keypad to open automatically on mobile devices and prevent non-numeric input. Which input type is most appropriate?

- A) `<input type="text" inputmode="numeric">`
- B) `<input type="tel">`
- C) `<input type="number">`
- D) `<input type="integer">`

> **Answer: C**  
> `type="number"` opens the numeric keyboard on mobile and restricts input to valid numbers. While `inputmode="numeric"` on a `type="text"` opens a numeric keyboard, it does not restrict non-numeric input at the browser level.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q14.** A website's search bar should suggest previously entered searches from the browser history AND from a server-provided list of popular queries as the user types. Which HTML5 feature supports the server-provided suggestions natively?

- A) `<input type="search" autocomplete="on">`
- B) `<input type="search" list="suggestions"> <datalist id="suggestions">...</datalist>`
- C) `<input type="search" suggestions="popular-queries.json">`
- D) `<input type="search" data-source="server">`

> **Answer: B**  
> The `list` attribute paired with a `<datalist>` element provides a dropdown of predefined options that the browser merges with its autocomplete history.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q15.** A developer uses `<input type="hidden">` to pass a CSRF token through a form. A colleague suggests this is a security risk because the value is visible in the page source. What is the correct assessment?

- A) Hidden inputs are fully secure — the value cannot be seen by anyone.
- B) The colleague is correct — hidden inputs should never store sensitive tokens.
- C) Hidden inputs are visible in the page source but are appropriate for CSRF tokens, which are not secret from the page itself; the protection comes from server-side validation.
- D) Hidden inputs are encrypted by the browser before sending.

> **Answer: C**  
> CSRF tokens are not secret from the current page — they must be readable by the legitimate form. The protection relies on the server validating that the token in the request matches the user's session, which cross-origin requests cannot access.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 4. Media — Audio, Video & Canvas

**Q16.** A developer is embedding a promotional video that should play automatically and silently when the page loads, loop continuously, and never show playback controls. Which attribute combination achieves this?

- A) `autoplay loop muted`
- B) `autoplay loop controls="false"`
- C) `auto loop silent`
- D) `autostart loop nocontrols`

> **Answer: A**  
> `autoplay`, `loop`, and `muted` are valid HTML5 `<video>` attributes. Most browsers require `muted` for `autoplay` to work without user interaction. There is no `controls="false"` — omitting `controls` hides them.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q17.** A video element must support three formats to maximise browser compatibility. The browser should pick the first format it supports. How should this be marked up?

- A)
```html
<video src="movie.mp4,movie.webm,movie.ogv"></video>
```
- B)
```html
<video>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  <source src="movie.ogv" type="video/ogg">
</video>
```
- C)
```html
<video formats="mp4,webm,ogv" src="movie"></video>
```
- D)
```html
<video src="movie.mp4" fallback="movie.webm,movie.ogv"></video>
```

> **Answer: B**  
> Multiple `<source>` child elements inside `<video>` allow the browser to try each in order and use the first one it can decode.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q18.** A data dashboard needs to draw a bar chart that updates every second with live data. The chart involves pixel-level custom rendering. Which HTML5 element is the best fit?

- A) `<svg>`
- B) `<canvas>`
- C) `<picture>`
- D) `<figure>`

> **Answer: B**  
> `<canvas>` provides a pixel-based 2D (and WebGL) drawing API suited for dynamic, frequently updated graphics. SVG is better for static or interactively-selected vector graphics.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q19.** A developer writes the following Canvas code but the text never appears:

```javascript
const canvas = document.getElementById('myCanvas');
const ctx = canvas.getContext('2d');
ctx.font = '20px Arial';
ctx.fillText('Hello World', 10, 50);
```

A colleague points out the canvas element in HTML has no `width` or `height` attributes. What is the likely issue?

- A) `fillText` is not a valid Canvas API method.
- B) The default canvas size is 300×150 px, so the text may render but be clipped if coordinates exceed those bounds; additionally CSS-only sizing distorts the coordinate space without adjusting the internal resolution.
- C) Canvas requires `getContext('canvas')` not `getContext('2d')`.
- D) `ctx.font` must be set after `fillText`.

> **Answer: B**  
> Without explicit `width`/`height` attributes the canvas defaults to 300×150 px. Sizing only with CSS stretches the canvas, distorting the coordinate system. Always set `width` and `height` as HTML attributes to define the drawing buffer size.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q20.** An accessibility auditor flags that an `<audio>` element on a podcast page has no text alternative. What is the recommended HTML5-compliant fix?

- A) Add `alt="Podcast audio"` to the `<audio>` element.
- B) Add `controls` and provide a transcript or `<track kind="descriptions">` alongside the `<audio>` element.
- C) Replace `<audio>` with `<video>` so subtitles can be added.
- D) Wrap the `<audio>` in a `<figure>` with a `<figcaption>`.

> **Answer: B**  
> `<audio>` does not support `alt`. Accessibility best practice is to provide `controls` (so keyboard users can operate it) and a text transcript. `<track>` elements can also be used for descriptions.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 5. Browser Storage

**Q21.** A single-page application stores the user's theme preference (dark/light). The preference should persist across browser restarts but only for that origin. Which storage mechanism is most appropriate?

- A) `sessionStorage`
- B) `localStorage`
- C) A session cookie
- D) `IndexedDB`

> **Answer: B**  
> `localStorage` persists data with no expiry across sessions for the same origin. `sessionStorage` is cleared when the tab is closed, cookies expire and travel with every HTTP request, and IndexedDB is overkill for a single string value.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q22.** A collaborative document editor needs to store megabytes of structured JSON data (revision history) client-side and query it efficiently. Which browser storage option is the best fit?

- A) `localStorage`
- B) `sessionStorage`
- C) `IndexedDB`
- D) Cookies

> **Answer: C**  
> `IndexedDB` is a transactional, indexed, NoSQL database in the browser designed for large amounts of structured data. `localStorage` is limited to ~5 MB of strings and has no query capability.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q23.** A developer stores a JWT in `localStorage` to keep a user logged in. A security consultant flags this. What is the primary concern?

- A) `localStorage` data is deleted after 24 hours.
- B) `localStorage` is accessible via JavaScript, making it vulnerable to XSS attacks that could steal the token.
- C) JWTs cannot be stored as strings.
- D) `localStorage` is shared between browser tabs which exposes the token.

> **Answer: B**  
> Any JavaScript running on the page — including injected malicious scripts — can read `localStorage`. An `HttpOnly` cookie prevents this because it is inaccessible to JavaScript.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q24.** A user fills out a long multi-step form. The developer uses `sessionStorage` to save progress between steps. The user accidentally closes the tab and reopens the page. What happens to the saved form data?

- A) The data is still available because `sessionStorage` lasts for the browser session.
- B) The data is lost because `sessionStorage` is cleared when the tab is closed.
- C) The data is available because closing a tab does not end the session.
- D) The browser will prompt to restore the `sessionStorage` data.

> **Answer: B**  
> `sessionStorage` is scoped to the tab (browsing context). Closing the tab destroys the session and all its `sessionStorage` data.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q25.** Examine the following code:

```javascript
localStorage.setItem('cart', { items: ['book', 'pen'], total: 150 });
console.log(localStorage.getItem('cart'));
```

What does the console output?

- A) `{ items: ['book', 'pen'], total: 150 }`
- B) `[object Object]`
- C) `null`
- D) `undefined`

> **Answer: B**  
> `localStorage` stores only strings. When an object is passed to `setItem` without `JSON.stringify()`, the object's `.toString()` is called, producing `"[object Object]"`. Use `JSON.stringify()` before storing and `JSON.parse()` after retrieving.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 6. Accessibility

**Q26.** A designer creates a decorative divider image (a horizontal flourish). A screen reader user is reading the page. What is the correct way to mark up this image so screen readers skip it?

- A) `<img src="divider.png" alt="divider">`
- B) `<img src="divider.png" alt="">`
- C) `<img src="divider.png">`
- D) `<img src="divider.png" role="none">`

> **Answer: B**  
> An empty `alt=""` tells screen readers the image is decorative and should be skipped. Omitting `alt` entirely causes some screen readers to announce the file name. `role="none"` suppresses the role but does not replace the need for an empty `alt`.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q27.** A modal dialog opens when a user clicks a "Help" button. A keyboard-only user reports they cannot interact with the modal content because the Tab key moves focus to elements behind the modal. What ARIA or HTML technique addresses this?

- A) Add `tabindex="-1"` to all elements inside the modal.
- B) Implement a focus trap — keep Tab and Shift+Tab cycling within the modal's focusable elements while it is open, and add `aria-modal="true"` to the dialog.
- C) Add `role="dialog"` to the modal and nothing else.
- D) Use `pointer-events: none` on the background.

> **Answer: B**  
> A focus trap ensures keyboard focus cannot leave the modal. `aria-modal="true"` signals to assistive technologies that content behind the dialog is inert. `role="dialog"` alone does not trap focus.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q28.** A form has a custom-styled checkbox built from a `<div>`. A screen reader user cannot determine the checkbox state or interact with it. What is the minimum change to make it accessible without replacing the `<div>`?

- A) Add `class="checkbox"` to the `<div>`.
- B) Add `role="checkbox"`, `aria-checked="false"`, and `tabindex="0"` to the `<div>`, then toggle `aria-checked` on interaction.
- C) Wrap it in a `<label>`.
- D) Add `aria-label="checkbox"` to the `<div>`.

> **Answer: B**  
> `role="checkbox"` declares the element's purpose, `aria-checked` communicates its state, and `tabindex="0"` makes it keyboard-focusable. All three are required for basic accessibility.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q29.** A developer adds the following to a navigation landmark:

```html
<nav aria-label="Main navigation">...</nav>
<nav aria-label="Footer navigation">...</nav>
```

A colleague says using `aria-label` on `<nav>` is redundant. Who is correct?

- A) The colleague — `<nav>` already has an implicit landmark role, so `aria-label` adds no value.
- B) The developer — when multiple `<nav>` landmarks exist on a page, `aria-label` distinguishes them so screen reader users can identify each one.
- C) The colleague — `aria-labelledby` must be used instead of `aria-label`.
- D) Both are wrong — only one `<nav>` is allowed per page.

> **Answer: B**  
> When a page has more than one landmark of the same type, WCAG recommends labelling each with `aria-label` or `aria-labelledby` so users can distinguish between them in the landmark list.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q30.** An icon-only button uses a magnifying glass SVG for "Search". A blind user navigates to the button and hears nothing descriptive. Which is the correct accessible fix?

- A) Add `title="Search"` to the `<button>`.
- B) Add `aria-label="Search"` to the `<button>` and `aria-hidden="true"` to the SVG inside it.
- C) Add `alt="Search"` to the `<button>`.
- D) Wrap the SVG in a `<figure>` with `<figcaption>Search</figcaption>`.

> **Answer: B**  
> `aria-label="Search"` on the `<button>` provides the accessible name. `aria-hidden="true"` on the SVG prevents the screen reader from announcing SVG internals (paths, groups) as duplicate content.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 7. Semantics (Advanced)

**Q31.** A developer adds the following markup to a product listing:

```html
<div itemscope itemtype="https://schema.org/Product">
  <span itemprop="name">Wireless Headphones</span>
  <span itemprop="price">$49.99</span>
</div>
```

What HTML5 feature is being used and what is its purpose?

- A) ARIA landmarks — to improve keyboard navigation.
- B) Microdata — to embed structured data that search engines can parse to produce rich results.
- C) RDFa — to link the product to a semantic knowledge graph.
- D) Custom data attributes — to store product metadata for JavaScript.

> **Answer: B**  
> `itemscope`, `itemtype`, and `itemprop` are HTML5 Microdata attributes. They annotate content with structured data vocabularies (such as Schema.org) that search engines use to generate rich results.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q32.** A developer must mark up an abbreviation on first use so that its full form is available to all users including those using screen readers. Which markup is correct?

- A) `<acronym title="World Health Organization">WHO</acronym>`
- B) `<abbr title="World Health Organization">WHO</abbr>`
- C) `<dfn>WHO (World Health Organization)</dfn>`
- D) `<span aria-label="World Health Organization">WHO</span>`

> **Answer: B**  
> `<abbr>` is the correct semantic element for abbreviations and acronyms. The `title` attribute provides the expansion, which browsers display as a tooltip and some screen readers announce. `<acronym>` was removed in HTML5.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q33.** A legal document page contains a passage that was recently changed. The old price "$40" was replaced with "$35". Which HTML5 markup correctly represents this edit so that the change is semantically conveyed?

- A) `<strike>$40</strike> <b>$35</b>`
- B) `<del>$40</del> <ins>$35</ins>`
- C) `<s>$40</s> $35`
- D) `<del>$40</del> <b>$35</b>`

> **Answer: B**  
> `<del>` marks content that has been removed and `<ins>` marks content that has been inserted. Both carry semantic meaning that assistive technologies and search engines can interpret. `<s>` indicates content that is no longer accurate but does not imply an edit.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q34.** A blog engine outputs breadcrumbs as an ordered list: Home > Blog > Article. Which semantic element should wrap the breadcrumb trail?

- A) `<div class="breadcrumb">`
- B) `<nav aria-label="Breadcrumb"><ol>...</ol></nav>`
- C) `<section id="breadcrumb"><ul>...</ul></section>`
- D) `<menu type="breadcrumb"><li>...</li></menu>`

> **Answer: B**  
> Breadcrumbs are a navigational structure, so `<nav>` is the correct wrapper. An `<ol>` conveys the ordered hierarchy. `aria-label="Breadcrumb"` distinguishes this `<nav>` from others on the page.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q35.** A developer builds a side panel that shows supplementary content — author bio, related articles — next to the main article on a blog. Which element should wrap this side panel?

- A) `<section>`
- B) `<div>`
- C) `<aside>`
- D) `<sidebar>`

> **Answer: C**  
> `<aside>` represents content tangentially related to the surrounding content — perfect for author bios, ads, and related links placed beside the main content. `<sidebar>` is not a valid HTML5 element.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q36.** The following page outline is produced by a screen reader's heading navigation:

```
H1: Company Name
H3: Our Products
H2: Contact Us
```

What is wrong with this structure?

- A) There is nothing wrong; headings can be used in any order.
- B) The heading hierarchy skips from H1 to H3, breaking the logical document outline and confusing screen reader users who rely on sequential headings.
- C) H1 should not contain the company name.
- D) H2 must always come before H3.

> **Answer: B**  
> Heading levels should not skip ranks (e.g., H1 → H3) because screen reader users navigate by heading level to understand document structure. Skipping levels breaks the expected outline.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q37.** A developer needs to display a table of data showing quarterly sales figures. Each column has a header. Which attribute ensures screen readers correctly associate data cells with column headers?

- A) `id` on each `<td>`
- B) `scope="col"` on each `<th>`
- C) `headers` on each `<th>`
- D) `aria-colheader` on each `<tr>`

> **Answer: B**  
> `scope="col"` on a `<th>` element explicitly declares that the header applies to all cells in its column. This is the standard HTML attribute for associating column headers with data cells.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q38.** An online magazine uses the following structure:

```html
<body>
  <header>...</header>
  <main>
    <article>
      <header><h1>Article Title</h1></header>
      <p>Content...</p>
      <footer><p>Published by Jane</p></footer>
    </article>
  </main>
  <footer>...</footer>
</body>
```

A reviewer says nesting `<header>` and `<footer>` inside `<article>` is invalid HTML5. Are they correct?

- A) Yes — `<header>` and `<footer>` are only valid as direct children of `<body>`.
- B) No — `<header>` and `<footer>` are valid inside any sectioning element, including `<article>`.
- C) Yes — `<article>` cannot contain block-level elements.
- D) No — but only `<footer>` is valid inside `<article>`; `<header>` is not.

> **Answer: B**  
> HTML5 allows `<header>` and `<footer>` inside any sectioning content elements (`<article>`, `<section>`, `<aside>`, `<nav>`). They represent the header/footer of that specific section, not the entire page.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q39.** A `<figure>` element contains a chart image. Which element should be used to provide a caption that is programmatically associated with the image?

- A) `<caption>`
- B) `<legend>`
- C) `<figcaption>`
- D) `<label>`

> **Answer: C**  
> `<figcaption>` is the correct child element of `<figure>` for providing a caption. `<caption>` is used inside `<table>`, `<legend>` inside `<fieldset>`, and `<label>` with form controls.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q40.** A developer is unsure whether to use a `<div>` or `<section>` for grouping related content. What is the key distinction?



- A) `<div>` is a block element; `<section>` is an inline element.
- B) `<section>` should be used only when the content has a heading and represents a thematic grouping that would appear in a document outline; `<div>` is a generic container with no semantic meaning.
- C) `<section>` renders with a visible border by default; `<div>` does not.
- D) `<div>` and `<section>` are completely interchangeable in HTML5.

> **Answer: B**  
> `<section>` is a thematic grouping element that typically contains a heading and contributes to the document outline. `<div>` carries no semantic meaning and should be used for purely presentational or scripting groupings.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 8. Responsive Images

**Q41.** A news site serves hero images. On mobile (viewport ≤ 600 px) it should display a 480 px wide image; on desktop it should display a 1200 px wide image — both in WebP format with JPEG fallbacks. Which HTML5 element is designed for this use case?

- A) `<img srcset="small.jpg 480w, large.jpg 1200w">`
- B) `<picture>` with multiple `<source>` elements
- C) CSS `background-image` with media queries
- D) `<img data-mobile="small.jpg" data-desktop="large.jpg">`

> **Answer: B**  
> `<picture>` allows specifying multiple `<source>` elements with `media` and `type` conditions. The browser selects the first matching source, enabling both art direction and format selection. `srcset` alone on `<img>` handles resolution switching but not art direction or format fallback together.

**Example:**
```html
<picture>
  <source media="(max-width: 600px)" srcset="hero-small.webp" type="image/webp">
  <source media="(max-width: 600px)" srcset="hero-small.jpg" type="image/jpeg">
  <source srcset="hero-large.webp" type="image/webp">
  <img src="hero-large.jpg" alt="Breaking news hero image">
</picture>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q42.** A developer writes:

```html
<img src="photo.jpg"
     srcset="photo-480.jpg 480w, photo-800.jpg 800w, photo-1200.jpg 1200w"
     sizes="(max-width: 600px) 100vw, 50vw"
     alt="Mountain landscape">
```

What does the `sizes` attribute tell the browser?

- A) The pixel dimensions of each image listed in `srcset`.
- B) The rendered display width of the image at different viewport sizes, so the browser can pick the best `srcset` candidate before downloading.
- C) The maximum file size allowed for each source.
- D) The number of columns the image occupies in a CSS grid.

> **Answer: B**  
> `sizes` describes how wide the image will be rendered at various viewport breakpoints. The browser uses this information together with the device pixel ratio to choose the most appropriate `srcset` candidate — all before making any network request.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q43.** An e-commerce page lists product thumbnails. Each thumbnail is always rendered at exactly 200 px wide regardless of viewport. The same image is available at 200 px, 400 px (for 2× Retina), and 600 px (for 3× Retina). Which markup serves the correct resolution to each device?

- A) `<img src="thumb-200.jpg" srcset="thumb-400.jpg 2x, thumb-600.jpg 3x" alt="Product">`
- B) `<img src="thumb-200.jpg" srcset="thumb-400.jpg 400w, thumb-600.jpg 600w" alt="Product">`
- C) `<picture><source srcset="thumb-600.jpg"><img src="thumb-200.jpg" alt="Product"></picture>`
- D) `<img src="thumb-600.jpg" alt="Product">`

> **Answer: A**  
> When the rendered size is fixed, descriptor `2x` and `3x` (device pixel ratio descriptors) precisely target the correct image for each screen density without needing a `sizes` attribute.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q44.** A developer removes the `alt` attribute entirely from an `<img>` to save bytes. What is the impact?

- A) The browser displays a broken-image icon and announces the file path to screen reader users.
- B) The image is treated as decorative and screen readers skip it — identical to `alt=""`.
- C) It is a validation error and the browser refuses to render the image.
- D) The browser falls back to the `title` attribute as the text alternative.

> **Answer: A**  
> Omitting `alt` is invalid HTML5. Most screen readers fall back to announcing the `src` URL or filename, which is unhelpful. An empty `alt=""` is the correct way to mark a decorative image.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q45.** A developer wants to defer loading of below-the-fold images so they only load when the user scrolls near them, using a native browser feature and no JavaScript library. Which attribute enables this?

- A) `<img src="photo.jpg" defer>`
- B) `<img src="photo.jpg" loading="lazy">`
- C) `<img src="photo.jpg" async>`
- D) `<img src="photo.jpg" fetchpriority="low">`

> **Answer: B**  
> The `loading="lazy"` attribute instructs the browser to defer loading the image until it is near the viewport. It is a native HTML attribute requiring zero JavaScript.

**Example:**
```html
<!-- Hero image — load immediately -->
<img src="hero.jpg" loading="eager" alt="Hero banner">

<!-- Below-the-fold images — load lazily -->
<img src="card1.jpg" loading="lazy" alt="Card 1">
<img src="card2.jpg" loading="lazy" alt="Card 2">
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 9. Web APIs

**Q46.** A ride-sharing app needs the user's current GPS coordinates. The user's browser supports the HTML5 Geolocation API. Which JavaScript call correctly retrieves the position once?

- A) `navigator.location.get(callback)`
- B) `navigator.geolocation.getCurrentPosition(successCallback, errorCallback)`
- C) `window.gps.getPosition()`
- D) `document.geolocation.getCoords()`

> **Answer: B**  
> `navigator.geolocation.getCurrentPosition()` is the standard HTML5 API call. It requires user permission and invokes `successCallback` with a `GeolocationPosition` object, or `errorCallback` on failure.

**Example:**
```html
<button onclick="getLocation()">Find Me</button>
<p id="output"></p>

<script>
  function getLocation() {
    if (!navigator.geolocation) {
      document.getElementById('output').textContent = 'Geolocation not supported.';
      return;
    }
    navigator.geolocation.getCurrentPosition(
      (pos) => {
        document.getElementById('output').textContent =
          `Lat: ${pos.coords.latitude}, Lng: ${pos.coords.longitude}`;
      },
      (err) => {
        document.getElementById('output').textContent = `Error: ${err.message}`;
      }
    );
  }
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q47.** A project management app allows users to drag tasks between columns. A developer implements drag-and-drop using the HTML5 Drag and Drop API. Which event on the **drop target** must call `event.preventDefault()` to allow a drop?

- A) `dragstart`
- B) `dragend`
- C) `dragover`
- D) `drop`

> **Answer: C**  
> By default, most elements do not accept drops. Calling `event.preventDefault()` inside the `dragover` handler signals to the browser that this element is a valid drop target, enabling the `drop` event to fire.

**Example:**
```html
<div id="task" draggable="true" ondragstart="drag(event)">Task A</div>
<div id="column" ondragover="allowDrop(event)" ondrop="drop(event)">
  Drop here
</div>

<script>
  function allowDrop(e) { e.preventDefault(); }          // required!
  function drag(e)      { e.dataTransfer.setData('text', e.target.id); }
  function drop(e) {
    e.preventDefault();
    const id = e.dataTransfer.getData('text');
    e.target.appendChild(document.getElementById(id));
  }
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q48.** A data-processing web app runs a complex sorting algorithm that freezes the UI for several seconds. A colleague suggests moving it to a Web Worker. What is the primary benefit?

- A) Web Workers allow direct DOM manipulation on a background thread, speeding up rendering.
- B) Web Workers run scripts on a separate thread, keeping the main (UI) thread responsive while heavy computation executes in the background.
- C) Web Workers compile JavaScript to machine code for faster execution.
- D) Web Workers cache computation results in `localStorage` automatically.

> **Answer: B**  
> Web Workers operate on a separate OS thread. Because they cannot touch the DOM, the main thread remains free to handle user events and rendering, preventing UI freezes.

**Example:**
```html
<!-- main.html -->
<script>
  const worker = new Worker('sorter.js');
  worker.postMessage({ data: [5, 3, 1, 4, 2] });
  worker.onmessage = (e) => console.log('Sorted:', e.data.result);
</script>
```
```javascript
// sorter.js  (Web Worker script — no DOM access)
self.onmessage = function (e) {
  const sorted = e.data.data.slice().sort((a, b) => a - b);
  self.postMessage({ result: sorted });
};
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q49.** A financial trading dashboard streams live price updates from a server. The connection must remain open and push data to the client continuously. Which HTML5 API is purpose-built for this one-way server-to-client streaming?

- A) `XMLHttpRequest` with long polling
- B) `WebSocket`
- C) `EventSource` (Server-Sent Events)
- D) `fetch` with `keepalive: true`

> **Answer: C**  
> `EventSource` (Server-Sent Events) is designed for one-way, server-to-client streaming over HTTP. It automatically reconnects on disconnect and supports event IDs. WebSockets are bidirectional and more appropriate when the client also needs to push data to the server.

**Example:**
```javascript
// Client
const source = new EventSource('/prices');
source.addEventListener('price-update', (e) => {
  const { symbol, price } = JSON.parse(e.data);
  updateUI(symbol, price);
});
source.onerror = () => console.warn('Connection lost, retrying…');
```
```php
// Server (PHP) — sse_prices.php
header('Content-Type: text/event-stream');
header('Cache-Control: no-cache');
while (true) {
    echo "event: price-update\n";
    echo 'data: {"symbol":"AAPL","price":' . rand(150, 200) . "}\n\n";
    ob_flush(); flush();
    sleep(1);
}
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q50.** A developer uses the HTML5 History API to build a single-page application with bookmarkable URLs. After calling `history.pushState({ page: 2 }, '', '/products')`, the user clicks the browser's Back button. Which event fires and where can the state be retrieved?

- A) `hashchange` event; state from `location.hash`
- B) `popstate` event on `window`; state from `event.state`
- C) `navigate` event on `document`; state from `history.current`
- D) `statechange` event on `history`; state from `history.state`

> **Answer: B**  
> Clicking Back/Forward after `pushState`/`replaceState` fires the `popstate` event on `window`. The state object passed to `pushState` is available as `event.state`.

**Example:**
```javascript
// Navigate programmatically
document.getElementById('nextPage').addEventListener('click', () => {
  history.pushState({ page: 2 }, '', '/products');
  renderPage(2);
});

// Handle browser back/forward
window.addEventListener('popstate', (e) => {
  if (e.state) renderPage(e.state.page);
});
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 10. Custom Data Attributes

**Q51.** A developer stores product IDs on list items using the `data-*` attribute pattern:

```html
<li data-product-id="SKU-9821" data-category="electronics">Laptop</li>
```

How is `data-product-id` accessed in JavaScript?

- A) `element.getAttribute('data-product-id')`  — only method
- B) `element.dataset.productId`  — only method
- C) Both `element.getAttribute('data-product-id')` and `element.dataset.productId` return the value; `dataset` converts kebab-case to camelCase.
- D) `element.data['product-id']`

> **Answer: C**  
> `getAttribute('data-product-id')` returns the raw attribute value. `element.dataset.productId` uses the `DOMStringMap` API which automatically converts `data-product-id` (kebab-case) to `productId` (camelCase). Both are valid.

**Example:**
```html
<ul>
  <li id="item" data-product-id="SKU-9821" data-category="electronics">Laptop</li>
</ul>
<script>
  const el = document.getElementById('item');
  console.log(el.getAttribute('data-product-id')); // "SKU-9821"
  console.log(el.dataset.productId);               // "SKU-9821"
  console.log(el.dataset.category);                // "electronics"
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q52.** A team stores sensitive user data such as credit card numbers in `data-*` attributes to pass them around the DOM. A security reviewer objects. Who is correct, and why?

- A) The reviewer is wrong — `data-*` attributes are invisible to users.
- B) The reviewer is correct — `data-*` attributes are part of the DOM and accessible to any JavaScript running on the page, including malicious scripts injected via XSS.
- C) The reviewer is wrong — `data-*` attributes are encrypted by the browser.
- D) The reviewer is correct — `data-*` attributes are sent with every HTTP request like cookies.

> **Answer: B**  
> `data-*` attributes are visible in the page source and fully accessible via JavaScript. Storing sensitive data there exposes it to XSS attacks. Sensitive data should never be embedded in the DOM.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q53.** A developer uses CSS to style a button differently based on its state using a `data-*` attribute. Which CSS selector targets a button where `data-state="active"`?

- A) `button.data-state-active`
- B) `button[data-state="active"]`
- C) `button:data(state, active)`
- D) `button#active`

> **Answer: B**  
> CSS attribute selectors (`[attr="value"]`) work with `data-*` attributes just like any other HTML attribute.

**Example:**
```html
<button data-state="inactive" id="btn">Toggle</button>
<style>
  button[data-state="active"]   { background: green; color: white; }
  button[data-state="inactive"] { background: grey; }
</style>
<script>
  document.getElementById('btn').addEventListener('click', function () {
    this.dataset.state = this.dataset.state === 'active' ? 'inactive' : 'active';
  });
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q54.** A developer needs to store a multi-word string `"free shipping"` in a `data-*` attribute and retrieve it via `dataset`. What is the correct attribute name so that `element.dataset.shippingType` returns `"free shipping"`?

- A) `data-shippingType="free shipping"`
- B) `data-shipping-type="free shipping"`
- C) `data-shipping_type="free shipping"`
- D) `data-SHIPPING-TYPE="free shipping"`

> **Answer: B**  
> The Dataset API converts `data-` attribute names from kebab-case to camelCase: `data-shipping-type` → `dataset.shippingType`. Uppercase letters in the attribute name are not allowed per the HTML5 specification.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q55.** A developer writes a tooltip library that reads the tooltip text from a `data-tooltip` attribute and creates a `<div>` dynamically. The text is inserted with `innerHTML`. A colleague warns this is dangerous. What is the correct fix?

- A) Use `data-tooltip-safe` instead of `data-tooltip`.
- B) Sanitise the `data-tooltip` value or use `textContent` / `innerText` instead of `innerHTML` to prevent XSS.
- C) Encode the value in Base64 before storing it in the attribute.
- D) There is no risk because `data-*` values are automatically HTML-escaped by the browser.

> **Answer: B**  
> `innerHTML` interprets the string as HTML, so a crafted `data-tooltip` value like `<img onerror="stealCookies()">` would execute malicious code. Always use `textContent` for plain text or a trusted sanitiser for HTML.

**Example:**
```javascript
// Unsafe
tooltip.innerHTML = element.dataset.tooltip;

// Safe
tooltip.textContent = element.dataset.tooltip;
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 11. Meta & Document Head

**Q56.** A mobile web app's layout looks zoomed-out on smartphones, showing the desktop-sized page scaled down. Which `<meta>` tag instructs the browser to match the device's screen width and set the initial zoom to 100%?

- A) `<meta name="mobile" content="width=device, zoom=1">`
- B) `<meta name="viewport" content="width=device-width, initial-scale=1">`
- C) `<meta name="screen" content="responsive">`
- D) `<meta http-equiv="viewport" content="device-width">`

> **Answer: B**  
> The `viewport` meta tag is the standard way to control how the browser scales and sizes the page on mobile devices. `width=device-width` matches the physical screen width; `initial-scale=1` sets 1:1 zoom.

**Example:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Page</title>
</head>
<body>...</body>
</html>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q57.** A developer wants to load a third-party analytics script without blocking HTML parsing, but the script depends on the fully parsed DOM. Which `<script>` attribute should be used?

- A) `async`
- B) `defer`
- C) `type="module"`
- D) `preload`

> **Answer: B**  
> `defer` downloads the script in parallel with HTML parsing and executes it in order after the document is fully parsed, but before `DOMContentLoaded`. `async` also downloads in parallel but executes immediately when ready, potentially before parsing is complete.

**Example:**
```html
<head>
  <!-- Parsed after DOM is ready, in document order -->
  <script src="analytics.js" defer></script>

  <!-- Parsed as soon as downloaded, order not guaranteed -->
  <script src="widget.js" async></script>
</head>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q58.** A developer wants to hint to the browser to establish a connection to `https://api.example.com` early — before any actual fetch is made — to reduce latency. Which `<link>` relationship achieves this?

- A) `<link rel="prefetch" href="https://api.example.com">`
- B) `<link rel="preload" href="https://api.example.com" as="fetch">`
- C) `<link rel="preconnect" href="https://api.example.com">`
- D) `<link rel="dns-prefetch" href="https://api.example.com">`

> **Answer: C**  
> `rel="preconnect"` instructs the browser to perform the DNS lookup, TCP handshake, and TLS negotiation with the target origin early. `rel="dns-prefetch"` only resolves the DNS without establishing the full connection.

**Example:**
```html
<head>
  <!-- Full connection (DNS + TCP + TLS) -->
  <link rel="preconnect" href="https://api.example.com">

  <!-- DNS only — lightweight fallback for older browsers -->
  <link rel="dns-prefetch" href="https://api.example.com">
</head>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q59.** A developer sets the following `<meta>` tag to prevent search engines from indexing a staging site:

```html
<meta name="robots" content="noindex, nofollow">
```

A colleague says this is unreliable because Google can still index the page. Under what condition is the colleague correct?

- A) `noindex` is not a valid value; the correct value is `none`.
- B) If the page is linked from another indexed page, Google ignores the meta tag.
- C) If the page is blocked in `robots.txt`, Google may never receive the meta tag and index the page from external links anyway; the most reliable solution combines `robots.txt` disallow with the `noindex` meta tag and HTTP authentication.
- D) Google only respects `noindex` on the `<body>` element, not `<meta>`.

> **Answer: C**  
> If `robots.txt` blocks crawling, the bot never reads the meta tag but may still list the URL in search results based on link signals. The robust solution is no `robots.txt` block (so the bot can read the tag) combined with `noindex` — or use HTTP authentication to restrict access entirely.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q60.** A developer wants shareable links to their news article to show a rich preview card (title, description, image) when posted on social media. Which set of `<meta>` tags is responsible for this?

- A) `<meta name="keywords">` and `<meta name="description">`
- B) Open Graph tags — `<meta property="og:title">`, `<meta property="og:description">`, `<meta property="og:image">`
- C) `<meta name="twitter:title">` alone is sufficient for all platforms.
- D) `<link rel="icon">` controls the preview image.

> **Answer: B**  
> Open Graph protocol (`og:*`) meta tags are the standard adopted by most social platforms (Facebook, LinkedIn, WhatsApp, Slack) to generate link preview cards. Twitter additionally supports its own `twitter:*` card tags, but most platforms fall back to Open Graph.

**Example:**
```html
<head>
  <meta property="og:type"        content="article">
  <meta property="og:title"       content="HTML5 Best Practices in 2026">
  <meta property="og:description" content="A deep dive into modern HTML5 features.">
  <meta property="og:image"       content="https://example.com/preview.jpg">
  <meta property="og:url"         content="https://example.com/html5-guide">

  <!-- Twitter Card fallback -->
  <meta name="twitter:card"       content="summary_large_image">
  <meta name="twitter:title"      content="HTML5 Best Practices in 2026">
  <meta name="twitter:image"      content="https://example.com/preview.jpg">
</head>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 12. SVG

**Q61.** A company logo must remain crisp at every screen resolution and be styleable with CSS (colour changes on hover). A developer is choosing between embedding the logo as a PNG, a `<canvas>` drawing, or inline SVG. Which approach is best suited?

- A) PNG — it is universally supported and requires no extra markup.
- B) `<canvas>` — it renders at any resolution without quality loss.
- C) Inline SVG — it is resolution-independent, can be targeted by CSS selectors, and its elements are part of the DOM.
- D) An `<img>` pointing to an `.svg` file — it is resolution-independent and CSS-styleable.

> **Answer: C**  
> Inline SVG embeds the SVG DOM directly into the HTML document, making individual paths and shapes targetable by CSS and JavaScript. An `<img src="logo.svg">` is resolution-independent but its internals are isolated and cannot be styled by the page's CSS. PNG is raster-based and pixelates at high DPR. `<canvas>` is pixel-based and not resolution-independent without manual DPR scaling.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q62.** An icon library defines reusable SVG shapes with `<symbol>` and references them with `<use>`. A developer writes:

```html
<svg style="display:none">
  <symbol id="icon-bell" viewBox="0 0 24 24">
    <path d="M12 22c1.1 0 2-.9 2-2h-4c0 1.1.9 2 2 2z"/>
    <path d="M18 16v-5c0-3.07-1.64-5.64-4.5-6.32V4c0-.83-.67-1.5-1.5-1.5s-1.5.67-1.5 1.5v.68C7.63 5.36 6 7.92 6 11v5l-2 2v1h16v-1l-2-2z"/>
  </symbol>
</svg>

<svg aria-label="Notifications" role="img"><use href="#icon-bell"></use></svg>
```

What is the primary benefit of this pattern?

- A) The browser caches each `<symbol>` as a separate HTTP request.
- B) The SVG markup for each icon is defined once and referenced many times, reducing HTML duplication and keeping a single source of truth.
- C) `<symbol>` automatically resizes the icon to fit its container without a `viewBox`.
- D) `<use>` allows scripts to modify the original `<symbol>` paths from any reference site.

> **Answer: B**  
> The `<symbol>` + `<use>` pattern is an SVG sprite technique. The shape is defined once inside a hidden `<svg>`, and `<use href="#id">` clones it wherever needed, eliminating markup repetition. `viewBox` on `<symbol>` still needs to be set for correct scaling.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q63.** A developer embeds an SVG with the following `viewBox`:

```html
<svg viewBox="0 0 100 50" width="400" height="200">
  <rect x="0" y="0" width="100" height="50" fill="steelblue"/>
</svg>
```

What does `viewBox="0 0 100 50"` define?

- A) The pixel dimensions the SVG will be rendered at on screen.
- B) The internal coordinate system of the SVG — the area of SVG space mapped onto the element's width and height.
- C) The minimum and maximum zoom levels allowed.
- D) The clipping region that hides content outside those bounds.

> **Answer: B**  
> `viewBox="min-x min-y width height"` establishes the internal coordinate system. The SVG engine maps the 100×50 unit canvas onto the 400×200 px element, scaling all child elements automatically. This is what makes SVGs resolution-independent.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q64.** A developer compares two approaches for displaying a search icon button:

```html
<!-- A -->
<button>
  <img src="search.svg" alt="Search">
</button>

<!-- B -->
<button aria-label="Search">
  <svg aria-hidden="true" focusable="false" viewBox="0 0 24 24">
    <path d="M21 21l-4.35-4.35M17 11A6 6 0 1 1 5 11a6 6 0 0 1 12 0z"/>
  </svg>
</button>
```

Which approach is preferred and why?

- A) Approach A — `<img>` with `alt` is always the correct way to provide accessible text.
- B) Approach B — inline SVG with `aria-hidden` on the SVG and `aria-label` on the button avoids redundant announcements and keeps the accessible name on the interactive element.
- C) Both are equally accessible; choose based on file size.
- D) Approach A — external SVG files load faster than inline SVG.

> **Answer: B**  
> With inline SVG, `aria-hidden="true"` prevents screen readers from announcing SVG internals (paths, groups) and `focusable="false"` prevents IE/Edge from placing focus on the SVG itself. The button's `aria-label` provides the single, clear accessible name. Approach A works but provides less control over how assistive technology announces the icon.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q65.** A developer adds a CSS animation to an inline SVG path to draw a loading spinner. The animation uses `stroke-dashoffset`. Which statement correctly describes SVG versus Canvas for this scenario?

- A) Canvas is better because CSS animations cannot target SVG elements.
- B) SVG is better because individual SVG elements are DOM nodes that CSS transitions and animations can target directly; Canvas pixels have no DOM representation.
- C) They are equivalent — both support CSS `stroke-dashoffset`.
- D) Canvas is better because SVG animations are not hardware-accelerated.

> **Answer: B**  
> SVG shapes are DOM elements, so CSS properties like `stroke-dasharray`, `stroke-dashoffset`, `opacity`, and `transform` can be animated with CSS or the Web Animations API. Canvas draws pixels with no persistent DOM nodes, so animations require imperative JavaScript redraws each frame.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 13. WebSocket API

**Q66.** A multiplayer game needs the server to push position updates to all connected players, and each player's browser must simultaneously send its own position back to the server — all in real time with minimal latency. Which HTML5 API is the correct choice?

- A) Server-Sent Events (`EventSource`) — it is built for real-time server push.
- B) `fetch` with `keepalive: true` — it maintains a persistent connection.
- C) WebSocket — it provides a full-duplex, bidirectional, persistent connection over a single TCP connection.
- D) Long polling with `XMLHttpRequest` — it simulates real-time communication.

> **Answer: C**  
> WebSocket is the only option that allows simultaneous, low-latency, bidirectional data flow. `EventSource` is one-way (server → client only). `keepalive` fetch is for request persistence, not streaming. Long polling has high latency and overhead.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q67.** A WebSocket client connects using `ws://chat.example.com/socket`. A security engineer flags the connection as insecure. What is the correct fix and why?

- A) Use `wss://chat.example.com/socket` — `wss` tunnels WebSocket traffic through TLS, encrypting data in transit.
- B) Add `secure="true"` to the `WebSocket` constructor options.
- C) Switch from WebSocket to `https://` — HTTPS automatically secures WebSocket connections.
- D) No change is needed — WebSocket data is binary and therefore unreadable to eavesdroppers.

> **Answer: A**  
> `ws://` transmits data in plain text; `wss://` (WebSocket Secure) wraps the connection in TLS — the same protocol used by HTTPS. It is mandatory on HTTPS pages (browsers block mixed-content `ws://` connections from secure origins).

**Example:**
```javascript
// Insecure — avoid on production
const unsafeSocket = new WebSocket('ws://chat.example.com/socket');

// Secure — always use in production
const socket = new WebSocket('wss://chat.example.com/socket');
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q68.** A developer opens a WebSocket and needs to handle incoming messages, connection errors, and clean closure. Which set of event handlers covers all three?

- A) `socket.ondata`, `socket.onfail`, `socket.ondone`
- B) `socket.onmessage`, `socket.onerror`, `socket.onclose`
- C) `socket.receive`, `socket.error`, `socket.end`
- D) `socket.onopen`, `socket.onmessage`, `socket.onclose`

> **Answer: B**  
> The four WebSocket events are `onopen` (connection established), `onmessage` (data received), `onerror` (connection error), and `onclose` (connection closed). To handle incoming messages, errors, and closure, you need `onmessage`, `onerror`, and `onclose`.

**Example:**
```javascript
const socket = new WebSocket('wss://example.com/ws');

socket.onopen    = ()  => console.log('Connected');
socket.onmessage = (e) => console.log('Received:', e.data);
socket.onerror   = (e) => console.error('Error:', e);
socket.onclose   = (e) => console.log('Closed, code:', e.code);
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q69.** A developer sends an object over a WebSocket:

```javascript
const socket = new WebSocket('wss://example.com/ws');
socket.onopen = () => {
  socket.send({ type: 'chat', text: 'Hello!' });
};
```

What is the actual data received by the server?

- A) `{ "type": "chat", "text": "Hello!" }` — the WebSocket API serialises objects automatically.
- B) `"[object Object]"` — `send()` calls `.toString()` on non-string values.
- C) A binary `Blob` containing the object.
- D) Nothing — `send()` throws a `TypeError` for object arguments.

> **Answer: B**  
> `WebSocket.send()` accepts `string`, `Blob`, `ArrayBuffer`, or `ArrayBufferView`. Passing a plain object invokes `.toString()`, yielding `"[object Object]"`. Always use `JSON.stringify()` for structured data.

**Example:**
```javascript
// Wrong
socket.send({ type: 'chat', text: 'Hello!' }); // sends "[object Object]"

// Correct
socket.send(JSON.stringify({ type: 'chat', text: 'Hello!' }));

// Receiving
socket.onmessage = (e) => {
  const msg = JSON.parse(e.data);
  console.log(msg.type, msg.text);
};
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q70.** A WebSocket-based chat app sends the user's session token as a query parameter: `wss://example.com/ws?token=eyJhbGci...`. A security reviewer objects. What is the primary concern and the recommended alternative?

- A) Query parameters are encrypted by `wss://`, so there is no concern.
- B) Query parameters appear in server access logs, browser history, and referrer headers, potentially exposing the token. The recommended alternative is to send the token in the first WebSocket message after the connection opens, or use a short-lived ticket issued by the server over HTTPS.
- C) WebSocket does not support query parameters; the connection will fail.
- D) The token should be Base64-encoded in the query string to make it safe.

> **Answer: B**  
> Even over TLS, URLs (including query strings) are recorded in server logs, proxy logs, and browser history. Sensitive tokens in URLs are a known OWASP risk. The safer pattern is to exchange a short-lived, opaque ticket via a secure HTTPS endpoint and pass that ticket as the first WebSocket message, or use cookies with `HttpOnly` and `Secure` flags for authentication.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 14. IFrame & Sandbox

**Q71.** A content management platform embeds third-party widgets using `<iframe>`. A security auditor recommends adding the `sandbox` attribute with no value:

```html
<iframe src="https://widget.example.com" sandbox></iframe>
```

What restrictions does a value-less `sandbox` apply?

- A) No restrictions — `sandbox` must be given explicit permission values to do anything.
- B) It blocks all scripts, form submission, popups, pointer lock, top-level navigation, and same-origin access within the iframe.
- C) It only blocks JavaScript but allows forms and navigation.
- D) It enables HTTPS enforcement but no other restrictions.

> **Answer: B**  
> A bare `sandbox` attribute applies the maximum restriction set: scripts disabled, forms blocked, popups blocked, plugins blocked, same-origin access denied, and top-level navigation prevented. Each capability must be explicitly re-enabled with a `allow-*` token.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q72.** An embedded payment iframe must be able to submit a form but must not be allowed to run JavaScript or open popups. Which `sandbox` value is correct?

- A) `sandbox="allow-scripts allow-forms"`
- B) `sandbox="allow-forms"`
- C) `sandbox="allow-forms allow-popups"`
- D) `sandbox="forms-only"`

> **Answer: B**  
> `allow-forms` re-enables form submission while keeping scripts and popups blocked (the default sandbox behaviour). Adding `allow-scripts` would permit JavaScript execution, which is not desired here.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q73.** A developer adds `sandbox="allow-scripts allow-same-origin"` to an iframe loading content from the same origin as the parent page. A colleague warns this is dangerous. Why?

- A) It is not dangerous — same-origin content should always be trusted.
- B) Combining `allow-scripts` with `allow-same-origin` allows the sandboxed content to access `document.cookie`, `localStorage`, and the parent's DOM via `parent.document`, effectively bypassing the sandbox entirely.
- C) `allow-same-origin` is an invalid value and will be silently ignored.
- D) The combination causes the iframe to inherit the parent's Content Security Policy.

> **Answer: B**  
> `allow-same-origin` grants the iframe the same origin as the parent, giving it access to the parent's storage and DOM. `allow-scripts` lets it run JavaScript. Together, a script inside the iframe can call `parent.document.body.innerHTML = ''` or steal cookies — negating all sandbox protections. This combination should be avoided for same-origin embedded content.

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q74.** A media article embeds dozens of YouTube iframes below the fold. Page load performance is poor because all iframes load immediately. Which HTML5 attribute defers iframe loading until the user scrolls near them, with no JavaScript required?

- A) `<iframe src="..." defer>`
- B) `<iframe src="..." async>`
- C) `<iframe src="..." loading="lazy">`
- D) `<iframe src="..." fetchpriority="low">`

> **Answer: C**  
> The `loading="lazy"` attribute, supported natively on `<iframe>` as well as `<img>`, instructs the browser to defer loading until the element is near the viewport. No JavaScript or Intersection Observer is needed.

**Example:**
```html
<!-- Loads immediately (above-the-fold embed) -->
<iframe src="https://www.youtube.com/embed/abc123"
        title="Intro video"
        loading="eager"
        allowfullscreen></iframe>

<!-- Deferred until near viewport -->
<iframe src="https://www.youtube.com/embed/xyz789"
        title="Related video"
        loading="lazy"
        allowfullscreen></iframe>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

## 15. Progress, Meter, Time & Dialog

**Q75.** A file upload UI must show a progress bar that reflects the percentage of bytes uploaded. While the upload is in progress but the total size is unknown, the bar should display an animated indeterminate state. Which markup produces the indeterminate state?

- A) `<progress value="0" max="100"></progress>`
- B) `<progress></progress>` — omitting the `value` attribute
- C) `<progress value="unknown" max="100"></progress>`
- D) `<progress indeterminate></progress>`

> **Answer: B**  
> A `<progress>` element without a `value` attribute renders in an indeterminate state (typically an animated looping bar). Once the total size is known, setting `value` and `max` switches it to a determinate percentage display.

**Example:**
```html
<!-- Indeterminate — total unknown -->
<progress></progress>

<!-- Determinate — 60 % complete -->
<progress value="60" max="100"></progress>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q76.** A server dashboard shows disk usage. The developer must choose between `<progress>` and `<meter>` for the display. The disk is 60 % full — considered high but not critical; values above 80 % are dangerous. Which element is semantically correct and which attributes communicate the threshold levels?

- A) `<progress>` — it natively supports `low`, `high`, and `optimum` attributes for thresholds.
- B) `<meter value="60" min="0" max="100" low="30" high="80" optimum="10">60%</meter>` — `<meter>` represents a scalar measurement within a known range and supports threshold attributes.
- C) `<progress value="60" max="100" high="80">` — `<progress>` supports threshold styling via the `high` attribute.
- D) Both elements are identical for this use case; choose based on visual preference.

> **Answer: B**  
> `<meter>` is designed for scalar gauge measurements (disk space, temperature, score) within a known range. Its `low`, `high`, and `optimum` attributes let browsers colour-code the bar (green/yellow/red). `<progress>` is designed for task completion and does not support threshold attributes.

**Example:**
```html
<label for="disk">Disk usage:</label>
<meter id="disk" value="60" min="0" max="100"
       low="50" high="80" optimum="20">60 GB of 100 GB used</meter>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q77.** A news article displays its publication date as `"April 13, 2026"`. A developer wants search engines and screen readers to interpret the date programmatically. Which markup is correct?

- A) `<date>April 13, 2026</date>`
- B) `<span class="date">April 13, 2026</span>`
- C) `<time datetime="2026-04-13">April 13, 2026</time>`
- D) `<abbr title="2026-04-13">April 13, 2026</abbr>`

> **Answer: C**  
> The `<time>` element semantically marks up dates and times. The `datetime` attribute provides a machine-readable value in a standard format (ISO 8601 for dates). This enables search engines to display rich snippets and assistive technologies to surface date information accurately.

**Example:**
```html
<article>
  <h2>HTML5 in 2026</h2>
  <p>Published on <time datetime="2026-04-13">April 13, 2026</time></p>
  <p>Event starts at <time datetime="2026-04-13T09:00:00+05:30">9:00 AM IST</time></p>
</article>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q78.** A mortgage calculator form has two number inputs (`principal` and `rate`) and must display the computed monthly payment in a read-only field that is semantically associated with the form. Which HTML5 element is purpose-built for this?

- A) `<input type="text" readonly>`
- B) `<span id="result"></span>`
- C) `<output name="payment" for="principal rate"></output>`
- D) `<data value="0">Payment</data>`

> **Answer: C**  
> `<output>` is an HTML5 element specifically designed to display the result of a calculation or user action. Its `for` attribute takes a space-separated list of input element IDs, establishing a programmatic relationship between inputs and their computed result.

**Example:**
```html
<form oninput="payment.value = (principal.valueAsNumber * rate.valueAsNumber / 1200).toFixed(2)">
  <label>Principal: <input type="number" id="principal" name="principal" value="100000"></label>
  <label>Rate (%): <input type="number" id="rate" name="rate" step="0.01" value="6"></label>
  <label>Monthly payment: <output name="payment" for="principal rate">0.00</output></label>
</form>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q79.** A developer includes the following in the HTML:

```html
<template id="card-tpl">
  <div class="card">
    <h2 class="card-title"></h2>
    <p class="card-body"></p>
  </div>
</template>
```

Which statement correctly describes the `<template>` element?

- A) The `<template>` content is rendered invisibly; CSS can hide it with `display:none`.
- B) The `<template>` content is parsed by the browser but not rendered, not evaluated (scripts/images do not load), and not accessible to `querySelector` until cloned into the document.
- C) `<template>` is identical to a `<div style="display:none">` wrapper.
- D) The `<template>` element requires a `type="text/html"` attribute to activate.

> **Answer: B**  
> Content inside `<template>` is inert: it is parsed into a `DocumentFragment` stored in `template.content`, but it is not rendered, images are not fetched, scripts are not run, and the content is isolated from the main document until explicitly cloned with `document.importNode()` or `template.content.cloneNode(true)`.

**Example:**
```javascript
const tpl   = document.getElementById('card-tpl');
const clone = tpl.content.cloneNode(true);
clone.querySelector('.card-title').textContent = 'HTML5 Templates';
clone.querySelector('.card-body').textContent  = 'Reusable markup patterns.';
document.getElementById('container').appendChild(clone);
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>

**Q80.** A web app needs a modal confirmation dialog. Previously the team used a `<div>` overlay with ARIA roles. HTML5.2 introduced a native element for this. Which element and method correctly open a modal dialog that traps focus and adds an `::backdrop` overlay?

- A) `<dialog open>` with no JavaScript needed.
- B) `<dialog>` element opened with `dialogElement.showModal()` — this renders it as a modal, adds the native `::backdrop`, and traps focus within the dialog.
- C) `<dialog>` element opened with `dialogElement.show()` — this opens it as a true modal.
- D) `<modal>` element with `open` attribute.

> **Answer: B**  
> `HTMLDialogElement.showModal()` opens the dialog as a modal: it sits on the top layer above all other content, a `::backdrop` pseudo-element darkens the page, and the browser constrains Tab/Shift+Tab focus to elements inside the dialog. `show()` opens it as a non-modal (no backdrop, no focus trap). `<modal>` is not a valid HTML element.

**Example:**
```html
<button id="open-btn">Delete Account</button>

<dialog id="confirm-dialog">
  <h2>Confirm Deletion</h2>
  <p>This action cannot be undone.</p>
  <button id="cancel-btn">Cancel</button>
  <button id="confirm-btn">Delete</button>
</dialog>

<script>
  const dialog    = document.getElementById('confirm-dialog');
  const openBtn   = document.getElementById('open-btn');
  const cancelBtn = document.getElementById('cancel-btn');

  openBtn.addEventListener('click',   () => dialog.showModal());
  cancelBtn.addEventListener('click', () => dialog.close());
</script>
```

<div align="right">
    <b><a href="#table-of-contents">↥ back to top</a></b>
</div>
