#Images, Colour & Text

[HTML Media](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
[Using images in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Images_in_HTML)
[Common Image Types](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types)
[Choosing Image Formats](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Image_types#choosing_an_image_format)

##What is a real world use case for the alt attribute being used in a website?
> The alt attribute in HTML is primarily used to provide alternative text for images. One real-world use case is improving web accessibility for visually impaired users who rely on screen readers. By providing descriptive alternative text, screen readers can read aloud the text to provide context and information about the image. This allows visually impaired users to understand the content and purpose of the image, even if they cannot see it. The alt attribute is also helpful in situations where images fail to load or are slow to load, as it displays the alternative text in place of the image

##How can you improve accessibility of images in an HTML document?

- **Use the alt attribute:** Include concise, descriptive alternative text using the alt attribute for each image. This text should convey the essential information or purpose of the image.
- **Provide meaningful descriptions:** Avoid using generic phrases like "image.jpg" or leaving the alt attribute empty. Instead, describe the image content accurately and succinctly.
- **Consider context:** Take into account the surrounding content when writing alternative text. Ensure that it provides enough information to understand the image's relevance to the page.
- **Decorative images:** For purely decorative images that don't convey meaningful content, use an empty alt attribute (alt="") or CSS techniques like background images instead.
- **Long descriptions:** If an image requires more detailed information, consider using the longdesc attribute or linking to a separate page providing a comprehensive description.
- **Captions and captions:** For images with associated captions or captions, use appropriate HTML elements like <figure>, <figcaption>, or <figurecaption> to provide a clear relationship between the image and its text.

##Provide an example of when the figure element would be useful in an HTML document.

>Example of when the figure element would be useful:
The <figure> element in HTML is useful when you want to associate a caption or explanatory text with an image, illustration, diagram, or similar content. It establishes a semantic relationship between the image and its description. Here's an example:

<figure>
  <img src="image.jpg" alt="A cat playing with a ball of yarn">
  <figcaption>A playful cat enjoying a ball of yarn.</figcaption>
</figure>

In this example, the <figure> element wraps the image, and the <figcaption> element provides a caption or description for the image. This helps visually impaired users and search engines understand the relationship between the image and its accompanying text.

##Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

> A GIF image is a type of image file that contains a series of frames that are displayed in a sequence, creating an animation. It is commonly used for simple animations, like animated icons or banners. GIF images have a limited color palette and can support transparency. They are like a flipbook, where each page has a slightly different drawing, and when you flip through the pages quickly, it looks like the drawing is moving.

On the other hand, an SVG image stands for Scalable Vector Graphics. SVG images are created using mathematical equations to define shapes, lines, and colors. They are not made up of individual pixels like GIF images but rather use a combination of shapes and lines. SVG images are highly scalable, meaning they can be resized without losing quality or becoming pixelated. They are great for logos, icons, and illustrations that need to look sharp on different devices.

##What image type would you use to display a screenshot on your website and why?

> To display a screenshot on a website, the recommended image type is typically PNG (Portable Network Graphics). PNG images provide lossless compression, meaning they retain high image quality while keeping the file size relatively small. This is important for screenshots, as they often contain detailed visuals that need to be accurately represented.

[Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
[Using Colour in CSS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Colors/Applying_color)
[Styling Text Elements](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

##Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

> Foreground and background colors in HTML elements refer to the colors used for the text and the area behind the text, respectively. Imagine you have a piece of paper with writing on it. The foreground color would be the color of the ink used for the writing, while the background color would be the color of the paper itself.

##Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

- **Choose a color palette:** Select a set of colors that work well together and align with the desired mood or theme of the blog. Consider using complementary or harmonious colors to create a visually pleasing effect.

- **Apply color to headings and text:** Use different colors for headings, body text, links, and other elements. For headings, you can choose a bold and eye-catching color to make them stand out, while using a more neutral color for regular text to ensure readability.

- **Add color accents:** Introduce pops of color to specific elements like buttons, icons, or borders to draw attention and create visual interest. This can help highlight important sections or interactive elements on the blog.

- **Balance with white space:** Remember to balance the use of color with ample white space or neutral background colors. This will prevent the website from appearing overwhelming and ensure the content remains easy to read and navigate.

##What should you consider when choosing fonts for an HTML document?

- **Readability:** Choose fonts that are easy to read, especially for body text. Avoid overly decorative or complex fonts that might strain the reader's eyes or make the text difficult to understand.

- **Compatibility:** Use web-safe fonts or include custom fonts using web font services to ensure that the chosen fonts can be displayed across different devices and browsers.

- **Branding and style:** Consider the overall style and branding of the website. Choose fonts that align with the website's tone, purpose, and target audience. For example, a formal website might benefit from a serif font, while a modern and minimalist website could use a clean and sans-serif font.

##What do font-size, font-weight, and font-style do to HTML text elements?
> Font-size, font-weight, and font-style are CSS properties that can be applied to HTML text elements:

- **font-size:** It determines the size of the text. You can specify it using different units such as pixels (px), percentages (%), or relative units like em or rem. Increasing the font-size will make the text larger, while decreasing it will make it smaller.

- **font-weight:** It controls the thickness or boldness of the text. You can use values like "normal" or "bold" to adjust the weight. Increasing the font-weight makes the text bolder, while decreasing it makes it lighter.

- **font-style:** It defines the style of the text, such as italic or normal. Italic text slants to the right, conveying emphasis or a different tone. The "normal" value displays the text in a regular, upright style.

##Describe two ways you could add spacing around the characters displayed in an h1 element.

Two ways to add spacing around the characters displayed in an h1 element are:

- **Padding:** Use CSS padding property to add space around the text within the h1 element. For example, you can add padding of 10 pixels to all sides of the h1 element to create spacing around the text:

h1 {
  padding: 10px;
}

- **Margin:** Apply CSS margin property to add space around the entire h1 element, pushing other elements away from it. For instance, you can add a margin of 20 pixels to the top and bottom of the h1 element:

h1 {
  margin-top: 20px;
  margin-bottom: 20px;
}

Both padding and margin can be adjusted to add the desired spacing around the characters in the h1 element.