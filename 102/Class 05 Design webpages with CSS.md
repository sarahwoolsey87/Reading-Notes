#Design Webpages with CSS

### What is the purpose of CSS?

CSS, or Cascading Style Sheets, is a language used to style the presentation of web pages. It can be used to control the appearance of text, images, and other elements on a web page. CSS is a powerful tool that can be used to create visually appealing and user-friendly web pages.

### What are the three ways to insert CSS into your project?

There are three ways to insert CSS into your project:

1.  **Inline CSS:** This is the simplest way to insert CSS, and it involves adding the CSS code directly to the HTML code. For example, the following code would set the text color of all paragraphs to red:

@?
```plaintext
<p style="color:red;">This is a red paragraph.</p>
```

1.  **Internal CSS:** This is a more structured way to insert CSS, and it involves adding the CSS code to a `style` element in the `head` section of the HTML code. For example, the following code would set the text color of all paragraphs to red:

```plaintext
<head>
  <style>
    p {
      color: red;
    }
  </style>
</head>
```

1.  **External CSS:** This is the most flexible way to insert CSS, and it involves creating a separate CSS file that contains all of the CSS code for your project. This file can then be linked to from the HTML code using a `link` element. For example, the following code would link to an external CSS file called `style.css`:

```plaintext
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

### Write an example of a CSS rule that would give all \<p> elements red text

The following CSS rule would give all `p` elements red text:


```plaintext
p {
  color: red;
}
```