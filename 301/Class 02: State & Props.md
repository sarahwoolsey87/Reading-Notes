
# State and Props
[React 
Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

## What is the very first thing to happen in the lifecycle of React?
> In the lifecycle of React, the very first thing to happen is the constructor. It is the initial step where the component's state and initial values are set.

## Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- **constructor**: This is where the component is initialized, and state and props are set. It is called before the component is mounted.

- **render:** This method is responsible for rendering the component's JSX (or other components) into the DOM. It determines the structure and appearance of the component.

- **componentDidMount:** This method is invoked immediately after the component is mounted. It is called once the component is rendered to the DOM, making it suitable for performing side effects like fetching data from an API or setting up event listeners.

- **React Updates:** This is a continuous process that occurs whenever the component's state or props change. React will compare the previous state/props with the new ones, and if there are differences, it will trigger a re-render.

- **componentWillUnmount:** This method is called just before the component is unmounted and removed from the DOM. It provides an opportunity to clean up any resources or event listeners established in the componentDidMount method.

## What does componentDidMount do?

> The componentDidMount method is used for performing actions after the component has been rendered to the DOM. It is commonly used to fetch data from APIs, set up subscriptions or timers, or interact with other JavaScript frameworks. It is considered a good place to start asynchronous operations or initialization tasks related to the component.

[React State V Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

## What types of things can you pass in the props?

> In React, props (short for "properties") are used to pass data from a parent component to a child component. You can pass various types of data as props, including:

- **Primitives:** Such as strings, numbers, booleans, etc.
- **Objects:** Including plain objects or instances of custom classes.
- **Functions:** You can pass functions as props, allowing child components to invoke them.
- **React elements:** You can pass other React components as props, enabling composition and reuse.

## What is the big difference between props and state?

> The big difference between props and state is that props are passed from a parent component and are read-only to the child component. They cannot be modified directly by the child component. On the other hand, state is managed within a component and can be modified using setState() method. State is used to store data that can change over time and affects the component's rendering.

## When do we re-render our application?

> Re-rendering of a React application occurs when there are changes to the component's state or props. When the state or props of a component change, React will automatically trigger a re-render, updating the component's UI to reflect the new data.

## What are some examples of things that we could store in state?

- **Form input values:** Storing the values entered in form fields.
- **Component configuration:** Controlling the visibility, appearance, or behavior of a component.
- **Data fetched from an API:** Storing the retrieved data for display or further processing.
- **User authentication status:** Keeping track of whether a user is logged in or not.
- **UI state:** Managing the state of UI components, such as dropdown menus, modals, or tabs.
> In general, state is used for data that is internal to a component and may change over time, while props are used for passing data from a parent component to its child components.

[React Docs: State and Lifestyle](https://reactjs.org/docs/state-and-lifecycle.html)
[React Docs: Handling Events](https://reactjs.org/docs/handling-events.html)
[React tutorial through 'Developer Tools'](https://reactjs.org/tutorial/tutorial.html)
[React Bootstrap Documentation](https://react-bootstrap.github.io/)
[Bootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
[Bootstrap Shuffle: a class 'sandbox'](https://bootstrapshuffle.com/classes)
[Netlify](https://www.netlify.com/)