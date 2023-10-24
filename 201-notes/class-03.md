## Class 03 Notes

### HTML, Ordered and Unordered lists

1. **When should you use an unordered list in your HTML document?**

    >You should use an unordered list when the order of the items doesn't matter. Common use cases include listing features of a product, displaying a list of related links, or presenting a set of topics or categories.

2. **How do you change the bullet style of unordered list items?**

    >You can change the bullet style of unordered list items using CSS. The list-style-type property is used to define the type of bullet point.<div>
    Some values include: <div>
    >- `disc`
    >- `circle`
    >- `square`

3. **When should you use an ordered list vs an unordered list in your HTML document?**

    >You should use an ordered list when the sequence or order of the items matters. For instance, step-by-step instructions, rankings, guide style content or any other list where the order provides meaningful information.

4. **Describe two ways you can change the numbers on list items provided by an ordered list?**

    >Using HTML you can use the `<ol>` tag to specify the starting number. You can also use the value attribute on the `<li>` to specify the number for that particular list item. <div>
    >Using CSS, the list-style-type property can be used on ordered lists `<ol>` to change the type of numbering or counters.

### CSS, Box Model

1. **Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?**
    >Margin was like the diplomat of the Box Kingdom. Always conscious of the space between different territories, Margin ensured that there was a respectful distance between one kingdom (element) and its neighboring kingdoms (adjacent elements). This distance ensured that the territories didn't clash or encroach upon one another. Margin was all about the outward space, making sure everyone had room to breathe. <div>
    >Padding, on the other hand, was the trusted advisor to the rulers within each Box Kingdom. While Margin looked outward, Padding was more concerned about the space inside the kingdom's walls. He ensured there was ample space between the kingdom's walls and its content, providing a buffer zone to make the kingdom's interior look more aesthetically pleasing and structured. Padding was all about the inward space, ensuring comfort and structure inside the kingdom. <div>
    **Source: ChadGPT**
2. **List and describe the four parts of an HTML elements box as referred to by the box model.**
    > 1. **Content** - This holds the actual substance of the box(text,images,etc)
    > 2. **Padding** - This separated the content from the border, this make's it look more presentable to the eyes. It's like the ice cream in fried ice cream.
    > 3. **Border** - This is the border of the box, it keeps everything inside. It's like fried dough in fried ice cream.
    > 4. **Margin** - This is the outermost layer that represents the space between this box and everything else.  It's like the container in which you put the fried ice cream in.

### JavaScript, Arrays, Operators, and all the fun stuff

1. **What data types can you store inside of an Array?**
    >Apparently you can put any data type in an Array, what I mean is that you can mix and match different types that normally dont mesh well in other languages. These data types include: <div>
    >- Numbers (e.g., 5, 3.14)
    >- Strings (e.g., 'hello', "world")
    >- Booleans (e.g., true, false)
    >- Objects (including other arrays)
    >- null and undefined
    >- Functions

2. **Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?**


    >It is valid because you can have an array inside another array. You can access what piece of data you want by manipulating the Element associated with it. <div>
    To get to "pete" you need to do `people[0][0]`, the first `[0]` is the first element and the second `[0]` is the first value within that element. ***(I hate arrays :D )***

```
const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

3. **List five shorthand operators for assignment in javascript and describe what they do.**
    >- **+=** : Addition assignment. Adds the right operand to the left operand and assigns the result to the left operand.
    >- **=** : Subtraction assignment. Subtracts the right operand from the left operand and assigns the result to the left operand.
    >- ***=** : Multiplication assignment. Multiplies the left operand by the right operand and assigns the result to the left operand.
    >- **/=** : Division assignment. Divides the left operand by the right operand and assigns the result to the left operand.
    >- **%=** : Modulus (remainder) assignment. Divides the left operand by the right operand, returns the remainder, and assigns it to the left operand.

.

4. **Read the code below and evaluate the last expression and explain what the result would be and why.**

    >It'll result with '10dog', because this programming language does not care about data types not being able to mesh together etc, etc. It's like your supervisor that doesn't know anything about what you do but forces you to work with another department that has nothing to do with your work.  To break it down, `(a + c) + b`, we do `(a + c)` first which equates to 10 because false is considered 0 and `b` is a String but who cares let's just force the integer to be a String too, they won't care.

```
let a = 10;
let b = 'dog';
let c = false;

// evaluate this
(a + c) + b;
```

5. **Describe a real world example of when a conditional statement should be used in a JavaScript program.**
    >Let's say you are building an online shopping platform. When the user clicks the "Checkout" button, you'd use a conditional statement to check if their shopping cart is empty. If it is empty, you might display a message like "Your cart is empty!", otherwise you proceed to the checkout process. <div>
    **Source: ChadGPT**

6.  **Give an example of when a Loop is useful in JavaScript.**
    > Loops are amazing in any language, you can use them for input validations, repetitive instructions or just being an ass.  I like using `while (true)`, loops for smaller programs because it doesn't require you to change the condition if you're only planning on maybe running less than 100 lines.  You can just `break;` once you're done to break out of the loop. Or use a `For` loop if you know how many iterations you need it to go through.