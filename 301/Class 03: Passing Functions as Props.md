# Passing Functions as Props

[React Docs: Lists & Keys](https://reactjs.org/docs/lists-and-keys.html)

## 1.  What does .map() return?
>In React, the `.map()` function returns a new array with the same length as the original array, where each element is the result of the provided function being called on each element of the original array.
>
## 2.  If I want to loop through an array and display each value in JSX, how do I do that in React?

To loop through an array and display each value in JSX, you can use the `.map()` function in combination with JSX. Here's an example:

`const items = ['Item 1', 'Item 2', 'Item 3'];

const listItems = items.map((item, index) => (
  <li key={index}>{item}</li>
));

return <ul>{listItems}</ul>;` 

In the above example, we create an array called `items` and then use the `.map()` function to iterate over each element of the `items` array. For each item, we create a `<li>` element with a unique `key` attribute set to the `index` of the item. The `index` serves as a unique identifier for each list item.

## 3.  What is the purpose of a key?

> The purpose of a key in React is to help React identify each list item uniquely when rendering lists dynamically. When rendering lists in React, each item in the list should have a unique `key` prop. React uses the `key` prop to efficiently update the components and maintain the correct state when the list changes. Using unique keys helps React determine which items have changed, been added, or been removed, enabling it to perform updates more efficiently.

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

## 1.  What is the spread operator?

The spread operator (`...`) in JavaScript allows you to expand iterable objects, such as arrays or objects, into individual elements. It can be used in several ways to perform different operations. 

## 2.  List 4 things that the spread operator can do.

1.  **Copying Arrays and Objects:** The spread operator can create a shallow copy of an array or an object. This is useful when you want to create a new array or object with the same elements or properties as the original.
    
2.  **Concatenating Arrays:** The spread operator can be used to concatenate multiple arrays into a single array.
    
3.  **Passing Arguments:** The spread operator can spread the elements of an array as individual arguments when calling a function.
    
4.  **Merging Objects:** The spread operator can merge the properties of multiple objects into a new object.

## 3.  Give an example of using the spread operator to combine two arrays.

const array1 = [1, 2, 3];
const array2 = [4, 5, 6];

const combinedArray = [...array1, ...array2];
console.log(combinedArray); // Output: [1, 2, 3, 4, 5, 6]


## 4.  Give an example of using the spread operator to add a new item to an array.

const originalArray = [1, 2, 3];
const newItem = 4;

const newArray = [...originalArray, newItem];
console.log(newArray); // Output: [1, 2, 3, 4]


## 5.  Give an example of using the spread operator to combine two objects into one.

const object1 = { name: 'John', age: 25 };
const object2 = { city: 'New York', country: 'USA' };

const combinedObject = { ...object1, ...object2 };
console.log(combinedObject);
// Output: { name: 'John', age: 25, city: 'New York', country: 'USA' }

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

## 1.  In the video, what is the first step that the developer does to pass functions between components?

> To pass functions between components in React, the first step typically involves defining the function in the parent component that you want to pass to a child component. This function is usually defined as a method within the parent component's class or as a regular function within the parent component.

## 2.  In your own words, what does the  `increment`  function do?

> In simple terms, the `increment` function is a custom function that increases a counter or updates a value. Its exact functionality depends on the specific implementation. It could increment a counter by a fixed amount, update a state variable, or perform any other desired operation.
> 
## 3.  How can you pass a method from a parent component into a child component?

> To pass a method from a parent component to a child component in React, you can pass the method as a prop to the child component. This allows the child component to access and invoke the method
> 
## 4.  How does the child component invoke a method that was passed to it from a parent component?

> By invoking `this.props.increment` in the child component, it calls the `increment` method defined in the parent component, allowing the child component to trigger the parent's functionality.

It's important to note that the naming and structure may vary based on specific implementation patterns and preferences, but the concept of passing a method from a parent component to a child component remains the same.

[React tutorial through 'Declaring a Winner'](https://reactjs.org/tutorial/tutorial.html)

[React Docs: Lifting State up](https://reactjs.org/docs/lifting-state-up.html)