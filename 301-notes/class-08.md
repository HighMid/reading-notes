## Class 08 Notes

### API Design Practices

1. **What does REST stand for?**

    - REST(Representational State Transfer), it's an archtitectural style for designing networked applications.

2. **REST APIs are designed around a ____.**

    - Resources, these range from objects, data or services that are accessed by the client.

3. **What is an identifier of a resource? Give an example.**

    - https://www.prydwen.gg/counter-side/characters/hilde , "hilde" is the unique identfier in the resources.


4. **What are the most common HTTP verbs?**

    - GET
    - POST
    - PUT
    - DELETE
    - PATCH

5. **What should the URIs be based on?**

    - Should be based on nouns as the resource and not the actions(how the operations work on the resource)

6. **Give an example of a good URI.**

    - https://www.prydwen.gg/counter-side/characters/ - All characters
    - https://www.prydwen.gg/counter-side/characters/hilde - Specific character

7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**

    - It's considered bad because it involves making many small requests and responses which is infficient as this increases system resources and overall slower performance.

8. **What status code does a successful GET request return?**

    - Status Code 200(OK)

9. **What status code does an unsuccessful GET request return?**

    - Either a 404 code for the website not being found or 400 a bad request when the request has either degraded or was malformed

10. **What status code does a successful POST request return?**

    - Status code 201(Created)

11. **What status code does a successful DELETE request return?**

    - Status code 200 upon successful deletion or 204(no content) which indicates success however no content to send in response.