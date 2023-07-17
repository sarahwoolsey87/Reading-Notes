# Introduction to Components and React

[Component Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

## What is a “component”?
> A "component" refers to a modular and self-contained unit of software that performs a specific function or provides a specific feature. Components are designed to be reusable and can be combined or composed together to build larger systems or applications.

## What are the characteristics of a component?

- **Encapsulation:** A component encapsulates its internal implementation details and exposes a well-defined interface through which other components or systems can interact with it. This promotes information hiding and allows components to be developed, tested, and maintained independently.

- **Reusability:** Components are designed to be reusable across different projects or applications. By encapsulating specific functionality, components can be easily reused in multiple contexts, saving development time and effort.

- **Modularity:** Components are independent and self-contained units that can be developed, deployed, and maintained separately. This modularity allows for better code organisation, easier collaboration among developers, and the ability to update or replace components without affecting the entire system.

- **Interoperability:** Components are designed to work together with other components or systems using well-defined interfaces or communication protocols. This enables integration with different technologies, platforms, or programming languages, promoting interoperability and system integration.

## What are the advantages of using component-based architecture?

- **Reusability:** Components promote code reuse, reducing development time and effort. Once developed and tested, components can be used in multiple projects or applications, improving efficiency and consistency.

- **Modularity and Maintainability:**  Components allow for better code organization and separation of concerns. They enable developers to focus on specific functionalities or features, making codebases more manageable, easier to maintain, and less prone to bugs.

- **Scalability:** Component-based architectures provide scalability by allowing systems to be built by assembling and integrating individual components. As the system requirements grow, new components can be added or existing components can be replaced or upgraded without impacting the entire system.

- **Collaboration:** Components facilitate collaboration among development teams. By dividing the system into smaller, independent components, different teams or individuals can work on different components simultaneously, promoting parallel development and improving overall productivity.

- **Testability:** Components can be tested in isolation, making it easier to write unit tests and perform integration testing. This ensures that each component functions correctly and interfaces with other components as expected, enhancing overall software quality.

- **Flexibility:** Component-based architectures provide flexibility and adaptability. Components can be easily swapped, updated, or replaced, allowing systems to evolve and adapt to changing requirements or technologies without requiring a complete system overhaul.

[What is props & how to use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)

## What is “props” short for?

> "Props" is short for "properties" in React. Props are a mechanism for passing data from a parent component to its child components.

## How are props used in React?

In React, props are used to provide data and configuration to components. They are similar to function arguments or parameters. Props are passed as attributes to component instances when they are used in JSX (React's syntax extension for JavaScript). The parent component can define and pass props to its child components when rendering them.

Props can be any type of data, such as strings, numbers, booleans, objects, or even functions. They are read-only and cannot be modified by the component receiving them. Props allow parent components to communicate and share data with their child components, enabling the composition of complex user interfaces.

## What is the flow of props?

> The flow of props follows a top-down, or "unidirectional," approach in React. Props are passed from parent components to child components, but not the other way around. This means that data flows in a single direction, from higher-level components to lower-level components.

For example, consider a parent component that renders multiple instances of a child component and provides each child with a different value for a prop called "name." The parent component can define the value of the "name" prop for each child component, and the child components can access and use the prop's value within their own rendering logic or behavior.

This unidirectional flow ensures that changes in props only originate from higher-level components, making the data flow more predictable and easier to reason about. It also helps maintain a clear separation of concerns, as child components rely on the props passed to them without affecting or modifying their parent components.

[React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
[React Docs - Hello world](https://reactjs.org/docs/hello-world.html)
[React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
[https://reactjs.org/docs/rendering-elements.html](https://reactjs.org/docs/rendering-elements.html)
[https://reactjs.org/docs/components-and-props.html](https://reactjs.org/docs/components-and-props.html)





