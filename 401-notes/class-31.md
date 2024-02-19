## Class 31 Notes

1. **What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?**

    - **Dockerfile:** A Dockerfile is a script containing a series of instructions and commands for building a Docker image. It specifies the base image to use, software to install, environment variables to set, and files to copy into the image.

    - **Images:** Docker images are the static templates from which containers are created. They include the application code, libraries, dependencies, and environment settings needed to run the application.

    - **Containers:** Containers are runtime instances of Docker images. They encapsulate the application and its environment. Multiple containers can be created from the same image and run independently.

    - **Volumes:** Volumes are used for data persistence in Docker. They enable data to be stored in a particular directory on the host machine outside the container's union file system, ensuring data persists even after the container is deleted.

    - **Docker Compose:** Docker Compose is a tool for defining and running multi-container Docker applications. With a YAML file, developers can configure application services, networks, and volumes, and then start the entire application stack with a single command.

    - **Docker Hub/Registry:** Docker Hub is a cloud-based registry service that allows you to link to code repositories, build your images, test them, store manually pushed images, and link to Docker Cloud for deployment.

2. **Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.**

    1. **Set Up a Django Project:** Initialize a new Django project by creating a virtual environment, installing Django, and running django-admin startproject mylibrary.

    2. **Create an App:** Within your project, create a Django app with python manage.py startapp books for handling books in your library.

    3. **Define Models:** In `books/models.py`, define models representing the data you want to store, such as Book, Author, and Genre. Models are Python classes that define the structure of your database tables.

    4. **Migrate Database:** Apply migrations to create database tables for your models using `python manage.py makemigrations` and `python manage.py migrate`.

    5. **Create Views:** In `books/views.py`, define views to manage the business logic. Views interact with models and decide what to display in templates.

    6. **Define URLs:** In books/urls.py, map URLs to the corresponding views. This step involves defining the routes for your web application.

    7. **Develop Templates:** Create HTML templates in the books/templates directory. Templates define the structure and layout of web pages, allowing dynamic content to be displayed.

    8. **Admin Interface:** Use Django’s built-in admin site to manage the data for your models. Register your models in `books/admin.py` to make them available in the admin interface.

    9. **Test and Run the Server:** Test your application locally by running `python manage.py runserver` and visiting http://localhost:8000 in your web browser. Adjust your models, views, and templates as needed based on testing.

3. **Can you explain the primary differences between Django and Django REST framework?**

    - **Django:** A high-level Python web framework that encourages rapid development and clean, pragmatic design. It provides a full-featured framework for building web applications and sites with content management, authentication, and more.

    - **Django REST Framework:** An extension for Django that adds support for easily building web APIs. DRF is intended for developers to quickly create RESTful APIs, offering features like serialization for converting complex data types to JSON or XML, authentication, and customizable endpoints.

        - **Purpose:** Django is used for building standard web applications. DRF is specifically aimed at building RESTful APIs.

        - **Components:** Django includes ORM, templates, and forms for rendering web pages. DRF provides serializers for data representation and mechanisms for handling API requests and responses.

        - **Use Case:** Use Django when building web applications that serve HTML. Use DRF when you need to provide data as JSON/XML or interact with other services via API.

        - **Client-Side Integration:** DRF is often used in combination with client-side frameworks (like React or Angular) to build SPA (Single Page Applications) or mobile applications that consume data from a Django backend.

> Source: **ChatGPT**