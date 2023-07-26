# Functional Programming

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

## What is functional programming?

Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data. In functional programming, the focus is on the evaluation of expressions and the use of pure functions to perform operations on immutable data.

## What is a pure function and how do we know if something is a pure function?

> A pure function is a function that always produces the same output for the same input and has no side effects. It means that the function does not modify any data outside its scope or have any observable interactions with the outside world. A pure function relies only on its input arguments to produce the output and doesn't depend on any external state.

To determine if a function is pure, you can check the following criteria:

- It always produces the same output for the same input.
- It does not modify any external state or data.
- It does not have any side effects like I/O operations or network requests.

## What are the benefits of a pure function?

- **Predictability:** Since pure functions have no side effects, they are easier to reason about and predict their behavior.
- **Testability:** Pure functions are easy to test because their behaviour is deterministic and isolated from external factors.
- **Concurrency:** Pure functions can be safely used in concurrent environments without worrying about race conditions or conflicts.
Concurrency: Pure functions can be safely used in concurrent environments without worrying about race conditions or conflicts.

## What is immutability?

> Immutability refers to the property of data that cannot be changed after it is created. In functional programming, immutability is encouraged to prevent unintended side effects and to ensure data integrity. Instead of modifying existing data, functional programs create new data structures with the desired changes.

## What is Referential transparency?

> Referential transparency is a concept closely related to pure functions. It means that a function can be replaced with its return value without affecting the correctness of the program. In other words, if a function is referentially transparent, calling it with the same arguments will always produce the same result, and the function call can be substituted with the result anywhere in the code without changing the program's behaviour. This property allows for easier reasoning about code and optimising evaluations.

[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

## What is a module?

> A module is a self-contained unit of code in Node.js that encapsulates functionality and exposes certain parts of it to be used by other parts of the application. It helps in organising code, promoting reusability, and avoiding global namespace pollution.

## What does the word ‘require’ do?

> The word 'require' is used in Node.js to include and use modules in your code. It is a built-in function that allows you to import external modules or files into your current file. When you use 'require', Node.js searches for the specified module in its built-in modules or in the node_modules directory of your project and returns the exported functionalities from that module.

## How do we bring another module into the file the we are working in?

> To bring another module into the file you are working in, you use the 'require' function followed by the path to the module you want to include. For example:

const myModule = require('./myModule');

In this example, we are bringing the 'myModule' module into the current file, assuming it is located in the same directory.

## What do we have to do to make a module available?

> To make a module available for other files to use, you need to export the functionalities or data you want to expose from that module. In Node.js, you can use the 'module.exports' object to specify what parts of the module you want to make accessible to other files. 

For example:

// myModule.js
const someFunction = () => {
  // ...
};

const someData = 'Hello, world!';

module.exports = {
  someFunction,
  someData
};

In this example, we are exporting the 'someFunction' and 'someData' from the 'myModule' module, and other files can now import and use these functionalities using the 'require' function as shown in the previous answer.