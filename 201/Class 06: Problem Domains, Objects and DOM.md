# Problem Domains, Objects & The DOM

[Javscript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)

## How would you describe an object to a non-technical friend you grew up with?

## What are some advantages to creating object literals?

> A JavaScript object is a collection of key-value pairs where each key represents a property and each value represents the data associated with that property. It's like a container that holds related information and allows you to organize and access that information easily.

-**Simplicity:** Object literals provide a straightforward and concise way to define and initialize objects without the need for complex syntax or constructors.

-**Flexibility:** Object literals allow you to add or remove properties dynamically, making them suitable for scenarios where the structure of the object may change over time.

-**Readability:** Object literals use a simple syntax that is easy to read and understand, making the code more maintainable.

## How do objects differ from arrays?

**Structure:** Objects are collections of key-value pairs, whereas arrays are ordered lists of values accessed by numeric indices.

**Accessing data:** In objects, you access data using property names as keys, while in arrays, you access data using numeric indices.

**Purpose:** Objects are typically used to represent complex entities or concepts with multiple properties, while arrays are used to store collections of similar or related values.

## Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

> You would need to use bracket notation (object[property]) to access an object's property instead of dot notation (object.property) in the following situations:

**Dynamic property names:** If you want to access a property using a variable or an expression as the property name, you must use bracket notation. For example:

let propertyName = "age";
let person = { name: "John", age: 25 };

console.log(person[propertyName]); // Output: 25

**Special characters or reserved words:** If a property name contains special characters or is a reserved word, you need to use bracket notation. For example:

let person = { "first name": "John", class: "A" };

console.log(person["first name"]); // Output: John
console.log(person["class"]); // Output: A

In general, dot notation is preferred for its simplicity and readability, but bracket notation provides more flexibility in accessing object properties.

## Evaluate the code below. What does the term this refer to and what is the advantage to using this?

const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}

> The code provided defines an object called dog with properties such as name, age, color, and a method called humanAge.

 #Here's an evaluation of the code:

The term this refers to the current object, which, in this case, is the dog object. Inside the humanAge method, this is used to access the properties (name and age) of the dog object.

Using this has the following advantages:

**Contextual reference:** this allows you to refer to the current object within its own methods. It provides a way to access and manipulate the object's properties and methods, making the code more self-contained and reusable.

**Dynamic binding:** Since this is dynamically bound to the object, it enables different instances of the same object or different objects to have their own unique context when accessing properties or invoking methods.

In the given code, this.name retrieves the name property of the dog object, and this.age retrieves the age property. This allows the humanAge method to calculate and log the dog's age in human years.

For example, if we call the humanAge method like this:

dog.humanAge();
The output will be:

Spot is 14 in human years

By using this, the humanAge method can dynamically reference the current object's properties, providing a convenient and flexible way to work with the data encapsulated within the object.

[Introduction to the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

## What is the DOM?

> The DOM stands for Document Object Model. It is a programming interface for HTML and XML documents, representing the structure of a web page as a tree-like structure of objects. The DOM allows programs, such as JavaScript, to dynamically access, manipulate, and update the content, structure, and style of a document.

## Briefly describe the relationship between the DOM and JavaScript.

> The relationship between the DOM and JavaScript is that JavaScript provides a way to interact with and manipulate the DOM. JavaScript can access and modify the elements, attributes, and text within an HTML document through the DOM API.

Here's a brief description of the relationship between the DOM and JavaScript:

**Accessing elements:** JavaScript can use methods like getElementById, querySelector, or getElementsByClassName to retrieve specific elements from the DOM based on their IDs, classes, tags, or other criteria.

**Manipulating elements:** JavaScript can modify element properties, such as changing the content (text or HTML), modifying attributes, adding or removing classes, or adjusting the style and appearance of elements.

**Adding and removing elements:** JavaScript can create new elements dynamically and append them to the DOM or remove existing elements from the document.

**Handling events:** JavaScript can register event handlers using the DOM's addEventListener method to respond to user interactions or other events triggered by elements on the web page.

**Dynamic updates:** JavaScript can continuously update and modify the DOM based on user actions, server responses, or other external factors, providing a dynamic and interactive user experience.

In summary, JavaScript and the DOM work together to enable web developers to create interactive and responsive web pages by allowing JavaScript to manipulate and update the content and structure of the page in real-time.

[Understanding the problem domain is the hardest part of programming](http://simpleprogrammer.com/2013/07/15/understanding-the-problem-domain-is-the-hardest-part-of-programming)

[Whats the difference between primitive values and object references in Javascript?](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)