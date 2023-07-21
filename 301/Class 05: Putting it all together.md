# Putting it all together

[React Docs: Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

## What is the single responsibility principle and how does it apply to components?

**Single Responsibility Principle (SRP) and its application to components**:

The Single Responsibility Principle is a design principle in software development that states that a class, module, or component should have only one reason to change. In other words, a component should have only one responsibility or job, making it easier to understand, maintain, and extend.

When it comes to components in software development, applying the SRP means that each component should be focused on handling a specific functionality or feature. By ensuring that a component has a single responsibility, you improve the code's modularity and reduce the risk of unintended side effects when making changes.

## What does it mean to build a ‘static’ version of your application?

> Building a "static" version of an application typically refers to creating a version that lacks dynamic or interactive elements. In this context, "static" means that the application's content is fixed and doesn't change based on user interactions or real-time data updates. Instead, the static version represents a snapshot of the application with hardcoded data.

## Once you have a static application, what do you need to add?

> After building a static version of an application, the next step is to introduce interactivity and dynamic behaviour. This involves adding functionalities such as user input handling, data fetching from servers, and updating the application's interface based on user actions or real-time data changes.

## What are the three questions you can ask to determine if something is state?

- a. Does it change over time? State is all about representing data that can be modified or updated during the application's lifecycle.

- b. Can you derive it from other state or props? If the information can be derived from existing data in the application, it might not be considered state in itself.

- c. Does it need to be passed as props from a parent component? If data needs to be passed down from a parent component to a child component via props, it may be considered state.

## How can you identify where state needs to live?

Determining where state should reside can be critical to managing an application's data effectively. Here are some strategies to help identify where state needs to live:

- a. Identify which components need the data: Determine which components in your application require access to the specific piece of data.

- b. Find the common parent: Look for the closest common ancestor of these components, as this is usually the ideal location for the state.

- c. Consider the flow of data: Analyze how data flows through your application and find the most logical place to manage and store the data to ensure it's accessible by the relevant components.

- d. Think about the lifecycle of the data: Consider the lifespan of the data and choose a location that allows the data to persist and update as needed during the application's runtime.

Remember that state management patterns, like Redux or React's built-in useState, can also help you centralise and manage state in larger applications.

[Higher Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

## What is a “higher-order function”?

A "higher-order function" is a concept in programming where a function takes one or more functions as arguments, returns a function as a result, or both. In other words, it treats functions as first-class citizens, enabling them to be manipulated and passed around like any other data types (e.g., integers, strings).

## Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

function greaterThan(n) {
  return (m) => m > n;
}
In this function, greaterThan is a higher-order function. It takes a single argument n, and it returns an anonymous function (a closure) that takes another argument m. The returned function checks whether m is greater than the original n and returns true or false accordingly.

So, in summary, line 2 of the greaterThan function is creating and returning an anonymous function that captures the value of n and uses it to perform a comparison with the argument m.

## Explain how either map or reduce operates, with regards to higher-order functions.

**Map:**
The map function is a higher-order function used in many programming languages, including JavaScript. It takes an array and a transformation function as arguments. The transformation function is applied to each element of the array, creating a new array with the results of the transformations. The new array has the same length as the original array, but each element is transformed according to the function provided.

Example:

const numbers = [1, 2, 3, 4, 5];
const squaredNumbers = numbers.map((num) => num * num);
// squaredNumbers will be [1, 4, 9, 16, 25]

In this example, map takes an array numbers and applies the transformation function (num) => num * num to each element, resulting in the squaredNumbers array.

**Reduce:**

The reduce function is another higher-order function in JavaScript. It is used to "reduce" an array to a single value by applying a function that accumulates the elements of the array into a final result. The function passed to reduce typically takes two arguments: an accumulator and the current element of the array. The accumulator is updated with each iteration, and at the end, it represents the final result.
Example:

const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((accumulator, num) => accumulator + num, 0);
// sum will be 15
In this example, reduce takes the array numbers, and the provided function (accumulator, num) => accumulator + num sums up all the elements in the array, starting with an initial value of 0.

Both map and reduce are powerful higher-order functions that enable developers to perform transformations and aggregations on arrays in a concise and expressive manner.