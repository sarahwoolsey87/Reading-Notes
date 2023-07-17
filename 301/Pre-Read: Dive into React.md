# Dive into React
[A high level overview of React](https://www.youtube.com/watch?v=FRjlF74_EZk)

## What is React?
> React is a JavaScript library for building user interfaces. It allows developers to create reusable UI components and efficiently update the UI in response to changes in application state.

## What is a component?
> A component in React is a reusable and self-contained piece of UI that can be composed together to build complex user interfaces. Components can be thought of as building blocks that encapsulate the logic and presentation of a specific part of the UI.

## What is the dataflow of React?

> The data flow in React follows a unidirectional flow, commonly known as "one-way data binding." This means that data is passed from a parent component to its child components through props. Changes to the data typically originate from user interactions or updates to the application's state, and these changes propagate down the component hierarchy to update the affected components.

## How do we make a React element a DOM element?

To make a React element a DOM element, you need to render it into the DOM. React provides a method called ReactDOM.render() that takes a React element and a DOM node as arguments. This method will then mount the React element as a child of the specified DOM node, making it a part of the actual HTML document.

## React is a User Interface ______.

> React is a User Interface library. It focuses on the view layer of an application and provides the tools and abstractions necessary for building interactive UIs.

## Which direction does data flow in React?

> In React, data flows in a single direction, from parent components to child components. Parent components pass data down to their children through props. This one-way data flow ensures predictable and maintainable code as changes are always propagated from higher-level components to lower-level components.

## Every component manages its own ____.

Every component in React manages its own state. State is a JavaScript object that represents the internal data and the current state of a component. It allows components to store and update their own data independently. State can be changed using the setState() method, and when the state is updated, React automatically re-renders the component and its children to reflect the new state.