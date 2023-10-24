## Class 01 Notes

### [Poem about HTTP sending data](class-01poem.md)

### Parsing HTML, CSS and JS Files

1. **HTML Parsing:** When a web page is loaded, the browser starts parsing the HTML file from top to bottom. HTML parsing involves identifying elements, their attributes, and their relationships.

2. **CSS Parsing:** After parsing HTML, the browser looks for linked or embedded CSS files. It parses the CSS to create the CSS Object Model (CSSOM), which defines styles and how they apply to HTML elements.

3. **JS Parsing:** JavaScript files can be external or inline. The browser identifies and parses external JavaScript files first. Inline JavaScript is parsed and executed as it's encountered in the HTML file.

### Finding Images Online

There are plenty of places to find images, most commonly is using a search engine.  [Stock Photos like this](https://pixabay.com), can also be found here, it's important to find royalty free images or check permissions/fair use before using images.

### JavaScript Variables

In JavaScript you can create a String or Number using the `let` keyword when you declare a variable.  You can make a number by using numbers without any "" or ''.

`let example = "I'm a String"`

`let number = 1337`

### HTML Section

>An HTML attribute is addtional information within the HTML tag that modifies the properties of an HTML element.  It gives instruction on how it should be displayed or how it behaves.

>Each HTML element has 4 parts, an Opening Tag, Closing Tag, and the Content in the element.

>Difference between `<section>` and `<article>` is that `<section>` is redistributable and repurposed content that can be used for different things. `<article>` is where the content is grouped together within a document.

>Elements in a Typical Website:
A typical website includes a variety of HTML elements to structure its content and functionality. Common elements include:

1. **Headings** `<h1>, <h2>`
1. **Paragraphs** `<p>`
1. **Links** `<a>`
1. **Images** `<img>`
1. **Lists** `(<ul>, <ol>, <li>)`
1. **Headers** `<header>`
1. **Navigation menus** `<nav>`
1. **Footers** `<footer>`
1. **Articles** `<article>`
1. **Sections** `<section>`
1. **Metadata** `(<meta> for SEO)`

>Using the `<meta>` HTML Tag for Metadata:<div>
The `<meta>` tag is used to specify various metadata attributes within the `<head>` section of an HTML document.

### First Steps to making a website

>The first step to making a website is decide what you want the website to accomplish, whether you want it to be an info hub, forums, a crappy crypto coin or even something simple like a list.  Then you start planning on how it's going to present itself, what other capabilities you want it to do etc. , the most important question at least to me is how accessible it is?  When I mean by accessible I mean how can I use this website to present the goal I want it to be.

#### Semantics

>Why use `<h1>` element over a `<span>` element? Do you want balloon arms imitating muscle or actual muscle? `<h1>` is meant to be used as the highest level of headings as it's the biggest wording on the document and has the semantic element that also give's it more meaning when used. `<span>` does make the text bigger but nothing else, doesn't add any meaning to the content they're used on.

### What is <small> Javascipt . . . </small>

>Two common thing's that use JavaScript is Form Validation and Interactive UI.  Form validation is the process in which JavaScript takes information and validates it before submitting information and Interactive UI could mean mean a lot of things such as responsive menus, interactive maps, suika game, etc.<div> 
You can add JavaScript to an HTML Document by either doing it Inline which is making a `<script>` element in either the `<head>` or near the closing `<body>` tags and using JavaScript code.<div>  
You can also do External JavaScript File which uses JavaScript code in a separate external file with a .js extension. Then, include a reference to the external file in your HTML document using the `<script>` element's src attribute.