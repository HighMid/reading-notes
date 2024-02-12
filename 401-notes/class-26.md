## Class 26 Notes

1. **What are the key components of the Django framework, and how do they contribute to building a web application?**

    - Django is a high-level web framework for python that emphasizes reusability and pluggability of components.

        - **URL Dispatcher:** A URL mapper that directs incoming web requests to views based on the request URL. It allows you to design clean, elegant URLs, which are a key part of a web application’s interface.

        - **Admin Interface:** A built-in, ready-to-use interface for administrative activities. It provides a rapid interface to manage site content, and it's one of Django’s most celebrated features.

        - **Forms:** Handle the generation and processing of HTML forms. Django forms simplify the task of validating and processing form data.

        - **Security Features:** Django has built-in protection against many security threats like SQL injection, cross-site scripting, cross-site request forgery, and clickjacking. Its user authentication system provides a secure way to manage user accounts and passwords.

2. **Explain the role of Django’s MTV (Model-View-Template) architecture and how it handles a typical web request-response cycle.**

    - **Model** is the data access layer. It represents the database structure or the data structure used by the application.

    - **Template** is the presentation layer. It describes how the data received from the models should be displayed.

    - **View** acts as the controller and handles the business logic. It processes requests, interacts with the model, and renders a response using the appropriate template.

    1. A request is received by Django from a web client.
    2. The URL dispatcher matches the request URL to a view function.
    3. The view interacts with the model as necessary to retrieve data.
    4. The view delegates formatting of the retrieved data to a template.
    5. The rendered template (as HTML) is returned to the client as a response.

3. **What is the purpose of Tailwind CSS, and how does it differ from Bootstrap CSS?**

    - Tailwind CSS is a framework that provides custom designs directly in you rmarkup. This allows for more hands on and unique approach on styles as you are tailoring each class directly in HTML. It differs from bootstrap as bootstrap comes with a wide variety of pre-designed components that allow for rapid prototyping. Bootstrap is more aligned with uniformed design while Tailwind gives more of the design to the developer.