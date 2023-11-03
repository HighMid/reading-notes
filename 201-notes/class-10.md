## Class 10 Notes

### JavaScript

1. **Name some key differences between a Syntax Error and a Logic Error.**

    - **Syntax Errors** are mistakes that are made in the code that prevents the code from running, these range from mispelling keywords, missing that one semicolon somewhere in lines 1 - 1000, etc.  These are easier to find as the program will often point out what is considered invalid code or stop running once it reaches that point *(interpreted languages)*
    - **Logic Errors** are errors that give you an unintended result.  The program runs but the desired output is not what was expected.  These tend to be more difficult as it varies from code to code as more complex codes requires more attention and could be difficult to pinpoint the point in which the logic is flawed.

2. **List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.**

    This is actually a neat idea, I should compile all the times I thought something made sense and put it into a folder to see all the sheningans of coding.
    
    - Passing `undefined` or `null` values is a classic, I have to confess I have been really lazy when it comes to them but normally I would set up a statement to catch those values and if I need to input a value in that spot when I recieved one of the two above, I just assign the value myself.

    - Another one is the referencing a variable that hasn't been declared or defined, most cases it's just thinking to far ahead and jumped over one too many steps.  Maintaining a checklist is really nice in those cases as it helps me keep track on what needs to be done and not get too gung-ho on an idea I came up with while working.

3. **How will this topic continue to influence your long term goals?**

    > These will always be things to consider because it's just part of the whole journey.  Syntax Errors or Logic Errors are just another way of saying mistakes, they'll always be around no matter how good you get.  Important thing is to learn/acknowledge them and grow so yeah I would say it'll always influence anything I do in the future.


### JavaScript Debugger

1. **How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?**

    - It's a tool that allows you to navigate through your code and inspect it as if you're watching a movie.  It gives you the ability to hop in and out of your code while running it, it can give you details on what's happening during certain parts of the code such as what variables are set to, what events are currently active, or why your for loop decided to just ignore all your statements.  

2. **Breakpoints**

    - Something I wish I utilize more but these allow you to set points in time in the code that you can pause and examine what execution is happening in the code at that point.  It allows you to see how the program was flowing until that point and what variables values are set.  This essentially allows you to test run your code and isolate any potential problems that happen during runtime.

3. **Call Stack**

    - The call stack is a mechanism that keeps track of the execution context. In simpler terms, it's like a to-do list for the JavaScript engine, showing it which functions are to be executed and in what order. When a function is called, a new frame (a record of the function call) is pushed onto the stack. When a function returns, its frame is popped off the stack. The call stack also holds the local variables and context for each function call, allowing you to trace the sequence of function calls that led to a particular point in your program. This is especially useful for debugging, as it shows you the path that the execution took to reach a certain line of code.
    
        **Source: ChatGPT**