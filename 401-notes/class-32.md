## Class 32 Notes

1. **What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?**

- **Key Components and Purpose:**

    - **Permissions in DRF:** DRF permissions determine whether a request should be granted or denied access to certain API functionality. Permissions are used to protect API resources and ensure that only authorized users can perform specific actions, such as creating, updating, or deleting resources.

    - **How They Work:** Permissions in DRF are handled through permission classes. When a request is made, DRF checks the permission classes associated with the view handling the request. Each permission class implements a .has_permission() method (and sometimes a .has_object_permission() method for object-level permissions) to determine if the request should be allowed.

    - **Default Permission Policies:** DRF comes with a set of default permission classes such as AllowAny, IsAuthenticated, IsAdminUser, and IsAuthenticatedOrReadOnly. These can be applied globally in the DRF settings or individually to views or viewsets.

    - **Custom Permissions:** You can define custom permission classes by extending BasePermission and overriding the .has_permission() and/or .has_object_permission() methods to implement custom logic.

- **How DRF Permissions Help in Securing an API:**

    - **Access Control:** By specifying who can access what resources and actions, permissions help in implementing access control policies, protecting sensitive data and functionality from unauthorized access.

    - **Fine-grained Permissions:** DRF allows for both view-level and object-level permissions, providing fine-grained control over access. This means you can restrict actions not just based on who the user is, but also based on the properties of the object being accessed.

    - **Customizable:** The ability to create custom permission classes enables developers to implement complex access control logic tailored to their application's specific needs.

2. **In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?**

    - The SELECT statement in SQL is used to query the database and retrieve selected data from one or more tables. It is the most commonly used statement in SQL for data retrieval.

    Usage Example:

    - To retrieve all columns from a table called employees, you would use the following SQL statement:

    ```
    SELECT * FROM employees;
    Here, * is a wildcard character that represents all columns in the table. This statement fetches all records and all fields from the employees table.
    ```

3. **Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?**

    - DRF's generic views simplify the task of building API views by providing a set of classes for common CRUD (Create, Read, Update, Delete) operations. These views encapsulate common behavior, reducing the amount of code you need to write for your API.

        1. **ListAPIView:** Used for read-only endpoints to represent a collection of model instances. It provides a get method handler.

        ```
        from rest_framework.generics import ListAPIView
        from .models import Employee
        from .serializers import EmployeeSerializer

        class EmployeeList(ListAPIView):
            queryset = Employee.objects.all()
            serializer_class = EmployeeSerializer
        ```

        2. **RetrieveAPIView:** Used for read-only endpoints to represent a single model instance. It provides a get method handler for fetching a specific record.

        ```
        from rest_framework.generics import RetrieveAPIView

        class EmployeeDetail(RetrieveAPIView):
            queryset = Employee.objects.all()
            serializer_class = EmployeeSerializer
        ```

        3. **CreateAPIView, UpdateAPIView, DestroyAPIView:** These are used for creating, updating, and deleting a model instance, respectively. They provide post, put/patch, and delete method handlers.

        4. **ListCreateAPIView and RetrieveUpdateDestroyAPIView:** These are combined views that provide methods for listing and creating, or retrieving, updating, and deleting, reducing the need for separate views for each operation.

> Source **CHATGPT**