## Class 42 Notes

1. **What are dunder methods in Python, and how do they allow for the customization of built-in behavior in classes? Provide an example of a common dunder method and its purpose.**

    - Dunder methods, short for "double underscore" methods, are special methods in Python that begin and end with double underscores (__). They are also known as magic methods. Dunder methods allow for the customization of built-in behavior for classes, enabling classes to integrate more seamlessly with Python's built-in features and syntax. These methods can override the behavior of built-in functions or operations, such as arithmetic operations, attribute access, item access, and more.

2. **Explain the concept of an iterator in Python. How do you create a custom iterator using the iter() and next() methods, and why are they important for enabling iteration in a class?**

    - Iterators in Python

        - An iterator in Python is an object that implements the iterator protocol, which consists of the methods __iter__() and __next__(). The __iter__() method returns the iterator object itself and is called by the iter() built-in function. The __next__() method returns the next item from the collection and is called by the next() built-in function. When there are no more items to return, __next__() should raise a StopIteration exception.

    Creating a Custom Iterator:

    ```python
    class Count:
        def __init__(self, low, high):
            self.current = low
            self.high = high

        def __iter__(self):
            return self

        def __next__(self):
            if self.current > self.high:
                raise StopIteration
            else:
                self.current += 1
                return self.current - 1
    ```

    >Iterators are important for enabling custom classes to support iteration with a for loop or other iteration contexts.

3. **What is a generator in Python, and how does it differ from a regular function? Illustrate your answer with an example of a generator function using the ‘yield’ keyword.**

    - Generators in Python

        - A generator in Python is a type of iterable, like a list or tuple, but it generates items on-the-fly and stores only one item at a time, making it more memory efficient. Generators are created using functions that utilize the yield keyword to yield values one at a time, pausing execution between each one.

    - Example of a Generator Function:

    ```python
    def countdown(n):
        while n > 0:
            yield n
            n -= 1
    ```

    >When called, this function returns a generator object that yields the next number in the countdown each time next() is called on it.

4. **Define decorators in Python and explain their primary use case. How can you create and apply a custom decorator to a function or method? Provide a simple example to demonstrate this concept.**

    - Decorators in Python

        - Decorators in Python are functions that modify the behavior of another function, method, or class. They are a powerful and expressive tool for extending and modifying the behavior of callable objects without permanently modifying them.

    - Creating and Applying a Custom Decorator:

    ```python
    def my_decorator(func):
        def wrapper():
            print("Something is happening before the function is called.")
            func()
            print("Something is happening after the function is called.")
        return wrapper

    @my_decorator
    def say_hello():
        print("Hello!")

    say_hello()
    ```

    > This decorator, my_decorator, wraps the behavior of the say_hello function, allowing additional code to be executed before and after the say_hello function without modifying its internal logic. Decorators are widely used for logging, enforcing access control, instrumentation, and more.