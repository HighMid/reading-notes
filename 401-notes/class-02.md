## Class 02 Notes

### Python

1. **What are the key principles of Test-Driven Development (TDD) in Python, and how do they contribute to the overall quality of code?**

    1. **Write Tests First :** You write tests first and have test cases for your functions before the actual function code. This helps defining a functions purpose and expected behavior.

    2. **Red, Green, Refactor :** Writing out a test first that fails, writing the minimal amount of code for the test to pass and then refactoring the code to make the process more efficient.

    3. **Small Changes :** Make small changes to make it easier to manage and debug as this allows for a stable code base.

    4. **Test Reliability and Documentation :** Most of the code will have been covered via tests which helps with reliability and these also server as documentation to help others understand the code and show how it's suppose to work.

2. **Explain the purpose of the if __name__ == '__main__': statement in Python scripts. What are some use cases for including this conditional in your code?**

    - The purpose of the `if __name__ == '__main__'` statement is for Python to check to see if the script is being imported as a module from another script or ran as the main program.
        - Use cases are to test code, determine the starting point of a program and to keep code to be executed separate from code that will be imported.

3. **Describe the concept of recursion in Python.**

    - The concept of recursion in Python is where a function calls itself to solve a problem. A typical use case is finding out a number in the Fibonacci sequence or calculating the factorial of a number.

    ```
    def myFactorial(n)
        if n == 1
            return 1
        else n * myFactorial(n-1)
    ```
    >In this example the user will put in a number greater than 1 to find the factorial of that number. The n == 1 is the base case so the recursion will eventually end once that number is reached and will then work it's way via LIFO(Last In First Out).

4. **What is the difference between Python modules and packages? Explain how to create, import, and use them in your Python programs.**

    - **Modules :** are files containing Python code, these are typically code that can be used via `import`. This allows you to access functions and classes defined in them and it helps keep the code cleaner and more organized as a result.

    - **Packages :** are ways of organizing Python modules, similar to how it's handled in many other OOP languages.  Packages contain a directory that houses other modules that contains all the relevant modules.
