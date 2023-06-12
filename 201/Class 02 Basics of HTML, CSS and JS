# Basics of HTML, CSS and JS

[Cont.Intro to HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML) 

[HTML Text Fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)

[Advanced Text Formatting](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)

## Why is it important to use semantic elements in our HTML?

**Accessibility:** Semantic elements improve web accessibility by enabling screen readers and other assistive technologies to understand the content and present it to users with disabilities accurately.
**Search Engine Optimization (SEO):** Search engines rely on semantic structure to better understand and index web pages. Proper use of semantic elements can improve the visibility and ranking of a website in search engine results.
**Readability and Maintainability:** Semantic elements make the HTML code more readable and understandable, both for developers **and other collaborators. It enhances code maintainability and allows for easier future updates or modifications.
**Device Adaptability:** Semantic structure helps in creating responsive web designs and layouts that adapt to different devices and screen sizes.
**Future Compatibility:** Using semantic elements ensures that your web content remains compatible with future HTML standards and technologies.

## How many levels of headings are there in HTML?

HTML provides six levels of headings, ranging from <h1> to <h6>. The hierarchy is as follows:
<h1> represents the highest level heading, typically used for the main title or heading of a page.
<h2> is used for section headings that are subheadings of <h1>.
<h3> is used for subheadings of <h2>, and so on, up to <h6>, which represents the lowest level heading.
It is good practice to follow the hierarchical structure and use headings appropriately to provide a logical outline of the content.  

## What are some uses for the <sup> and <sub> elements?  

<sup> (Superscript): The <sup> element is used to display text or characters as superscript. It is commonly used for mathematical exponents, footnotes, or indicating small, raised elements such as the trademark symbol (TM) or the degree symbol (°).

<sub> (Subscript): The <sub> element is used to display text or characters as subscript. It is often used for chemical formulas, mathematical equations, or indicating small, lowered elements such as subscripts in chemical compounds (e.g., H₂O) or mathematical indices.  

## When using the <abbr> element, what attribute must be added to provide the full expansion of the term?

To provide the full expansion or explanation of an abbreviation or acronym using the <abbr> element, the "title" attribute must be added. The "title" attribute contains the expanded version of the term, which is displayed as a tooltip when the user hovers over the abbreviation. For example:
html  

<abbr title="Hypertext Markup Language">HTML</abbr>  

In the above example, when the user hovers over "HTML," the tooltip will display "Hypertext Markup Language."

[How CSS is Structured](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured) 

## What are ways we can apply CSS to our HTML?  

**Inline Styles:** CSS can be directly added to HTML elements using the "style" attribute. For example: <h1 style="color: blue;">Hello World</h1>. However, this method is generally discouraged for larger stylesheets as it mixes content and presentation, making the code harder to maintain.

**Internal CSS:** CSS can be included within the <style> tags in the <head> section of an HTML document. This allows CSS rules to be applied to multiple elements within the same HTML file.

**External CSS:** CSS can be stored in separate external files with a ".css" extension and linked to the HTML document using the <link> element in the <head> section. This approach allows for the reuse of CSS across multiple HTML files, promoting code organization and maintainability.

**CSS in JavaScript:** CSS can also be dynamically applied to HTML elements using JavaScript. This approach is useful when applying styles based on user interactions or other dynamic conditions.  

## Why should we avoid using inline styles?

**Separation of Concerns:** Inline styles mix the presentation and content within HTML, violating the principle of separating the structure (HTML), presentation (CSS), and behavior (JavaScript) of a web page. This makes the codebase harder to understand, maintain, and update.
**Code Reusability:** Inline styles cannot be reused across multiple elements or pages, leading to code duplication and increased file sizes.
**Specificity and Overriding:** Inline styles have higher specificity than external or internal stylesheets, which can cause conflicts and make it difficult to override styles.
**Collaboration:** Inline styles can make collaboration between designers and developers more challenging, as it requires modification of HTML code for visual changes.  

