## Class 10 Notes

### JavaScript

1. **What is a ‘call’?**

    - A call in programming is normally referred to as a function call, it's when the program invokes the execution of a function.

2. **How many ‘calls’ can happen at once?**

    - You are able to call as you need per the execution, however you are only able to execute them one at a time in the context of JavaScript.

3. **What does LIFO mean?**

    - Last In First Out, is a principle where the last element added will be the first element removed as well.

4. **Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

    - Here is a function call that invokes other functions,
    ```
    function third() { /*...*/ }
    function second() { third(); }
    function first() { second(); }

    first();
    ```
    - We call the `first()` function that has `second()` nested with that function having `third()` nested, we called them in that order and how it resolves is in reverse so `third()` will resolve and get removed, then `second()`, and lastly `first()` will resolve.

5. **What causes a Stack Overflow?**

    - When there are too many on the call stack which could result in the base stack never being reached.

6. **What is a ‘reference error’?**

    - This occurs when trying to use a variable that is either out of scope or not declared.

7. **What is a ‘syntax error’?**

    - This occurs when you incorrectly use the languages rules, this ranges from many things such as missing keywords, not using keywords, missing arguments or just general unexpected behavior that are not in the rules.

8. **What is a ‘range error’?**

    - This occurs when trying to access a value outside of a set range such as trying to access elements outside of an array that has a set size.

9. **What is a ‘type error’?**

    - This occurs when the resulting type isn't what was expected, in JavaScript this is typically your `null` or `undefined`.

10. **What is a breakpoint?**

    - Breakpoints are used in debugging certain areas of your code by allowing the developer to check the flow from one point to the breakpoint. This allows the developer to pause and check for data that is currently in use at the time of the execution.

11. **What does the word ‘debugger’ do in your code?**

    - Debugger are used in code as a breakpoint, when JavaScript reaches the breakpoint it'll pause the execution and allow developer tools to be access to allow debugging.