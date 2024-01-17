## Class 07 Notes

1. **Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.**

    - Local Scope is a variable defined within a function, this means that the variable is not accessible outside of the function as it is limited inside of the function. It is created and disposed off when the function is called.

    - Global Scope are variables that can accessed anywhere in the program, it is created at the start of a program and is destroyed when the program ends.

    ```
    global_variable = "I am everywhere"

    def this_function():

        local_variable = "I'm only inside here"

    this_function()

    print(global_variable) # This will be print out "I am everywhere"
    print(local_variable) # This will give an error because it is out of scope and not defined
    ```

2. **How do the global and nonlocal keywords work in Python, and in what situations might you use them?**

    - Global Keywords refer to global variables and can be modified when needed
    - Nonlocal Keywords are variables that are defined in en enclosing scope, these can be modified by the nearest function in scope, these are not defined in a global scope

    ```
    z = 10  # Global variable

    def outer_function():
        z = 20  # Local to outer_function

        def inner_function():
            global z  # Refers to the global z
            z = 30

            nonlocal y
            y = 40  # Refers to y in outer_function

        inner_function()
        print("In outer_function, z =", z)  # z is 20 here
        print("In outer_function, y =", y)  # y is modified to 40

    outer_function()
    print("Globally, z =", z)  # z is modified to 30 globally

    ```

3. **In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.**

    - Big O notation is important because it is a concept that describes the performance of an algorithm. It provides a way to compare efficiency of algorithms by input size and also helps with the amount of requirements such as time and memory needed per algorithm.

4. **Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.**

    - You can import the random module in Python which gives you access to use random.randint(1, 6). This allows Python to random select a number between 1 and 6. You can make a function that takes in a number of trials and the value you wish to keep a count of.

    ```
    import random

    def roll_dice():
        return random.randint(1, 6)

    def simulate_dice_rolls(trials, target):
        count = 0
        for _ in range(trials):
            if roll_dice() == target:
                count += 1
        probability = count / trials
        return probability

    # Simulating the probability of rolling a 6 in 10000 trials
    probability_of_six = simulate_dice_rolls(10000, 6)
    print("Probability of rolling a 6:", probability_of_six)

    ```
    > The function will loop 10000 times and keep a counter if the number is whatever the user passes, in this case 6. It then divides the total count of 6 by the trials to return the probability of hitting 6 out of 10000 trials.