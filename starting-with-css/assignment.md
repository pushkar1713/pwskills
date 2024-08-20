### 1. Create a Simple Page with Some Div Tags and Show Different Ways to Add CSS as Well as What Happens When You Target the Same Elements with Inline, Internal, and External CSS

**Solution:**

**HTML Code:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>CSS Targeting Example</title>

    <!-- Internal CSS -->
    <style>
      .box {
        background-color: lightblue;
        color: white;
        padding: 20px;
        border: 2px solid black;
      }
    </style>

    <!-- External CSS (Assume this is in an external stylesheet "styles.css") -->
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <!-- Inline CSS -->
    <div class="box" style="background-color: green;">
      This is a box with multiple CSS sources.
    </div>
  </body>
</html>
```

**Explanation:**

1. **Inline CSS:** The green background color applied here has the highest specificity, so it overrides the internal and external CSS background colors.

2. **Internal CSS:** The internal CSS sets the background color to light blue, which will be overridden by the inline CSS.

3. **External CSS:** The external CSS sets the background color to blue (this would be in a separate `styles.css` file), but it has the lowest priority compared to inline and internal CSS.

---

### 2. Build an HTML Page with Multiple Paragraphs, Each Assigned a Unique Class Name Using BEM Naming Convention

**Solution:**

**HTML Code:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>BEM Naming Convention Example</title>
    <style>
      .paragraph__first {
        color: red;
      }
      .paragraph__second {
        color: blue;
      }
      .paragraph__third {
        color: green;
      }
    </style>
  </head>
  <body>
    <p class="paragraph__first">This is the first paragraph.</p>
    <p class="paragraph__second">This is the second paragraph.</p>
    <p class="paragraph__third">This is the third paragraph.</p>
  </body>
</html>
```

**Explanation:**

- **BEM Naming Convention:** BEM stands for Block, Element, Modifier. It's a methodology that helps you to create reusable components and code sharing in front-end development.

  - **Block:** A standalone entity that is meaningful on its own, e.g., `.paragraph`.

  - **Element:** A part of a block that has no standalone meaning and is semantically tied to its block, e.g., `__first`, `__second`, `__third`.

  - **Modifier:** A flag on a block or element. It changes the look or behavior of a block, e.g., `--active`.

In this example, `paragraph` is the block, and `__first`, `__second`, and `__third` are elements.

---

### 3. Develop an HTML Form with Various Input Elements. Use CSS to Style the Form, Including Setting Background Colors for Input Fields. Create a Custom Color Palette for the Form Elements, and Demonstrate How to Apply Opacity to One of the Form Sections

**Solution:**

**HTML and CSS Code:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Styled Form Example</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        background-color: #f4f4f4;
        margin: 20px;
      }
      .form__container {
        background-color: #fff;
        padding: 20px;
        border-radius: 8px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        width: 300px;
        margin: 0 auto;
      }
      .form__container--transparent {
        opacity: 0.7; /* Applying opacity to one section */
      }
      .form__input {
        width: 100%;
        padding: 10px;
        margin: 10px 0;
        border-radius: 4px;
        border: 1px solid #ccc;
        background-color: #f9f9f9;
      }
      .form__input--submit {
        background-color: #007bff;
        color: white;
        border: none;
        cursor: pointer;
      }
      .form__input--submit:hover {
        background-color: #0056b3;
      }
    </style>
  </head>
  <body>
    <div class="form__container form__container--transparent">
      <form>
        <label for="name">Name:</label>
        <input
          type="text"
          id="name"
          class="form__input"
          placeholder="Enter your name"
        />

        <label for="email">Email:</label>
        <input
          type="email"
          id="email"
          class="form__input"
          placeholder="Enter your email"
        />

        <label for="password">Password:</label>
        <input
          type="password"
          id="password"
          class="form__input"
          placeholder="Enter your password"
        />

        <input
          type="submit"
          class="form__input form__input--submit"
          value="Submit"
        />
      </form>
    </div>
  </body>
</html>
```

**Explanation:**

- **Custom Color Palette:** The form uses a simple color palette with a white background, gray borders, and a blue submit button. The hover effect on the submit button adds an interactive element.
- **Opacity:** The `.form__container--transparent` class is applied to the form container, making it semi-transparent with `opacity: 0.7`.

---
