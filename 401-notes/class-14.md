## Class 14 Notes

1. **What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.**

    - [Matplotlib](https://matplotlib.org/stable/tutorials/index): Features a low-level library for creating static, animated and interactive visualizations in Python. Use cases are customizable line graphs showing time-series data.

    - [Seaborn](https://seaborn.pydata.org/tutorial.html): Built on top of Matplotlib, this provides a high-level interface for making your graph look cool. Use cases are heatmaps that show correlation between different feature of a dataset.

    - [Bokeh](https://mybinder.org/v2/gh/bokeh/bokeh-notebooks/master?filepath=tutorial%2F00%20-%20Introduction%20and%20Setup.ipynb): Deisgned for creating interactive plots that can be embedded in web applications. That one interactive dashboard that your teach probably used online to show real-time data.

2. **In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.**

    - **Relational Plots:** `sns.scatterplot` and `sns.lineplot`, this visualizes relationships between two or more variables.

        - **Use case** is plotting a scatterplot to examine a relationship between variables.

    - **Categorical Plots:** `sns.boxplot`, `sns.barplot`, `sns.violinplot`, this is to show the distribution of a numerical variable across different categories.

        - **Use case** is using boxplot to compare the distribution of test scores across different classrooms.

    - **Distribution Plots:** `sns.distplot`, `sns.kdeplot`, `sns.jointplot`, visualize the distribution of a dataset and check for underlying patterns

        - **Use case** to view distribution of a continuous variable like age or income

3. **Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?**

    - The Seaborn cheat sheet like many other things, is a reference guides that help you efficiently work through the process with key sections like,

        - **Plot Types:** A quick reference on plot functions

        - **Customization Options:** Colors man COLORS, themes and other styles that can make the plots better on the eyes.

        - **Data Format Tips:** Standard ways to structure data for plotting

        - **Examples and Syntax:** Shows examples of code of commonly used plot types while offering a template on how the developer can modify to suit their needs
    