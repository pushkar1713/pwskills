1.  Task1
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Responsive Header</title>
    <style>
      body {
        font-family: Arial, sans-serif;
      }

      header {
        background-color: lightgray;
        padding: 20px;
        text-align: center;
      }

      main {
        padding: 20px;
      }

      footer {
        background-color: lightgray;
        padding: 10px;
        text-align: center;
      }

      /* Media Query */
      @media (max-width: 600px) {
        header {
          background-color: blue;
          color: white;
        }
      }
    </style>
  </head>
  <body>
    <header>
      <h1>Welcome to My Website</h1>
    </header>
    <main>
      <p>This is the main content section.</p>
    </main>
    <footer>
      <p>Footer content goes here.</p>
    </footer>
  </body>
</html>
```

2.  Task2
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Image Gallery</title>
    <style>
      .gallery {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 10px;
      }

      img {
        width: 100%;
        height: auto;
      }

      /* Media Queries */
      @media (max-width: 800px) {
        .gallery {
          grid-template-columns: repeat(2, 1fr);
        }
      }

      @media (max-width: 500px) {
        .gallery {
          grid-template-columns: 1fr;
        }
      }
    </style>
  </head>
  <body>
    <div class="gallery">
      <img
        src="https://fastly.picsum.photos/id/618/200/300.jpg?hmac=t4SGgbCgeW1bbJFjW8RY4vawWUkBDkj5AVuhzkvFEek"
        alt="Image 1"
      />
      <img
        src="https://fastly.picsum.photos/id/618/200/300.jpg?hmac=t4SGgbCgeW1bbJFjW8RY4vawWUkBDkj5AVuhzkvFEek"
        alt="Image 2"
      />
      <img
        src="https://fastly.picsum.photos/id/618/200/300.jpg?hmac=t4SGgbCgeW1bbJFjW8RY4vawWUkBDkj5AVuhzkvFEek"
        alt="Image 3"
      />
    </div>
  </body>
</html>
```

3. Task3
   Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Responsive Navbar</title>
    <style>
      nav ul {
        display: flex;
        list-style-type: none;
        padding: 0;
        background-color: lightgray;
      }

      nav ul li {
        flex: 1;
        text-align: center;
        padding: 10px;
      }

      nav ul li a {
        text-decoration: none;
        color: black;
      }

      /* Media Query */
      @media (max-width: 768px) {
        nav ul {
          flex-direction: column;
          background-color: gray;
        }

        nav ul li {
          text-align: left;
          padding: 10px 20px;
        }
      }
    </style>
  </head>
  <body>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">Portfolio</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </body>
</html>
```

4.  Task4
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Responsive Grid Layout</title>
    <style>
      .grid-container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 10px;
      }

      .grid-item {
        background-color: lightblue;
        padding: 20px;
        text-align: center;
      }

      /* Media Queries */
      @media (max-width: 1024px) {
        .grid-container {
          grid-template-columns: repeat(2, 1fr);
        }
      }

      @media (max-width: 768px) {
        .grid-container {
          grid-template-columns: 1fr;
        }
      }
    </style>
  </head>
  <body>
    <div class="grid-container">
      <div class="grid-item">Item 1</div>
      <div class="grid-item">Item 2</div>
      <div class="grid-item">Item 3</div>
      <div class="grid-item">Item 4</div>
    </div>
  </body>
</html>
```

4.  Task5
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Responsive Flexbox Layout</title>
    <style>
      .flex-container {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
      }

      .flex-item {
        background-color: lightcoral;
        padding: 20px;
        margin: 10px;
        text-align: center;
        flex-basis: 200px;
      }

      /* Media Queries */
      @media (max-width: 768px) {
        .flex-item {
          flex-basis: 100%;
        }
      }
    </style>
  </head>
  <body>
    <div class="flex-container">
      <div class="flex-item">Item 1</div>
      <div class="flex-item">Item 2</div>
      <div class="flex-item">Item 3</div>
      <div class="flex-item">Item 4</div>
    </div>
  </body>
</html>
```
