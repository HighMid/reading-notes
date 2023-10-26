## Class 04 Notes

### HTML

1. **To create a basic link, we wrap text or other content inside what element?**
    >To create a basic link in HTML, we use the link or content within an `<a>` (anchor) element. <div><a href=<https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks>Looks> a little like this.</a>

2. **The href attribute contains what information?**
    >`href`(Hypertext Reference) is an attribute used in `<a>` that specifies the URL the link goes to. This can link to webpages, images or files.

3. **What are some ways we can ensure links on our pages are accessible to all readers?**
    1. You can use link text to describe what the link is suppose to look like if you're using an image or provide a description of the link. <div>
    2. Can also use the `alt` attribute to provide a description for an image.<div>`<img src="tabbycat.jpg" alt="This is a tabby cat picture">`

### CSS

1. **What is “normal flow”?**

    >**Normal Flow**, is how browsers arrange the elements on the page by default when there isn't any CSS involved.  If you were to make a website using only HTML, there is a certain amount of CSS applied by default such as spacing, fonts etc.

2. **What are a few differences between block-level and inline elements?**

    - **Block-level** occupies the full width of their parent container, they start on a new line and end on a new line.
    - **Inline elements** occupy as much width as necessary, they flow within content and do not start on a new line.

3. **___ positioning is the default for every html element.**

    >`Static` is the default positioning for HTML elements

4. **Name a few advantages to using absolute positioning on an element.**

    >Allows you to percisely posistion elements, by percise I mean pixel-perfect. These elements can be layered using **z-index**, this is used to determine what elements get displayed if they overlap.  Think of the sky and clouds as elements, you can **z-index** to have the clouds overlap the sky so you see the clouds before the sky.

5. **What is a key difference between fixed positioning and absolute positioning?**

    - **Fixed Positioning** does not move if the page is scrolled, they are fixed relative to the browser.<div>

    - **Absolute Positioning** does move if the page or container is scrolled, it's position is relative to the nearest positioned ancestor.<div>
    **Source: ChatGPT**

### JavaScript

1. **Difference between a function declaration and a function invocation:**

    - **Function Declaration** is the process of defining the function, this is when you assign it a name, parameters if needed and the body of the function which is the code and the purpose of it.<div>

    ```
    function prototype(name) 
    {
    console.log("Hello, " + name + "!");
    }
    ```

    - **Function Invocation** is the process of calling the function for use.<div>

    ```
    prototype("Nugget");
    ```

2. **Difference between a parameter and an argument:**

    >- **Parameters** are variables used when a function is declared.  It's a placeholder for values that get passed to the function when the function is called. In the above example `function prototype(name)` "name" is the parameter.
    >- **Argument** this is the value that gets passed to the function when called. In the above example `prototype("Nugget");` "Nugget" is the argument.

### Pair Programming

>- Having someone else check your code and pool knowledge is always very helpful. There were times when I missed something so obvious but spent an extended period of time trying to figure it out.  Only to have one of my friends QC my code to find it in an instant.  Now I have ChatGPT but having another person look over your work is still very beneficial as much as I like ChatGPT to check my work, being able to bounce idea's with someone else and hear their experiences on how they used this block of code in a different environment only to have it fail is just priceless knowledge.
>- Also, **JOLLY COOPERATION IS ALWAYS NICE**
![Dark Souls Solaire sunBro](https://pm1.aminoapps.com/7787/923b9092a29fb9152ce74445bfa8e4855d81372br1-600-900v2_uhq.jpg)
