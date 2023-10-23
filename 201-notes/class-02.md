## Class 02 Notes

>This Module covers the basics of HTML, CSS & JS.  The reason why these languages are used, how they can be incorporated together and how they are used.

### Why use Semantic Elements in HTML

>Semantics are important in HTML as it makes the code more accessible and easier to read.  

- Accessible in ways that help your webpage come up on search engines, help users that user screen readers better understand the content and encourages cross-platform compatability.

- Makes it easier to read so other developers can easily understand the code which can happen during collaborations, maintenance or just the overall user experience.

### Heading Levels

>There are six heading levels starting from h1(largest) to h6(smallest), used to provide emphasis such as titles.

<h1>H1</h1>
<h2>H2</h2>
<h3>H3</h3>
<h4>H4</h4>
<h5>H5</h5>
<h6>H6</h6>

### Usage of `<sup>` & `<sub>`

>These display superscript and subscript text, these are normally used to format equations that use Exponents and Chemical formulas respectively.

- Examples

    1. E=mc<sup>2</sup>
        >Use of sup to add the 2 exponent on 'c'.

    2. H<sub>2</sub>O
        >Use of sub to add the 2 to Hydrogen.

### Usage of `<abbr>`

><'abbr'> or abbreviation should be used in tandom with title, this allows the users to understand with the acronym in use is.

`<abbr title="Pure Freaking Magic">PFM</abbr>`

## Applying CSS to HTML

>CSS is used to present the webpage to the user in a easily digestable way.  This gives the HTML structure it's colors so to speak by allowing the user to accurately target the audience the webpage is used for.

### Applying CSS

>You can apply CSS to HTML by either using Inline CSS, Internal CSS and External CSS

1. Inline CSS is applying styles to individual HTML elements using the `style` attribute. Useful for elements that require a specific style, however this practice is **not recommended** as changing one line might require many lines that could potentially make it more difficult to understand.

`<p style="color: blue; background-color: beige">Im blue but my background is beige!</p>`


2. Internal CSS is used when styling a single HTML page.  This is implemented in the `<style>` element in the `<head>` section on the document.

`<head>
    <style>
        .header{
            background-color: bisque;
            color: brown;
        }
    </style> </head>`

3. External CSS is used to style multiple pages by making a seperate CSS file and linking it to your HTML file.
`<link rel="stylesheet" type="text/css" href="styles.css">`

### Understanding this block of code

   ``h2 {
     color: black;
     padding: 5px;
   }``

1. The Selector is the `h2`, this CSS rule applies to all `h2` elements in the document.
2. `color: black;` and `padding: 5px;` are declarations that house a property and a value
3. The `color` and `padding` are both properties

## JavaScript Basics

>Javascript gives interactivity to the website, it gives the user the ability to interact with the website ranging from data entry, animations, dynamic styling and more.

### Data Types

1. **String** - Encased in '' or ""
2. **boolean** - true/false
3. **Numbers** - integers/doubles

### Operators

1. Arithmetic Operators - `+ , - , * , /`
1. Comparison Operators - `== , != , > , <`
1. Logical Operators - `&& , || , !`
1. Assignment Operators - `+= , -= , *= , /= , %=`

### Example use case for Function

>Functions can be used for many things and they can easily cut down the time needed for the programmer to not only finish their code but make it easier to read.

1. Could use a function as a calculator in case for some reason your computer calculator goes on strike or your phone explodes in your face and an angry waitor wants his 15% tip.

### Conditionals

1. An if statement checks a condition, and if it evaluates to true, then the code block associated with it will execute.
2. else if, can be used to evaluate the following condition if the condition above wasn't met
3. Comparison Operators:
    1. Equality (==)
    2. Strict Equality (===)
    3. Inequality (!=)
    4. Strict Inequality (!==)

4. Difference between && and `||` is && requires both conditions to evaluate to true to equal true while `||` requires only one condition to equal true.