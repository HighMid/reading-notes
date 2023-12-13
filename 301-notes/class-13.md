## Class 13 Notes

### **C R U D** *(Create Read Update Delete)*

1. **Which HTTP method would you use to update a record through an API?**

    - You can use these two methods:

        - **PUT:** You can use this if you plan on updating the resource completely.  This replaces the existed resource with the new one.

        - **PATCH:** You use this method when you only want to update specific data you want to update.

2. **Which REST methods require an ID parameter?**

    - **GET:** Retrieval of a single resource via ID
    - **PUT:** Update a resource completely by replacing
    - **PATCH:** Partial updates to a resource
    - **DELETE:** Removal of a resource via ID

3. **What’s the relationship between REST and CRUD?**

    - **REST(Representational State Transfer)** - is an architectural style for designing networked applications. It uses a stateless communication protocol, usually HTTP. RESTful APIs are designed around the concept of resources, which can be manipulated using a standard set of operations (HTTP methods).

    - **CRUD** - refers to the four basic operations of persistent storage: Create, Read, Update, Delete. In the context of a RESTful API, these operations correspond to HTTP methods:

4. **If you had to describe the process of creating a RESTful API in 5 steps, what would they be?**

    1. **Define Resource** - Identify what resources the API will use.
    2. **Design Endpoints and HTTP Methods** - Determine how the API endpoints will represent the resources.
    3. **Definte Data Formats** - Decide on the format and ensure consistency on how data is structured
    4. **Implement Business Logic** - Write code to handle CRUD operations per resource.  This involves validation, authentication and authorization as needed.
    5. **Testing** - Test each endpoint for all possible use cases and document your instructions on how to use endpoints.