## Class 28 Notes

1. **How do Django Forms facilitate user input handling, and what are some key components of creating a form using the Django framework?**

    - Django can validate user inputs to ensure that the data is formatted correctly or is considered safe before being stored in a database. Django can also render HTML forms which cuts back the code needed for developers to write and if any sort of error occurs, the forms can provide immediate feedback on what needs to be fixed.
    
    - **Key Components:**
        - **Form** - Django forms is a subclass that allows what was mentioned above and also allows customization to define certain fields needed.

        - **View** - Instantiates the form to be able to handle submission and validate data, afterwards decides what is the next step

        - **Templates** - Once the form class is defined you can use it as a template to create more forms of a similar context

2. **Explain the purpose of Django Templates in web development and describe how template inheritance can be utilized to improve code reusability and maintainability.**

    - The purpose of Django Templates is to define the structure of HTML dynamically, this follows the MVC(Model-View-Controller) architecture in which the templates are playholders for dynamic content.

    - **Template Inheritance** allows for code to be reused in easily maintained, this defines how the structure should look for most of your website if not all.

        - **Base Template** - This is an HTML file that defines the structure of the website that has `{block block_name}, { endblock }` used for child templates to override.

        - **Child Template** - Inherits the base template and can ovveride blocks with its own content.

3. **Describe the function of Django Views in handling HTTP requests, and outline the differences between function-based views and class-based views.**

    - Django views is able to process HTTP requests to interact with the model to access and process data, it then returns a HTTP response with a template filled with data.

    - **Function-Based Views**(FBVs): are simple python functions that take a web request and return a response, because of this it allows for,
        - Simplicity: helpful when all you want is just a simple roadmap to one point to another

        - Explicitness: since these are small and simple by nature it's easy to control the flow and understand the logic

        - Decorators: because who doesn't like adding a `hell yeah` after every response.

    - **Class-Based Views**(CBVs): are defined classes instead of cuntions, they are used to handle common patterns and idioms. These are most useful for,
        - **Reusability:** this allows for reusable code for implementation of common patterns

        - **Extensibility:** able to make small classes within to add more functionality to the views

        - **Organization:** because looking at a class with methods is better than looking at a module with a bunch of functions. Mainly it allows you to organize the code better
