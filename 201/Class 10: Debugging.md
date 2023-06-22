# Debugging

[What Went Wrong: Troubleshooting Javascript](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/What_went_wrong)

## Name some key differences between a Syntax Error and a Logic Error.

> **Syntax errors** occur when the code violates the rules of the programming language's syntax.
They prevent the code from being parsed or compiled successfully.
Examples of syntax errors include missing parentheses, incorrect variable declarations, and using reserved keywords incorrectly.

> **Logic errors** occur when the code is syntactically correct but does not produce the desired or expected result.
They cause the code to behave incorrectly or produce incorrect output.
Examples of logic errors include incorrect conditional statements, improper loop conditions, and incorrect algorithmic implementation.

## List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them.
'
> I've made numerous 'name errors' which occur when trying to use a variable or function that is not defined or out of scope. To fix them, the code needs to be checked for correct variable/function names and scoping issues.

> Syntax errors are a frequent occurence because I'm brand new to (even seeing) code, such as missing parentheses, semicolons, or mismatched brackets. I spend a lot of time reviewing this. If it's nearing midnight, I have been known to ask Chat GPT to check my syntax...

## How will this topic continue to influence your long term goals?

My long term goal is never to make a mistake ;)

I undersand that debugging and understanding reasons for errors is essential for becoming a proficient programmer. By improving error detection and debugging skills, developers can write more reliable and efficient code. The ability to identify and fix errors quickly is essentia;;y going to result in high-quality software, achieving project goals, and meeting client requirements. Continuous learning and staying updated on programming languages and best practices further enhance the ability to prevent and resolve errors effectively, leading to long-term growth and success in the field of software development.

[The Javscript Debugger](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_are_browser_developer_tools#the_javascript_debugger)

## How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

> The JavaScript Debugger tool is a powerful feature available in most modern web browsers and integrated development environments (IDEs) that helps developers debug and troubleshoot their JavaScript code. It allows you to pause the execution of your code at specific points, examine the current state of variables and objects, step through the code line by line, and track the flow of execution. It's an essential tool for identifying and fixing errors, understanding code behavior, and improving code efficiency.

## Define what a breakpoint is.

> When you start the debugger, you can set breakpoints in your code. A breakpoint is a designated line or point in your code where you want the execution to pause. When the program encounters a breakpoint during execution, it suspends operation, and control is handed over to the debugger. This enables you to inspect the current values of variables, evaluate expressions, and analyze the program's state at that particular moment.

## What is the call stack?

> The call stack, also known as the execution stack or function stack, is a data structure that keeps track of the execution context of function calls in a program. Whenever a function is called, a new frame is added to the top of the call stack, representing that function's execution context. This frame contains information such as the function's arguments, local variables, and the position to return to after the function completes. The call stack operates on a last-in, first-out (LIFO) principle, meaning that the most recently added function is the first one to be executed and completed. Once a function completes, its frame is removed from the call stack, and execution continues with the next function in the stack.

> The call stack is crucial for understanding the order in which functions are called and how they interact with each other. It helps the debugger keep track of the program's flow and allows you to trace back the sequence of function calls and identify any errors or unexpected behavior. By inspecting the call stack, you can gain insights into the program's execution path and better understand the context in which functions are operating.

[Debugging HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Debugging_HTML)
[Debugging CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Debugging_CSS)