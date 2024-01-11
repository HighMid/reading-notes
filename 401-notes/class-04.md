## Class 04 Notes

1. **What are the key differences between classes and objects in Python, and how are they used to create and manage instances of a class?**

[Classes and Objects](https://www.learnpython.org/en/Classes_and_Objects)

    - Classes in Python are the design in which Object are based off of when created.  Classes hold the data member and methods while Objects are used to access the data and methods of the class it's instantiatied from.

2. **Explain the concept of recursion and provide an example of how it can be used to solve a problem in Python. What are some best practices to follow when implementing a recursive function?**

    - Recursion is when a function calls upon itself to solve a problem. This involves taking a problem and breaking it down into smaller parts where the same subproblems are needed to be solved multiple times.

    ```
    def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

    my_num = factorial(5)
    print(my_num) # Expected result is 120
    ```

    - Good practices are to ensure that there is a base case to prevent infinite recursions and to make sure that each repeated process reduces the problem size.

    [Recursion](https://realpython.com/python-thinking-recursively/)

3. **What is the purpose of pytest fixtures and code coverage in testing Python code? Explain how they can be used together to improve the quality and maintainability of a project.**


    - **Pytest Fixtures:**

        - **Purpose:** Fixtures in pytest are used for setting up preconditions like database connections, URLs, or input data before running tests. They help in writing more manageable and scalable test cases.
        - **Usage:** Defined using the @pytest.fixture decorator and can be injected into test functions as arguments.

    - **Code Coverage:**

        - **Purpose:** Code coverage measures how many lines of your code are executed while the automated tests run. It's a way to check the effectiveness of your tests.
        - **Tool:** Tools like coverage.py can be used to measure code coverage.

    - **Using Together:**

        - **Integration:** By combining pytest fixtures with code coverage tools, you can ensure that your tests not only run correctly but also that they effectively cover a significant portion of your code.
        - **Improves Quality:** This combination helps in identifying parts of the code that are not tested, leading to more comprehensive tests and higher code quality.

        [Pytest, fixtures and coverage](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)

    **Source: ChatGPT**