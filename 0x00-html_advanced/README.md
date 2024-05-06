# 0x00. Advanced HTML
<kbd>HTML</kbd> <kbd>Front-end</kbd>
```
 Weight: 1
 Project will start May 2, 2024 7:00 AM, must end by May 8, 2024 7:00 AM
 Checker was released at May 3, 2024 7:00 PM
 An auto review will be launched at the deadline
```
<h4>Concepts</h4>

For this project, we expect you to look at this concept:

- <a href="https://intranet.alxswe.com/concepts/543">HTML - elements of a web page</a>


<h2>Welcome!</h2>

Welcome to the Web Stack specialization. The 3 first projects will give you all basics of the Web development: HTML, CSS and Developer tools.

In this project, you will learn how to use HTML tags to structure a web page. No CSS, no styling - don’t worry, the final page will be “ugly” it’s normal, it’s not the purpose of this project.

Important note: **details are important!** lowercase vs uppercase / wrong letter… be careful!

<h2>Resources</h2>

<h5>Read or watch:</h5>

- <a href="https://html.spec.whatwg.org/multipage/">HTML 5.2</a>
- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"> HTML: HyperText Markup Language | MDN</a>
- <a href="https://htmlreference.io/">HTML Reference - A free guide to all HTML elements and attributes</a>
- <a href="https://caniuse.com/">Can I use… Support tables for HTML5, CSS3, etc</a>
- <a href="https://websitesetup.org/html5-cheat-sheet/"> HTML Cheat Sheet - WebsiteSetup</a>

<h2>Learning Objectives</h2>

At the end of this project, you are expected to be able to <a href="https://fs.blog/feynman-learning-technique/">explain to anyone</a>, **without the help of Google:**

* Which guidelines to follow for HTML
* How to create the skeleton of an HTML5 page
* How to use semantic HTML tags to structure a web page
* Which use cases to use `div` vs `span`
* The semantic value’s of `header`, `main`, `footer`, `article`, `nav`, `section`, `aside`
* How to use headings (and why it’s important to follow the hierarchical order)
* How to make lists in HTML
* The differences between medias (SVG, GIF, PNG, JPG)
* How to structure data in a table
* How to integrate a video in a webpage
* How to integrate an audio file in a webpage
* How to embed external content
* How to correctly structure an HTML page

<h2>Requirements</h2>

* A `README.md` file at the root of the folder of the project is mandatory
* Your code should be W3C compliant and validate with <a href="https://github.com/alx-tools/W3C-Validator">W3C-Validator</a>
* `Techium` will be the name of the company we will use across our webpages.

<h2>HTML - elements of a web page</h2>

Create the foundation of any HTML page.

HTML is about content. CSS is about the look and feel.

<h3>Doctype</h3>

The `<doctype>` is necessary at the top of every HTML page to force the browser to render the page according to relevant specifications.
```
<!-- Doctype HTML5 -->
<!DOCTYPE html>
<!-- Lowercase is also valid -->
<!doctype html>
```
<h4>Resources</h4>

- <a href="https://developer.mozilla.org/en-US/docs/Glossary/Doctype">Doctype - MDN Web Docs Glossary: Definitions of Web-related terms | MDN</a>
- <a href="https://htmlhead.dev/">HEAD - A free guide to head elements</a>

`HTML` **tag**

The `<html>` HTML tag tells the browser that the document is an HTML webpage. It is used as a container for all the HTML elements.

Warning!

The doctype is the only element living outside the html tag.
```
<html lang="fr" dir="ltr">
```
<h4>Language and reading direction</h4>

- <a href="https://hacks.mozilla.org/2015/09/building-rtl-aware-web-apps-and-websites-part-1/?ref=frontendchecklist">Building RTL-Aware Web Apps & Websites: Part 1 - Mozilla Hacks - the Web developer blog</a>

`head` **tag**

The `head` tag element contains all the metadatas related to your page. All the elements put in the head are not visible in the window of the browser.

A lot of metadatas exist, some specific to some CMS.

<h5>Usage</h5>

You can find inside the `head`:

* title of the webpage
* asynchronous script calls
* metadata
* CSS code embed (critical CSS)
* JavaScript code embed

<h4>Resources</h4>

- <a href="https://htmlhead.dev/">HEAD - A free guide to head elements</a>

<h3>Meta charset</h3>

The `meta` charset declares the page’s character encoding.
```
...
<head>
    <!-- Set character encoding for the document -->
    <meta charset="value">
</head>
...
```
<h4>Resources</h4>

- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/meta#attr-charset">meta: The Document-level Metadata element - HTML: Hypertext Markup Language | MDN</a>
- <a href="https://www.w3.org/International/questions/qa-html-encoding-declarations">Declaring character encodings in HTML</a>
- <a href="https://bitsofco.de/meta-charset/">Meta Charset</a>

<h3>Viewport</h3>

The meta `viewport` gives information about the initial size of the viewport.

Tip: The viewport is used by mobile devices only.

Accessibility tip: Never use `maximum-scale=1.0`. <a href="https://www.a11yproject.com/posts/never-use-maximum-scale/">It prevents the user from zooming in on the website</a>. It causes an accessibility issue.
```
...
<head>
    ...
    <!-- Viewport for responsive web design -->
    <meta name="viewport" content="key=value, key=value">
</head>
...
```
<h4>Resources</h4>

- <a href="https://bitsofco.de/responsive-design-viewport/">Responsive Design With Viewport Control</a>

<h3>Title</h3>

The `title` meta tag defines the title of the web page.

Tip: The title is only visible on the tab/window of your browser.

Warning! The title should always have less than 56 characters.
```
...
  <head>
    ...
    <!-- Document Title -->
    <title>Page title</title>
  </head>
...
```
<h4>Resources</h4>

- <a href="https://yoast.com/page-titles-seo/">The ideal width of the SEO title • Yoast</a>

<h3>Meta description</h3>
```
<head>
    ...
    <!-- Meta Description -->
    <meta name="description" content="Description of the page less than 150 characters">
  </head>
```
<h4>Resources</h4>

- <a href="https://yoast.com/meta-descriptions/">The ideal length of a meta description • Yoast</a>

<h3>Favicons</h3>
```
<head>
    ...
    <!-- Standard favicon -->
    <link rel="icon" type="image/x-icon" href="https://example.com/favicon.ico">
    <!-- Recommended favicon format -->
    <link rel="icon" type="image/png" href="https://example.com/favicon.png">
    ...
  </head>
```
<h4>Resources</h4>

- <a href="https://www.favicon-generator.org/">Favicon & App Icon Generator</a>
- <a href="https://realfavicongenerator.net/">Favicon Generator for all platforms: iOS, Android, PC/Mac…</a>
- <a href="https://github.com/audreyfeldroy/favicon-cheat-sheet">Obsessive cheat sheet to favicon sizes/types.)</a>
- <a href="https://css-tricks.com/favicon-quiz/">Favicons, Touch Icons, Tile Icons, etc. Which Do You Need? | CSS-Tricks</a>
- <a href="https://caniuse.com/link-icon-png">PNG favicons - caniuse</a>

<h3>Tag attributes</h3>

Attributes provide additional information or instruction for an HTML element. It is **always** included inside the opening tag.

<h4>Data-* attribute</h4>

It is possible to declare any attribute using the `data-` prefix
```
<tag data-extra-attr="value">some content</tag>
```
<h4>Resources</h4>

- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes">HTML attribute reference - HTML: Hypertext Markup Language | MDN</a>

`header` **tag**

The `<header>` HTML tag element is used to identify the top of a webpage, article, section, or other segment of a page. The header is normally always the same across all pages of your website.



<h4>Usage</h4>

* logo of the website
* navigation
* search form
```
...
<body>
    <header>This is my header<header/>
</body>
```
Warning! The `main` element should never be a descendant of an `article`, `aside`, `header`, `footer`, or `nav` element.

Don’t confuse `header` with the `head` element of the page.

<h4>Resources</h4>

- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header">header - HTML: Hypertext Markup Language | MDN</a>

`main` **tag**

The `<main>` HTML tag is a structural element located generally between the `<header>` and the `<footer>` and contains the content of your web page.


```
...
<body>
    <header>This is my header</header>
    <main>
        This is where I put my content
    </main>
</body>
```
`footer` **tag**

The `<footer>` HTML tag is a structural element used to identify the footer of a page, article, or section.



<h4>Usage</h4>

* copyright information
* authorship information
* navigation elements
* social icons or links
```
...
<body>
    <header>This is my header<header/>
    <main>
        This is where I put my content
    </main>
    <footer>This is the footer of my page</footer>
</body>
```
<h4>Resources</h4>

- <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/footer">footer - HTML: Hypertext Markup Language | MDN</a>


<h2>Author</h2>
_Ifechukwu C. Anyika_
