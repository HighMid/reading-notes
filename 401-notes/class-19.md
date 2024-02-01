## Class 19 Notes

1. **How can you use regular expressions in Python to search for specific patterns in a string, and what is the primary module to work with them?**

    - You can use [regular expressions](https://www.datacamp.com/tutorial/python-regular-expression-tutorial) by importing `re` . This gives you access with functions such as:

        - `re.search()` returns a match object for the first occurrence of the pattern.

        - `re.findall()` returns a list of all non-overlapping matches of the pattern.

        - `re.match()` is used for matching the pattern at the beginning of the string.

        - `re.compile()` compiles a regular expression pattern into a regular expression object, which can be used for pattern matching.

2. **What is the purpose of the shutil module in Python, and provide an example of a common use case for file or directory management with this module?**

    - `shutil` is a module that provides [high-level file operations](https://pymotw.com/3/shutil/) such as copying, moving, renaming and deleting files and directories.

    - Common Use Case: Will involve copying and moving files and directories

    ```
    import shutil

    # Copy file from source to destination
    shutil.copy('source.txt', 'destination.txt')
    ```

3. **Compare and contrast the os and shutil modules. When would you choose to use one over the other?**

    - `os` focuses more on interacting with the operating system, this is more commonly used to perform simple, single-file operations while needing to manipulate file paths.

    - `shutil` is used more on higher level operations especially when working with multiple or files in bulk. Also if you need to preserve metadata such as date of creation any modifications etc.

    - Both `os` and `shutil` have their use cases with `os` being more lenient in just needing the operation to happen without the need to save metadata while `shutil` being used to preserve any metadata by copying the files contents and its metadata.