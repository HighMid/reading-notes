## Class 12 Notes

### Status Codes

1. **In your own words, describe what each group of status code represents:**

    - **100’s**: Received the request and the process is continuing
    - **200’s**: The request has been accepted and understood by the server.
    - **300’s**: Requires additional actions to be taken by the user
    - **400’s**: Errors via client side, range from bad links, requests or faulty request routing
    - **500’s**: Server sided errors, not client side fault

2. **What is a status code 202?**

    - Indicated that the request is processing but the process isn't complete.  It's been acknowledged and understood but the action may or may not be acted upon.
2. **What is a status code 308?**

    - This code means the resource that is currently trying to be accessed has been permanent moved to another URL.  The POST request is still active after the redirection.

3. **What code would you use if an update didn’t return data to a client?**

    - Status code 204, this shows that the data has been accepted and it does not need to return any data back.

4. **What code would you use if a resource used to exist but no longer does?**

    - Status code 410, this indicates that the resource requested is no longer available and will not be available again.

5. **What is the ‘Forbidden’ status code?**

    - Status codes 401 Unauthorized and 403 Forbidden, 
        - 401 indicates that authentication is required and will deny access until given.
        - 403 Indicates that the server understands the request but denies access

### MongoDB, REST API

1. **Why do we need to pull our MongoDB database string out of our server and put it into our .env?**

    - Security, it's important to keep the connection string or just any sensitive information in an `.env` that is secure and not included in the code. It also allows for testing in different environments with diferent `.env` files.

2. **What is middleware?**

    - These are functions that has access to the request and response object. These can execute code and make changes to request and reponse objects.


3. **What does app.use(express.json()) do?**

    - It's middleware function in Express, it parses incoming requests with JSON payloads and converts JSON data into a JavaScript object.

4. **What does the /:id mean in a route?**

    - It's a route parameter that represents a variable part of the URL.  It can be replaced with any value to represent different user IDs.

5. **What is the difference between PUT and PATCH?**

    - PUT is used to update a resource completely, when sending a PUT request is replaces the entire resource.

    - PATCH is used for partial updates, when sending a PATCH request you update specific data that you want to update.

6. **How do you make a default value in a schema?**

    - In MongoDB, when defining a schema you can set a default value for a field by using the `default` keyword.

7. **What does a 500 error status code mean?**

    - That status code indicates that the server has encountered a problem in the request.

8. **What is the difference between a status 200 and a status 201?**

    - Status 200 is a standard response for successful requests, the request has been received, understood and processed.
    - Status 201 is when a resource has been successfully created in response to the clients request.