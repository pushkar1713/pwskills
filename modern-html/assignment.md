1.  List out the features of HTML5
    Ans.
    HTML5 introduced several new features and improvements over previous versions of HTML:

    - Semantic Elements: New tags like <header>, <footer>, <article>, and <section> help define the structure of web pages more meaningfully.
    - Multimedia Support: Native support for audio (<audio>) and video (<video>) elements without requiring plugins like Flash.
    - Canvas and SVG: The <canvas> element allows for dynamic, scriptable rendering of 2D shapes and bitmap images, while SVG is used for scalable vector graphics.
    - Form Enhancements: New input types like date, email, range, and more, along with attributes like placeholder, required, and pattern that improve form validation and usability.
    - APIs: Various APIs like Geolocation, Web Storage (localStorage and sessionStorage), Web Workers, and more for enhanced interactivity and performance.

2.  What are HTML Entities? List out 5 commonly used HTML entities.
    Ans.
    HTML Entities are special characters reserved in HTML that need to be represented differently in the code to avoid being interpreted as HTML code. They are used to display characters such as <, >, &, and others that have special meanings in HTML.

        5 commonly used HTML entities are:

        &lt; : Represents the less-than sign (<).
        &gt; : Represents the greater-than sign (>).
        &amp; : Represents the ampersand (&).
        &quot; : Represents a double quotation mark (").
        &apos; : Represents a single quotation mark or apostrophe (').

3.  Define accessibility in the context of web development. Explain why it's essential to create accessible websites and how it benefits different user groups.
    Ans.
    Accessibility in web development refers to the practice of designing and building websites that can be used by everyone, including people with disabilities. This includes users with visual, auditory, motor, or cognitive impairments, as well as those with temporary or situational disabilities.

        Why accessibility is essential:

        - Legal Requirements: Many countries have laws and regulations (like the Americans with Disabilities Act in the U.S.) that require websites to be accessible.
        - Inclusivity: It ensures that everyone, regardless of their abilities, can access and benefit from the content and services provided on the web.
        - User Experience: Accessibility often improves the overall user experience, making websites easier to navigate and interact with.
        - SEO Benefits: Accessible websites often have better SEO because they are structured more semantically and are easier for search engines to crawl.

        Benefits for different user groups:

        - People with Disabilities: Provides them equal access to information and services.
        - Older Users: Addresses age-related impairments like reduced vision or dexterity.
        - Users with Temporary Disabilities: For example, someone with a broken arm can still navigate a website using keyboard shortcuts.
        - Situational Disabilities: Helps users in challenging environments, like accessing a website in bright sunlight or in a noisy place.

4.  List any ways which help in improving the accessibility of HTML5.
    Ans.
    Here are some methods to improve the accessibility of HTML5:

        - Use Semantic HTML: Using appropriate tags (<header>, <footer>, <nav>, <main>) helps screen readers and other assistive technologies understand the structure of a page.
        - Provide Text Alternatives: Use alt attributes for images, transcripts for videos, and labels for form controls to ensure all content is accessible to screen readers.
        - Keyboard Accessibility: Ensure that all interactive elements (links, buttons, forms) can be accessed and operated using a keyboard.
        - Aria Roles and Landmarks: Use ARIA (Accessible Rich Internet Applications) roles and landmarks to enhance the accessibility of dynamic content and complex user interfaces.
        - Color Contrast: Ensure sufficient contrast between text and background colors to make content readable for people with visual impairments.
        - Responsive Design: Create responsive layouts that work well on different devices and screen sizes, ensuring content is accessible on all platforms.

5.  Create a web page that highlights the features of HTML5.
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML5 Features</title>
  </head>
  <body>
    <header>
      <h1>Features of HTML5</h1>
    </header>
    <main>
      <section>
        <h2>1. Semantic Elements</h2>
        <p>
          HTML5 introduces semantic elements that provide meaning to the
          structure of a webpage, making it easier for search engines and
          assistive technologies to understand.
        </p>
      </section>
      <section>
        <h2>2. Multimedia Support</h2>
        <p>
          HTML5 natively supports video and audio playback using the
          <code>&lt;video&gt;</code> and <code>&lt;audio&gt;</code> tags without
          requiring third-party plugins.
        </p>
      </section>
      <section>
        <h2>3. APIs for Modern Web Apps</h2>
        <p>
          HTML5 includes APIs like Geolocation, Web Storage, and Web Workers
          that allow developers to create powerful web applications.
        </p>
      </section>
    </main>
    <footer>
      <p>&copy; 2024 HTML5 Feature Showcase</p>
    </footer>
  </body>
</html>
```

6.  Create a simple web page which has a table. The table must have 2 columns: HTML4 and HTML5. The table should include a minimum of three rows describing the differences between HTML4 and HTML5.
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML4 vs HTML5</title>
</head>
<body>
    <h1>Differences between HTML4 and HTML5</h1>
    <table border="1">
        <thead>
            <tr>
                <th>HTML4</th>
                <th>HTML5</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Uses `<div>` elements extensively for layout.</td>
                <td>Introduces semantic elements like `<header>`, `<footer>`, `<article>`, and `<section>` for a more meaningful structure.</td>
            </tr>
            <tr>
                <td>Relies on third-party plugins like Flash for multimedia.</td>
                <td>Native support for audio and video through `<audio>` and `<video>` tags.</td>
            </tr>
            <tr>
                <td>Forms had limited input types like text and password.</td>
                <td>HTML5 introduces new input types like `email`, `date`, `range`, and more, enhancing form functionality.</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```
