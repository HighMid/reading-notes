## Class 29 Notes

1. **What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?**

    - The key benefit for using Custom User Models is that you can customize it to fit the needs of your application. It also allows it to be easily extended because it gets rid of the need to refactor much of the code.

    - It's different from the default model because the default model is not a one size fits all, it's good to use the default model if you're trying to make a prototype of an idea as a proof of concept but ideally it's better to make a custom user model when building an application with specific needs.

2. **Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.**

    > Here is a checklist that has been graciously given to me by ChatGPT,

    1. **Define the Custom User Model**:

        - **Create a new model** that extends AbstractBaseUser and possibly PermissionsMixin for handling permissions.
        - Specify the fields you need, such as email, name, etc. Mark one of the fields (usually email) as the USERNAME_FIELD for authentication purposes.

    2. **Update settings.py**:

        - In your Django project's settings.py file, add or update the AUTH_USER_MODEL setting to point to your custom model. This tells Django to use your custom model for all user-related functionalities.

        ```
        AUTH_USER_MODEL = 'myapp.MyCustomUser'
        ```
        
        - Replace 'myapp.MyCustomUser' with the actual app label and model name of your custom user model.

    3. **Create a Custom User Manager:**

        - Implement a custom manager for your user model by extending BaseUserManager. This manager should override the create_user and create_superuser methods to handle user creation.

    4. **Run Migrations:**

        - After defining your custom user model and manager, run migrations to update the database schema.

        ```
        python manage.py makemigrations
        python manage.py migrate
        ```

3. **What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.**


    - DjangoX is a project template that gives you a head start on projects. It's like a cheatcode that allows you to skip the tutorial and go into the first stage, the focus is to save development time by giving the user a comprehensive starting point such as,
        - Offering a ready-to-use project structure with best practices and configurations that might take significant time to set up from scratch.
        - Docker support, pre-configured user authentication views, and more, which are not provided out of the box by Django.

    - A use is that I wanna make a web application that allows some sort of user authentication and I want API endpoints for some leaderboard showing how much points they can get in minesweeper. I could just start up my project in DjangoX and pretty much have all of that done