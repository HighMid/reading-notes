## Class 02 Notes

### React LifeCycle

[React Life Cycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

1. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

    - ***RENDER***

2. **What is the very first thing to happen in the lifecycle of React?**

    - The mounting phase is the first one starting with the Constructor.

3. **Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`**

    1. **Constructor**
    2. **render**
    3. **React Updates**
    4. **componentDidMount**
    5. **componentWillUnmount**

4. **What does `componentDidMount` do?**

    - It is executed after the component is mounted and rendered to the DOM for the first time. This lifecycle method is typically used for performing operations that require the DOM nodes to be present or setting up subscriptions.

### React State or Props

1. **What types of things can you pass in the props?**

    - You can pass different data types, objects, arrays, Components or Functions.

2. **What is the big difference between props and state?**

    - Props are passed from a parent component that doesn't need to updated inside the component it's passing to.  Examples are titles or images that are considered static and will not change.
    
    - States are managed within a component that can be change.  This is useful for data that changes overtime and will affect how components will render.

3. **When do we re-render our application?**

    - Applications get re-rendered when the component changes due to states or if it receives different props from it's parent. Can also be re-rendered by using `forceUpdate`.

4. **What are some examples of things that we could store in state?**

    - User Input
    - Counters or Timers
    - Styling Information
    - UI States