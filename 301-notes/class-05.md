## Class 05 Notes

### React

1. **What is the single responsibility principle and how does it apply to components?**

    - Single Responsibility principle is a concept in that any component should have only one reason to change, this makes it so it only has one job to accomplish.
    - This makes it easier to understand as looking through a component that is in charge of performing many different tasks it could potentially make it difficult to maintain and understand.

2. **What does it mean to build a ‘static’ version of your application?**

    - a 'static' version is essentially the structure of your application.  This version has no functionality and is only made to render the UI.

3. **Once you have a static application, what do you need to add?**

    - Once the static is made you can start implementing functionality, maybe instead of using placeholder images you can add appropriate images that give the user information if they click or hover over it.  Maybe add a button to move the user from one place to another.

4. **What are the three questions you can ask to determine if something is state?**

    1. **Passed via Props** - If passed via props, it most likely isn't a state
    2. **Unchanged over time** - If it doesn't change as time goes on, it's most likely not a state
    3. **Compute it based on existing states** - Not likely a state

5. **How can you identify where state needs to live?**

    - Identification of Components that render based on the state,
    - Finding the Common Owner Component
    - If no Common Owner Exists you make one

### Higher-Order Functions

1. **What is a “higher-order function”?**

    - Higher-order functions are functions that operate on other functions.  They take function as arguments and can return a function.

2. **Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**

    - It looks like `return m => m < n` is returning a function with a parameter of `m` and I think the body is `m < n`.

3. **Explain how either map or reduce operates, with regards to higher-order functions.**

    - `map` goes into each element in an array and returns a new array with the results of each element that the function has gone through.
    - `reduce` accumulates all the values in an array into one by assigning an accumulator to add the value in each element.