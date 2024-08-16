1. Write a simple program in HTML that displays the heading "HTML defines the content and structure of your website” on the web browser.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>HTML defines the content and structure of your website</h1>
  </body>
</html>
```

2. Explain the purpose of comments in HTML and provide an example of how to use comments in an HTML document.

Ans.  
 Comments in HTML are used as non-displayed text that provides context or notes about the code to other developers. They are helpful for explaining parts of the code, marking sections for future updates, or temporarily disabling code sections without removing them. Browsers ignore comments, so they do not affect the website's display.
```html
<!-- This is a comment that won't appear on the page -->
<p>This is visible content.</p>

    ```

3. Write an HTML program that includes a heading, a paragraph of text, a horizontal line, and a line break. Arrange these elements to create a simple web page layout.

   ```html
   <!DOCTYPE html>
   <html lang="en">
     <head>
       <meta charset="UTF-8" />
       <meta name="viewport" content="width=device-width, initial-scale=1.0" />
       <title>Basic Web Page Layout</title>
     </head>
     <body>
       <!-- Main heading of the page -->
       <h1>Welcome to My Web Page</h1>

       <!-- Brief introduction paragraph -->
       <p>
         This is a simple paragraph providing an introduction to the content of
         this page.
       </p>

       <!-- Horizontal rule for separation -->
       <hr />

       <!-- Additional text after a line break -->
       <p>
         Here is some more information,<br />
         displayed after a line break.
       </p>
     </body>
   </html>
   ```

4. Write a short note on Tag and element with an example.

   - tags
     An HTML tag is a piece of code enclosed in angle brackets (< and >), used to define the role and format of a specific element on a webpage. Tags serve as instructions to the web browser on how to present the content they surround. Typically, tags come in pairs: a start tag and an end tag, with the element's name placed between the brackets.
     example:

   ```html
   <p>This is a paragraph tag.</p>
   ```

   - Element:
     An HTML element is a complete structure consisting of an opening tag, content, and a closing tag. It represents a distinct part of the webpage's structure or content. An element is essentially the combination of the tags and the enclosed content.

   Example of an Element:

   ```html
   <p>This is a paragraph element.</p>
   ```

5. What is the DOCTYPE Declaration in HTML?

   The DOCTYPE declaration in HTML is a directive that appears at the very top of an HTML document, serving to indicate the HTML version that the document adheres to. It helps web browsers correctly interpret and display the content by ensuring the document is rendered using the appropriate standards. The most widely used declaration, <!DOCTYPE html>, signifies that the document is written in HTML5, the current version of HTML.
