## Class 12 Notes

### JavaScript Canvas

1. **What does the `<canvas>` allows a developer to achieve?**

    > Allows you to draw 2D graphics using JavaScript(Kinda sounds a lot like using turtle in Python). Can also be used to make dynamic graphs based on data and can also be used in web-based game dev for the graphics.

2. **What is the importance of the closing `</canvas>` tag?**

    - It's important to use the closing tag as it helps with documentation and readability, not to mention is a requirement for valid HTML.
    - Also ensures the type of information you wish to present as anything written between the open and closing tag will be displayed if it's supported

3. **Explain what the `getContext()` method does.**

    - Gives access to the drawing content which is an object that contains all the properties needed to draw on the canvas.
    - Passing arugments through `getContext()` allows you to specify what type of drawing context you wish to work with that also maintains any styles, transformations and other properties.

### Chart.js Documentation

1. **What is Chart.js and how it can be brought into your project?**

    > **Chart.js** is an open-source library that can be imported to allow developers to create interactive and responsive charts in their applications.  It can be brought to in different ways like downloading [Chart.js GitHub repository](https://github.com/chartjs/Chart.js) and including it to your project then simply link it using `<script>`. You can also link it using `<script>` to the CDN link as well.

2. **List 3 different Chart types you can create using Chart.js.**

    - **Line Charts**: used for showing trends over time or categories with containuous dataset.
    - **Bar Charts**: good for comparing different groups or categories
    - **Pie and Doughnut Charts**: used to show parts of a circle divided into proportional segments.

3. **What are some advantages to displaying data via a chart over a table?**

    - Visual Appeal: Charts are more visually engaging than tables. A well-designed chart can catch the viewer's attention and make a stronger impression than rows of numbers.

    - Immediate Insights: Charts can often convey trends, patterns, and outliers more quickly than tables. Viewers can immediately grasp the big picture without getting into the details.

    - Comparative Analysis: It is easier to compare different datasets visually. In a chart, differences in line heights, bar lengths, or pie segments are more apparent than comparing figures in a table.

    - Space Efficiency: Charts can display large amounts of data in a more compact space. This is particularly useful for dashboards and reports where space is at a premium.

    - Understandable for Diverse Audiences: Charts are universally understood and can be interpreted by people with various levels of expertise, including those who may not be comfortable with numerical data.

    >**Source: ChatGPT**

4. **How could Chart.js aid your previously created applications visually?**

    >- It would make the overall experience much more interactive I would say. I could add tooltips, making everything feel consistent in it's layout and make data more dynamic alongside the layout also adjusting across various different platforms. 