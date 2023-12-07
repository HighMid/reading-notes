## Class 09 Notes

### Functional Programming

1. **What is functional programming?**

    - Functional programming is a programming standard that emphasizes the use of functions only to be used in mathematical fashions and to avoid changing data outside of the given inputs.

2. **What is a pure function and how do we know if something is a pure function?**

    - Pure functions a concept of functions that return the same output given the same input, which means that the output in the function is based solely on the input values. Ways to identify a pure function is if it doesn't have any external data like classes or global variables, no changes in the input arguments and the result returns the same input values.

3. **What are the benefits of a pure function?**

    - **Predictability**: Since there are no external factors in pure functions this makes it easier to predict behavior from them
    - **Testability**: Since they are very declarative this makes them easier as the logic involved is most likely straightforward
    - **Reusability**: Functions that do not rely on global or state values are easier to implement in other parts of a program

4. **What is immutability?**

    - Immutability is a concept in functional programming that states if you need to modify an existing structure you should instead make a new object with the modifications.

5. **What is Referential transparency?**

    - Referential transparency is a property of expressions in a program where they can be replaced without changing the programs behavior. 

### Node.js

1. **What is a module?**

    - Modules are seperate units of software that contains functions, variables or classes that can be reused in different parts of applications/code. These focus on encapsulation that allows modular design and seperation.

2. **What does the word ‘require’ do?**

    - `require` is used to include modules into a file, this acts as a gateway to allow the libaries or frameworks to be used in your current file.

3. **How do we bring another module into the file the we are working in?**

    - To bring a module into the file you have to declare a variable with the module's name inside `require`,
    ```
    const express = require('express');
    ```
4. **What do we have to do to make a module available?**

    - To make a module available to be used in other files, you need to export the functionalities (functions, objects, classes, etc.) from the module. In Node.js, this is typically done using module.exports or exports.
    
    ```
    // myModule.js
    const myFunction = () => {
    console.log('Hello from my module');
    };

    module.exports = myFunction;

    Source: ChatGPT
    ```