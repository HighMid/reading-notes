## Class 06 Notes

### JavaScript Object Basics

>Objects in JavaScript are collections of data that are refered to properties inside themselves.  They house unique strings and can be of any type, these object typically have a certain degree of relevence to each other like a person's information or in a game sense what pokemon are in your party.

1.**How would you describe an object to a non-technical friend you grew up with?**

- Think of an object like a personal ID card. On the card, there are different pieces of information (like name, birthdate, address, etc.), and each piece of information has a label. In the world of programming, we call this card an "object". The labels (like name, birthdate) are called "properties", and the information tied to those labels (like 'John Doe', '01/01/2000') are called values. <div>
**Source: ChatGPT**

2.**What are some advantages to creating object literals?**

- From what I read object literals are pretty useful to clearly define what type of data is meant to be stored in the object.
- Can store varied types of data together such as string, numbers, boolean and strangely enough functions.
- Helps reading code because when making an object you can give it a meaningful name to specifiy what's in it.

3.**How do objects differ from arrays?**

- Objects store data in key-value pairs, what that means is that each data point has a unique name associated with the data.
- Arrays are ordered list that can be accessed by the position in the list via numbers.  This makes it so if you're trying to find specific data in an array you have to know what the number in the element it is.

4.**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**

> You would use brackets when:

- There are special charaters in the property name or spaces
- The property name is stored in a variable
- The property name is a number outside of an array.

5.**Evaluate the code below. What does the term `this` refer to and what is the advantage to using this?**
```
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

- `this` refers to the object it's located in.  In this case it'll refer to "dog" and will dynamicly change depending on the context.  It's a way for it to access properties of the object and change if needed to fit the context.

### DOM

>DOM *(Document Object Model)* is an interface for web document that allows programs and scripts to actively access and update structures, content and style of web documents.  It represents the structure of documents where each object corresponds to a part of the document, any changes to the DOM are immediately reflected in the rendered document.

1. **Briefly describe the relationship between the DOM and JavaScript.**

>- Manipulation & Interaction: JavaScript is commonly used to interact with and manipulate the DOM to update the content, structure, and style of a webpage. For instance, when you see dynamic content changes, animations, or form validation on a website, it's often JavaScript working with the DOM to make those changes.
>- Events: JavaScript can also add event listeners to DOM elements. This means JavaScript can execute specific functions in response to certain events like a button being clicked, a form being submitted, or the mouse hovering over an element.
>- Dynamic Content Creation: With JavaScript, you can create new DOM elements, modify existing ones, or remove them entirely. This is fundamental to making interactive and dynamic web applications.
>- Interface to Web Documents: The DOM provides the necessary methods and properties for JavaScript to interact with and manipulate the structure of web documents. While the DOM is language-agnostic (meaning you can technically interface with it using various programming languages), JavaScript is the most widely used language for this purpose in the realm of web development. <div>
>  **Source: ChatGPT**