# React & Forms

[React Docs: Form](https://reactjs.org/docs/forms.html)

## What is a ‘Controlled Component’?

In the context of web development and React, a "Controlled Component" refers to a form element (e.g., input, textarea, select) whose value is controlled by React state. In other words, the value of the form element is not stored locally within the element (uncontrolled component), but rather, it is derived from the state of the React component. The component updates its state based on user input, and the value of the form element is then updated through the state binding.

## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

When it comes to storing user responses from a form, there are two common approaches: uncontrolled and controlled components.

**Uncontrolled Component Approach:**
In this approach, you don't store the form data in React state immediately as the user enters it. Instead, you wait until the user submits the form, and then you extract the data from the form elements directly. This is typically achieved by accessing the form element's values directly from the DOM using references or other methods.

**Controlled Component Approach (Storing in State as They Enter):**
With controlled components, you update the React state as the user enters data into the form. This means that the form elements' values are always in sync with the corresponding state variables. This approach allows you to access the form data directly from the state at any time, even before the form is submitted.

So, should you wait to store the user's responses in state when they submit the form, or should you update the state with their responses as soon as they enter them? The answer depends on your specific use case and requirements.

**Controlled Component Approach (Updating State as They Enter):**

- *Pros:* You have access to the user's input data at any time, even before form submission. This enables you to perform real-time validation, show instant feedback, or use the input data for other purposes before the final submission.
- *Cons:* It might lead to more frequent state updates, potentially affecting performance in very complex forms. However, in most cases, this is not a significant concern.
Uncontrolled Component Approach (Storing in State on Submission):

- *Pros:* You might have fewer state updates, which could be beneficial for performance in very large forms.
- *Cons:* You won't have immediate access to the user's input data until they submit the form. Real-time validation or providing instant feedback might be more challenging with this approach.

Ultimately, if you need to access the user's input data before submission (e.g., for real-time validation or other purposes), the controlled component approach is generally more suitable.

## How do we target what the user is entering if we have an event handler on an input field?

When you have an event handler on an input field, you can target what the user is entering through the event object passed to the handler function. Specifically, you can access the user's input from the value property of the input element associated with the event. For example:

import React, { useState } from 'react';

const MyForm = () => {
  const [inputValue, setInputValue] = useState('');

  const handleChange = (event) => {
    const userInput = event.target.value;
    setInputValue(userInput);
  };

  return (
    <form>
      <input type="text" value={inputValue} onChange={handleChange} />
    </form>
  );
};

In this example, as the user types into the input field, the handleChange function updates the inputValue state with the current value entered by the user. This demonstrates how you can target and capture the user's input using an event handler on an input field in a controlled component.

[The Conditional Ternary Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

## Why would we use a ternary operator?

The ternary operator is a concise way of writing simple conditional statements in JavaScript. It's a shorthand form of the if-else statement and is often used when you need to assign a value to a variable based on a condition.

The syntax of the ternary operator is: condition ? expressionIfTrue : expressionIfFalse

## Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

Here's how you can rewrite the provided if-else statement using a ternary operator:

console.log(x === y ? true : false);
In this example, if the condition x === y is true, it will log true to the console; otherwise, it will log false. The ternary operator simplifies the code by eliminating the need for the if and else blocks.

[React Bootstrap: Forms](https://react-bootstrap.github.io/forms/overview/)
[React Docs: Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)





