### Task 1

**HTML:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Image Gallery</title>
    <style>
      body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
      }

      .gallery {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
        gap: 10px;
        padding: 10px;
      }

      .gallery-item img {
        width: 100%;
        height: auto;
        display: block;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        transition: transform 0.3s ease;
      }

      .gallery-item img:hover {
        transform: scale(1.05);
      }
    </style>
  </head>
  <body>
    <div class="gallery">
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27396740/pexels-photo-27396740/free-photo-of-a-man-with-a-bandana-covering-his-face.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 1"
        />
      </div>
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27068600/pexels-photo-27068600/free-photo-of-skyscrapers-in-new-york-city.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 2"
        />
      </div>
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27396740/pexels-photo-27396740/free-photo-of-a-man-with-a-bandana-covering-his-face.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 3"
        />
      </div>
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27068600/pexels-photo-27068600/free-photo-of-skyscrapers-in-new-york-city.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 4"
        />
      </div>
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27396740/pexels-photo-27396740/free-photo-of-a-man-with-a-bandana-covering-his-face.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 5"
        />
      </div>
      <div class="gallery-item">
        <img
          src="https://images.pexels.com/photos/27068600/pexels-photo-27068600/free-photo-of-skyscrapers-in-new-york-city.jpeg?auto=compress&cs=tinysrgb&w=600&lazy=load"
          alt="Image 6"
        />
      </div>
    </div>
  </body>
</html>
```

### Task 2

**HTML:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .container {
        display: grid;
        grid-template-columns: 2fr 1fr;
        gap: 20px;
        width: 500px;
      }

      .left-column {
        display: grid;
        grid-template-rows: 1fr 1fr;
        gap: 20px;
      }

      .left-upper {
        background-color: lightblue;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .left-lower {
        display: grid;
        grid-template-columns: 1fr 1fr; /* Fixed typo from '/' to ';' */
      }

      .box {
        background-color: pink;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
      }

      .right-column {
        background-color: lightgreen;
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: center;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="left-column">
        <div class="left-upper">A</div>
        <div class="left-lower">
          <div class="box">C</div>
          <div class="box">D</div>
        </div>
      </div>
      <div class="right-column">B</div>
    </div>
  </body>
</html>
```

### Task 3

**Description:**

CSS Grid Layout provides powerful features for creating complex layouts. Among these features are `grid-auto-rows` and `grid-auto-columns`, which are used to define the size of implicitly created rows and columns when the grid container has more items than defined tracks.

- **`grid-auto-rows`**: Specifies the size of rows that are automatically created by the grid container. This applies to rows that are not explicitly defined in the `grid-template-rows` property but are needed to accommodate additional grid items.

- **`grid-auto-columns`**: Specifies the size of columns that are automatically created by the grid container. This applies to columns that are not explicitly defined in the `grid-template-columns` property but are needed to accommodate additional grid items.

**Example:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Dynamic Grid Sizes</title>
    <style>
      .grid-container {
        display: grid;
        grid-template-columns: repeat(
          2,
          1fr
        ); /* Two columns with dynamic width */
        grid-auto-rows: minmax(
          100px,
          auto
        ); /* Rows will be at least 100px, but can grow */
        grid-auto-columns: minmax(
          150px,
          auto
        ); /* Columns will be at least 150px, but can grow */
        gap: 10px;
      }

      .grid-item {
        background-color: lightseagreen;
        border: 1px solid darkslategray;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-size: 16px;
      }
    </style>
  </head>
  <body>
    <div class="grid-container">
      <div class="grid-item">1</div>
      <div class="grid-item">2</div>
      <div class="grid-item">3</div>
      <div class="grid-item">4</div>
      <div class="grid-item">5</div>
      <div class="grid-item">6</div>
      <div class="grid-item">7</div>
      <div class="grid-item">8</div>
      <div class="grid-item">9</div>
      <div class="grid-item">10</div>
      <div class="grid-item">11</div>
    </div>
  </body>
</html>
```

### Task 4

**HTML:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      body {
        margin: 100px;
      }

      .box {
        background-color: #444;
        color: white;
        border-radius: 10px;
        padding: 20px;
        order: 1;
      }

      .box:nth-child(even) {
        background-color: #ccc;
        color: white;
      }

      .container {
        width: 600px;
        display: grid;
        grid-template-columns: repeat(6, 100px);
        grid-gap: 10px;
      }

      .box1 {
        order: 3;
      }

      .box2 {
        order: 6;
      }

      .box8 {
        order: 2;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="box box1">1</div>
      <div class="box box2">2</div>
      <div class="box box3">3</div>
      <div class="box box4">4</div>
      <div class="box box5">5</div>
      <div class="box box6">6</div>
      <div class="box box7">7</div>
      <div class="box box8">8</div>
    </div>
  </body>
</html>
```

### Task 5

**Description:**

In CSS Grid Layout, `justify-items` and `justify-self` are used to align grid items along the horizontal (inline) axis. They provide different levels of control over the alignment of items within the grid container and within individual grid items.

- **`justify-items`**: Applied to the grid container, it specifies the default horizontal alignment of all grid items within their grid areas.

- **`justify-self`**: Applied to individual grid items, it overrides the `justify-items` alignment for that specific item, allowing for fine-tuned horizontal alignment.

  **Examples:**

  **Using `justify-items`:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 100px);
        gap: 10px;
        justify-items: center; /* Align all grid items to center */
      }

      .grid-item {
        background-color: lightcoral;
        color: white;
        padding: 20px;
        border-radius: 5px;
      }
    </style>
  </head>
  <body>
    <div class="grid-container">
      <div class="grid-item">1</div>
      <div class="grid-item">2</div>
      <div class="grid-item">3</div>
    </div>
  </body>
</html>
```

**Using `justify-self`:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .grid-container {
        display: grid;
        grid-template-columns: repeat(3, 100px);
        gap: 10px;
      }

      .grid-item {
        background-color: lightcoral;
        color: white;
        padding: 20px;
        border-radius: 5px;
      }

      .item1 {
        justify-self: start; /* Align item1 to the start of its grid cell */
      }

      .item2 {
        justify-self: center; /* Align item2 to the center of its grid cell */
      }

      .item3 {
        justify-self: end; /* Align item3 to the end of its grid cell */
      }
    </style>
  </head>
  <body>
    <div class="grid-container">
      <div class="grid-item item1">1</div>
      <div class="grid-item item2">2</div>
      <div class="grid-item item3">3</div>
    </div>
  </body>
</html>
```
