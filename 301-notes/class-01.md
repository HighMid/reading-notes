## Class 01 Notes

### Introduction to React and Components

1. **What is a "Component"?**

    - Components are units that manages a portion of the UI, these are self-contained similiar to functions in JavaScript and can range from something as small as a button to a whole app.

2. **What are the characteristics of a component?**

    - **Reusability:** Components are designed to be reused across different parts or different applications.

    - **Encapsulation:** Similiar to functions they are self-contained which makes their behavior more predictable as they manage their own state and logic.

    - **Props:** This allows data to be received from the parent components.

    - **State Management:** They have local states that can be managed to respond to changes and update accordingly

3. **What are the advantages of using component-based architecture?**

    - **Reusability:** These can be reused to help code readability and reduce the amount of maintenance needed.  This in term makes components easily scalable and make everything feel consistent across your code.

    - **Development Effiency:** Due to components being reusable this improves the speed of the development cycle as there is continuity and because components are smaller and isolated this makes it easier to test compared to larger codebases.

4. **What is "props" short for?**

    - "props" are short for "properties"

5. **How are props used in React?**

    - **Passing Data to Components:** Props are used to pass data from parent components to child components.

    - **Customizing Components:** Props allow components to be customized, this means that if there is a button component it can have a different look compared to other button components.

6. **What is the flow of props?**

    - The flow of props is top-down, this unidirectional approach means that data can be passed down to the child components from the parent while child components are unable to pass up to the parent component.  This helps with consistency and predictable behavior.