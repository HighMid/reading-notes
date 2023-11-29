## Class 03 Notes



1. **What does .map() return?**

    - `.map()` returns a new array by applying changes to each element of the original array

2. **If I want to loop through an array and display each value in JSX, how do I do that in React?**

    - Using `.map` you can make a loop like this,

    ```
    const items = ['Item 1', 'Item 2', 'Item 3'];

    const itemList = items.map((item, index) => (
    <li key={index}>{item}</li>
    ));

    <ul>
    {itemList}
    </ul>
    ```

    ***or***

    ```
        function MyComponent({ items }) {
    return (
        <div>
        {items.map(item => (
            <div key={item.id}>{item.value}</div>
        ))}
        </div>
    );
    }
    ```

    - Both work the same way with the exception of the first block assigning the key with each iteration while the bottom one grabs the id from `item.id` prop that was provided.

3. **Each list item needs a unique ____.**

    - They require a `key` , this gives React a way to identify which UI gets updated.

4. **What is the purpose of a key?**

    - `key` gives React an identifier to update the appropriate elements within an array

### Spread Operator

1. **What is the spread operator?**

    - The spread operator `(...)` allows an iterable to be expanded in places where 0 or more arugments are expected.  

2. **List 4 things that the spread operator can do.**

    1. Combine Arrays
    2. Copy Arrays
    3. Combine Objects
    4. Pass into Functions

3. **Give an example of using the spread operator to combine two arrays.**

    - ```
        const array1 = [1, 2, 3];
        const array2 = [4, 5, 6];
        const combinedArray = [...array1, ...array2];
        ```
        This combines both array1 and array2, the `combinedArray` will look like this...

        ```
        combinedArray = [1, 2, 3, 4, 5, 6]
        ```

4. **Give an example of using the spread operator to add a new item to an array.**

    - ```
        const initialArray = ['a', 'b', 3];
        const newItem = 'd';
        const newArray = [...initialArray, newItem];
        ```
        This adds the item to the array, since JavaScript doesn't discriminate it you are able to add any data type using this.
        ```
        newArray = ['a', 'b', 3, 'd']
        ```

5. **Give an example of using the spread operator to combine two objects into one.**
    - ```
        const object1 = { name: 'Bob', age: 69 };
        const object2 = { occupation: 'Developer', country: 'GER' };
        const combinedObject = { ...object1, ...object2 };
        ```
        The combinedObject will look like this...
        ```
        combinedObject = { name: 'John', age: 30, occupation: 'Developer', country: 'USA' }
        ```

### Passing Functions between Components

1. **In the video, what is the first step that the developer does to pass functions between components?**

    - He uses the return function to pass the functions as a prop

2. **In your own words, what does the handleClick function do?**

    - It's like a switch that activates whatever the user has programmed in the `handleClick` function

3. **How can you pass a method from a parent component into a child component?**

    - You can use the return from the parent component to pass the method as a prop to the child component

4. **How does the child component invoke a method that was passed to it from a parent component?**

    - The child component can invoke the method when needed from the parent if it was passed as a prop.

    ***Parent Component***
    ```
    function ParentComponent() {
    const handleSomething = () => {
        console.log("Method invoked in Parent Component");
    };

    return (
        <ChildComponent onAction={handleSomething} />
    );
    }

    export default ParentComponent;
    ```

    ***Child Component***
    ```
    import React from 'react';

    function ChildComponent(props) {
    return (
        <button onClick={props.onAction}>Click Me</button>
    );
    }

    export default ChildComponent;
    ```