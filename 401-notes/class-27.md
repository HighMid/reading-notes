## Class 27 Notes

1. **Explain the purpose and basic structure of Django models. How do they help in creating and managing database schema in a Django application?**

    - Django models play a crucial role in abstracting and managing the database schema of a Django application. They are essentially Python classes that define the fields and behaviors of the data you’re storing. Each model maps to a single database table, with the model's attributes representing database fields

2. **Describe the primary features and functionality of the Django Admin interface. How can it be customized to suit the specific needs of a project?**

    - **CRUD Operations:** Create, Read, Update, and Delete operations on your models.

    - **Customization:** Customize the interface to display data in a way that makes sense for your application.

    - **Authentication and Authorization:** Comes with a built-in user authentication system to manage user permissions.

    - **Automatic Interface:** Automatically generates the admin interface for managing the models.

    >- These can be customized by modifying the `admin.py` app by allowing you to add your models onto the admin site, you can also use the `ModelAdmin` option to change the way they are displayed.

3. **Briefly outline the key components and workflow of a Django application, as discussed in the Beginner’s Guide to Django. How do these components interact with each other to create a functional web application?**

    - **Models:** Represent the application’s data and contain fields and behaviors of the stored data.
    - Views: Handle the business logic and are responsible for processing requests and returning responses.
    - **Templates:** Define the structure or layout of the output (usually HTML).
    - **URLs:** URL dispatchers that route incoming requests to the appropriate view based on the request URL.
    - **Admin:** An automatically generated admin interface for managing site content.

    - **Request Handling:** A request received by the application is routed to a view via a URL pattern defined in the urls.py file.
    - **View Processing:** The view processes the request, interacting with the necessary models and invoking any required business logic.
    - **Template Rendering:** The view renders a response, often by populating a template with data obtained from models. This template defines how the data should be presented.
    - **Response:** The rendered response is sent back to the client.

**Source: CHATGPT**