## Review the block of code below and answer the following questions:  

### What is representing the selector?
  
 **Selector:** The selector in the given code block is h2. It selects all the <h2> elements in the HTML document.  

### Which components are the CSS declarations?  

**CSS Declarations:** The CSS declarations in the code block are color: black; and padding: 5px;.  

### Which components are considered properties?  

**Properties:** The properties in the code block are color and padding. They define the specific aspects of the selected elements that will be modified.

 >  h2 {
     color: black;
     padding: 5px;
   }  

[Cont. Javascript Basics](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured) 

## What data type is a sequence of text enclosed in single quote marks?  

A sequence of text enclosed in single quote marks is a String data type in JavaScript.

## List 4 types of JavaScript operators.  

Four types of JavaScript operators are:

**Arithmetic Operators:** These operators perform mathematical calculations. Examples include addition (+), subtraction (-), multiplication (*), division (/), and modulus (%).

**Comparison Operators:** These operators compare values and return a boolean (true/false) result. Examples include equal to (==), not equal to (!=), greater than (>), less than (<), etc.

**Logical Operators:** These operators are used to combine and manipulate boolean values. Examples include logical AND (&&), logical OR (||), and logical NOT (!).

**Assignment Operators:** These operators are used to assign values to variables. Examples include the assignment operator (=), addition assignment (+=), subtraction assignment (-=), etc.

## Describe a real world Problem you could solve with a Function.

Let's consider a scenario where you are building a restaurant application. One common problem to solve with a function could be calculating the total bill for a customer, including tax and tip.

You could create a function, let's call it calculateBill, that takes inputs such as the cost of the meal, the tax rate, and the desired tip percentage. The function would then perform the necessary calculations, apply the tax and tip, and return the final total.

Here's an example of how the function could be implemented:

function calculateBill(mealCost, taxRate, tipPercentage) {
  const taxAmount = mealCost * (taxRate / 100);
  const tipAmount = mealCost * (tipPercentage / 100);
  const totalBill = mealCost + taxAmount + tipAmount;
  return totalBill;
}

// Example usage:
const mealCost = 50;
const taxRate = 8.5;
const tipPercentage = 15;

const total = calculateBill(mealCost, taxRate, tipPercentage);
console.log("Total bill:", total);

In this example, the calculateBill function takes the meal cost, tax rate, and tip percentage as inputs, performs the necessary calculations, and returns the total bill amount. This function can be used repeatedly with different inputs, allowing you to calculate the bill for any customer.

[Making Decisions in your Code: Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals) 

## An if statement checks a __ and if it evaluates to ___, then the code block will execute.  

### What is the use of an else if?  

An else if statement is used when there are multiple conditions that need to be checked sequentially after the initial if statement. It allows for branching logic based on different conditions. If the initial if statement evaluates to false, the else if statement is evaluated. If the condition in the else if statement evaluates to true, the code block associated with it will execute.

### List 3 different types of comparison operators.  

**Equal to (==):** Checks if two values are equal, disregarding their data types. For example, 5 == "5" would evaluate to true.

**Not equal to (!=):** Checks if two values are not equal, disregarding their data types. For example, 5 != 10 would evaluate to true.

**Greater than (>):** Checks if the value on the left is greater than the value on the right. For example, 10 > 5 would evaluate to true.

### What is the difference between the logical operator && and ||?

*Difference between the logical operators && and ||:*

**Logical AND (&&):** The && operator returns true if both operands are true. It evaluates the operands from left to right and stops as soon as it encounters the first false value. If all operands are true, the result is true. For example, true && false would evaluate to false.

**Logical OR (||):** The || operator returns true if at least one of the operands is true. It evaluates the operands from left to right and stops as soon as it encounters the first true value. If all operands are false, the result is false. For example, true || false would evaluate to true.

In summary, && requires both operands to be true for the result to be true, while || only requires one of the operands to be true for the result to be true.

[Git Commit Messages](https://cbea.ms/git-commit/)