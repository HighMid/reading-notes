## Class 06 Notes

### Python

1. **How can the random module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?**

    [Random](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)

    - Random can be utilized by importing random and using the functions associated with it such as:
        
        - **randint(a, b):** Returns a value equal or higher than 'a' and lower or equal to 'b'
        - **random():** Returns a floating point in range of 0.0 and 1.0
        - **choice(seq):** Returns a randomly selected element from a non-empty sequence
        - **shuffle(seq):** Shuffles the sequence in place


2. **In the context of software development, what is risk analysis, and what are the key steps involved in conducting a risk analysis for a software project?**

    [Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)

    - Risk anaylsis involves identifying, evaluating and prioritizing risks that could impact a project. It's a key part in project mangement as it's one of the tools that helps identify parts in a project that are in need of revaluation.

        1. **Identification:** Determine potential risks that could affect the project, such as technical challenges, resource limitations, or external factors.

        2. **Evaluation:** Assess the likelihood and impact of each risk. This helps in understanding the severity of the risk.

        3. **Prioritization:** Rank the risks based on their potential impact and likelihood of occurrence.

        4. **Mitigation Strategies:** Develop strategies to manage or mitigate the highest priority risks. This could involve contingency planning, risk avoidance, or acceptance.

        5. **Monitoring and Review:** Regularly monitor the risks and review the strategies to ensure they are effective and updated as the project progresses.

3. **What is test coverage and why is it an important (or potentially misleading) metric in software testing?**

    - **Test coverage** is a metric that's used to measure out code that is execute when a test runs. This leads to testing out code that isn't ready for production to help identify critical bugs and could also result in higher code quality. However, this could also be misleading as tests could potentially not be written out to fully test out code and lead people with a false sense of security.

4. **What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity.**

    - The BIG O, is used to describe a performance via time and space used. The time it took to complete the task and the amount of space required for the tasks using a worst-case scenario.

    - Cooking food could be considered O(n) with n being the amount of people you cook for. Stripping out all the nuances of cooking, generally if you cook for more people it will take more time so n representing people increases linearly as the time increases alongside the amount of people.