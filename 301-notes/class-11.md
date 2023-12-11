## Class 11 Notes

### SQL vs NoSQL

Differences between the two are:

    1. SQL databases have fixed schema, NoSQL have dynamic schema

    2. SQL tend to scale vertically while NoSQL scales horizontally

    3. SQL are table based, NoSQL range from document-based, key-value pairs or graph databases.

    4. SQL are more suited to complex transactions since they follow ACID(Atomitcity, Consistency, Isolation, Durability), NoSQL are more suited to simple transactions as speed and performance is prioritized.

    5. SQL is better at managing data integrity because of their fixed schema and this makes it easier to manage. NoSQL, while more flexible, sacrifices standardization which makes it harder to manage data as they can be in various data types.

1. **What kind of data is a good fit for an SQL database?**

    - Structured data are ideal as these adhere to a predefined schema.  
    - An example for this is customer transactions online, a customer has to fill in the appropriate information to purchase an item then the order number with their items gets assigned to the customer.

2. **What kind of data is a good fit a NoSQL database?**

    - NoSQL is suitable for unstructored data like JSON, where the information's structure can vary in order and size.
    - Managing information for individuals on a social media platform, these can vary in size and information provided.

3. **Which type of database is best for hierarchical data storage?**

    - NoSQL is better suited for this because they have a dynamic schema which allows for higher flexibility when handling data.

4. **Which type of database is best for scalability?**

    - NoSQL is better because of how they scale, they scale horizontally which allows them to handle large volumes of data from many servers.

5. **What does SQL stand for?**

    - Structured Query Language

6. **What is a relational database?**

    - Relational databases are structured to recognize relations among stored items of information.

7. **What type of structure does a relational database work with?**

    - They work with data stored in rows and columns

8. **What is a ‘schema’?**

    - Schemas are structures that defines the organization of data, this includes relationships with each other and other structures, tables and columns.

9. **What is a NoSQL database?**

    - A database that is designed to handle a variety of data models, including key-value, documents and graph formats, these are not limited to fixed schemas.

10. **How does it work?**

    - NoSQL works by storing and retrieving data in a way that enables high speed operations and flexibility.

11. **What is inside of a MongoDB database?**

    - MongoDB is a database built off NoSQL, it contains collections of documents that are similiar to JSON where there are key-value pairs and have a variety of structures.

12. **Which is more flexible - SQL or MongoDB? and why.**

    - MongoDB is more flexible because it operates on NoSQL so it has a flexible schema which can be used to handle various types of data

13. **What is the disadvantage of a NoSQL database?**

    - Lack of Standardization is a disadvantage as this makes it challenging to handle and manage as the data isn't consistent across different systems.
