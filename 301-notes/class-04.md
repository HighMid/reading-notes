## Class 04 Notes

### React

1. **What is a ‘Controlled Component’?**

    - Controlled components are components that handle form elements using states.  These forms are handled by the component's state rather than the DOM.

2. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

    >I think it's better to update the state real-time over completion because giving user feedback and validation immediately is way better than feedback after completion.  This makes it easier to understand and to better guide the user to the expected outcome. When using React is discouraged to manipulate the DOM over in favor of states and props as the DOM is considered temporary in memory and not encouraged to hold data.

3. **How do we target what the user is entering if we have an event handler on an input field?**

    - You can target it by using the event object and passing it to the event handler.

    ```
        class MyForm extends React.Component {
    state = { value: '' };

    handleChange = (event) => {
        this.setState({ value: event.target.value });
    };

    render() {
        return (
        <input type="text" value={this.state.value} onChange={this.handleChange} />
        );
    }
    }
    ```
    >- Source: ChatGPT
### Ternary Operator

1. **Why would we use a ternary operator?**

    - Ternary operators are useful if you want to make code more concise and readable, these are often used when making simple conditions.



2. **Rewrite the following statement using a ternary statement:**

```if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```
Converted will look like this,

    ```
    console.log(x === y ? true : false);
    ```