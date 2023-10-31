## Class07 Notes

### Domain Modeling

1. **Explain why we need domain modeling.**

    1. Understanding the Problem: Before you can write a solution, you have to fully understand the problem. Domain modeling helps developers, stakeholders, and other team members visualize and comprehend the core concepts, relationships, and behaviors the software needs to encapsulate.

    2. Communication: For projects with multiple stakeholders, including developers, managers, and business experts, a domain model provides a common language. It ensures everyone understands the core concepts and their relationships the same way.

    3. Reusability: Elements of the domain model, especially if well-abstracted, can often be reused in other projects or areas of the same project.

    **Source: ChatGPT**

### HTML Table Basics

1. **Why should tables not be used for page layouts?**

>- Tables shouldn't be used for page layouts because they can interfere with technologies such as screen readers as they can provide inaccurate interpretation of data.  These devices interpret tables like tabular data and are not at all useful for webpage structures.
>- There are other technologies that are better suited for webpage structure such as FlexBox and Grid as they are capable of adjusting themselves to fit various screen sizes while tables are not as adaptable.

2. **List and describe 3 different semantic HTML elements used in an HTML `<table>`.**

    1. `<table>`: This is the primary element that defines a table. It acts as a container for all the other table-related elements.

    2. `<tr>` (Table Row): This element represents a single row in a table. It contains a set of `<td>` or `<th>` elements which represent the individual cells of that row.

    3. `<td>` (Table Data): This element represents a single data cell in a table. It contains the actual data for that cell.

    4. `<th>` (Table Header): While similar in structure to the `<td>` element, the `<th>` represents a header cell. This is typically used in the first row or first column of a table to describe the type of data in that column or row. By default, the content in a `<th>` is bold and centered.
    
    **Source: ChatGPT**

### Constructors

1. **What is a constructor and what are some advantages to using it?**

>- Constructors is a function that is used to create and initalize objects. They are used to create multiple objects with the same structures without having to remake the object structure for each one. 

2. **How does the term this differ when used in an object literal versus when used in a constructor?**

>- `this` used in an object literal references the object itself while when used in a constructor it'll use the newly created object instead.