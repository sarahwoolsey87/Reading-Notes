# Memory Storage

[Understanding the Javascript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

## What is a ‘call’?

> In memory storage, a 'call' typically refers to a function call in a program. When a program executes, it encounters different functions (also known as subroutines or procedures) that perform specific tasks. When the program reaches a function call, it temporarily suspends the execution of the current function and jumps to the called function to execute its code. Once the called function completes its execution, the program returns to the point immediately after the function call in the original function.

## How many ‘calls’ can happen at once?

> The number of 'calls' that can happen at once depends on the available resources and the implementation of the program. In most programming languages, a call stack is used to manage function calls. The call stack is a data structure that keeps track of the active function calls. Each time a function is called, its information (return address, local variables, etc.) is pushed onto the call stack. When the function completes its execution, its information is popped off the stack. The size of the call stack is limited, and if the number of function calls exceeds this limit, a stack overflow can occur.

## What does LIFO mean?

> LIFO stands for "Last In, First Out," which means that the last element added to a stack is the first one to be removed. In the context of a call stack, this means that the most recently called function is the first one to be completed and removed from the stack.

## What causes a Stack Overflow?

> A "Stack Overflow" occurs when the call stack size exceeds its limit. This can happen due to excessive recursion or deeply nested function calls, where there are too many function calls and not enough space on the call stack to accommodate all the function information. When a stack overflow occurs, it usually results in a runtime error, causing the program to terminate unexpectedly.

[Javascript Error Messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

## What is a ‘reference error’?

> A reference error occurs in programming when you try to access a variable or function that is not defined or is outside the scope where it should be accessible. This could happen due to a typo in the variable or function name or attempting to use a variable that has not been declared. The interpreter or compiler cannot find the reference to the variable or function, resulting in a reference error.

## What is a ‘syntax error’?

> A syntax error occurs when the code violates the rules of the programming language's syntax. It means the code is not written in a valid and proper structure that the language understands. Syntax errors are usually detected by the compiler or interpreter during the compilation or parsing phase, and the code execution doesn't proceed until these errors are fixed.

## What is a ‘range error’?

> A range error occurs when a value is not within the acceptable range of values as expected by a function or operation. This usually happens with built-in functions that expect their arguments to be within certain bounds. For example, trying to access an array index that is outside the array's valid range or using a negative value for an operation that requires non-negative values may result in a range error.

## What is a ‘type error’?

> A type error occurs when an operation or function is performed on a data type that is not suitable or compatible for that operation. It usually happens when you try to perform an unsupported operation on a variable, such as trying to use arithmetic operations on a non-numeric variable or trying to access a property of a non-object data type.

## What is a breakpoint?

> In the context of debugging, a breakpoint is a designated point in the source code where the debugger will temporarily pause the program's execution. When the program reaches a breakpoint during runtime, it stops, and the developer can inspect the program's state, variables, and data at that specific moment. Breakpoints are instrumental in debugging because they allow developers to analyse the code step-by-step and identify issues or understand the program's behavior.

## What does the word ‘debugger’ do in your code?

> A debugger is a software tool used by developers to analyse and debug code. It helps identify and fix issues, such as bugs and errors, in a program. Debuggers allow developers to execute the code line-by-line, inspect the values of variables at different points during execution, set breakpoints to pause the program, and monitor the program's flow and behaviour. By usng a debugger, developers can gain valuable insights into the code's execution and find and resolve problems efficiently.

[JavaScript Errors Reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)






