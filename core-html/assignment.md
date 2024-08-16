Build a siple webpage that displays text as shown in the below image.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <p>
      <b> This text will be bolded. </b>
    </p>
    <p>
      <i> This text will be italic. </i>
    </p>
    <p>
      <ins> This text will be underlined</ins>
    </p>
    <mark> This text will be highlighted </mark>
    <p>
      This is normal text<sup> This will be super scripted </sup> This is normal
      again
    </p>
    <p>This is normal text <sub> This text will be subscripted </sub></p>
    <p>Normal Text <small> Smal Text </small></p>
    <p><del> This text will be deleted</del></p>
  </body>
</html>
```

2. Build a simple webpage that helps users navigate different web development-related websites.
   Note: On clicking the hyperlink the web pages should open in a new tab.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>Navigate Me:</h1>
    <p>
      Take me to
      <a href="https://pwskills.com/" target="_blank">PW Skills</a> to buy a
      course.
    </p>
    <p>
      Take me to
      <a href="https://developer.mozilla.org/en-US/" target="_blank"
        >MDN docs</a
      >
      to know more about Web Development.
    </p>
    <p>
      Take me to
      <a href="https://lab.pwskills.com/" target="_blank">PW Skills Lab</a> to
      practice live coding.
    </p>
  </body>
</html>
```

3. Build a simple blog web page with 3 pages home, web development, and web design. Each page must contain hyperlinks to other pages in the top, a heading of the page topic and a paragraph of information.
   For the home page you can add some information about yourself.

- home.html

  ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <title>Home</title>
    </head>
    <body>
      <nav>
        <a href="./home.html">Home</a> |
        <a href="./webDevelopment.html">Web Development</a> |
        <a href="./webDesign.html">Web Design</a>
      </nav>
      <section>
        <h1>Welcome to My Blog!</h1>
        <p>
          Hi, I'm Rahul, a full-stack web developer passionate about creating
          dynamic and responsive web applications. Explore my blog to learn more
          about web development and design!
        </p>
      </section>
    </body>
  </html>
  ```

- webDevelopment.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Web Development</title>
  </head>
  <body>
    <nav>
      <a href="./home.html">Home</a> |
      <a href="./webDevelopment.html">Web Development</a> |
      <a href="./webDesign.html">Web Design</a>
    </nav>
    <section>
      <h1>Web Development</h1>
      <p>
        Web development involves the creation of websites and web applications
        using various technologies like HTML, CSS, and JavaScript. It covers
        both front-end and back-end development.
      </p>
    </section>
  </body>
</html>
```

- webDesign.html

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Web Design</title>
  </head>
  <body>
    <nav>
      <a href="./home.html">Home</a> |
      <a href="./webDevelopment.html">Web Development</a> |
      <a href="./webDesign.html">Web Design</a>
    </nav>
    <section>
      <h1>Web Design</h1>
      <p>
        Web design is about planning and creating the visual layout of a
        website. This involves selecting color schemes, fonts, and images to
        make the site aesthetically pleasing and user-friendly.
      </p>
    </section>
  </body>
</html>
```

4. Create an ordered list of HTML tags. Each list item must include the tag name and some information about the tag.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>HTML Tags List</title>
  </head>
  <body>
    <h1>HTML Tags Overview</h1>
    <ol>
      <li><strong>&lt;h1&gt;</strong>: Defines the most important heading.</li>
      <li>
        <strong>&lt;p&gt;</strong>: Defines a block of text as a paragraph.
      </li>
      <li>
        <strong>&lt;div&gt;</strong>: Defines a container to group other
        elements.
      </li>
      <li><strong>&lt;table&gt;</strong>: Defines a table layout.</li>
      <li><strong>&lt;ul&gt;</strong>: Creates an unordered list of items.</li>
    </ol>
  </body>
</html>
```

5. create a description list of full stack web deKelopment tech stack, using the <dl> tag. Each term should be a tech stack name and each description should be a brief explanation of what the tech stack is used for.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Full Stack Tech Stack</title>
  </head>
  <body>
    <h1>Full Stack Web Development Overview</h1>
    <dl>
      <dt>HTML</dt>
      <dd>The foundation for structuring web content.</dd>

      <dt>CSS</dt>
      <dd>
        Styles and layouts for the web, ensuring it looks visually appealing.
      </dd>

      <dt>JavaScript</dt>
      <dd>Brings interactivity and dynamic content to websites.</dd>

      <dt>Node.js</dt>
      <dd>JavaScript runtime for executing server-side code.</dd>

      <dt>Express.js</dt>
      <dd>Framework for building server-side applications and APIs.</dd>

      <dt>MongoDB</dt>
      <dd>
        NoSQL database for storing data in a flexible, document-oriented format.
      </dd>

      <dt>React.js</dt>
      <dd>JavaScript library for building responsive user interfaces.</dd>
    </dl>
  </body>
