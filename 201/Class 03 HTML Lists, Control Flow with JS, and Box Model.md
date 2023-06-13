# Class 03: HTML Lists, Control Flow with JS, and the CSS Box Model

[Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
[Ordered Lists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
[Unordered Lists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

## When should you use an unordered list in your HTML document?
> You should use an unordered list (`<ul>`) in your HTML document when you want to represent a list of items that don't have a specific order or sequence. Examples include a list of options, features, or items that are not arranged in any particular order.

## How do you change the bullet style of unordered list items?
> To change the bullet style of unordered list items, you can use CSS. You can target the `<ul>` element or the individual `<li>` elements within it. Here's an example:

`<style> ul {
    list-style-type: square; /* Change the bullet style to square */
  }

  /* Alternatively, you can target the <li> elements */
  ul li {
    list-style-type: circle; /* Change the bullet style to circle */
  } </style>

<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>`

*In this example, the bullet style of the unordered list is set to square, and each individual list item has a bullet style of circle.*

## When should you use an ordered list vs an unordered list in your HTML document?
> You should use an ordered list (`<ol>`) in your HTML document when you want to represent a list of items that have a specific order or sequence. Examples include step-by-step instructions, a numbered list of items, or a hierarchy of elements.## Describe two ways you can change the numbers on list items provided by an ordered list?

There are two ways you can change the numbers on list items provided by an ordered list:

1.  Using the `type` attribute: The `<ol>` element supports the `type` attribute, which allows you to specify the numbering style. The `type` attribute can take values such as "1" (decimal numbers), "A" (uppercase letters), "a" (lowercase letters), "I" (uppercase Roman numerals), or "i" (lowercase Roman numerals). Here's an example:

htmlCopy code

`<ol type="A">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>`

In this example, the list items will be numbered using uppercase letters (A, B, C).

2.  Using CSS: You can also use CSS to change the appearance of the numbers on list items. By targeting the `<li>` elements within the `<ol>` element, you can modify their styling, including the numbering. Here's an example:

## Describe two ways you can change the numbers on list items provided by an ordered list?
>There are two ways you can change the numbers on list items provided by an ordered list:

> 1.  Using the `type` attribute: The `<ol>` element supports the `type` attribute, which allows you to specify the numbering style. The `type` attribute can take values such as "1" (decimal numbers), "A" (uppercase letters), "a" (lowercase letters), "I" (uppercase Roman numerals), or "i" (lowercase Roman numerals). Here's an example:

`<ol type="A">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>`

In this example, the list items will be numbered using uppercase letters (A, B, C).

> 2.  Using CSS: You can also use CSS to change the appearance of the numbers on list items. By targeting the `<li>` elements within the `<ol>` element, you can modify their styling, including the numbering. Here's an example:

`<style> ol {
    counter-reset: my-counter; /* Reset the counter */
  }

  ol li {
    counter-increment: my-counter; /* Increment the counter */
  }

  ol li::before {
    content: counter(my-counter) ") "; /* Add the counter value before each list item */
  } </style>

<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>`



*In this example, the numbers on the list items will be displayed as "1)", "2)", "3)" using the CSS `::before` pseudo-element and the `counter` property. You can customize the numbering format by modifying the content property inside `::before` pseudo-element.*

[Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
[Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

## 1.  Describe the CSS properties of  `margin`  and  `padding`  as characters in a story. What is their role in a story titled: “The Box Model”?

*The story goes as such: Peter the Padding was a romantic optimist and he was fiercely protective of his love interest, Connie the Content. Sometimes she felt stifled by his excessive affection and he was forced to give her space as, she felt, at times her style was being cramped. Connie preferred to be a bit of a lone ranger and prided herself on her autonomy. Her bigger (and more overweight sister) Margaret the Margin was insanely jealous of her laissez-faire attitude to courtship. She's been enamoured by Peter the Padding for years but couldn't get remotely close to him. He was shielded by his over protective mother, Barbara the border. Barbara thought Margaret was a massive square and always stood between the potential opportunity that they might ever meet.*
**© Sarah Woolsey**

# 1.  Padding:
   
    -   The padding is the space between the content of an element and its border.
    -   It is defined using the CSS `padding` property.
    -   The padding can be set individually for each side of an element (top, right, bottom, left) using `padding-top`, `padding-right`, `padding-bottom`, and `padding-left`, or it can be set using shorthand notation (e.g., `padding: 10px 20px 10px 20px`).
    -   Padding values can be specified in various units such as pixels (`px`), ems (`em`), or percentages (`%`).
    -   Padding adds to the total width and height of an element. For example, if an element has a width of 200px and a left padding of 10px, the total width of the element will be 220px.
# 2.  Margin:
   
    -   The margin is the space outside the border of an element.
    -   It is defined using the CSS `margin` property.
    -   The margin can also be set individually for each side of an element (top, right, bottom, left) using `margin-top`, `margin-right`, `margin-bottom`, and `margin-left`, or it can be set using shorthand notation (e.g., `margin: 10px 20px 10px 20px`).
    -   Margin values can be specified in the same units as padding.
    -   Margins do not contribute to the width and height of an element. They create space between elements, pushing them apart.
    -   When two adjacent elements have margins, they collapse, resulting in a single margin equal to the larger of the two margins. This collapsing behavior does not occur with padding.

Both padding and margin properties are useful for controlling the spacing and layout of elements within a document. Padding is primarily used to create space between the content and the border of an element, while margin is used to create space between elements. By adjusting these properties, you can control the overall spacing and positioning of elements on a webpage.

## 2.  List and describe the  **four**  parts of an HTML elements box as referred to by the  `box model`.

The box model in HTML defines the structure and layout of an element, dividing it into four main parts. Here are the four parts of an HTML element's box model:

1.  Content:
   
    -   The content refers to the actual information or visual elements contained within the element, such as text, images, or nested elements.
    -   It is represented by the width and height of the content area.
    -   The content area does not include padding, border, or margin.
2.  Padding:
   
    -   The padding is the space between the content and the element's border.
    -   It provides a buffer between the content and the border, creating internal space within the element.
    -   Padding can be set individually for each side (top, right, bottom, left) or using shorthand notation.
    -   The size of the padding affects the overall dimensions of the element.
3.  Border:
   
    -   The border is a line that surrounds the content and padding of an element, separating it from the surrounding elements.
    -   The border can have different styles, thicknesses, and colors, which can be defined using CSS properties.
    -   The border is positioned immediately outside the padding and is drawn around the content and padding area.
4.  Margin:
   
    -   The margin is the space between the border of an element and the adjacent elements.
    -   It provides spacing and separation between elements on a webpage.
    -   Margins can be set individually for each side (top, right, bottom, left) or using shorthand notation.
    -   The size of the margin does not affect the dimensions of the element but determines the space between elements.

To visualize the box model, you can imagine the content area as the innermost part of the box, surrounded by padding, then the border, and finally the margin on the outermost part. The sum of the content area, padding, border, and margin determines the total dimensions of the element.

[Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
[Expressions & Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

## 1. What `data types` can you store inside of an `Array`?
1.  Numbers: Integer or floating-point values, such as 1, 2.5, -10, etc.
2.  Strings: Textual data enclosed in single ('') or double ("") quotes, like 'hello', "world", etc.
3.  Booleans: True or false values representing logical conditions.
4.  Objects: JavaScript objects, which can contain key-value pairs or complex structures.
5.  Arrays: Arrays can be nested inside other arrays, allowing for multidimensional data storage.
6.  Null: Represents the intentional absence of any object value.
7.  Undefined: Represents the absence of a value or an uninitialized variable.
8.  Symbols: Unique and immutable data type used to identify object properties.

## 2. Is the `people` array a valid JavaScript array? If so, how can I access the values stored? If not, why?

Regarding the `people` array you provided:

`const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];`

Yes, the `people` array is a valid JavaScript array. To access the values stored within it, you can use array indexing. Here's an example:

`console.log(people[0]); // Output: ['pete', 32, 'librarian', null]
console.log(people[1][2]); // Output: 'accountant'`

In the above example, `people[0]` retrieves the first element of the `people` array, which is `['pete', 32, 'librarian', null]`. Similarly, `people[1][2]` retrieves the third element within the second nested array, which is `'accountant'`.

## 3. List **five** shorthand operators for assignment in javascript and describe what they do.

Five shorthand operators for assignment in JavaScript are:

1.  `+=`: Adds the value on the right side to the variable on the left side and assigns the result to the left side variable. For example: `a += 5;` is equivalent to `a = a + 5;`.
2.  `-=`: Subtracts the value on the right side from the variable on the left side and assigns the result to the left side variable. For example: `a -= 3;` is equivalent to `a = a - 3;`.
3.  `*=`: Multiplies the variable on the left side by the value on the right side and assigns the result to the left side variable. For example: `a *= 2;` is equivalent to `a = a * 2;`.
4.  `/=`: Divides the variable on the left side by the value on the right side and assigns the result to the left side variable. For example: `a /= 4;` is equivalent to `a = a / 4;`.
5.  `++`: Increments the value of the variable by 1. For example: `a++;` is equivalent to `a = a + 1;`.


## 4. Read the code below and evaluate the last `expression` and explain what the result would be and why.

     let a = 10;
     let b = 'dog';
     let c = false;
   
     // evaluate this
     (a + c) + b;
   
The last expression `(a + c) + b;` performs addition between `a` and `c`, which results in the numeric addition of `10 + 0` (since `false` is treated as 0 in arithmetic operations). The resulting sum is then concatenated with the string value of `b`, resulting in the final expression `"10false"`. The addition operation is performed first due to the parentheses, and then the concatenation takes place.
   
## 5. Describe a real world example of when a conditional statement should be used in a JavaScript program.

A real-world example of when a conditional statement should be used in a JavaScript program is in an e-commerce website's shopping cart functionality.

Let's consider a scenario where a user adds items to their shopping cart and proceeds to the checkout page. At the checkout page, a conditional statement can be used to check if the user has any items in their cart. If the cart is empty, the website can display a message like "Your cart is empty. Please add items before proceeding." If the cart has items, the checkout process can continue.

Here's an example of how this scenario can be implemented in JavaScript:

`// Assume there is an array called "cartItems" that stores the items in the shopping cart
const cartItems = ['Item 1', 'Item 2', 'Item 3'];

// Check if the cart is empty
if (cartItems.length === 0) {
  console.log("Your cart is empty. Please add items before proceeding.");
} else {
  // Proceed with the checkout process
  console.log("Proceeding to checkout...");
  // Additional code to handle the checkout process
}`

In this example, the `if` statement checks if the length of the `cartItems` array is equal to 0, indicating an empty cart. If it is empty, the program logs a message informing the user to add items. If the cart has items (length greater than 0), the program proceeds with the checkout process.

This conditional statement helps ensure that the user has added items to their cart before allowing them to proceed with the checkout, providing a better user experience and preventing potential errors or confusion during the purchase process.

## 6. Give an example of when a `Loop` is useful in JavaScript.

A common example of when a loop is useful in JavaScript is when you want to iterate over a collection or perform a repetitive task. Let's consider an example where you have an array of numbers and you want to calculate the sum of all the numbers in the array using a loop.

`const numbers = [1, 2, 3, 4, 5];
let sum = 0;

for (let i = 0; i < numbers.length; i++) {
  sum += numbers[i];
}
console.log("The sum is:", sum);`

In this example, a `for` loop is used to iterate over each element in the `numbers` array. The loop starts with initializing the loop variable `i` to 0, and the loop continues as long as `i` is less than the length of the `numbers` array. On each iteration, the loop adds the value of the current element (`numbers[i]`) to the `sum` variable. After the loop finishes, the final sum is displayed using `console.log()`.

By using a loop, you can dynamically process each element of the array, perform calculations, or apply any desired operation. Loops are powerful tools in JavaScript for automating repetitive tasks, processing data structures, and iterating over collections of values.
