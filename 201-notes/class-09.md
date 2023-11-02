## Class09 Notes

### HTML

1. **Why are forms so important in web development?**

    1. User Interaction: Forms are the primary means through which users can interact with a web application. They can submit data, make requests, and perform other interactive tasks through forms.

    2. Data Collection: They are crucial for collecting data from users, whether it's for creating an account, making a purchase, or any other data-driven task.

    3. Feedback Gathering: Forms enable businesses and developers to gather feedback from users to improve the website or application.

    4. Search Functionality: Forms often power search functionality, allowing users to enter search queries and retrieve relevant results.

    5. Ease of Communication: They facilitate communication between the users and the web administrators or other users.<div>
    **Source: ChatGPT**

2. **When designing a form, what are some key things to keep in mind when it comes to user experience?**

    1. Accessibility and Simplicity are important as making sure the form is able to accomodate as many people as possible is crucial.  With how technology is readily available almost always it's important to make sure the user is able to find what they need as quickly and painless as possible, thus Simplicity is a god send.

    2. Input validation is important because no one likes to be told they're wrong without giving a reason as to why.  Also validation is needed to make sure the data is what was requested from the user and not fluff.

    3. Progress indication is nice as it shows the users that they're not throwing information into a black-hole hoping it'll stop one day.  Visual indication of progress is the quickiest way for a user to understand that they're moving forward.

3. **List 5 form elements and explain their importance.**

    1. Text Input: Allows users to enter plain text. It's important for collecting basic information like name, email, etc.

    2. Password Input: Lets users enter passwords securely. It's crucial for authentication processes.

    3. Radio Buttons: Enable users to select one option from a predefined set of options. Useful for multiple-choice questions.

    4. Checkboxes: Allow users to select multiple options from a set. Essential for any form where multiple selections are possible.

    5. Dropdown Lists: Provide a list of options users can select from, saving space and ensuring data consistency.

### JavaScript

1. **How would you describe events to a non-technical friend?**

    > Imagine you're at a party and you have a bunch of balloons. Each balloon has a note inside that gives instructions like "pop me" or "let me float." In this scenario, the balloons are like elements on a webpage, and the notes inside are like events. When you pop a balloon (like clicking a button on a webpage), it triggers the instruction on the note inside (the event) which tells what should happen next. <div>
    **Source: ChatGPT**
2. **When using the addEventListener() method, what 2 arguments will you need to provide?**

    1. **Event Type** : This event is a signal provided by the user's interactions such as clicks, keys on keyboard, webpage finishing loading etc.

    2. **Function** : What happens when the event starts

3. **Describe the event object. Why is the target within the event object useful?**

    - Event objects are parameters that pass information to event handlers to provide additional information.  It's useful because it can contain information on what the user has done so the event handler can act appropriately if needed.

4. **What is the difference between event bubbling and event capturing?**

    - **Event bubbling** is describing how the browser handles events targeted at nested elements.  It started from the innermost element and makes it's way to the outermost one.

    - **Event Capturing** is the opposite, it does the same as handling events but it instead starts from the outermost and makes it's way to the innermost.