</html>
```

6. Create an ordered list of the full stack web development tech stack HTML,CSS and JS. For each tech stack, create a table that llists the tech stack name, its primary use cases, and some key features or benifits.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Full Stack Web Development Tech Stack</title>
  </head>
  <body>
    <h1>Full Stack Web Development Tech Stack</h1>

    <ol>
      <li>HTML</li>
      <table border="1">
        <tr>
          <th>Tech Stack</th>
          <th>Primary Use Cases</th>
          <th>Key Features/Benefits</th>
        </tr>
        <tr>
          <td>HTML (HyperText Markup Language)</td>
          <td>
            <ul>
              <li>Structuring web content</li>
              <li>Defining headings, paragraphs, links, and other elements</li>
            </ul>
          </td>
          <td>
            <ul>
              <li>Basic building block of web pages</li>
              <li>Easy to learn and use</li>
              <li>Supports multimedia elements (images, videos)</li>
            </ul>
          </td>
        </tr>
      </table>

      <li>CSS</li>
      <table border="1">
        <tr>
          <th>Tech Stack</th>
          <th>Primary Use Cases</th>
          <th>Key Features/Benefits</th>
        </tr>
        <tr>
          <td>CSS (Cascading Style Sheets)</td>
          <td>
            <ul>
              <li>Styling web pages</li>
              <li>Creating layouts and designs</li>
            </ul>
          </td>
          <td>
            <ul>
              <li>Separates content from presentation</li>
              <li>Supports responsive design</li>
              <li>Allows customization of fonts, colors, and layouts</li>
            </ul>
          </td>
        </tr>
      </table>

      <li>JavaScript</li>
      <table border="1">
        <tr>
          <th>Tech Stack</th>
          <th>Primary Use Cases</th>
          <th>Key Features/Benefits</th>
        </tr>
        <tr>
          <td>JavaScript</td>
          <td>
            <ul>
              <li>Adding interactivity to web pages</li>
              <li>Handling dynamic content updates</li>
              <li>Building web applications</li>
            </ul>
          </td>
          <td>
            <ul>
              <li>Client-side and server-side scripting</li>
              <li>Wide support across browsers</li>
              <li>
                Rich ecosystem of libraries and frameworks (e.g., React,
                Angular)
              </li>
            </ul>
          </td>
        </tr>
      </table>
    </ol>
  </body>
</html>
```

7. Build a complex nested list structure representing a multi-level table of contents. Use unordered lists (<ul>) and list items (<li>) with inline-block styling to create a structured layout. Apply formatting tags to enhance the presentation of list items.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Table of Contents</title>
    <style>
      body {
        font-family: Arial, sans-serif;
      }
      ul {
        list-style-type: none;
        padding-left: 0;
      }
      li {
        margin: 5px 0;
        position: relative;
      }
      li > ul {
        margin-left: 20px;
      }
      .toc-title {
        font-weight: bold;
        font-size: 1.2em;
      }
      .toc-subtitle {
        font-style: italic;
      }
      .toc-item {
        display: inline-block;
        margin-right: 10px;
      }
      .toc-item::before {
        content: "• ";
        color: #333;
        font-weight: bold;
      }
    </style>
  </head>
  <body>
    <h1>Table of Contents</h1>
    <ul>
      <li class="toc-title">
        Introduction
        <ul>
          <li class="toc-item">Overview</li>
          <li class="toc-item">Purpose</li>
        </ul>
      </li>
      <li class="toc-title">
        Chapter 1: Getting Started
        <ul>
          <li class="toc-item">
            Installation
            <ul>
              <li class="toc-item">System Requirements</li>
              <li class="toc-item">Setup Instructions</li>
            </ul>
          </li>
          <li class="toc-item">Configuration</li>
        </ul>
      </li>
      <li class="toc-title">
        Chapter 2: Advanced Topics
        <ul>
          <li class="toc-item">
            Performance Optimization
            <ul>
              <li class="toc-item">Caching Strategies</li>
              <li class="toc-item">Load Balancing</li>
            </ul>
          </li>
          <li class="toc-item">
            Security
            <ul>
              <li class="toc-item">Authentication</li>
              <li class="toc-item">Authorization</li>
            </ul>
          </li>
        </ul>
      </li>
      <li class="toc-title">
        Appendices
        <ul>
          <li class="toc-item">Glossary</li>
          <li class="toc-item">References</li>
        </ul>
      </li>
    </ul>
  </body>
</html>
```
