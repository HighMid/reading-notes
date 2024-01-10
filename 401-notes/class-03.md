## Class 03 Notes

**1. What is the purpose of the ‘with’ statement when opening a file in Python, and how does it help manage resources while reading and writing files?**

[I hate reading files](https://realpython.com/read-write-files-python/)

- `with` in Python is used to manage resources when handling files.  It's a built-in statement that handles the memory needed such as opening, reading/writing and even closing the file once the operation finishes. This auto management of the process allows better management of memory and reduces the chance of errors in files.

    ```
    with open('example.txt', 'r') as file:
    data = file.read()
    ```

**2. Explain the difference between the ‘read()’ and ‘readline()’ methods for file objects in Python. Provide examples of when to use each method.**

- `read()` is the method used when processing a file in it's entirety, this allows you to get all the files contents at once.

- `readline()` is the method when you read the files contents line by line, this allows you to also set conditions to determine how you would want to use the contents.

**3. Briefly describe the concept of exception handling in Python. How can the ‘try’, ‘except’, and ‘finally’ blocks be used to handle exceptions and ensure proper execution of code? Provide a simple example.**

[Exceptions in Python](https://realpython.com/python-exceptions/)

- `try` , `except` , and `finally` blocks are used to allow the developer to catch and respond to errors or exceptions.  This provides the user with feedback when something is not within expectation and also prevent a program from blowing itself up.

```
def GetLength():
    while True:
        try:
            length = float(input("What is the length of the rectangle.: "))
            if length >= 0:
                return length
            elif length < 0:
                print("No Negatives please.")
            else:
                print("Idk what you did but try again please, no negative numbers.")
            
        except ValueError:
            print("Need a number please, no negatives.")

        finally:
            print("Pull out a airsoft gun")
```

- `try` is used to encapsulate a block where you might need to handle errors or exceptions
- `except` is the block in which handles the appropriate exceptions, in this case a ValueError, length is expecting a float but instead gets something else
- `finally` is the block in which it doesn't matter, it'll always run no matter what